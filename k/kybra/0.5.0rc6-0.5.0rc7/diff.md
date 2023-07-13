# Comparing `tmp/kybra-0.5.0rc6.tar.gz` & `tmp/kybra-0.5.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kybra-0.5.0rc6.tar", last modified: Wed Jul 12 16:32:29 2023, max compression
+gzip compressed data, was "kybra-0.5.0rc7.tar", last modified: Thu Jul 13 18:51:08 2023, max compression
```

## Comparing `kybra-0.5.0rc6.tar` & `kybra-0.5.0rc7.tar`

### file list

```diff
@@ -1,323 +1,324 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.334834 kybra-0.5.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-12 16:32:29.334834 kybra-0.5.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.286833 kybra-0.5.0rc6/kybra/
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-07-12 16:32:11.000000 kybra-0.5.0rc6/kybra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16629 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/build_wasm_binary_or_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.286833 kybra-0.5.0rc6/kybra/canisters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/canisters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.290833 kybra-0.5.0rc6/kybra/canisters/ledger/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/canisters/ledger/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/canisters/ledger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.290833 kybra-0.5.0rc6/kybra/canisters/management/
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/canisters/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/canisters/management/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/canisters/management/bitcoin.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/canisters/management/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/canisters/management/tecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    80489 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/cargotoml.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.290833 kybra-0.5.0rc6/kybra/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.290833 kybra-0.5.0rc6/kybra/compiler/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-12 16:32:29.000000 kybra-0.5.0rc6/kybra/compiler/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.290833 kybra-0.5.0rc6/kybra/compiler/custom_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/custom_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.290833 kybra-0.5.0rc6/kybra/compiler/custom_modules/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-12 16:32:29.000000 kybra-0.5.0rc6/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-12 16:32:29.000000 kybra-0.5.0rc6/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/custom_modules/principal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/install_rust_dependencies.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.290833 kybra-0.5.0rc6/kybra/compiler/kybra_deployer/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_deployer/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.294833 kybra-0.5.0rc6/kybra/compiler/kybra_deployer/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_deployer/src/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_deployer/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.294833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.294833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.298833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/
--rw-r--r--   0 runner    (1001) docker     (123)    24510 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/candid.rs
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/does_interpreter_exist.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.298833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/array.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.298833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.298833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/opt.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/record/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/tuple/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/variant/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/warnings/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.302833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.306833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/init_method/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.306833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.306833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.306833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.306833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/rust.rs
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/constants.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.310833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/
--rw-r--r--   0 runner    (1001) docker     (123)    33809 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/analyze.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/display_string.rs
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/test_error.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.310833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/errors/collect_results.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/errors/unreachable.rs
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/exit_codes.rs
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/get_child_class_of.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/get_name.rs
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.310833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/guard_function/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.310833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/guard_function/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/guard_function/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.310833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/header/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/header/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/header/ref_cells.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/header/traits.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/header/use_statements.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.310833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.318833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.322833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/keywords.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.322833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.322833 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/params.rs
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/returns.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.326834 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/py_ast/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/py_ast/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/py_ast/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.326834 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/source_map/
--rw-r--r--   0 runner    (1001) docker     (123)    22031 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/source_map/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.326834 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/source_map/token_length/
--rw-r--r--   0 runner    (1001) docker     (123)    28330 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.326834 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.330834 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.330834 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/tuple.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.330834 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.330834 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.330834 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.330834 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.334834 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/dfx.rs
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/generate_candid.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/install_app_canister.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/permissions.rs
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/upload_app_canister.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/upload_chunk.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.334834 kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.334834 kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.334834 kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.334834 kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.334834 kybra-0.5.0rc6/kybra/compiler/shared_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/shared_utils/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.334834 kybra-0.5.0rc6/kybra/compiler/shared_utils/src/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/shared_utils/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.334834 kybra-0.5.0rc6/kybra/compiler/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/compiler/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/module_bundler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/run_kybra_generate_or_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/timed.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/kybra/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:32:29.286833 kybra-0.5.0rc6/kybra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-12 16:32:29.000000 kybra-0.5.0rc6/kybra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16600 2023-07-12 16:32:29.000000 kybra-0.5.0rc6/kybra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:32:29.000000 kybra-0.5.0rc6/kybra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 16:32:29.000000 kybra-0.5.0rc6/kybra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 16:32:29.000000 kybra-0.5.0rc6/kybra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:32:29.338834 kybra-0.5.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-12 16:29:42.000000 kybra-0.5.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.144364 kybra-0.5.0rc7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-13 18:51:08.144364 kybra-0.5.0rc7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.088363 kybra-0.5.0rc7/kybra/
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-07-13 18:50:47.000000 kybra-0.5.0rc7/kybra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16629 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/build_wasm_binary_or_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.088363 kybra-0.5.0rc7/kybra/canisters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/canisters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.088363 kybra-0.5.0rc7/kybra/canisters/ledger/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/canisters/ledger/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/canisters/ledger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.088363 kybra-0.5.0rc7/kybra/canisters/management/
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/canisters/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/canisters/management/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/canisters/management/bitcoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/canisters/management/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/canisters/management/tecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80489 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/cargotoml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.092363 kybra-0.5.0rc7/kybra/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.092363 kybra-0.5.0rc7/kybra/compiler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-13 18:51:07.000000 kybra-0.5.0rc7/kybra/compiler/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.092363 kybra-0.5.0rc7/kybra/compiler/custom_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/custom_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.092363 kybra-0.5.0rc7/kybra/compiler/custom_modules/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 18:51:07.000000 kybra-0.5.0rc7/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-13 18:51:07.000000 kybra-0.5.0rc7/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/custom_modules/principal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/install_rust_dependencies.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.092363 kybra-0.5.0rc7/kybra/compiler/kybra_deployer/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_deployer/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.092363 kybra-0.5.0rc7/kybra/compiler/kybra_deployer/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_deployer/src/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_deployer/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.092363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.096363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.096363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/
+-rw-r--r--   0 runner    (1001) docker     (123)    24510 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/candid.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/does_interpreter_exist.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.096363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/array.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.100363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.100363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.100363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/opt.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.100363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/record/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.100363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.100363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.104363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.104363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/tuple/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.104363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/variant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.104363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.104363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/warnings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.104363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.104363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.104363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.108363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/init_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.108363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.108363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.108363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.108363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/constants.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.112363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)    33809 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/analyze.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/display_string.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/test_error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.112363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/errors/collect_results.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/errors/unreachable.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/exit_codes.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/get_child_class_of.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/get_name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.112363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/guard_function/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.112363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/guard_function/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/guard_function/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.112363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/header/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/header/ref_cells.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/header/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/header/use_statements.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.112363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.124364 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.124364 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/keywords.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.128363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.128363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/params.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/returns.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.128363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/py_ast/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/py_ast/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/py_ast/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.128363 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/source_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    22031 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/source_map/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.132364 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/source_map/token_length/
+-rw-r--r--   0 runner    (1001) docker     (123)    28330 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.132364 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.132364 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.136364 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/tuple.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.136364 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.136364 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.136364 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.140364 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.140364 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/clear_chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/dfx.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/generate_candid.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/install_app_canister.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/permissions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/upload_app_canister.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/upload_chunk.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.140364 kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.140364 kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.140364 kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.140364 kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.140364 kybra-0.5.0rc7/kybra/compiler/shared_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/shared_utils/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.144364 kybra-0.5.0rc7/kybra/compiler/shared_utils/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/shared_utils/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.144364 kybra-0.5.0rc7/kybra/compiler/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/compiler/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/module_bundler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/run_kybra_generate_or_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/timed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/kybra/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:51:08.088363 kybra-0.5.0rc7/kybra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-13 18:51:08.000000 kybra-0.5.0rc7/kybra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-07-13 18:51:08.000000 kybra-0.5.0rc7/kybra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:51:08.000000 kybra-0.5.0rc7/kybra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 18:51:08.000000 kybra-0.5.0rc7/kybra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 18:51:08.000000 kybra-0.5.0rc7/kybra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:51:08.144364 kybra-0.5.0rc7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-13 18:47:46.000000 kybra-0.5.0rc7/setup.py
```

### Comparing `kybra-0.5.0rc6/LICENSE` & `kybra-0.5.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/NOTICE` & `kybra-0.5.0rc7/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/PKG-INFO` & `kybra-0.5.0rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kybra
-Version: 0.5.0rc6
+Version: 0.5.0rc7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 <div align="center">
     <a href="https://github.com/demergent-labs/kybra" target="_blank" rel="noopener noreferrer">
         <img height="150" src="https://raw.githubusercontent.com/demergent-labs/kybra/main/logo/logo.svg" alt="kybra logo">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kybra Version: 0.5.0rc6 Description-Content-Type:
