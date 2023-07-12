# Comparing `tmp/web3-6.6.0.tar.gz` & `tmp/web3-6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3-6.6.0.tar", last modified: Wed Jul 12 20:05:25 2023, max compression
+gzip compressed data, was "web3-6.6.1.tar", last modified: Wed Jul 12 22:14:03 2023, max compression
```

## Comparing `web3-6.6.0.tar` & `web3-6.6.1.tar`

### file list

```diff
@@ -1,340 +1,343 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.684013 web3-6.6.0/
--rw-r--r--   0 eve        (501) staff       (20)     1090 2023-07-07 19:12:15.000000 web3-6.6.0/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      260 2023-04-06 21:34:13.000000 web3-6.6.0/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)     2198 2023-07-12 20:05:25.683845 web3-6.6.0/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     1294 2023-06-26 17:45:20.000000 web3-6.6.0/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.626588 web3-6.6.0/ens/
--rw-r--r--   0 eve        (501) staff       (20)      285 2023-06-26 17:45:20.000000 web3-6.6.0/ens/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    17017 2023-07-07 17:27:16.000000 web3-6.6.0/ens/_normalization.py
--rw-r--r--   0 eve        (501) staff       (20)    34745 2023-07-07 19:12:15.000000 web3-6.6.0/ens/abis.py
--rw-r--r--   0 eve        (501) staff       (20)    20926 2023-07-12 16:45:08.000000 web3-6.6.0/ens/async_ens.py
--rw-r--r--   0 eve        (501) staff       (20)       41 2023-06-26 17:45:20.000000 web3-6.6.0/ens/auto.py
--rw-r--r--   0 eve        (501) staff       (20)     3477 2023-07-12 16:45:08.000000 web3-6.6.0/ens/base_ens.py
--rw-r--r--   0 eve        (501) staff       (20)      601 2023-06-26 17:45:20.000000 web3-6.6.0/ens/constants.py
--rw-r--r--   0 eve        (501) staff       (20)   199089 2023-06-26 17:45:20.000000 web3-6.6.0/ens/contract_data.py
--rw-r--r--   0 eve        (501) staff       (20)    20020 2023-07-12 16:45:08.000000 web3-6.6.0/ens/ens.py
--rw-r--r--   0 eve        (501) staff       (20)     2390 2023-06-26 17:45:20.000000 web3-6.6.0/ens/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)     9279 2023-07-12 16:45:08.000000 web3-6.6.0/ens/utils.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.628317 web3-6.6.0/ethpm/
--rw-r--r--   0 eve        (501) staff       (20)      580 2023-06-07 20:55:14.000000 web3-6.6.0/ethpm/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.629470 web3-6.6.0/ethpm/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2511 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/_utils/backend.py
--rw-r--r--   0 eve        (501) staff       (20)     1477 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/_utils/cache.py
--rw-r--r--   0 eve        (501) staff       (20)     2848 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/_utils/chains.py
--rw-r--r--   0 eve        (501) staff       (20)     1030 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/_utils/contract.py
--rw-r--r--   0 eve        (501) staff       (20)     5263 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/_utils/deployments.py
--rw-r--r--   0 eve        (501) staff       (20)     2717 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/_utils/ipfs.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.629770 web3-6.6.0/ethpm/_utils/protobuf/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/_utils/protobuf/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1938 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/_utils/protobuf/ipfs_file_pb2.py
--rw-r--r--   0 eve        (501) staff       (20)     1488 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/_utils/registry.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.629978 web3-6.6.0/ethpm/assets/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.630101 web3-6.6.0/ethpm/assets/ens/
--rw-r--r--   0 eve        (501) staff       (20)    74682 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/ens/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.630550 web3-6.6.0/ethpm/assets/escrow/
--rw-r--r--   0 eve        (501) staff       (20)     8007 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/escrow/with_bytecode_v3.json
--rw-r--r--   0 eve        (501) staff       (20)      760 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/assets/ipfs_file.proto
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.630835 web3-6.6.0/ethpm/assets/owned/
--rw-r--r--   0 eve        (501) staff       (20)     2655 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/owned/output_v3.json
--rw-r--r--   0 eve        (501) staff       (20)      746 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/owned/with_contract_type_v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.632870 web3-6.6.0/ethpm/assets/registry/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.634980 web3-6.6.0/ethpm/assets/registry/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     3129 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/registry/contracts/Authority.sol
--rw-r--r--   0 eve        (501) staff       (20)     2876 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol
--rw-r--r--   0 eve        (501) staff       (20)     6380 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/registry/contracts/PackageDB.sol
--rw-r--r--   0 eve        (501) staff       (20)    10553 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/registry/contracts/PackageRegistry.sol
--rw-r--r--   0 eve        (501) staff       (20)     2966 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol
--rw-r--r--   0 eve        (501) staff       (20)     9041 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/registry/contracts/ReleaseDB.sol
--rw-r--r--   0 eve        (501) staff       (20)     4980 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/registry/contracts/ReleaseValidator.sol
--rw-r--r--   0 eve        (501) staff       (20)     1046 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/registry/solc_input.json
--rw-r--r--   0 eve        (501) staff       (20)   727775 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/registry/solc_output.json
--rw-r--r--   0 eve        (501) staff       (20)   270218 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/registry/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.635112 web3-6.6.0/ethpm/assets/safe-math-lib/
--rw-r--r--   0 eve        (501) staff       (20)     2845 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.636715 web3-6.6.0/ethpm/assets/simple-registry/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.637760 web3-6.6.0/ethpm/assets/simple-registry/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     1841 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/simple-registry/contracts/Ownable.sol
--rw-r--r--   0 eve        (501) staff       (20)    12350 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol
--rw-r--r--   0 eve        (501) staff       (20)     3278 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol
--rw-r--r--   0 eve        (501) staff       (20)      950 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/simple-registry/solc_input.json
--rw-r--r--   0 eve        (501) staff       (20)   199338 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/simple-registry/solc_output.json
--rw-r--r--   0 eve        (501) staff       (20)    75677 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/simple-registry/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.638297 web3-6.6.0/ethpm/assets/standard-token/
--rw-r--r--   0 eve        (501) staff       (20)    22292 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/standard-token/output_v3.json
--rw-r--r--   0 eve        (501) staff       (20)     8765 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/standard-token/with_bytecode_v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.638916 web3-6.6.0/ethpm/assets/vyper_registry/
--rw-r--r--   0 eve        (501) staff       (20)    81363 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/vyper_registry/0.1.0.json
--rw-r--r--   0 eve        (501) staff       (20)     6339 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/vyper_registry/registry.vy
--rw-r--r--   0 eve        (501) staff       (20)     7596 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/assets/vyper_registry/registry_with_delete.vy
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.639654 web3-6.6.0/ethpm/backends/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/backends/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      956 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/backends/base.py
--rw-r--r--   0 eve        (501) staff       (20)     3006 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/backends/http.py
--rw-r--r--   0 eve        (501) staff       (20)     6551 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/backends/ipfs.py
--rw-r--r--   0 eve        (501) staff       (20)     4174 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/backends/registry.py
--rw-r--r--   0 eve        (501) staff       (20)      405 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     6303 2023-07-07 17:27:16.000000 web3-6.6.0/ethpm/contract.py
--rw-r--r--   0 eve        (501) staff       (20)     1890 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/dependencies.py
--rw-r--r--   0 eve        (501) staff       (20)     2134 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/deployments.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.621128 web3-6.6.0/ethpm/ethpm-spec/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.620935 web3-6.6.0/ethpm/ethpm-spec/examples/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.640449 web3-6.6.0/ethpm/ethpm-spec/examples/escrow/
--rw-r--r--   0 eve        (501) staff       (20)     6810 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     5361 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.640753 web3-6.6.0/ethpm/ethpm-spec/examples/escrow/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      888 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol
--rw-r--r--   0 eve        (501) staff       (20)      644 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol
--rw-r--r--   0 eve        (501) staff       (20)    11598 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     8669 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/escrow/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.641352 web3-6.6.0/ethpm/ethpm-spec/examples/owned/
--rw-r--r--   0 eve        (501) staff       (20)      544 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      443 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/owned/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.641495 web3-6.6.0/ethpm/ethpm-spec/examples/owned/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      222 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/owned/contracts/Owned.sol
--rw-r--r--   0 eve        (501) staff       (20)      728 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      478 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/owned/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.642152 web3-6.6.0/ethpm/ethpm-spec/examples/piper-coin/
--rw-r--r--   0 eve        (501) staff       (20)     5272 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     5030 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json
--rw-r--r--   0 eve        (501) staff       (20)     5220 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     4993 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/piper-coin/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.642896 web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/
--rw-r--r--   0 eve        (501) staff       (20)     3976 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     3143 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.643151 web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      802 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol
--rw-r--r--   0 eve        (501) staff       (20)     5517 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     3289 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.643838 web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/
--rw-r--r--   0 eve        (501) staff       (20)     3794 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     3238 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.644107 web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     1155 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol
--rw-r--r--   0 eve        (501) staff       (20)     2949 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol
--rw-r--r--   0 eve        (501) staff       (20)    17129 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     6100 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.644983 web3-6.6.0/ethpm/ethpm-spec/examples/transferable/
--rw-r--r--   0 eve        (501) staff       (20)      590 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      507 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/transferable/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.645273 web3-6.6.0/ethpm/ethpm-spec/examples/transferable/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      396 2022-04-27 21:13:00.000000 web3-6.6.0/ethpm/ethpm-spec/examples/transferable/contracts/Transferable.sol
--rw-r--r--   0 eve        (501) staff       (20)      786 2022-04-27 21:13:00.000000 web3-6.6.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)      548 2022-04-27 21:13:00.000000 web3-6.6.0/ethpm/ethpm-spec/examples/transferable/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.645962 web3-6.6.0/ethpm/ethpm-spec/examples/wallet/
--rw-r--r--   0 eve        (501) staff       (20)     6669 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     5456 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.646908 web3-6.6.0/ethpm/ethpm-spec/examples/wallet/contracts/
--rw-r--r--   0 eve        (501) staff       (20)     1454 2022-04-27 21:13:00.000000 web3-6.6.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol
--rw-r--r--   0 eve        (501) staff       (20)     9710 2022-04-27 21:13:00.000000 web3-6.6.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     7326 2022-04-27 21:13:00.000000 web3-6.6.0/ethpm/ethpm-spec/examples/wallet/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.646603 web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/
--rw-r--r--   0 eve        (501) staff       (20)     8052 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     6657 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.646743 web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/
--rw-r--r--   0 eve        (501) staff       (20)      621 2022-04-27 21:13:00.000000 web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol
--rw-r--r--   0 eve        (501) staff       (20)    12191 2022-04-27 21:13:00.000000 web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json
--rw-r--r--   0 eve        (501) staff       (20)     9503 2022-04-27 21:13:00.000000 web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.647339 web3-6.6.0/ethpm/ethpm-spec/spec/
--rw-r--r--   0 eve        (501) staff       (20)    10302 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/spec/package.spec.json
--rw-r--r--   0 eve        (501) staff       (20)    12879 2021-02-11 20:53:14.000000 web3-6.6.0/ethpm/ethpm-spec/spec/v3.spec.json
--rw-r--r--   0 eve        (501) staff       (20)     1194 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)    14493 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/package.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.648064 web3-6.6.0/ethpm/tools/
--rw-r--r--   0 eve        (501) staff       (20)      103 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/tools/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    27045 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/tools/builder.py
--rw-r--r--   0 eve        (501) staff       (20)    10373 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/tools/checker.py
--rw-r--r--   0 eve        (501) staff       (20)      475 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/tools/get_manifest.py
--rw-r--r--   0 eve        (501) staff       (20)     4368 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/uri.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.649009 web3-6.6.0/ethpm/validation/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/validation/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4716 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/validation/manifest.py
--rw-r--r--   0 eve        (501) staff       (20)     1072 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/validation/misc.py
--rw-r--r--   0 eve        (501) staff       (20)     2317 2023-04-06 21:34:13.000000 web3-6.6.0/ethpm/validation/package.py
--rw-r--r--   0 eve        (501) staff       (20)     4873 2023-06-26 17:45:20.000000 web3-6.6.0/ethpm/validation/uri.py
--rw-r--r--   0 eve        (501) staff       (20)     1202 2023-07-07 17:27:16.000000 web3-6.6.0/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       38 2023-07-12 20:05:25.684047 web3-6.6.0/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     3076 2023-07-12 20:05:20.000000 web3-6.6.0/setup.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.652680 web3-6.6.0/web3/
--rw-r--r--   0 eve        (501) staff       (20)      752 2023-06-26 17:45:20.000000 web3-6.6.0/web3/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.660619 web3-6.6.0/web3/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/web3/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    31000 2023-07-12 16:45:08.000000 web3-6.6.0/web3/_utils/abi.py
--rw-r--r--   0 eve        (501) staff       (20)      456 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/async_caching.py
--rw-r--r--   0 eve        (501) staff       (20)     8123 2023-07-07 19:12:15.000000 web3-6.6.0/web3/_utils/async_transactions.py
--rw-r--r--   0 eve        (501) staff       (20)     2059 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      992 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/caching.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.660750 web3-6.6.0/web3/_utils/compat/
--rw-r--r--   0 eve        (501) staff       (20)      580 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/compat/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5195 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_error_handling.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.661055 web3-6.6.0/web3/_utils/contract_sources/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/contract_sources/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     6492 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/compile_contracts.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.667437 web3-6.6.0/web3/_utils/contract_sources/contract_data/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      517 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py
--rw-r--r--   0 eve        (501) staff       (20)     5344 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/address_reflector.py
--rw-r--r--   0 eve        (501) staff       (20)    18852 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/arrays_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    14783 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     6089 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     6334 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py
--rw-r--r--   0 eve        (501) staff       (20)    37881 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/emitter_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     5573 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/event_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)    15824 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/extended_resolver.py
--rw-r--r--   0 eve        (501) staff       (20)     1651 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     7637 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/math_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    16716 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py
--rw-r--r--   0 eve        (501) staff       (20)    32645 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py
--rw-r--r--   0 eve        (501) staff       (20)    15579 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/panic_errors_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     1825 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/payable_tester.py
--rw-r--r--   0 eve        (501) staff       (20)    17290 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     5264 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     4264 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/revert_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     3555 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/simple_resolver.py
--rw-r--r--   0 eve        (501) staff       (20)     8238 2023-07-07 19:12:15.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/storage_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    11586 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/string_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    23180 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py
--rw-r--r--   0 eve        (501) staff       (20)    14980 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/contracts.py
--rw-r--r--   0 eve        (501) staff       (20)     1640 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/datatypes.py
--rw-r--r--   0 eve        (501) staff       (20)     1738 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/decorators.py
--rw-r--r--   0 eve        (501) staff       (20)      144 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/empty.py
--rw-r--r--   0 eve        (501) staff       (20)     9065 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/encoding.py
--rw-r--r--   0 eve        (501) staff       (20)     2388 2023-07-12 16:45:08.000000 web3-6.6.0/web3/_utils/ens.py
--rw-r--r--   0 eve        (501) staff       (20)    17198 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/events.py
--rw-r--r--   0 eve        (501) staff       (20)     2113 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/fee_utils.py
--rw-r--r--   0 eve        (501) staff       (20)    11886 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/filters.py
--rw-r--r--   0 eve        (501) staff       (20)     3071 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/formatters.py
--rw-r--r--   0 eve        (501) staff       (20)       55 2023-04-06 21:34:13.000000 web3-6.6.0/web3/_utils/function_identifiers.py
--rw-r--r--   0 eve        (501) staff       (20)      195 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/http.py
--rw-r--r--   0 eve        (501) staff       (20)      209 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/hypothesis.py
--rw-r--r--   0 eve        (501) staff       (20)     1047 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/math.py
--rw-r--r--   0 eve        (501) staff       (20)    29330 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/method_formatters.py
--rw-r--r--   0 eve        (501) staff       (20)     1146 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/miner.py
--rw-r--r--   0 eve        (501) staff       (20)     3147 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/module.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.669901 web3-6.6.0/web3/_utils/module_testing/
--rw-r--r--   0 eve        (501) staff       (20)      539 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/module_testing/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)   176335 2023-07-07 19:12:15.000000 web3-6.6.0/web3/_utils/module_testing/eth_module.py
--rw-r--r--   0 eve        (501) staff       (20)     3406 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/module_testing/go_ethereum_admin_module.py
--rw-r--r--   0 eve        (501) staff       (20)    10338 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/module_testing/go_ethereum_personal_module.py
--rw-r--r--   0 eve        (501) staff       (20)     1176 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/module_testing/go_ethereum_txpool_module.py
--rw-r--r--   0 eve        (501) staff       (20)     4825 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/module_testing/module_testing_utils.py
--rw-r--r--   0 eve        (501) staff       (20)     1272 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/module_testing/net_module.py
--rw-r--r--   0 eve        (501) staff       (20)     9613 2023-07-12 19:51:56.000000 web3-6.6.0/web3/_utils/module_testing/web3_module.py
--rw-r--r--   0 eve        (501) staff       (20)     7447 2023-07-12 16:45:08.000000 web3-6.6.0/web3/_utils/normalizers.py
--rw-r--r--   0 eve        (501) staff       (20)     8833 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/request.py
--rw-r--r--   0 eve        (501) staff       (20)     9509 2023-07-12 16:45:08.000000 web3-6.6.0/web3/_utils/rpc_abi.py
--rw-r--r--   0 eve        (501) staff       (20)     4207 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/threads.py
--rw-r--r--   0 eve        (501) staff       (20)     8737 2023-07-07 17:27:16.000000 web3-6.6.0/web3/_utils/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      816 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/type_conversion.py
--rw-r--r--   0 eve        (501) staff       (20)     1669 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/utility_methods.py
--rw-r--r--   0 eve        (501) staff       (20)     6291 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/validation.py
--rw-r--r--   0 eve        (501) staff       (20)      994 2023-06-26 17:45:20.000000 web3-6.6.0/web3/_utils/windows.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.670291 web3-6.6.0/web3/auto/
--rw-r--r--   0 eve        (501) staff       (20)       44 2023-06-26 17:45:20.000000 web3-6.6.0/web3/auto/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      263 2023-04-06 21:34:13.000000 web3-6.6.0/web3/auto/gethdev.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.670924 web3-6.6.0/web3/beacon/
--rw-r--r--   0 eve        (501) staff       (20)       91 2023-06-26 17:45:20.000000 web3-6.6.0/web3/beacon/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1516 2023-06-26 17:45:20.000000 web3-6.6.0/web3/beacon/api_endpoints.py
--rw-r--r--   0 eve        (501) staff       (20)     5421 2023-06-26 17:45:20.000000 web3-6.6.0/web3/beacon/async_beacon.py
--rw-r--r--   0 eve        (501) staff       (20)     4772 2023-06-26 17:45:20.000000 web3-6.6.0/web3/beacon/main.py
--rw-r--r--   0 eve        (501) staff       (20)      396 2023-06-26 17:45:20.000000 web3-6.6.0/web3/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.671831 web3-6.6.0/web3/contract/
--rw-r--r--   0 eve        (501) staff       (20)      215 2023-06-26 17:45:20.000000 web3-6.6.0/web3/contract/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    19820 2023-07-07 19:12:15.000000 web3-6.6.0/web3/contract/async_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    35727 2023-07-07 17:27:16.000000 web3-6.6.0/web3/contract/base_contract.py
--rw-r--r--   0 eve        (501) staff       (20)    18940 2023-07-07 17:27:16.000000 web3-6.6.0/web3/contract/contract.py
--rw-r--r--   0 eve        (501) staff       (20)    12309 2023-07-07 19:12:15.000000 web3-6.6.0/web3/contract/utils.py
--rw-r--r--   0 eve        (501) staff       (20)     9104 2023-07-07 17:27:16.000000 web3-6.6.0/web3/datastructures.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.672616 web3-6.6.0/web3/eth/
--rw-r--r--   0 eve        (501) staff       (20)      166 2023-06-26 17:45:20.000000 web3-6.6.0/web3/eth/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    20588 2023-07-07 17:27:16.000000 web3-6.6.0/web3/eth/async_eth.py
--rw-r--r--   0 eve        (501) staff       (20)     5943 2023-06-26 17:45:20.000000 web3-6.6.0/web3/eth/base_eth.py
--rw-r--r--   0 eve        (501) staff       (20)    19339 2023-07-07 19:12:15.000000 web3-6.6.0/web3/eth/eth.py
--rw-r--r--   0 eve        (501) staff       (20)     6445 2023-07-07 17:27:16.000000 web3-6.6.0/web3/exceptions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.673155 web3-6.6.0/web3/gas_strategies/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/web3/gas_strategies/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      430 2023-06-26 17:45:20.000000 web3-6.6.0/web3/gas_strategies/rpc.py
--rw-r--r--   0 eve        (501) staff       (20)     9010 2023-06-26 17:45:20.000000 web3-6.6.0/web3/gas_strategies/time_based.py
--rw-r--r--   0 eve        (501) staff       (20)    11826 2023-06-26 17:45:20.000000 web3-6.6.0/web3/geth.py
--rw-r--r--   0 eve        (501) staff       (20)      198 2023-04-06 21:34:13.000000 web3-6.6.0/web3/logs.py
--rw-r--r--   0 eve        (501) staff       (20)    12797 2023-07-12 19:51:56.000000 web3-6.6.0/web3/main.py
--rw-r--r--   0 eve        (501) staff       (20)     7888 2023-07-12 16:45:08.000000 web3-6.6.0/web3/manager.py
--rw-r--r--   0 eve        (501) staff       (20)     8430 2023-07-07 17:27:26.000000 web3-6.6.0/web3/method.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.676625 web3-6.6.0/web3/middleware/
--rw-r--r--   0 eve        (501) staff       (20)     3848 2023-07-12 16:45:08.000000 web3-6.6.0/web3/middleware/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      239 2023-04-06 21:34:13.000000 web3-6.6.0/web3/middleware/abi.py
--rw-r--r--   0 eve        (501) staff       (20)     3222 2023-07-07 17:27:16.000000 web3-6.6.0/web3/middleware/async_cache.py
--rw-r--r--   0 eve        (501) staff       (20)     1779 2023-06-26 17:45:20.000000 web3-6.6.0/web3/middleware/attrdict.py
--rw-r--r--   0 eve        (501) staff       (20)     1785 2023-06-26 17:45:20.000000 web3-6.6.0/web3/middleware/buffered_gas_estimate.py
--rw-r--r--   0 eve        (501) staff       (20)    12880 2023-07-07 17:27:16.000000 web3-6.6.0/web3/middleware/cache.py
--rw-r--r--   0 eve        (501) staff       (20)     1167 2023-06-26 17:45:20.000000 web3-6.6.0/web3/middleware/exception_handling.py
--rw-r--r--   0 eve        (501) staff       (20)     4453 2023-07-07 19:12:15.000000 web3-6.6.0/web3/middleware/exception_retry_request.py
--rw-r--r--   0 eve        (501) staff       (20)    21131 2023-06-26 17:45:20.000000 web3-6.6.0/web3/middleware/filter.py
--rw-r--r--   0 eve        (501) staff       (20)     5396 2023-07-07 19:12:15.000000 web3-6.6.0/web3/middleware/fixture.py
--rw-r--r--   0 eve        (501) staff       (20)     4829 2023-07-07 17:27:16.000000 web3-6.6.0/web3/middleware/formatting.py
--rw-r--r--   0 eve        (501) staff       (20)     4212 2023-06-26 17:45:20.000000 web3-6.6.0/web3/middleware/gas_price_strategy.py
--rw-r--r--   0 eve        (501) staff       (20)     1657 2023-06-26 17:45:20.000000 web3-6.6.0/web3/middleware/geth_poa.py
--rw-r--r--   0 eve        (501) staff       (20)     3336 2023-07-12 16:45:08.000000 web3-6.6.0/web3/middleware/names.py
--rw-r--r--   0 eve        (501) staff       (20)      246 2023-06-15 16:48:05.000000 web3-6.6.0/web3/middleware/normalize_request_parameters.py
--rw-r--r--   0 eve        (501) staff       (20)      351 2023-06-15 16:48:05.000000 web3-6.6.0/web3/middleware/pythonic.py
--rw-r--r--   0 eve        (501) staff       (20)     6605 2023-07-07 19:12:15.000000 web3-6.6.0/web3/middleware/signing.py
--rw-r--r--   0 eve        (501) staff       (20)     1014 2023-06-26 17:45:20.000000 web3-6.6.0/web3/middleware/simulate_unmined_transaction.py
--rw-r--r--   0 eve        (501) staff       (20)     3739 2023-06-26 17:45:20.000000 web3-6.6.0/web3/middleware/stalecheck.py
--rw-r--r--   0 eve        (501) staff       (20)     4548 2023-07-12 16:45:08.000000 web3-6.6.0/web3/middleware/validation.py
--rw-r--r--   0 eve        (501) staff       (20)     3615 2023-06-26 17:45:20.000000 web3-6.6.0/web3/module.py
--rw-r--r--   0 eve        (501) staff       (20)     1562 2023-06-26 17:45:20.000000 web3-6.6.0/web3/net.py
--rw-r--r--   0 eve        (501) staff       (20)    21609 2023-06-26 17:45:20.000000 web3-6.6.0/web3/pm.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.677809 web3-6.6.0/web3/providers/
--rw-r--r--   0 eve        (501) staff       (20)      432 2023-07-07 19:12:15.000000 web3-6.6.0/web3/providers/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4178 2023-07-07 17:27:16.000000 web3-6.6.0/web3/providers/async_base.py
--rw-r--r--   0 eve        (501) staff       (20)     2879 2023-07-07 19:12:15.000000 web3-6.6.0/web3/providers/async_rpc.py
--rw-r--r--   0 eve        (501) staff       (20)     3447 2023-07-07 17:27:16.000000 web3-6.6.0/web3/providers/auto.py
--rw-r--r--   0 eve        (501) staff       (20)     4111 2023-07-07 17:27:16.000000 web3-6.6.0/web3/providers/base.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.678588 web3-6.6.0/web3/providers/eth_tester/
--rw-r--r--   0 eve        (501) staff       (20)       97 2023-06-26 17:45:20.000000 web3-6.6.0/web3/providers/eth_tester/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    14740 2023-07-12 16:45:08.000000 web3-6.6.0/web3/providers/eth_tester/defaults.py
--rw-r--r--   0 eve        (501) staff       (20)     5512 2023-07-07 17:27:16.000000 web3-6.6.0/web3/providers/eth_tester/main.py
--rw-r--r--   0 eve        (501) staff       (20)    12861 2023-07-07 17:27:16.000000 web3-6.6.0/web3/providers/eth_tester/middleware.py
--rw-r--r--   0 eve        (501) staff       (20)     6399 2023-07-07 17:27:16.000000 web3-6.6.0/web3/providers/ipc.py
--rw-r--r--   0 eve        (501) staff       (20)     2686 2023-06-26 17:45:20.000000 web3-6.6.0/web3/providers/rpc.py
--rw-r--r--   0 eve        (501) staff       (20)     3919 2023-06-26 17:45:20.000000 web3-6.6.0/web3/providers/websocket.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/web3/py.typed
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.678732 web3-6.6.0/web3/scripts/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/web3/scripts/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.678904 web3-6.6.0/web3/scripts/release/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/web3/scripts/release/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1534 2023-06-26 17:45:20.000000 web3-6.6.0/web3/scripts/release/test_package.py
--rw-r--r--   0 eve        (501) staff       (20)      951 2023-04-06 21:34:13.000000 web3-6.6.0/web3/testing.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.679051 web3-6.6.0/web3/tools/
--rw-r--r--   0 eve        (501) staff       (20)       73 2023-04-06 21:34:13.000000 web3-6.6.0/web3/tools/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.681593 web3-6.6.0/web3/tools/benchmark/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/web3/tools/benchmark/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5886 2023-06-26 17:45:20.000000 web3-6.6.0/web3/tools/benchmark/main.py
--rw-r--r--   0 eve        (501) staff       (20)     3435 2023-07-07 17:27:16.000000 web3-6.6.0/web3/tools/benchmark/node.py
--rw-r--r--   0 eve        (501) staff       (20)      912 2023-06-26 17:45:20.000000 web3-6.6.0/web3/tools/benchmark/reporting.py
--rw-r--r--   0 eve        (501) staff       (20)     1722 2023-04-06 21:34:13.000000 web3-6.6.0/web3/tools/benchmark/utils.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.682681 web3-6.6.0/web3/tools/pytest_ethereum/
--rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.6.0/web3/tools/pytest_ethereum/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4158 2023-06-26 17:45:20.000000 web3-6.6.0/web3/tools/pytest_ethereum/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)     1423 2023-06-26 17:45:20.000000 web3-6.6.0/web3/tools/pytest_ethereum/deployer.py
--rw-r--r--   0 eve        (501) staff       (20)      380 2023-04-06 21:34:13.000000 web3-6.6.0/web3/tools/pytest_ethereum/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)     3927 2023-06-26 17:45:20.000000 web3-6.6.0/web3/tools/pytest_ethereum/linker.py
--rw-r--r--   0 eve        (501) staff       (20)      645 2023-06-26 17:45:20.000000 web3-6.6.0/web3/tools/pytest_ethereum/plugins.py
--rw-r--r--   0 eve        (501) staff       (20)     2968 2023-07-07 17:27:16.000000 web3-6.6.0/web3/tracing.py
--rw-r--r--   0 eve        (501) staff       (20)    10909 2023-07-07 17:27:16.000000 web3-6.6.0/web3/types.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.683622 web3-6.6.0/web3/utils/
--rw-r--r--   0 eve        (501) staff       (20)      454 2023-06-26 17:45:20.000000 web3-6.6.0/web3/utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      498 2023-06-26 17:45:20.000000 web3-6.6.0/web3/utils/abi.py
--rw-r--r--   0 eve        (501) staff       (20)      967 2023-06-26 17:45:20.000000 web3-6.6.0/web3/utils/address.py
--rw-r--r--   0 eve        (501) staff       (20)     3096 2023-06-26 17:45:20.000000 web3-6.6.0/web3/utils/async_exception_handling.py
--rw-r--r--   0 eve        (501) staff       (20)     1521 2023-06-26 17:45:20.000000 web3-6.6.0/web3/utils/caching.py
--rw-r--r--   0 eve        (501) staff       (20)     3052 2023-06-26 17:45:20.000000 web3-6.6.0/web3/utils/exception_handling.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-12 20:05:25.653571 web3-6.6.0/web3.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)     2198 2023-07-12 20:05:25.000000 web3-6.6.0/web3.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     9869 2023-07-12 20:05:25.000000 web3-6.6.0/web3.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-07-12 20:05:25.000000 web3-6.6.0/web3.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)       64 2023-07-12 20:05:25.000000 web3-6.6.0/web3.egg-info/entry_points.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-07-12 20:05:25.000000 web3-6.6.0/web3.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)     1139 2023-07-12 20:05:25.000000 web3-6.6.0/web3.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)       15 2023-07-12 20:05:25.000000 web3-6.6.0/web3.egg-info/top_level.txt
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.697481 web3-6.6.1/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1090 2023-07-12 17:40:11.000000 web3-6.6.1/LICENSE
+-rw-r--r--   0 fselmo     (501) staff       (20)      291 2023-07-12 22:11:00.000000 web3-6.6.1/MANIFEST.in
+-rw-r--r--   0 fselmo     (501) staff       (20)     2198 2023-07-12 22:14:03.696772 web3-6.6.1/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)     1294 2023-07-06 23:00:21.000000 web3-6.6.1/README.md
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.298303 web3-6.6.1/ens/
+-rw-r--r--   0 fselmo     (501) staff       (20)      285 2023-07-11 21:56:12.000000 web3-6.6.1/ens/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    17017 2023-07-12 17:40:11.000000 web3-6.6.1/ens/_normalization.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    34745 2023-07-12 17:40:11.000000 web3-6.6.1/ens/abis.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    20926 2023-07-12 22:07:02.000000 web3-6.6.1/ens/async_ens.py
+-rw-r--r--   0 fselmo     (501) staff       (20)       41 2023-07-06 23:00:21.000000 web3-6.6.1/ens/auto.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3477 2023-07-12 22:07:02.000000 web3-6.6.1/ens/base_ens.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      601 2023-07-12 20:52:31.000000 web3-6.6.1/ens/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)   199089 2023-07-12 20:52:31.000000 web3-6.6.1/ens/contract_data.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    20020 2023-07-12 22:07:02.000000 web3-6.6.1/ens/ens.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2390 2023-07-06 23:00:21.000000 web3-6.6.1/ens/exceptions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.300562 web3-6.6.1/ens/specs/
+-rw-r--r--   0 fselmo     (501) staff       (20)    48402 2023-07-12 17:40:11.000000 web3-6.6.1/ens/specs/nf.json
+-rw-r--r--   0 fselmo     (501) staff       (20)  3115333 2023-07-12 17:40:11.000000 web3-6.6.1/ens/specs/normalization_spec.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     9279 2023-07-12 22:07:02.000000 web3-6.6.1/ens/utils.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.318993 web3-6.6.1/ethpm/
+-rw-r--r--   0 fselmo     (501) staff       (20)      580 2023-07-12 17:40:11.000000 web3-6.6.1/ethpm/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.328175 web3-6.6.1/ethpm/_utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/_utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2511 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/_utils/backend.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1477 2023-03-13 21:36:03.000000 web3-6.6.1/ethpm/_utils/cache.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2848 2023-03-13 21:36:03.000000 web3-6.6.1/ethpm/_utils/chains.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1030 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/_utils/contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5263 2023-03-13 21:36:03.000000 web3-6.6.1/ethpm/_utils/deployments.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2717 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/_utils/ipfs.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.329867 web3-6.6.1/ethpm/_utils/protobuf/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-11-22 17:31:20.000000 web3-6.6.1/ethpm/_utils/protobuf/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1938 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/_utils/protobuf/ipfs_file_pb2.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1488 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/_utils/registry.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.332655 web3-6.6.1/ethpm/assets/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.334230 web3-6.6.1/ethpm/assets/ens/
+-rw-r--r--   0 fselmo     (501) staff       (20)    74682 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/assets/ens/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.336282 web3-6.6.1/ethpm/assets/escrow/
+-rw-r--r--   0 fselmo     (501) staff       (20)     8007 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/assets/escrow/with_bytecode_v3.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      760 2023-03-13 21:36:03.000000 web3-6.6.1/ethpm/assets/ipfs_file.proto
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.338291 web3-6.6.1/ethpm/assets/owned/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2655 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/assets/owned/output_v3.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      746 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/assets/owned/with_contract_type_v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.345587 web3-6.6.1/ethpm/assets/registry/
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.355250 web3-6.6.1/ethpm/assets/registry/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)     3129 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/registry/contracts/Authority.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     2876 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     6380 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/registry/contracts/PackageDB.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)    10553 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/registry/contracts/PackageRegistry.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     2966 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/registry/contracts/PackageRegistryInterface.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     9041 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/registry/contracts/ReleaseDB.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     4980 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/registry/contracts/ReleaseValidator.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     1046 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/registry/solc_input.json
+-rw-r--r--   0 fselmo     (501) staff       (20)   727775 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/registry/solc_output.json
+-rw-r--r--   0 fselmo     (501) staff       (20)   270218 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/assets/registry/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.356188 web3-6.6.1/ethpm/assets/safe-math-lib/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2845 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.360517 web3-6.6.1/ethpm/assets/simple-registry/
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.364998 web3-6.6.1/ethpm/assets/simple-registry/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1841 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/simple-registry/contracts/Ownable.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)    12350 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/simple-registry/contracts/PackageRegistry.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     3278 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)      950 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/simple-registry/solc_input.json
+-rw-r--r--   0 fselmo     (501) staff       (20)   199338 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/simple-registry/solc_output.json
+-rw-r--r--   0 fselmo     (501) staff       (20)    75677 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/assets/simple-registry/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.367271 web3-6.6.1/ethpm/assets/standard-token/
+-rw-r--r--   0 fselmo     (501) staff       (20)    22292 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/assets/standard-token/output_v3.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     8765 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/assets/standard-token/with_bytecode_v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.371671 web3-6.6.1/ethpm/assets/vyper_registry/
+-rw-r--r--   0 fselmo     (501) staff       (20)    81363 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/vyper_registry/0.1.0.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     6339 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/vyper_registry/registry.vy
+-rw-r--r--   0 fselmo     (501) staff       (20)     7596 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/assets/vyper_registry/registry_with_delete.vy
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.422039 web3-6.6.1/ethpm/backends/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/backends/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      956 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/backends/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3006 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/backends/http.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6551 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/backends/ipfs.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4174 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/backends/registry.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      405 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6303 2023-07-12 17:40:11.000000 web3-6.6.1/ethpm/contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1890 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/dependencies.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2134 2023-03-13 21:36:03.000000 web3-6.6.1/ethpm/deployments.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.277935 web3-6.6.1/ethpm/ethpm-spec/
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.277064 web3-6.6.1/ethpm/ethpm-spec/examples/
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.429280 web3-6.6.1/ethpm/ethpm-spec/examples/escrow/
+-rw-r--r--   0 fselmo     (501) staff       (20)     6810 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     5361 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/escrow/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.431392 web3-6.6.1/ethpm/ethpm-spec/examples/escrow/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)      888 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)      644 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)    11598 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/escrow/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     8669 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/escrow/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.434966 web3-6.6.1/ethpm/ethpm-spec/examples/owned/
+-rw-r--r--   0 fselmo     (501) staff       (20)      544 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      443 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/owned/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.436208 web3-6.6.1/ethpm/ethpm-spec/examples/owned/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)      222 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/owned/contracts/Owned.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)      728 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/owned/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      478 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/owned/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.439516 web3-6.6.1/ethpm/ethpm-spec/examples/piper-coin/
+-rw-r--r--   0 fselmo     (501) staff       (20)     5272 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     5030 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     5220 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     4993 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/piper-coin/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.443126 web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/
+-rw-r--r--   0 fselmo     (501) staff       (20)     3976 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     3143 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.443937 web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)      802 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     5517 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     3289 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.448072 web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/
+-rw-r--r--   0 fselmo     (501) staff       (20)     3794 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     3238 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.449921 web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1155 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     2949 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)    17129 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     6100 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.453652 web3-6.6.1/ethpm/ethpm-spec/examples/transferable/
+-rw-r--r--   0 fselmo     (501) staff       (20)      590 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      507 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/transferable/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.461600 web3-6.6.1/ethpm/ethpm-spec/examples/transferable/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)      396 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/transferable/contracts/Transferable.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)      786 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/transferable/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)      548 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/transferable/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.507544 web3-6.6.1/ethpm/ethpm-spec/examples/wallet/
+-rw-r--r--   0 fselmo     (501) staff       (20)     6669 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     5456 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/wallet/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.511195 web3-6.6.1/ethpm/ethpm-spec/examples/wallet/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1454 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)     9710 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/wallet/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     7326 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/wallet/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.509912 web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/
+-rw-r--r--   0 fselmo     (501) staff       (20)     8052 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     6657 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.510589 web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/contracts/
+-rw-r--r--   0 fselmo     (501) staff       (20)      621 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol
+-rw-r--r--   0 fselmo     (501) staff       (20)    12191 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     9503 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/v3.json
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.512624 web3-6.6.1/ethpm/ethpm-spec/spec/
+-rw-r--r--   0 fselmo     (501) staff       (20)    10302 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/spec/package.spec.json
+-rw-r--r--   0 fselmo     (501) staff       (20)    12879 2023-01-03 18:30:11.000000 web3-6.6.1/ethpm/ethpm-spec/spec/v3.spec.json
+-rw-r--r--   0 fselmo     (501) staff       (20)     1194 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/exceptions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    14493 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/package.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.515844 web3-6.6.1/ethpm/tools/
+-rw-r--r--   0 fselmo     (501) staff       (20)      103 2023-03-13 21:36:03.000000 web3-6.6.1/ethpm/tools/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    27045 2023-03-13 21:36:03.000000 web3-6.6.1/ethpm/tools/builder.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    10373 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/tools/checker.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      475 2023-03-13 21:36:03.000000 web3-6.6.1/ethpm/tools/get_manifest.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4368 2023-03-13 21:36:03.000000 web3-6.6.1/ethpm/uri.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.519028 web3-6.6.1/ethpm/validation/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.6.1/ethpm/validation/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4716 2023-03-13 21:36:03.000000 web3-6.6.1/ethpm/validation/manifest.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1072 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/validation/misc.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2317 2022-08-03 17:01:33.000000 web3-6.6.1/ethpm/validation/package.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4873 2023-07-06 23:00:21.000000 web3-6.6.1/ethpm/validation/uri.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1202 2023-07-06 23:00:21.000000 web3-6.6.1/pyproject.toml
+-rw-r--r--   0 fselmo     (501) staff       (20)       38 2023-07-12 22:14:03.697705 web3-6.6.1/setup.cfg
+-rw-r--r--   0 fselmo     (501) staff       (20)     3076 2023-07-12 22:13:44.000000 web3-6.6.1/setup.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.534529 web3-6.6.1/web3/
+-rw-r--r--   0 fselmo     (501) staff       (20)      752 2023-07-12 22:01:15.000000 web3-6.6.1/web3/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.583037 web3-6.6.1/web3/_utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-06-07 18:31:01.000000 web3-6.6.1/web3/_utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    31000 2023-07-12 22:07:02.000000 web3-6.6.1/web3/_utils/abi.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      456 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/async_caching.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8123 2023-07-12 17:40:11.000000 web3-6.6.1/web3/_utils/async_transactions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2059 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/blocks.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      992 2023-03-13 21:36:03.000000 web3-6.6.1/web3/_utils/caching.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.584113 web3-6.6.1/web3/_utils/compat/
+-rw-r--r--   0 fselmo     (501) staff       (20)      580 2023-07-12 17:40:11.000000 web3-6.6.1/web3/_utils/compat/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5195 2023-07-12 17:40:11.000000 web3-6.6.1/web3/_utils/contract_error_handling.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.586174 web3-6.6.1/web3/_utils/contract_sources/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6492 2023-07-12 17:40:11.000000 web3-6.6.1/web3/_utils/contract_sources/compile_contracts.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.613529 web3-6.6.1/web3/_utils/contract_sources/contract_data/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      517 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/_custom_contract_data.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5344 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/address_reflector.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    18852 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/arrays_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    14783 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/bytes_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6089 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/constructor_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6334 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/contract_caller_tester.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    37881 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/emitter_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5573 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/event_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    15824 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/extended_resolver.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1651 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/fallback_function_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     7637 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/math_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    16716 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/offchain_lookup.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    32645 2023-07-07 18:03:19.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/offchain_resolver.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    15579 2023-07-12 17:40:11.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/panic_errors_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1825 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/payable_tester.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    17290 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/receive_function_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5264 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/reflector_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4264 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/revert_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3555 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/simple_resolver.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8238 2023-07-12 17:40:11.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/storage_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    11586 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/string_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    23180 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/contract_sources/contract_data/tuple_contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    14980 2023-07-07 21:28:03.000000 web3-6.6.1/web3/_utils/contracts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1640 2023-03-13 21:36:03.000000 web3-6.6.1/web3/_utils/datatypes.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1738 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/decorators.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      144 2023-03-13 21:36:03.000000 web3-6.6.1/web3/_utils/empty.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9065 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/encoding.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2388 2023-07-12 22:07:02.000000 web3-6.6.1/web3/_utils/ens.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    17198 2023-07-12 17:40:11.000000 web3-6.6.1/web3/_utils/events.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2113 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/fee_utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    11886 2023-07-07 21:28:03.000000 web3-6.6.1/web3/_utils/filters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3071 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/formatters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)       55 2022-01-11 17:23:55.000000 web3-6.6.1/web3/_utils/function_identifiers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      195 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/http.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      209 2023-03-13 21:36:03.000000 web3-6.6.1/web3/_utils/hypothesis.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1047 2023-03-13 21:36:03.000000 web3-6.6.1/web3/_utils/math.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    29330 2023-07-12 22:01:15.000000 web3-6.6.1/web3/_utils/method_formatters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1146 2023-03-13 21:36:03.000000 web3-6.6.1/web3/_utils/miner.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3147 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/module.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.623726 web3-6.6.1/web3/_utils/module_testing/
+-rw-r--r--   0 fselmo     (501) staff       (20)      539 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/module_testing/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)   176335 2023-07-12 17:40:11.000000 web3-6.6.1/web3/_utils/module_testing/eth_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3406 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/module_testing/go_ethereum_admin_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    10338 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/module_testing/go_ethereum_personal_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1176 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/module_testing/go_ethereum_txpool_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4825 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/module_testing/module_testing_utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1272 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/module_testing/net_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9613 2023-07-12 22:07:02.000000 web3-6.6.1/web3/_utils/module_testing/web3_module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     7447 2023-07-12 22:07:02.000000 web3-6.6.1/web3/_utils/normalizers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8833 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/request.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9509 2023-07-12 22:07:02.000000 web3-6.6.1/web3/_utils/rpc_abi.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4207 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/threads.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8737 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/transactions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      816 2023-07-06 23:00:21.000000 web3-6.6.1/web3/_utils/type_conversion.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1669 2023-03-13 21:36:03.000000 web3-6.6.1/web3/_utils/utility_methods.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6291 2023-07-07 21:28:03.000000 web3-6.6.1/web3/_utils/validation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      994 2023-03-13 21:36:03.000000 web3-6.6.1/web3/_utils/windows.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.625275 web3-6.6.1/web3/auto/
+-rw-r--r--   0 fselmo     (501) staff       (20)       44 2023-07-06 23:00:21.000000 web3-6.6.1/web3/auto/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      263 2023-02-18 04:25:14.000000 web3-6.6.1/web3/auto/gethdev.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.629709 web3-6.6.1/web3/beacon/
+-rw-r--r--   0 fselmo     (501) staff       (20)       91 2023-07-06 23:00:21.000000 web3-6.6.1/web3/beacon/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1516 2023-07-06 23:00:21.000000 web3-6.6.1/web3/beacon/api_endpoints.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5421 2023-07-06 23:00:21.000000 web3-6.6.1/web3/beacon/async_beacon.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4772 2023-07-06 23:00:21.000000 web3-6.6.1/web3/beacon/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      396 2023-03-13 21:36:03.000000 web3-6.6.1/web3/constants.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.635328 web3-6.6.1/web3/contract/
+-rw-r--r--   0 fselmo     (501) staff       (20)      215 2023-07-06 23:00:21.000000 web3-6.6.1/web3/contract/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    19820 2023-07-12 17:40:11.000000 web3-6.6.1/web3/contract/async_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    35727 2023-07-12 17:40:11.000000 web3-6.6.1/web3/contract/base_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    18940 2023-07-12 17:40:11.000000 web3-6.6.1/web3/contract/contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    12309 2023-07-12 17:40:11.000000 web3-6.6.1/web3/contract/utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9104 2023-07-06 23:00:21.000000 web3-6.6.1/web3/datastructures.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.640950 web3-6.6.1/web3/eth/
+-rw-r--r--   0 fselmo     (501) staff       (20)      166 2023-07-06 23:00:21.000000 web3-6.6.1/web3/eth/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    20588 2023-07-12 22:01:15.000000 web3-6.6.1/web3/eth/async_eth.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5943 2023-07-06 23:00:21.000000 web3-6.6.1/web3/eth/base_eth.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    19339 2023-07-12 17:40:11.000000 web3-6.6.1/web3/eth/eth.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6445 2023-07-12 17:40:11.000000 web3-6.6.1/web3/exceptions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.644427 web3-6.6.1/web3/gas_strategies/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-06-07 18:31:01.000000 web3-6.6.1/web3/gas_strategies/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      430 2023-07-06 23:00:21.000000 web3-6.6.1/web3/gas_strategies/rpc.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9010 2023-07-06 23:00:21.000000 web3-6.6.1/web3/gas_strategies/time_based.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    11826 2023-07-06 23:00:21.000000 web3-6.6.1/web3/geth.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      198 2022-09-26 17:05:32.000000 web3-6.6.1/web3/logs.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    12797 2023-07-12 22:07:02.000000 web3-6.6.1/web3/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     7888 2023-07-12 22:07:02.000000 web3-6.6.1/web3/manager.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8430 2023-07-06 23:00:21.000000 web3-6.6.1/web3/method.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.664016 web3-6.6.1/web3/middleware/
+-rw-r--r--   0 fselmo     (501) staff       (20)     3848 2023-07-12 22:07:02.000000 web3-6.6.1/web3/middleware/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      239 2023-01-31 22:25:40.000000 web3-6.6.1/web3/middleware/abi.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3222 2023-07-12 17:40:11.000000 web3-6.6.1/web3/middleware/async_cache.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1779 2023-07-12 22:01:15.000000 web3-6.6.1/web3/middleware/attrdict.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1785 2023-07-06 23:00:21.000000 web3-6.6.1/web3/middleware/buffered_gas_estimate.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    12880 2023-07-12 17:40:11.000000 web3-6.6.1/web3/middleware/cache.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1167 2023-03-13 21:36:03.000000 web3-6.6.1/web3/middleware/exception_handling.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4453 2023-07-12 17:40:11.000000 web3-6.6.1/web3/middleware/exception_retry_request.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    21131 2023-07-06 23:00:21.000000 web3-6.6.1/web3/middleware/filter.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5396 2023-07-12 17:40:11.000000 web3-6.6.1/web3/middleware/fixture.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4829 2023-07-12 22:01:15.000000 web3-6.6.1/web3/middleware/formatting.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4212 2023-07-06 23:00:21.000000 web3-6.6.1/web3/middleware/gas_price_strategy.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1657 2023-07-06 23:00:21.000000 web3-6.6.1/web3/middleware/geth_poa.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3336 2023-07-12 22:07:02.000000 web3-6.6.1/web3/middleware/names.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      246 2022-12-08 21:12:34.000000 web3-6.6.1/web3/middleware/normalize_request_parameters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      351 2023-02-03 21:22:38.000000 web3-6.6.1/web3/middleware/pythonic.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6605 2023-07-12 17:40:11.000000 web3-6.6.1/web3/middleware/signing.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1014 2023-07-06 23:00:21.000000 web3-6.6.1/web3/middleware/simulate_unmined_transaction.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3739 2023-07-06 23:00:21.000000 web3-6.6.1/web3/middleware/stalecheck.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4548 2023-07-12 22:07:02.000000 web3-6.6.1/web3/middleware/validation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3615 2023-07-12 22:01:15.000000 web3-6.6.1/web3/module.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1562 2023-03-13 21:36:03.000000 web3-6.6.1/web3/net.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    21609 2023-07-06 23:00:21.000000 web3-6.6.1/web3/pm.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.671257 web3-6.6.1/web3/providers/
+-rw-r--r--   0 fselmo     (501) staff       (20)      432 2023-07-12 22:01:15.000000 web3-6.6.1/web3/providers/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4178 2023-07-12 22:01:15.000000 web3-6.6.1/web3/providers/async_base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2879 2023-07-12 17:40:11.000000 web3-6.6.1/web3/providers/async_rpc.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3447 2023-07-06 23:00:21.000000 web3-6.6.1/web3/providers/auto.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4111 2023-07-06 23:00:21.000000 web3-6.6.1/web3/providers/base.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.675281 web3-6.6.1/web3/providers/eth_tester/
+-rw-r--r--   0 fselmo     (501) staff       (20)       97 2023-07-06 23:00:21.000000 web3-6.6.1/web3/providers/eth_tester/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    14740 2023-07-12 22:07:02.000000 web3-6.6.1/web3/providers/eth_tester/defaults.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5512 2023-07-06 23:00:21.000000 web3-6.6.1/web3/providers/eth_tester/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    12861 2023-07-06 23:00:21.000000 web3-6.6.1/web3/providers/eth_tester/middleware.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     6399 2023-07-12 17:40:11.000000 web3-6.6.1/web3/providers/ipc.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2686 2023-03-13 21:36:03.000000 web3-6.6.1/web3/providers/rpc.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3919 2023-07-06 23:00:21.000000 web3-6.6.1/web3/providers/websocket.py
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-01-11 17:23:55.000000 web3-6.6.1/web3/py.typed
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.676180 web3-6.6.1/web3/scripts/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-01-11 17:23:55.000000 web3-6.6.1/web3/scripts/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.677470 web3-6.6.1/web3/scripts/release/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-01-11 17:23:55.000000 web3-6.6.1/web3/scripts/release/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1534 2023-03-13 21:36:03.000000 web3-6.6.1/web3/scripts/release/test_package.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      951 2023-03-13 21:36:03.000000 web3-6.6.1/web3/testing.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.678477 web3-6.6.1/web3/tools/
+-rw-r--r--   0 fselmo     (501) staff       (20)       73 2022-09-26 17:05:32.000000 web3-6.6.1/web3/tools/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.682996 web3-6.6.1/web3/tools/benchmark/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-08-03 17:01:33.000000 web3-6.6.1/web3/tools/benchmark/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5886 2023-07-06 23:00:21.000000 web3-6.6.1/web3/tools/benchmark/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3435 2023-07-12 17:40:11.000000 web3-6.6.1/web3/tools/benchmark/node.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      912 2023-03-13 21:36:03.000000 web3-6.6.1/web3/tools/benchmark/reporting.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1722 2023-02-13 20:41:33.000000 web3-6.6.1/web3/tools/benchmark/utils.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.690432 web3-6.6.1/web3/tools/pytest_ethereum/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.6.1/web3/tools/pytest_ethereum/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4158 2023-07-06 23:00:21.000000 web3-6.6.1/web3/tools/pytest_ethereum/_utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1423 2023-07-06 23:00:21.000000 web3-6.6.1/web3/tools/pytest_ethereum/deployer.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      380 2021-11-01 21:09:29.000000 web3-6.6.1/web3/tools/pytest_ethereum/exceptions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3927 2023-03-13 21:36:03.000000 web3-6.6.1/web3/tools/pytest_ethereum/linker.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      645 2023-07-06 23:00:21.000000 web3-6.6.1/web3/tools/pytest_ethereum/plugins.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2968 2023-07-06 23:00:21.000000 web3-6.6.1/web3/tracing.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    10909 2023-07-12 22:01:15.000000 web3-6.6.1/web3/types.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.695822 web3-6.6.1/web3/utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)      454 2023-07-06 23:00:21.000000 web3-6.6.1/web3/utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      498 2023-03-13 21:36:03.000000 web3-6.6.1/web3/utils/abi.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      967 2023-07-06 23:00:21.000000 web3-6.6.1/web3/utils/address.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3096 2023-07-06 23:00:21.000000 web3-6.6.1/web3/utils/async_exception_handling.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1521 2023-07-06 23:00:21.000000 web3-6.6.1/web3/utils/caching.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3052 2023-07-06 23:00:21.000000 web3-6.6.1/web3/utils/exception_handling.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-07-12 22:14:03.542810 web3-6.6.1/web3.egg-info/
+-rw-r--r--   0 fselmo     (501) staff       (20)     2198 2023-07-12 22:14:03.000000 web3-6.6.1/web3.egg-info/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)     9921 2023-07-12 22:14:03.000000 web3-6.6.1/web3.egg-info/SOURCES.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-07-12 22:14:03.000000 web3-6.6.1/web3.egg-info/dependency_links.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)       64 2023-07-12 22:14:03.000000 web3-6.6.1/web3.egg-info/entry_points.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-07-12 22:12:07.000000 web3-6.6.1/web3.egg-info/not-zip-safe
+-rw-r--r--   0 fselmo     (501) staff       (20)     1139 2023-07-12 22:14:03.000000 web3-6.6.1/web3.egg-info/requires.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)       15 2023-07-12 22:14:03.000000 web3-6.6.1/web3.egg-info/top_level.txt
```

### Comparing `web3-6.6.0/LICENSE` & `web3-6.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/PKG-INFO` & `web3-6.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3
-Version: 6.6.0
+Version: 6.6.1
 Summary: web3.py
 Home-page: https://github.com/ethereum/web3.py
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `web3-6.6.0/README.md` & `web3-6.6.1/README.md`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ens/_normalization.py` & `web3-6.6.1/ens/_normalization.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ens/abis.py` & `web3-6.6.1/ens/abis.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ens/async_ens.py` & `web3-6.6.1/ens/async_ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ens/base_ens.py` & `web3-6.6.1/ens/base_ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ens/constants.py` & `web3-6.6.1/ens/constants.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ens/contract_data.py` & `web3-6.6.1/ens/contract_data.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ens/ens.py` & `web3-6.6.1/ens/ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ens/exceptions.py` & `web3-6.6.1/ens/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ens/utils.py` & `web3-6.6.1/ens/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/__init__.py` & `web3-6.6.1/ethpm/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/_utils/backend.py` & `web3-6.6.1/ethpm/_utils/backend.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/_utils/cache.py` & `web3-6.6.1/ethpm/_utils/cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/_utils/chains.py` & `web3-6.6.1/ethpm/_utils/chains.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/_utils/contract.py` & `web3-6.6.1/ethpm/_utils/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/_utils/deployments.py` & `web3-6.6.1/ethpm/_utils/deployments.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/_utils/ipfs.py` & `web3-6.6.1/ethpm/_utils/ipfs.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/_utils/protobuf/ipfs_file_pb2.py` & `web3-6.6.1/ethpm/_utils/protobuf/ipfs_file_pb2.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/_utils/registry.py` & `web3-6.6.1/ethpm/_utils/registry.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/ens/v3.json` & `web3-6.6.1/ethpm/assets/ens/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/escrow/with_bytecode_v3.json` & `web3-6.6.1/ethpm/assets/escrow/with_bytecode_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/ipfs_file.proto` & `web3-6.6.1/ethpm/assets/ipfs_file.proto`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/owned/output_v3.json` & `web3-6.6.1/ethpm/assets/owned/output_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/owned/with_contract_type_v3.json` & `web3-6.6.1/ethpm/assets/owned/with_contract_type_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/registry/contracts/Authority.sol` & `web3-6.6.1/ethpm/assets/registry/contracts/Authority.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol` & `web3-6.6.1/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/registry/contracts/PackageDB.sol` & `web3-6.6.1/ethpm/assets/registry/contracts/PackageDB.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/registry/contracts/PackageRegistry.sol` & `web3-6.6.1/ethpm/assets/registry/contracts/PackageRegistry.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol` & `web3-6.6.1/ethpm/assets/registry/contracts/PackageRegistryInterface.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/registry/contracts/ReleaseDB.sol` & `web3-6.6.1/ethpm/assets/registry/contracts/ReleaseDB.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/registry/contracts/ReleaseValidator.sol` & `web3-6.6.1/ethpm/assets/registry/contracts/ReleaseValidator.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/registry/solc_input.json` & `web3-6.6.1/ethpm/assets/registry/solc_input.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/registry/solc_output.json` & `web3-6.6.1/ethpm/assets/registry/solc_output.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/registry/v3.json` & `web3-6.6.1/ethpm/assets/registry/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json` & `web3-6.6.1/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/simple-registry/contracts/Ownable.sol` & `web3-6.6.1/ethpm/assets/simple-registry/contracts/Ownable.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol` & `web3-6.6.1/ethpm/assets/simple-registry/contracts/PackageRegistry.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol` & `web3-6.6.1/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/simple-registry/solc_input.json` & `web3-6.6.1/ethpm/assets/simple-registry/solc_input.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/simple-registry/solc_output.json` & `web3-6.6.1/ethpm/assets/simple-registry/solc_output.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/simple-registry/v3.json` & `web3-6.6.1/ethpm/assets/simple-registry/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/standard-token/output_v3.json` & `web3-6.6.1/ethpm/assets/standard-token/output_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/standard-token/with_bytecode_v3.json` & `web3-6.6.1/ethpm/assets/standard-token/with_bytecode_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/vyper_registry/0.1.0.json` & `web3-6.6.1/ethpm/assets/vyper_registry/0.1.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/vyper_registry/registry.vy` & `web3-6.6.1/ethpm/assets/vyper_registry/registry.vy`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/assets/vyper_registry/registry_with_delete.vy` & `web3-6.6.1/ethpm/assets/vyper_registry/registry_with_delete.vy`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/backends/base.py` & `web3-6.6.1/ethpm/backends/base.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/backends/http.py` & `web3-6.6.1/ethpm/backends/http.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/backends/ipfs.py` & `web3-6.6.1/ethpm/backends/ipfs.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/backends/registry.py` & `web3-6.6.1/ethpm/backends/registry.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/contract.py` & `web3-6.6.1/ethpm/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/dependencies.py` & `web3-6.6.1/ethpm/dependencies.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/deployments.py` & `web3-6.6.1/ethpm/deployments.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/escrow/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol` & `web3-6.6.1/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol` & `web3-6.6.1/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/escrow/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/escrow/v3.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/escrow/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/owned/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/piper-coin/v3.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/piper-coin/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol` & `web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/safe-math-lib/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol` & `web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol` & `web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/standard-token/v3.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/standard-token/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/transferable/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/transferable/v3.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/transferable/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/wallet/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol` & `web3-6.6.1/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/wallet/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/wallet/v3.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/wallet/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol` & `web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json` & `web3-6.6.1/ethpm/ethpm-spec/examples/wallet-with-send/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/spec/package.spec.json` & `web3-6.6.1/ethpm/ethpm-spec/spec/package.spec.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/ethpm-spec/spec/v3.spec.json` & `web3-6.6.1/ethpm/ethpm-spec/spec/v3.spec.json`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/exceptions.py` & `web3-6.6.1/ethpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/package.py` & `web3-6.6.1/ethpm/package.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/tools/builder.py` & `web3-6.6.1/ethpm/tools/builder.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/tools/checker.py` & `web3-6.6.1/ethpm/tools/checker.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/uri.py` & `web3-6.6.1/ethpm/uri.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/validation/manifest.py` & `web3-6.6.1/ethpm/validation/manifest.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/validation/misc.py` & `web3-6.6.1/ethpm/validation/misc.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/validation/package.py` & `web3-6.6.1/ethpm/validation/package.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/ethpm/validation/uri.py` & `web3-6.6.1/ethpm/validation/uri.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/pyproject.toml` & `web3-6.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/setup.py` & `web3-6.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="web3",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="6.6.0",
+    version="6.6.1",
     description="""web3.py""",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/web3.py",
     include_package_data=True,