+Metadata-Version: 2.1 Name: kybra Version: 0.5.0rc7 Description-Content-Type:
 text/markdown License-File: LICENSE License-File: NOTICE
                                  [kybra_logo]
                        [Coverage_Status] [PyPI_version]
 # Kybra (Beta) Python CDK for the [Internet Computer](https://
 internetcomputer.org/). ## Disclaimer Things to keep in mind: - Kybra does not
 yet have many live, successful, continuously operating applications deployed to
 the IC - Kybra does not yet have extensive automated property tests - Kybra
```

### Comparing `kybra-0.5.0rc6/README.md` & `kybra-0.5.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/__init__.py` & `kybra-0.5.0rc7/kybra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     TypeAlias,
     Union,
 )
 
 # TODO I think we can simplify this just like we're doing with canisters
 from .compiler.custom_modules.principal import Principal as PrincipalRenamed
 
-__version__ = "0.5.0rc6"
+__version__ = "0.5.0rc7"
 __rust_version__ = "1.68.2"
 
 Principal = PrincipalRenamed
 
 int64 = int
 int32 = int
 int16 = int
```

### Comparing `kybra-0.5.0rc6/kybra/__main__.py` & `kybra-0.5.0rc7/kybra/__main__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/build_wasm_binary_or_exit.py` & `kybra-0.5.0rc7/kybra/build_wasm_binary_or_exit.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/canisters/ledger/NOTICE` & `kybra-0.5.0rc7/kybra/canisters/ledger/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/canisters/ledger/__init__.py` & `kybra-0.5.0rc7/kybra/canisters/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/canisters/management/__init__.py` & `kybra-0.5.0rc7/kybra/canisters/management/__init__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/canisters/management/basic.py` & `kybra-0.5.0rc7/kybra/canisters/management/basic.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/canisters/management/bitcoin.py` & `kybra-0.5.0rc7/kybra/canisters/management/bitcoin.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/canisters/management/http.py` & `kybra-0.5.0rc7/kybra/canisters/management/http.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/canisters/management/tecdsa.py` & `kybra-0.5.0rc7/kybra/canisters/management/tecdsa.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/cargotoml.py` & `kybra-0.5.0rc7/kybra/cargotoml.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc` & `kybra-0.5.0rc7/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul 12 16:29:42 2023 UTC, .py size: 4555 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f6d4 ae64 cb11 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 d246 b064 cb11 0000  o........F.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6404 5a08 6405 5a09 6406  m.Z...d.Z.d.Z.d.
 00000070: 5a0a 4700 6407 6408 8400 6408 6505 8303  Z.G.d.d...d.e...
```

### Comparing `kybra-0.5.0rc6/kybra/compiler/custom_modules/principal.py` & `kybra-0.5.0rc7/kybra/compiler/custom_modules/principal.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/install_rust_dependencies.sh` & `kybra-0.5.0rc7/kybra/compiler/install_rust_dependencies.sh`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_deployer/src/errors.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_deployer/src/errors.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_deployer/src/lib.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_deployer/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,27 @@
     ARG_DATA_RAW_REF_CELL.with(|arg_data_raw_ref_cell| {
         let mut arg_data_ref_mut = arg_data_raw_ref_cell.borrow_mut();
         *arg_data_ref_mut = call::arg_data_raw();
     });
 }
 
 #[update(guard = "controller_guard")]
+pub fn clear_chunks() {
+    WASM_REF_CELL.with(|wasm_ref_cell| {
+        let mut wasm_ref_mut = wasm_ref_cell.borrow_mut();
+        wasm_ref_mut.clear();
+    });
+
+    PYTHON_STDLIB_REF_CELL.with(|python_stdlib_ref_cell| {
+        let mut python_stdlib_ref_mut = python_stdlib_ref_cell.borrow_mut();
+        python_stdlib_ref_mut.clear();
+    });
+}
+
+#[update(guard = "controller_guard")]
 pub fn upload_wasm_chunk(bytes: Vec<u8>) {
     WASM_REF_CELL.with(|wasm_ref_cell| {
         let mut wasm_ref_mut = wasm_ref_cell.borrow_mut();
         wasm_ref_mut.extend(bytes);
     });
 }
 
@@ -83,19 +96,14 @@
 pub async fn install_wasm() -> Result<(), String> {
     stable_store_randomness().await?;
     stable_store_python_stdlib()?;
     install_code().map_err(|err| rejection_code_to_string(&err))
 
     // let wasm_module = WASM_REF_CELL.with(|wasm_ref_cell| wasm_ref_cell.borrow().clone());
 
-    // WASM_REF_CELL.with(|wasm_ref_cell| {
-    //     let mut wasm_ref_mut = wasm_ref_cell.borrow_mut();
-    //     wasm_ref_mut.clear();
-    // });
-
     // let result = ic_cdk::api::management_canister::main::install_code(
     //     ic_cdk::api::management_canister::main::InstallCodeArgument {
     //         mode: ic_cdk::api::management_canister::main::CanisterInstallMode::Upgrade,
     //         canister_id: ic_cdk::api::id(),
     //         wasm_module,
     //         arg: ARG_DATA_RAW_REF_CELL
     //             .with(|arg_data_raw_ref_cell| arg_data_raw_ref_cell.borrow().clone()),
@@ -140,19 +148,14 @@
 
     Ok(())
 }
 
 fn install_code() -> Result<(), ic_cdk::api::call::RejectionCode> {
     let wasm_module = WASM_REF_CELL.with(|wasm_ref_cell| wasm_ref_cell.borrow().clone());
 
-    WASM_REF_CELL.with(|wasm_ref_cell| {
-        let mut wasm_ref_mut = wasm_ref_cell.borrow_mut();
-        wasm_ref_mut.clear();
-    });
-
     let result = call::notify(
         Principal::management_canister(),
         "install_code",
         (management_canister::main::InstallCodeArgument {
             mode: management_canister::main::CanisterInstallMode::Upgrade,
             canister_id: ic_cdk::api::id(),
             wasm_module,
```

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/Cargo.toml` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/async_result_handler.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/async_result_handler.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/body/utils.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/body/utils.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/array.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/array.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/opt.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/opt.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/primitive.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/primitive.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/canister_method/rust.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/canister_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/constants.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/constants.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/analyze.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/analyze.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/display_string.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/display_string.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/test_error.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/test_error.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/debug/what_is_it.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/debug/what_is_it.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/errors/collect_results.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/errors/collect_results.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/errors/compiler_output.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/errors/compiler_output.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/errors/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/errors/unreachable.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/errors/unreachable.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/get_child_class_of.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/get_child_class_of.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/get_name.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/get_name.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/guard_function/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/guard_function/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/header/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/header/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/header/ref_cells.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/header/ref_cells.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/header/traits.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/header/traits.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/header/use_statements.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/header/use_statements.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/ic_object/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/ic_object/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/lib.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/main.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/main.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/params.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/params.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/method_utils/returns.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/method_utils/returns.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/py_ast/to_act.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/py_ast/to_act.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/source_map/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/source_map/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_post_install/Cargo.toml` & `kybra-0.5.0rc7/kybra/compiler/kybra_post_install/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_post_install/build.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_post_install/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/dfx.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/dfx.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/generate_candid.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/generate_candid.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/install_app_canister.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/install_app_canister.rs`

 * *Files 13% similar despite different names*