```

### Comparing `web3-6.6.0/web3/__init__.py` & `web3-6.6.1/web3/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/abi.py` & `web3-6.6.1/web3/_utils/abi.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/async_transactions.py` & `web3-6.6.1/web3/_utils/async_transactions.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/blocks.py` & `web3-6.6.1/web3/_utils/blocks.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/caching.py` & `web3-6.6.1/web3/_utils/caching.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/compat/__init__.py` & `web3-6.6.1/web3/_utils/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_error_handling.py` & `web3-6.6.1/web3/_utils/contract_error_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/compile_contracts.py` & `web3-6.6.1/web3/_utils/contract_sources/compile_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/_custom_contract_data.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/address_reflector.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/address_reflector.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/arrays_contract.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/arrays_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/bytes_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/constructor_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/contract_caller_tester.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/emitter_contract.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/emitter_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/event_contracts.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/event_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/extended_resolver.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/extended_resolver.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/fallback_function_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/math_contract.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/math_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/offchain_lookup.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/offchain_resolver.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/panic_errors_contract.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/panic_errors_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/payable_tester.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/payable_tester.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/receive_function_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/reflector_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/revert_contract.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/revert_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/simple_resolver.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/simple_resolver.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/storage_contract.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/storage_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/string_contract.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/string_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py` & `web3-6.6.1/web3/_utils/contract_sources/contract_data/tuple_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/contracts.py` & `web3-6.6.1/web3/_utils/contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/datatypes.py` & `web3-6.6.1/web3/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/decorators.py` & `web3-6.6.1/web3/_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/encoding.py` & `web3-6.6.1/web3/_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/ens.py` & `web3-6.6.1/web3/_utils/ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/events.py` & `web3-6.6.1/web3/_utils/events.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/fee_utils.py` & `web3-6.6.1/web3/_utils/fee_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/filters.py` & `web3-6.6.1/web3/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/formatters.py` & `web3-6.6.1/web3/_utils/formatters.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/math.py` & `web3-6.6.1/web3/_utils/math.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/method_formatters.py` & `web3-6.6.1/web3/_utils/method_formatters.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/miner.py` & `web3-6.6.1/web3/_utils/miner.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/module.py` & `web3-6.6.1/web3/_utils/module.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/module_testing/__init__.py` & `web3-6.6.1/web3/_utils/module_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/module_testing/eth_module.py` & `web3-6.6.1/web3/_utils/module_testing/eth_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/module_testing/go_ethereum_admin_module.py` & `web3-6.6.1/web3/_utils/module_testing/go_ethereum_admin_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/module_testing/go_ethereum_personal_module.py` & `web3-6.6.1/web3/_utils/module_testing/go_ethereum_personal_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/module_testing/go_ethereum_txpool_module.py` & `web3-6.6.1/web3/_utils/module_testing/go_ethereum_txpool_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/module_testing/module_testing_utils.py` & `web3-6.6.1/web3/_utils/module_testing/module_testing_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/module_testing/net_module.py` & `web3-6.6.1/web3/_utils/module_testing/net_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/module_testing/web3_module.py` & `web3-6.6.1/web3/_utils/module_testing/web3_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/normalizers.py` & `web3-6.6.1/web3/_utils/normalizers.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/request.py` & `web3-6.6.1/web3/_utils/request.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/rpc_abi.py` & `web3-6.6.1/web3/_utils/rpc_abi.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/threads.py` & `web3-6.6.1/web3/_utils/threads.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/transactions.py` & `web3-6.6.1/web3/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/type_conversion.py` & `web3-6.6.1/web3/_utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/utility_methods.py` & `web3-6.6.1/web3/_utils/utility_methods.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/validation.py` & `web3-6.6.1/web3/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/_utils/windows.py` & `web3-6.6.1/web3/_utils/windows.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/beacon/api_endpoints.py` & `web3-6.6.1/web3/beacon/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/beacon/async_beacon.py` & `web3-6.6.1/web3/beacon/async_beacon.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/beacon/main.py` & `web3-6.6.1/web3/beacon/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/contract/async_contract.py` & `web3-6.6.1/web3/contract/async_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/contract/base_contract.py` & `web3-6.6.1/web3/contract/base_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/contract/contract.py` & `web3-6.6.1/web3/contract/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/contract/utils.py` & `web3-6.6.1/web3/contract/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/datastructures.py` & `web3-6.6.1/web3/datastructures.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/eth/async_eth.py` & `web3-6.6.1/web3/eth/async_eth.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/eth/base_eth.py` & `web3-6.6.1/web3/eth/base_eth.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/eth/eth.py` & `web3-6.6.1/web3/eth/eth.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/exceptions.py` & `web3-6.6.1/web3/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/gas_strategies/time_based.py` & `web3-6.6.1/web3/gas_strategies/time_based.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/geth.py` & `web3-6.6.1/web3/geth.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/main.py` & `web3-6.6.1/web3/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/manager.py` & `web3-6.6.1/web3/manager.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/method.py` & `web3-6.6.1/web3/method.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/__init__.py` & `web3-6.6.1/web3/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/async_cache.py` & `web3-6.6.1/web3/middleware/async_cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/attrdict.py` & `web3-6.6.1/web3/middleware/attrdict.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/buffered_gas_estimate.py` & `web3-6.6.1/web3/middleware/buffered_gas_estimate.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/cache.py` & `web3-6.6.1/web3/middleware/cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/exception_handling.py` & `web3-6.6.1/web3/middleware/exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/exception_retry_request.py` & `web3-6.6.1/web3/middleware/exception_retry_request.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/filter.py` & `web3-6.6.1/web3/middleware/filter.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/fixture.py` & `web3-6.6.1/web3/middleware/fixture.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/formatting.py` & `web3-6.6.1/web3/middleware/formatting.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/gas_price_strategy.py` & `web3-6.6.1/web3/middleware/gas_price_strategy.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/geth_poa.py` & `web3-6.6.1/web3/middleware/geth_poa.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/names.py` & `web3-6.6.1/web3/middleware/names.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/signing.py` & `web3-6.6.1/web3/middleware/signing.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/simulate_unmined_transaction.py` & `web3-6.6.1/web3/middleware/simulate_unmined_transaction.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/stalecheck.py` & `web3-6.6.1/web3/middleware/stalecheck.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/middleware/validation.py` & `web3-6.6.1/web3/middleware/validation.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/module.py` & `web3-6.6.1/web3/module.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/net.py` & `web3-6.6.1/web3/net.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/pm.py` & `web3-6.6.1/web3/pm.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/providers/async_base.py` & `web3-6.6.1/web3/providers/async_base.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/providers/async_rpc.py` & `web3-6.6.1/web3/providers/async_rpc.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/providers/auto.py` & `web3-6.6.1/web3/providers/auto.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/providers/base.py` & `web3-6.6.1/web3/providers/base.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/providers/eth_tester/defaults.py` & `web3-6.6.1/web3/providers/eth_tester/defaults.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/providers/eth_tester/main.py` & `web3-6.6.1/web3/providers/eth_tester/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/providers/eth_tester/middleware.py` & `web3-6.6.1/web3/providers/eth_tester/middleware.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/providers/ipc.py` & `web3-6.6.1/web3/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/providers/rpc.py` & `web3-6.6.1/web3/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/providers/websocket.py` & `web3-6.6.1/web3/providers/websocket.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/scripts/release/test_package.py` & `web3-6.6.1/web3/scripts/release/test_package.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/testing.py` & `web3-6.6.1/web3/testing.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/tools/benchmark/main.py` & `web3-6.6.1/web3/tools/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/tools/benchmark/node.py` & `web3-6.6.1/web3/tools/benchmark/node.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/tools/benchmark/reporting.py` & `web3-6.6.1/web3/tools/benchmark/reporting.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/tools/benchmark/utils.py` & `web3-6.6.1/web3/tools/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/tools/pytest_ethereum/_utils.py` & `web3-6.6.1/web3/tools/pytest_ethereum/_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/tools/pytest_ethereum/deployer.py` & `web3-6.6.1/web3/tools/pytest_ethereum/deployer.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/tools/pytest_ethereum/linker.py` & `web3-6.6.1/web3/tools/pytest_ethereum/linker.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/tools/pytest_ethereum/plugins.py` & `web3-6.6.1/web3/tools/pytest_ethereum/plugins.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/tracing.py` & `web3-6.6.1/web3/tracing.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/types.py` & `web3-6.6.1/web3/types.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/utils/address.py` & `web3-6.6.1/web3/utils/address.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/utils/async_exception_handling.py` & `web3-6.6.1/web3/utils/async_exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/utils/caching.py` & `web3-6.6.1/web3/utils/caching.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3/utils/exception_handling.py` & `web3-6.6.1/web3/utils/exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.6.0/web3.egg-info/PKG-INFO` & `web3-6.6.1/web3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3
-Version: 6.6.0
+Version: 6.6.1
 Summary: web3.py
 Home-page: https://github.com/ethereum/web3.py
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `web3-6.6.0/web3.egg-info/SOURCES.txt` & `web3-6.6.1/web3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 ens/auto.py
 ens/base_ens.py
 ens/constants.py
 ens/contract_data.py
 ens/ens.py
 ens/exceptions.py
 ens/utils.py
+ens/specs/nf.json
+ens/specs/normalization_spec.json
 ethpm/__init__.py
 ethpm/constants.py
 ethpm/contract.py
 ethpm/dependencies.py
 ethpm/deployments.py
 ethpm/exceptions.py
 ethpm/package.py
```

### Comparing `web3-6.6.0/web3.egg-info/requires.txt` & `web3-6.6.1/web3.egg-info/requires.txt`

 * *Files identical despite different names*