```diff
@@ -44,30 +44,35 @@
 
     check_for_interpreter(canister_name)?;
 
     Ok(())
 }
 
 fn check_for_interpreter(canister_name: &str) -> Result<(), String> {
+    let err_message = "The RustPython interpreter could not be initialized. init or post_upgrade has most likely trapped. Check your local replica logs if available".to_string();
+
     let does_interpreter_exist_output = dfx(
         "canister",
         "call",
         &vec![canister_name, "does_interpreter_exist"],
     )?;
 
     if !does_interpreter_exist_output.status.success() {
-        return Err(create_error_string(&String::from_utf8_lossy(
-            &does_interpreter_exist_output.stderr,
-        )));
+        println!(
+            "{}",
+            String::from_utf8_lossy(&does_interpreter_exist_output.stderr,)
+        );
+
+        return Err(err_message);
     }
 
     let does_interpreter_exist = String::from_utf8_lossy(&does_interpreter_exist_output.stdout)
         .to_string()
         .trim()
         == "(true)";
 
     if does_interpreter_exist == false {
-        return Err("The RustPython interpreter could not be initialized. init or post_upgrade has most likely trapped. Check your local replica logs if available".to_string());
+        return Err(err_message);
     }
 
     Ok(())
 }
```

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/main.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/main.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-// TODO share with DFINITY how I'm doing this, maybe they can build that into dfx to overcome some of the Wasm binary limitations temporarily
-// TODO a future version of dfx should take care of all of this chunk uploading for us
-use std::{thread, time::Duration};
-
+use clear_chunks::clear_chunks;
 use error::create_error_string;
 use generate_candid::generate_candid;
 use install_app_canister::install_app_canister;
 use upload_app_canister::upload_app_canister;
 use upload_python_stdlib::upload_python_stdlib;
 
+mod clear_chunks;
 mod dfx;
 mod error;
 mod generate_candid;
 mod install_app_canister;
 mod permissions;
 mod upload_app_canister;
 mod upload_chunk;
@@ -25,14 +23,15 @@
         .get(1)
         .ok_or(create_error_string("Canister name argument not present"))?;
     let candid_path = args
         .get(2)
         .ok_or(create_error_string("Candid path argument not present"))?;
     let max_chunk_size = 2 * 1_000 * 1_000; // 2 MB message size limit currently on the Internet Computer
 
+    clear_chunks(canister_name)?;
     upload_app_canister(canister_name, max_chunk_size)?;
     upload_python_stdlib(canister_name, max_chunk_size)?;
     install_app_canister(canister_name)?;
     generate_candid(canister_name, candid_path)?;
 
     Ok(())
 }
```

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/permissions.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/permissions.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/upload_app_canister.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/upload_app_canister.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/upload_chunk.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/upload_chunk.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/compiler/kybra_vm_value_derive/src/lib.rs` & `kybra-0.5.0rc7/kybra/compiler/kybra_vm_value_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/module_bundler.py` & `kybra-0.5.0rc7/kybra/module_bundler.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/run_kybra_generate_or_exit.py` & `kybra-0.5.0rc7/kybra/run_kybra_generate_or_exit.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/timed.py` & `kybra-0.5.0rc7/kybra/timed.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra/types.py` & `kybra-0.5.0rc7/kybra/types.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc6/kybra.egg-info/PKG-INFO` & `kybra-0.5.0rc7/kybra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kybra
-Version: 0.5.0rc6
+Version: 0.5.0rc7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 <div align="center">
     <a href="https://github.com/demergent-labs/kybra" target="_blank" rel="noopener noreferrer">
         <img height="150" src="https://raw.githubusercontent.com/demergent-labs/kybra/main/logo/logo.svg" alt="kybra logo">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kybra Version: 0.5.0rc6 Description-Content-Type:
+Metadata-Version: 2.1 Name: kybra Version: 0.5.0rc7 Description-Content-Type:
 text/markdown License-File: LICENSE License-File: NOTICE
                                  [kybra_logo]
                        [Coverage_Status] [PyPI_version]
 # Kybra (Beta) Python CDK for the [Internet Computer](https://
 internetcomputer.org/). ## Disclaimer Things to keep in mind: - Kybra does not
 yet have many live, successful, continuously operating applications deployed to
 the IC - Kybra does not yet have extensive automated property tests - Kybra
```

### Comparing `kybra-0.5.0rc6/kybra.egg-info/SOURCES.txt` & `kybra-0.5.0rc7/kybra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -234,14 +234,15 @@
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
 kybra/compiler/kybra_post_install/Cargo.toml
 kybra/compiler/kybra_post_install/build.rs
+kybra/compiler/kybra_post_install/src/clear_chunks.rs
 kybra/compiler/kybra_post_install/src/dfx.rs
 kybra/compiler/kybra_post_install/src/error.rs
 kybra/compiler/kybra_post_install/src/generate_candid.rs
 kybra/compiler/kybra_post_install/src/install_app_canister.rs
 kybra/compiler/kybra_post_install/src/main.rs
 kybra/compiler/kybra_post_install/src/permissions.rs
 kybra/compiler/kybra_post_install/src/upload_app_canister.rs
```

