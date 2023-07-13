# Comparing `tmp/chia_rs-0.2.8.tar.gz` & `tmp/chia_rs-0.2.9.tar.gz`

## Comparing `chia_rs-0.2.8.tar` & `chia_rs-0.2.9.tar`

### file list

```diff
@@ -1,138 +1,140 @@
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 chia_rs-0.2.8/local_dependencies/clvm-utils/Cargo.toml
--rw-r--r--   0     1001      123      155 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/clvm-utils/README.md
--rw-r--r--   0     1001      123       36 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/clvm-utils/src/lib.rs
--rw-r--r--   0     1001      123     2914 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/clvm-utils/src/tree_hash.rs
--rw-r--r--   0     1001      123     6491 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/clvm-utils/src/uncurry.rs
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 chia_rs-0.2.8/local_dependencies/chia/Cargo.toml
--rw-r--r--   0     1001      123      224 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.cargo/config
--rw-r--r--   0     1001      123      290 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.github/workflows/audit-check.yml
--rw-r--r--   0     1001      123     3050 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.github/workflows/benchmark.yml
--rw-r--r--   0     1001      123     2843 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml
--rw-r--r--   0     1001      123    15546 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.github/workflows/build-test.yml
--rw-r--r--   0     1001      123       19 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.gitignore
--rw-r--r--   0     1001      123    11357 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/LICENSE
--rw-r--r--   0     1001      123      192 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/README.md
--rw-r--r--   0     1001      123      142 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/cl/README.md
--rw-r--r--   0     1001      123     4603 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/cl/deserialize_w_backrefs.cl
--rw-r--r--   0     1001      123     4474 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/docs/implementation-notes.md
--rw-r--r--   0     1001      123      882 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/examples/README.md
--rw-r--r--   0     1001      123    48843 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/examples/block-1519806.bin
--rw-r--r--   0     1001      123      299 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/examples/dump.py
--rw-r--r--   0     1001      123     1592 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/examples/streaming-patch.diff
--rw-r--r--   0     1001      123     2184 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/assert-puzzle-announce-fail.txt
--rw-r--r--   0     1001      123    12107 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834752-compressed.txt
--rw-r--r--   0     1001      123    28444 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834752.txt
--rw-r--r--   0     1001      123   132615 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834760.txt
--rw-r--r--   0     1001      123    26930 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834761.txt
--rw-r--r--   0     1001      123    74748 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834765.txt
--rw-r--r--   0     1001      123   124696 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834766.txt
--rw-r--r--   0     1001      123   104382 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834768.txt
--rw-r--r--   0     1001      123      665 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-different-amounts.txt
--rw-r--r--   0     1001      123      425 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-hint-duplicate-outputs.txt
--rw-r--r--   0     1001      123      808 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-hint.txt
--rw-r--r--   0     1001      123      832 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-hint2.txt
--rw-r--r--   0     1001      123      554 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/deep-recursion-plus.txt
--rw-r--r--   0     1001      123      413 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/double-spend.txt
--rw-r--r--   0     1001      123      631 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-coin-announce.txt
--rw-r--r--   0     1001      123      405 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-create-coin.txt
--rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute-div.txt
--rw-r--r--   0     1001      123      601 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute-substr-tail.txt
--rw-r--r--   0     1001      123      589 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute-substr.txt
--rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute.txt
--rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-relative.txt
--rw-r--r--   0     1001      123      281 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-outputs.txt
--rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-reserve-fee.txt
--rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-seconds-absolute.txt
--rw-r--r--   0     1001      123      557 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-seconds-relative.txt
--rw-r--r--   0     1001      123      546 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/height-absolute-ladder.txt
--rw-r--r--   0     1001      123      171 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/infinite-recursion1.txt
--rw-r--r--   0     1001      123      155 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/infinite-recursion2.txt
--rw-r--r--   0     1001      123     1431 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/infinite-recursion3.txt
--rw-r--r--   0     1001      123      219 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/infinite-recursion4.txt
--rw-r--r--   0     1001      123      110 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/invalid-conditions.txt
--rw-r--r--   0     1001      123     2380 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/just-puzzle-announce.txt
--rw-r--r--   0     1001      123   590784 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/many-create-coin.txt
--rw-r--r--   0     1001      123      796 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/many-large-ints-negative.txt
--rw-r--r--   0     1001      123      612 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/many-large-ints.txt
--rw-r--r--   0     1001      123      559 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/max-height.txt
--rw-r--r--   0     1001      123      373 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/multiple-reserve-fee.txt
--rw-r--r--   0     1001      123      598 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/negative-reserve-fee.txt
--rw-r--r--   0     1001      123      273 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/recursion-pairs.txt
--rw-r--r--   0     1001      123      367 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/unknown-condition.txt
--rw-r--r--   0     1001      123       93 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/mypy.ini
--rw-r--r--   0     1001      123      412 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/allocator.rs
--rw-r--r--   0     1001      123     1713 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/compression/compressor.rs
--rw-r--r--   0     1001      123      858 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin
--rw-r--r--   0     1001      123       20 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/compression/mod.rs
--rw-r--r--   0     1001      123     3120 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/fuzzing_utils.rs
--rw-r--r--   0     1001      123     3042 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/coin_id.rs
--rw-r--r--   0     1001      123     4493 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/condition_sanitizers.rs
--rw-r--r--   0     1001      123   140900 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/conditions.rs
--rw-r--r--   0     1001      123     2233 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/flags.rs
--rw-r--r--   0     1001      123     6447 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs
--rw-r--r--   0     1001      123      256 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/mod.rs
--rw-r--r--   0     1001      123    10135 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/opcodes.rs
--rw-r--r--   0     1001      123     2650 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/run_block_generator.rs
--rw-r--r--   0     1001      123     2352 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/run_puzzle.rs
--rw-r--r--   0     1001      123     2916 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/sanitize_int.rs
--rw-r--r--   0     1001      123     7440 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/test_generators.rs
--rw-r--r--   0     1001      123     5987 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/validation_error.rs
--rw-r--r--   0     1001      123     1990 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/generator_rom.rs
--rw-r--r--   0     1001      123      136 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/lib.rs
--rw-r--r--   0     1001      123    22862 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/merkle_set.rs
--rwxr-xr-x   0     1001      123     8264 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/generate-programs.py
--rwxr-xr-x   0     1001      123     3042 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/run-programs.py
--rwxr-xr-x   0     1001      123     1569 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/run.py
--rwxr-xr-x   0     1001      123     3563 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/run_gen.py
--rwxr-xr-x   0     1001      123     3014 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test-generators.py
--rw-r--r--   0     1001      123    11060 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test_coin.py
--rw-r--r--   0     1001      123      803 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test_run_block_generator.py
--rw-r--r--   0     1001      123     5587 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test_run_puzzle.py
--rw-r--r--   0     1001      123    10725 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test_streamable.py
--rw-r--r--   0     1001      123     1050 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test_tree_hash.py
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/Cargo.toml
--rw-r--r--   0     1001      123      722 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/bls.rs
--rw-r--r--   0     1001      123     5474 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/bytes.rs
--rw-r--r--   0     1001      123     1386 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/chia_error.rs
--rw-r--r--   0     1001      123     4701 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/chia_protocol.rs
--rw-r--r--   0     1001      123      862 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/classgroup.rs
--rw-r--r--   0     1001      123     1809 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin.rs
--rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin_spend.rs
--rw-r--r--   0     1001      123      540 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin_state.rs
--rw-r--r--   0     1001      123      743 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs
--rw-r--r--   0     1001      123      871 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/fee_estimate.rs
--rw-r--r--   0     1001      123     2316 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/foliage.rs
--rw-r--r--   0     1001      123     3679 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/from_json_dict.rs
--rw-r--r--   0     1001      123     1497 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/fullblock.rs
--rw-r--r--   0     1001      123     1388 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/header_block.rs
--rw-r--r--   0     1001      123     1288 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/lib.rs
--rw-r--r--   0     1001      123      810 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/message_struct.rs
--rw-r--r--   0     1001      123      540 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/pool_target.rs
--rw-r--r--   0     1001      123     1624 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/program.rs
--rw-r--r--   0     1001      123      679 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/proof_of_space.rs
--rw-r--r--   0     1001      123     1527 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/reward_chain_block.rs
--rw-r--r--   0     1001      123     1788 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/slots.rs
--rw-r--r--   0     1001      123      569 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/spend_bundle.rs
--rw-r--r--   0     1001      123    20212 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/streamable.rs
--rw-r--r--   0     1001      123     2217 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/to_json_dict.rs
--rw-r--r--   0     1001      123      679 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/vdf.rs
--rw-r--r--   0     1001      123     4016 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/wallet_protocol.rs
--rw-r--r--   0     1001      123     1225 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/weight_proof.rs
--rw-r--r--   0        0        0      458 1970-01-01 00:00:00.000000 chia_rs-0.2.8/local_dependencies/chia_py_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      123     9330 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia_py_streamable_macro/src/lib.rs
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 chia_rs-0.2.8/local_dependencies/chia_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      123     4715 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia_streamable_macro/src/lib.rs
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 chia_rs-0.2.8/Cargo.toml
--rw-r--r--   0     1001      123       77 2023-06-21 16:36:00.000000 chia_rs-0.2.8/README.md
--rw-r--r--   0     1001      123    68548 2023-06-21 16:36:00.000000 chia_rs-0.2.8/chia_rs.pyi
--rw-r--r--   0     1001      123     7645 2023-06-21 16:36:00.000000 chia_rs-0.2.8/generate_type_stubs.py
--rw-r--r--   0     1001      123        0 2023-06-21 16:36:00.000000 chia_rs-0.2.8/py.typed
--rw-r--r--   0     1001      123      112 2023-06-21 16:36:00.000000 chia_rs-0.2.8/pyproject.toml
--rw-r--r--   0     1001      123      559 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/adapt_response.rs
--rw-r--r--   0     1001      123     9671 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/api.rs
--rw-r--r--   0     1001      123      641 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/compression.rs
--rw-r--r--   0     1001      123      175 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/lib.rs
--rw-r--r--   0     1001      123     6961 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/run_generator.rs
--rw-r--r--   0     1001      123     2843 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/run_program.rs
--rw-r--r--   0     1001      123    22607 2023-06-21 16:36:09.000000 chia_rs-0.2.8/Cargo.lock
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 chia_rs-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 chia_rs-0.2.9/local_dependencies/chia_py_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      123     9135 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia_py_streamable_macro/src/lib.rs
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 chia_rs-0.2.9/local_dependencies/chia/Cargo.toml
+-rw-r--r--   0     1001      123      224 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/.cargo/config
+-rw-r--r--   0     1001      123      290 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/.github/workflows/audit-check.yml
+-rw-r--r--   0     1001      123     3029 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/.github/workflows/benchmark.yml
+-rw-r--r--   0     1001      123     2843 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml
+-rw-r--r--   0     1001      123    15498 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/.github/workflows/build-test.yml
+-rw-r--r--   0     1001      123        8 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/LICENSE
+-rw-r--r--   0     1001      123      192 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/README.md
+-rw-r--r--   0     1001      123      142 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/cl/README.md
+-rw-r--r--   0     1001      123     4603 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/cl/deserialize_w_backrefs.cl
+-rw-r--r--   0     1001      123     4474 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/docs/implementation-notes.md
+-rw-r--r--   0     1001      123      882 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/examples/README.md
+-rw-r--r--   0     1001      123    48843 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/examples/block-1519806.bin
+-rw-r--r--   0     1001      123      299 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/examples/dump.py
+-rw-r--r--   0     1001      123     1592 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/examples/streaming-patch.diff
+-rw-r--r--   0     1001      123     2184 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/assert-puzzle-announce-fail.txt
+-rw-r--r--   0     1001      123   468780 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-225758.env
+-rw-r--r--   0     1001      123     8068 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-225758.txt
+-rw-r--r--   0     1001      123    12107 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834752-compressed.txt
+-rw-r--r--   0     1001      123    28444 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834752.txt
+-rw-r--r--   0     1001      123   132615 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834760.txt
+-rw-r--r--   0     1001      123    26930 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834761.txt
+-rw-r--r--   0     1001      123    74748 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834765.txt
+-rw-r--r--   0     1001      123   124696 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834766.txt
+-rw-r--r--   0     1001      123   104382 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834768.txt
+-rw-r--r--   0     1001      123      665 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/create-coin-different-amounts.txt
+-rw-r--r--   0     1001      123      425 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/create-coin-hint-duplicate-outputs.txt
+-rw-r--r--   0     1001      123      808 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/create-coin-hint.txt
+-rw-r--r--   0     1001      123      832 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/create-coin-hint2.txt
+-rw-r--r--   0     1001      123      554 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/deep-recursion-plus.txt
+-rw-r--r--   0     1001      123      413 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/double-spend.txt
+-rw-r--r--   0     1001      123      631 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-coin-announce.txt
+-rw-r--r--   0     1001      123      405 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-create-coin.txt
+-rw-r--r--   0     1001      123      556 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-height-absolute-div.txt
+-rw-r--r--   0     1001      123      601 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-height-absolute-substr-tail.txt
+-rw-r--r--   0     1001      123      589 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-height-absolute-substr.txt
+-rw-r--r--   0     1001      123      556 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-height-absolute.txt
+-rw-r--r--   0     1001      123      556 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-height-relative.txt
+-rw-r--r--   0     1001      123      281 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-outputs.txt
+-rw-r--r--   0     1001      123      556 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-reserve-fee.txt
+-rw-r--r--   0     1001      123      556 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-seconds-absolute.txt
+-rw-r--r--   0     1001      123      557 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-seconds-relative.txt
+-rw-r--r--   0     1001      123      546 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/height-absolute-ladder.txt
+-rw-r--r--   0     1001      123      171 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/infinite-recursion1.txt
+-rw-r--r--   0     1001      123      155 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/infinite-recursion2.txt
+-rw-r--r--   0     1001      123     1431 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/infinite-recursion3.txt
+-rw-r--r--   0     1001      123      219 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/infinite-recursion4.txt
+-rw-r--r--   0     1001      123      110 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/invalid-conditions.txt
+-rw-r--r--   0     1001      123     2380 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/just-puzzle-announce.txt
+-rw-r--r--   0     1001      123   590784 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/many-create-coin.txt
+-rw-r--r--   0     1001      123      796 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/many-large-ints-negative.txt
+-rw-r--r--   0     1001      123      612 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/many-large-ints.txt
+-rw-r--r--   0     1001      123      559 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/max-height.txt
+-rw-r--r--   0     1001      123      373 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/multiple-reserve-fee.txt
+-rw-r--r--   0     1001      123      598 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/negative-reserve-fee.txt
+-rw-r--r--   0     1001      123      273 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/recursion-pairs.txt
+-rw-r--r--   0     1001      123      367 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/generator-tests/unknown-condition.txt
+-rw-r--r--   0     1001      123       93 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/mypy.ini
+-rw-r--r--   0     1001      123      412 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/allocator.rs
+-rw-r--r--   0     1001      123     1713 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/compression/compressor.rs
+-rw-r--r--   0     1001      123      858 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin
+-rw-r--r--   0     1001      123       20 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/compression/mod.rs
+-rw-r--r--   0     1001      123     3042 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/coin_id.rs
+-rw-r--r--   0     1001      123     4493 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/condition_sanitizers.rs
+-rw-r--r--   0     1001      123   148111 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/conditions.rs
+-rw-r--r--   0     1001      123     2233 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/flags.rs
+-rw-r--r--   0     1001      123     6447 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs
+-rw-r--r--   0     1001      123      284 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/mod.rs
+-rw-r--r--   0     1001      123    11245 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/opcodes.rs
+-rw-r--r--   0     1001      123     6368 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/run_block_generator.rs
+-rw-r--r--   0     1001      123     2589 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/run_puzzle.rs
+-rw-r--r--   0     1001      123     2916 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/sanitize_int.rs
+-rw-r--r--   0     1001      123    10954 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/solution_generator.rs
+-rw-r--r--   0     1001      123     8729 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/test_generators.rs
+-rw-r--r--   0     1001      123     5987 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/gen/validation_error.rs
+-rw-r--r--   0     1001      123     3133 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/generator_rom.rs
+-rw-r--r--   0     1001      123       96 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/lib.rs
+-rw-r--r--   0     1001      123    22862 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/src/merkle_set.rs
+-rwxr-xr-x   0     1001      123     8264 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/tests/generate-programs.py
+-rwxr-xr-x   0     1001      123     3042 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/tests/run-programs.py
+-rwxr-xr-x   0     1001      123     1569 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/tests/run.py
+-rwxr-xr-x   0     1001      123     4015 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/tests/run_gen.py
+-rwxr-xr-x   0     1001      123     4076 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/tests/test-generators.py
+-rw-r--r--   0     1001      123    11060 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/tests/test_coin.py
+-rw-r--r--   0     1001      123     1947 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/tests/test_run_block_generator.py
+-rw-r--r--   0     1001      123     5587 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/tests/test_run_puzzle.py
+-rw-r--r--   0     1001      123    13320 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/tests/test_streamable.py
+-rw-r--r--   0     1001      123     1050 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia/tests/test_tree_hash.py
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/Cargo.toml
+-rw-r--r--   0     1001      123      738 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/bls.rs
+-rw-r--r--   0     1001      123    11675 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/bytes.rs
+-rw-r--r--   0     1001      123     1386 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/chia_error.rs
+-rw-r--r--   0     1001      123     4701 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/chia_protocol.rs
+-rw-r--r--   0     1001      123      862 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/classgroup.rs
+-rw-r--r--   0     1001      123     3337 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/coin.rs
+-rw-r--r--   0     1001      123      556 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/coin_spend.rs
+-rw-r--r--   0     1001      123      540 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/coin_state.rs
+-rw-r--r--   0     1001      123      743 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs
+-rw-r--r--   0     1001      123      871 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/fee_estimate.rs
+-rw-r--r--   0     1001      123     2316 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/foliage.rs
+-rw-r--r--   0     1001      123     3682 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/from_json_dict.rs
+-rw-r--r--   0     1001      123     1497 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/fullblock.rs
+-rw-r--r--   0     1001      123     1388 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/header_block.rs
+-rw-r--r--   0     1001      123     1288 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/lib.rs
+-rw-r--r--   0     1001      123     1300 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/message_struct.rs
+-rw-r--r--   0     1001      123      540 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/pool_target.rs
+-rw-r--r--   0     1001      123     1624 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/program.rs
+-rw-r--r--   0     1001      123      679 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/proof_of_space.rs
+-rw-r--r--   0     1001      123     1527 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/reward_chain_block.rs
+-rw-r--r--   0     1001      123     1788 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/slots.rs
+-rw-r--r--   0     1001      123      569 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/spend_bundle.rs
+-rw-r--r--   0     1001      123    20212 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/streamable.rs
+-rw-r--r--   0     1001      123     2217 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/to_json_dict.rs
+-rw-r--r--   0     1001      123      679 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/vdf.rs
+-rw-r--r--   0     1001      123     4016 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/wallet_protocol.rs
+-rw-r--r--   0     1001      123     1225 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia-protocol/src/weight_proof.rs
+-rw-r--r--   0        0        0      363 1970-01-01 00:00:00.000000 chia_rs-0.2.9/local_dependencies/clvm-utils/Cargo.toml
+-rw-r--r--   0     1001      123      155 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/clvm-utils/README.md
+-rw-r--r--   0     1001      123       36 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/clvm-utils/src/lib.rs
+-rw-r--r--   0     1001      123     2908 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/clvm-utils/src/tree_hash.rs
+-rw-r--r--   0     1001      123     6491 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/clvm-utils/src/uncurry.rs
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 chia_rs-0.2.9/local_dependencies/chia_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      123     4715 2023-07-13 18:47:30.000000 chia_rs-0.2.9/local_dependencies/chia_streamable_macro/src/lib.rs
+-rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 chia_rs-0.2.9/Cargo.toml
+-rw-r--r--   0     1001      123       77 2023-07-13 18:47:30.000000 chia_rs-0.2.9/README.md
+-rw-r--r--   0     1001      123    69540 2023-07-13 18:47:30.000000 chia_rs-0.2.9/chia_rs.pyi
+-rw-r--r--   0     1001      123     8322 2023-07-13 18:47:30.000000 chia_rs-0.2.9/generate_type_stubs.py
+-rw-r--r--   0     1001      123        0 2023-07-13 18:47:30.000000 chia_rs-0.2.9/py.typed
+-rw-r--r--   0     1001      123      112 2023-07-13 18:47:30.000000 chia_rs-0.2.9/pyproject.toml
+-rw-r--r--   0     1001      123      559 2023-07-13 18:47:30.000000 chia_rs-0.2.9/src/adapt_response.rs
+-rw-r--r--   0     1001      123    11348 2023-07-13 18:47:30.000000 chia_rs-0.2.9/src/api.rs
+-rw-r--r--   0     1001      123      641 2023-07-13 18:47:30.000000 chia_rs-0.2.9/src/compression.rs
+-rw-r--r--   0     1001      123      175 2023-07-13 18:47:30.000000 chia_rs-0.2.9/src/lib.rs
+-rw-r--r--   0     1001      123     7863 2023-07-13 18:47:30.000000 chia_rs-0.2.9/src/run_generator.rs
+-rw-r--r--   0     1001      123     3092 2023-07-13 18:47:30.000000 chia_rs-0.2.9/src/run_program.rs
+-rw-r--r--   0     1001      123    22358 2023-07-13 18:47:35.000000 chia_rs-0.2.9/Cargo.lock
+-rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 chia_rs-0.2.9/PKG-INFO
```

### Comparing `chia_rs-0.2.8/local_dependencies/clvm-utils/src/tree_hash.rs` & `chia_rs-0.2.9/local_dependencies/clvm-utils/src/tree_hash.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     Cons,
 }
 
 pub fn tree_hash(a: &Allocator, node: NodePtr) -> [u8; 32] {
     let mut hashes: Vec<[u8; 32]> = vec![];
     let mut ops = vec![TreeOp::SExp(node)];
 
-    while !ops.is_empty() {
-        match ops.pop().unwrap() {
+    while let Some(op) = ops.pop() {
+        match op {
             TreeOp::SExp(node) => match a.sexp(node) {
                 SExp::Atom() => {
                     let mut sha256 = Sha256::new();
                     sha256.update([1_u8]);
                     sha256.update(a.atom(node));
-                    hashes.push(sha256.finalize().into())
+                    hashes.push(sha256.finalize().into());
                 }
                 SExp::Pair(left, right) => {
                     ops.push(TreeOp::Cons);
                     ops.push(TreeOp::SExp(left));
                     ops.push(TreeOp::SExp(right));
                 }
             },
```

### Comparing `chia_rs-0.2.8/local_dependencies/clvm-utils/src/uncurry.rs` & `chia_rs-0.2.9/local_dependencies/clvm-utils/src/uncurry.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/Cargo.toml` & `chia_rs-0.2.9/local_dependencies/chia/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # the "wheel" crate is excluded from the workspace because pyo3 has problems with
 # "cargo test" and "cargo bench"
 [workspace]
-members = ["wasm", "chia_streamable_macro", "chia-bls", "clvm-utils", "chia-protocol", "chia_py_streamable_macro", "chia-tools"]
+members = ["wasm", "chia_streamable_macro", "chia-bls", "clvm-utils", "chia-protocol", "chia_py_streamable_macro", "chia-tools", "fuzz", "clvm-utils/fuzz"]
 exclude = ["wheel"]
 
 [package]
 name = "chia"
-version = "0.2.8"
+version = "0.2.9"
 edition = "2021"
 license = "Apache-2.0"
 description = "Utility functions and types used by the Chia blockchain full node"
 authors = ["Richard Kiss <him@richardkiss.com>", "Arvid Norberg <arvid@chia.net>"]
 homepage = "https://github.com/Chia-Network/chia_rs/"
 repository = "https://github.com/Chia-Network/chia_rs/"
 
 [features]
 py-bindings = ["dep:pyo3"]
 
 [dependencies]
-clvmr = "=0.2.6"
+clvmr = "=0.2.7"
 hex = "=0.4.3"
-pyo3 = { version = "=0.15.1", features = ["extension-module"], optional = true }
+pyo3 = { version = ">=0.19.0", features = ["extension-module"], optional = true }
 clvm-utils = { version = "=0.2.7", path = "../clvm-utils" }
 chia-protocol = { version = "=0.2.7", path = "../chia-protocol" }
 hex-literal = "=0.4.1"
 
 [lib]
 name = "chia"
 crate-type = ["rlib"]
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia/.github/workflows/benchmark.yml` & `chia_rs-0.2.9/local_dependencies/chia/.github/workflows/benchmark.yml`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
   generator-benchmarks:
     name: Generator performance
     runs-on: benchmark
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 1
 
     - uses: chia-network/actions/setup-python@main
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml` & `chia_rs-0.2.9/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/.github/workflows/build-test.yml` & `chia_rs-0.2.9/local_dependencies/chia/.github/workflows/build-test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -39,67 +39,67 @@
               intel: [windows-latest]
         python:
           - major-dot-minor: '3.7'
             cibw-build: 'cp37-*'
             by-arch:
               arm:
                 manylinux-version: 2014
-                docker-url: quay.io/pypa/manylinux2014_aarch64
+                docker-url: ghcr.io/chia-network/build-images/centos-pypa-rust-aarch64
                 rustup-target: aarch64-unknown-linux-musl
               intel:
                 manylinux-version: 2014
-                docker-url: quay.io/pypa/manylinux2014_x86_64
+                docker-url: ghcr.io/chia-network/build-images/centos-pypa-rust-x86_64
                 rustup-target: x86_64-unknown-linux-musl
             matrix: '3.7'
           - major-dot-minor: '3.8'
             cibw-build: 'cp38-*'
             by-arch:
               arm:
                 manylinux-version: 2014
-                docker-url: quay.io/pypa/manylinux2014_aarch64
+                docker-url: ghcr.io/chia-network/build-images/centos-pypa-rust-aarch64
                 rustup-target: aarch64-unknown-linux-musl
               intel:
                 manylinux-version: 2014
-                docker-url: quay.io/pypa/manylinux2014_x86_64
+                docker-url: ghcr.io/chia-network/build-images/centos-pypa-rust-x86_64
                 rustup-target: x86_64-unknown-linux-musl
             matrix: '3.8'
           - major-dot-minor: '3.9'
             cibw-build: 'cp39-*'
             by-arch:
               arm:
                 manylinux-version: 2014
-                docker-url: quay.io/pypa/manylinux2014_aarch64
+                docker-url: ghcr.io/chia-network/build-images/centos-pypa-rust-aarch64
                 rustup-target: aarch64-unknown-linux-musl
               intel:
                 manylinux-version: 2014
-                docker-url: quay.io/pypa/manylinux2014_x86_64
+                docker-url: ghcr.io/chia-network/build-images/centos-pypa-rust-x86_64
                 rustup-target: x86_64-unknown-linux-musl
             matrix: '3.9'
           - major-dot-minor: '3.10'
             cibw-build: 'cp310-*'
             by-arch:
               arm:
                 manylinux-version: 2014
-                docker-url: quay.io/pypa/manylinux2014_aarch64
+                docker-url: ghcr.io/chia-network/build-images/centos-pypa-rust-aarch64
                 rustup-target: aarch64-unknown-linux-musl
               intel:
                 manylinux-version: 2014
-                docker-url: quay.io/pypa/manylinux2014_x86_64
+                docker-url: ghcr.io/chia-network/build-images/centos-pypa-rust-x86_64
                 rustup-target: x86_64-unknown-linux-musl
             matrix: '3.10'
           - major-dot-minor: '3.11'
             cibw-build: 'cp311-*'
             by-arch:
               arm:
                 manylinux-version: 2014
-                docker-url: quay.io/pypa/manylinux2014_aarch64
+                docker-url: ghcr.io/chia-network/build-images/centos-pypa-rust-aarch64
                 rustup-target: aarch64-unknown-linux-musl
               intel:
                 manylinux-version: 2014
-                docker-url: quay.io/pypa/manylinux2014_x86_64
+                docker-url: ghcr.io/chia-network/build-images/centos-pypa-rust-x86_64
                 rustup-target: x86_64-unknown-linux-musl
             matrix: '3.11'
         arch:
           - name: ARM
             matrix: arm
           - name: Intel
             matrix: intel
@@ -168,16 +168,14 @@
     - name: Build Linux with maturin on Python ${{ matrix.python }}
       if: matrix.os.matrix == 'ubuntu'
       run: |
         docker run --rm \
           -v ${{ github.workspace }}:/ws --workdir=/ws \
           ${{ matrix.python.by-arch[matrix.arch.matrix].docker-url }} \
           bash -exc '\
-            curl -L https://sh.rustup.rs > rustup-init.sh && \
-            sh rustup-init.sh -y && \
             yum -y install openssl-devel && \
             source $HOME/.cargo/env && \
             rustup target add ${{ matrix.python.by-arch[matrix.arch.matrix].rustup-target }} && \
             python${{ matrix.python.major-dot-minor }} -m venv /venv && \
             . /venv/bin/activate && \
             pip install --upgrade pip && \
             pip install maturin && \
@@ -299,16 +297,14 @@
             components: rustfmt, clippy
             override: true
       - name: fmt
         run: |
             cargo fmt --all -- --files-with-diff --check
             cd wheel
             cargo fmt -- --files-with-diff --check
-            cd ../fuzz
-            cargo fmt -- --files-with-diff --check
 
   clippy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
@@ -330,34 +326,34 @@
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
             toolchain: nightly
       - name: cargo-fuzz
         run: cargo +nightly install cargo-fuzz
       - name: cargo fuzz (chia_rs)
-        run: cargo fuzz list | xargs -I "%" sh -c "cargo +nightly fuzz run % -- -max_total_time=30 || exit 255"
+        run: cargo fuzz list | xargs -I "%" sh -c "cargo +nightly fuzz run % -- -max_total_time=20 || exit 255"
       - name: cargo fuzz (chia-bls)
         env:
           # we disable leak reports here because blspy appears to be allocating
           # memory that's not freed. It might be a false positive since python is
           # not unloaded before exiting
           LSAN_OPTIONS: detect_leaks=0
         run: |
           cd chia-bls
           python -m pip install blspy
-          cargo fuzz list | xargs -I "%" sh -c "cargo +nightly fuzz run % -- -max_total_time=3 || exit 255"
+          cargo fuzz list | xargs -I "%" sh -c "cargo +nightly fuzz run % -- -max_total_time=10 || exit 255"
       - name: cargo fuzz (clvm-utils)
         run: |
           cd clvm-utils
-          cargo fuzz list | xargs -I "%" sh -c "cargo +nightly fuzz run % -- -max_total_time=30 || exit 255"
+          cargo fuzz list | xargs -I "%" sh -c "cargo +nightly fuzz run % -- -max_total_time=20 || exit 255"
       - name: cargo fuzz (chia-protocol)
         run: |
           cd chia-protocol
           cargo +nightly fuzz build
-          cargo fuzz list | xargs -I "%" sh -c "cargo +nightly fuzz run % -- -max_total_time=30 || exit 255"
+          cargo fuzz list | xargs -I "%" sh -c "cargo +nightly fuzz run % -- -max_total_time=20 || exit 255"
 
   unit_tests:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [macos-latest, ubuntu-latest, windows-latest]
     name: Unit tests
@@ -391,18 +387,14 @@
           rustup component add llvm-tools-preview
           python -m venv venv
           source venv/bin/activate
           git clone https://github.com/Chia-Network/clvm_tools.git --branch=main --single-branch
           pip install ./clvm_tools
           pip install colorama maturin pytest
           maturin develop --release -m wheel/Cargo.toml
-          cd tests
-          python generate-programs.py
-          python run-programs.py || true
-          cd ..
           pytest tests
           grcov . --binary-path target -s . --branch --ignore-not-existing --ignore='*/.cargo/*' --ignore='tests/*' --ignore='venv/*' -o rust_cov.info
           python -c 'with open("rust_cov.info") as f: lines = [l for l in f if not (l.startswith("DA:") and int(l.split(",")[1].strip()) >= 2**63)]; open("lcov.info", "w").writelines(lines)'
       - name: Upload to Coveralls
         uses: coverallsapp/github-action@v2
         if: matrix.os == 'ubuntu-latest'
         env:
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia/LICENSE` & `chia_rs-0.2.9/local_dependencies/chia/LICENSE`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/cl/deserialize_w_backrefs.cl` & `chia_rs-0.2.9/local_dependencies/chia/cl/deserialize_w_backrefs.cl`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/docs/implementation-notes.md` & `chia_rs-0.2.9/local_dependencies/chia/docs/implementation-notes.md`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/examples/README.md` & `chia_rs-0.2.9/local_dependencies/chia/examples/README.md`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/examples/block-1519806.bin` & `chia_rs-0.2.9/local_dependencies/chia/examples/block-1519806.bin`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/examples/streaming-patch.diff` & `chia_rs-0.2.9/local_dependencies/chia/examples/streaming-patch.diff`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/assert-puzzle-announce-fail.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/assert-puzzle-announce-fail.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834752-compressed.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834752-compressed.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834752.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834752.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834760.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834760.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834761.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834761.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834765.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834765.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834766.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834766.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834768.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/block-834768.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-different-amounts.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/create-coin-different-amounts.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-hint.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/create-coin-hint.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-hint2.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/create-coin-hint2.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/deep-recursion-plus.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/deep-recursion-plus.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-coin-announce.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-coin-announce.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute-div.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-height-absolute-div.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute-substr-tail.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-height-absolute-substr-tail.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute-substr.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-height-absolute-substr.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-height-absolute.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-relative.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-height-relative.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-reserve-fee.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-reserve-fee.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-seconds-absolute.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-seconds-absolute.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-seconds-relative.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/duplicate-seconds-relative.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/height-absolute-ladder.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/height-absolute-ladder.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/infinite-recursion3.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/infinite-recursion3.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/just-puzzle-announce.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/just-puzzle-announce.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/many-create-coin.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/many-create-coin.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/many-large-ints-negative.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/many-large-ints-negative.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/many-large-ints.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/many-large-ints.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/max-height.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/max-height.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/generator-tests/negative-reserve-fee.txt` & `chia_rs-0.2.9/local_dependencies/chia/generator-tests/negative-reserve-fee.txt`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/compression/compressor.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/compression/compressor.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin` & `chia_rs-0.2.9/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/gen/coin_id.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/gen/coin_id.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/gen/condition_sanitizers.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/gen/condition_sanitizers.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/gen/conditions.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/gen/conditions.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 use super::coin_id::compute_coin_id;
 use super::condition_sanitizers::{parse_amount, sanitize_announce_msg, sanitize_hash};
 use super::opcodes::{
-    compute_unknown_condition_cost, parse_opcode, ConditionOpcode, AGG_SIG_COST, AGG_SIG_ME,
-    AGG_SIG_UNSAFE, ASSERT_BEFORE_HEIGHT_ABSOLUTE, ASSERT_BEFORE_HEIGHT_RELATIVE,
-    ASSERT_BEFORE_SECONDS_ABSOLUTE, ASSERT_BEFORE_SECONDS_RELATIVE, ASSERT_COIN_ANNOUNCEMENT,
-    ASSERT_CONCURRENT_PUZZLE, ASSERT_CONCURRENT_SPEND, ASSERT_EPHEMERAL, ASSERT_HEIGHT_ABSOLUTE,
-    ASSERT_HEIGHT_RELATIVE, ASSERT_MY_AMOUNT, ASSERT_MY_BIRTH_HEIGHT, ASSERT_MY_BIRTH_SECONDS,
-    ASSERT_MY_COIN_ID, ASSERT_MY_PARENT_ID, ASSERT_MY_PUZZLEHASH, ASSERT_PUZZLE_ANNOUNCEMENT,
-    ASSERT_SECONDS_ABSOLUTE, ASSERT_SECONDS_RELATIVE, CREATE_COIN, CREATE_COIN_ANNOUNCEMENT,
-    CREATE_COIN_COST, CREATE_PUZZLE_ANNOUNCEMENT, REMARK, RESERVE_FEE, SOFTFORK,
+    compute_unknown_condition_cost, parse_opcode, ConditionOpcode, AGG_SIG_AMOUNT, AGG_SIG_COST,
+    AGG_SIG_ME, AGG_SIG_PARENT, AGG_SIG_PARENT_AMOUNT, AGG_SIG_PARENT_PUZZLE, AGG_SIG_PUZZLE,
+    AGG_SIG_PUZZLE_AMOUNT, AGG_SIG_UNSAFE, ASSERT_BEFORE_HEIGHT_ABSOLUTE,
+    ASSERT_BEFORE_HEIGHT_RELATIVE, ASSERT_BEFORE_SECONDS_ABSOLUTE, ASSERT_BEFORE_SECONDS_RELATIVE,
+    ASSERT_COIN_ANNOUNCEMENT, ASSERT_CONCURRENT_PUZZLE, ASSERT_CONCURRENT_SPEND, ASSERT_EPHEMERAL,
+    ASSERT_HEIGHT_ABSOLUTE, ASSERT_HEIGHT_RELATIVE, ASSERT_MY_AMOUNT, ASSERT_MY_BIRTH_HEIGHT,
+    ASSERT_MY_BIRTH_SECONDS, ASSERT_MY_COIN_ID, ASSERT_MY_PARENT_ID, ASSERT_MY_PUZZLEHASH,
+    ASSERT_PUZZLE_ANNOUNCEMENT, ASSERT_SECONDS_ABSOLUTE, ASSERT_SECONDS_RELATIVE, CREATE_COIN,
+    CREATE_COIN_ANNOUNCEMENT, CREATE_COIN_COST, CREATE_PUZZLE_ANNOUNCEMENT, REMARK, RESERVE_FEE,
+    SOFTFORK,
 };
 use super::sanitize_int::{sanitize_uint, SanitizedUint};
 use super::validation_error::{first, next, rest, ErrorCode, ValidationErr};
 use crate::gen::flags::{
     AGG_SIG_ARGS, COND_ARGS_NIL, LIMIT_ANNOUNCES, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL,
     NO_UNKNOWN_CONDS, STRICT_ARGS_COUNT,
 };
@@ -55,14 +57,20 @@
 // )))
 
 #[derive(PartialEq, Hash, Eq, Debug)]
 pub enum Condition {
     // pubkey (48 bytes) and message (<= 1024 bytes)
     AggSigUnsafe(NodePtr, NodePtr),
     AggSigMe(NodePtr, NodePtr),
+    AggSigParent(NodePtr, NodePtr),
+    AggSigPuzzle(NodePtr, NodePtr),
+    AggSigAmount(NodePtr, NodePtr),
+    AggSigPuzzleAmount(NodePtr, NodePtr),
+    AggSigParentAmount(NodePtr, NodePtr),
+    AggSigParentPuzzle(NodePtr, NodePtr),
     // puzzle hash (32 bytes), amount-node, amount integer, hint is an optional
     // hash (32 bytes), may be left as null
     CreateCoin(NodePtr, u64, NodePtr),
     // amount
     ReserveFee(u64),
     // message (<= 1024 bytes)
     CreateCoinAnnouncement(NodePtr),
@@ -162,14 +170,40 @@
                     SExp::Pair(_, _) => Err(ValidationErr(c, ErrorCode::InvalidCondition)),
                     _ => Ok(Condition::AggSigMe(pubkey, message)),
                 }
             } else {
                 Ok(Condition::AggSigMe(pubkey, message))
             }
         }
+        AGG_SIG_PUZZLE
+        | AGG_SIG_PUZZLE_AMOUNT
+        | AGG_SIG_PARENT
+        | AGG_SIG_AMOUNT
+        | AGG_SIG_PARENT_PUZZLE
+        | AGG_SIG_PARENT_AMOUNT => {
+            let pubkey = sanitize_hash(a, first(a, c)?, 48, ErrorCode::InvalidPubkey)?;
+            c = rest(a, c)?;
+            let message = sanitize_announce_msg(a, first(a, c)?, ErrorCode::InvalidMessage)?;
+            // AGG_SIG_* take two parameters
+
+            if (flags & STRICT_ARGS_COUNT) != 0 {
+                check_nil(a, c)?;
+            }
+            match op {
+                AGG_SIG_PARENT => Ok(Condition::AggSigParent(pubkey, message)),
+                AGG_SIG_PUZZLE => Ok(Condition::AggSigPuzzle(pubkey, message)),
+                AGG_SIG_AMOUNT => Ok(Condition::AggSigAmount(pubkey, message)),
+                AGG_SIG_PUZZLE_AMOUNT => Ok(Condition::AggSigPuzzleAmount(pubkey, message)),
+                AGG_SIG_PARENT_AMOUNT => Ok(Condition::AggSigParentAmount(pubkey, message)),
+                AGG_SIG_PARENT_PUZZLE => Ok(Condition::AggSigParentPuzzle(pubkey, message)),
+                _ => {
+                    panic!("unexpected");
+                }
+            }
+        }
         CREATE_COIN => {
             let puzzle_hash = sanitize_hash(a, first(a, c)?, 32, ErrorCode::InvalidPuzzleHash)?;
             c = rest(a, c)?;
             let node = first(a, c)?;
             let amount = match sanitize_uint(a, node, 8, ErrorCode::InvalidCoinAmount)? {
                 SanitizedUint::PositiveOverflow => {
                     return Err(ValidationErr(node, ErrorCode::AmountExceedsMaximum));
@@ -468,15 +502,22 @@
     pub before_seconds_relative: Option<u64>,
     // all coins created by this spend. Duplicates are consensus failures
     // if the coin is asserting its birth height or timestamp, these are set
     pub birth_height: Option<u32>,
     pub birth_seconds: Option<u64>,
     pub create_coin: HashSet<NewCoin>,
     // Agg Sig Me conditions
+    // Maybe this should be an array of vectors
     pub agg_sig_me: Vec<(NodePtr, NodePtr)>,
+    pub agg_sig_parent: Vec<(NodePtr, NodePtr)>,
+    pub agg_sig_puzzle: Vec<(NodePtr, NodePtr)>,
+    pub agg_sig_amount: Vec<(NodePtr, NodePtr)>,
+    pub agg_sig_puzzle_amount: Vec<(NodePtr, NodePtr)>,
+    pub agg_sig_parent_amount: Vec<(NodePtr, NodePtr)>,
+    pub agg_sig_parent_puzzle: Vec<(NodePtr, NodePtr)>,
     // Flags describing properties of this spend. See flags above
     pub flags: u32,
 }
 
 // these are all the conditions and properties of a complete spend bundle.
 // some conditions that are created by individual spends are aggregated at the
 // spend bundle level, like reserve_fee and absolute time locks. Other
@@ -499,15 +540,14 @@
     // when set, this is the lowest (i.e. most restrictive) of all
     // ASSERT_BEFORE_HEIGHT_ABSOLUTE conditions
     pub before_height_absolute: Option<u32>,
     // ASSERT_BEFORE_SECONDS_ABSOLUTE conditions
     pub before_seconds_absolute: Option<u64>,
 
     // the cost of conditions (when returned by parse_spends())
-    // run_generator() will include the CLVM cost
     // run_block_generator() will include CLVM cost and byte cost (making this
     // the total cost)
     pub cost: u64,
 
     // the sum of all values of all spent coins
     pub removal_amount: u128,
 
@@ -624,14 +664,20 @@
         seconds_relative: None,
         before_height_relative: None,
         before_seconds_relative: None,
         birth_height: None,
         birth_seconds: None,
         create_coin: HashSet::new(),
         agg_sig_me: Vec::new(),
+        agg_sig_parent: Vec::new(),
+        agg_sig_puzzle: Vec::new(),
+        agg_sig_amount: Vec::new(),
+        agg_sig_puzzle_amount: Vec::new(),
+        agg_sig_parent_amount: Vec::new(),
+        agg_sig_parent_puzzle: Vec::new(),
         // assume it's eligible until we see an agg-sig condition
         flags: ELIGIBLE_FOR_DEDUP,
     };
 
     parse_conditions(a, ret, state, coin_spend, conditions, flags, max_cost)
 }
 
@@ -687,15 +733,22 @@
         match op {
             CREATE_COIN => {
                 if *max_cost < CREATE_COIN_COST {
                     return Err(ValidationErr(c, ErrorCode::CostExceeded));
                 }
                 *max_cost -= CREATE_COIN_COST;
             }
-            AGG_SIG_UNSAFE | AGG_SIG_ME => {
+            AGG_SIG_UNSAFE
+            | AGG_SIG_ME
+            | AGG_SIG_PUZZLE
+            | AGG_SIG_PUZZLE_AMOUNT
+            | AGG_SIG_PARENT
+            | AGG_SIG_AMOUNT
+            | AGG_SIG_PARENT_PUZZLE
+            | AGG_SIG_PARENT_AMOUNT => {
                 if *max_cost < AGG_SIG_COST {
                     return Err(ValidationErr(c, ErrorCode::CostExceeded));
                 }
                 *max_cost -= AGG_SIG_COST;
             }
             _ => (),
         }
@@ -891,14 +944,38 @@
                 decrement(&mut announce_countdown, id)?;
                 state.assert_concurrent_puzzle.insert(id);
             }
             Condition::AggSigMe(pk, msg) => {
                 spend.agg_sig_me.push((pk, msg));
                 spend.flags &= !ELIGIBLE_FOR_DEDUP;
             }
+            Condition::AggSigParent(pk, msg) => {
+                spend.agg_sig_parent.push((pk, msg));
+                spend.flags &= !ELIGIBLE_FOR_DEDUP;
+            }
+            Condition::AggSigPuzzle(pk, msg) => {
+                spend.agg_sig_puzzle.push((pk, msg));
+                spend.flags &= !ELIGIBLE_FOR_DEDUP;
+            }
+            Condition::AggSigAmount(pk, msg) => {
+                spend.agg_sig_amount.push((pk, msg));
+                spend.flags &= !ELIGIBLE_FOR_DEDUP;
+            }
+            Condition::AggSigPuzzleAmount(pk, msg) => {
+                spend.agg_sig_puzzle_amount.push((pk, msg));
+                spend.flags &= !ELIGIBLE_FOR_DEDUP;
+            }
+            Condition::AggSigParentAmount(pk, msg) => {
+                spend.agg_sig_parent_amount.push((pk, msg));
+                spend.flags &= !ELIGIBLE_FOR_DEDUP;
+            }
+            Condition::AggSigParentPuzzle(pk, msg) => {
+                spend.agg_sig_parent_puzzle.push((pk, msg));
+                spend.flags &= !ELIGIBLE_FOR_DEDUP;
+            }
             Condition::AggSigUnsafe(pk, msg) => {
                 ret.agg_sig_unsafe.push((pk, msg));
                 spend.flags &= !ELIGIBLE_FOR_DEDUP;
             }
             Condition::Softfork(cost) => {
                 if *max_cost < cost {
                     return Err(ValidationErr(c, ErrorCode::CostExceeded));
@@ -1533,25 +1610,31 @@
 #[case(ASSERT_MY_BIRTH_HEIGHT, "123")]
 #[case(ASSERT_MY_COIN_ID, "{coin12}")]
 #[case(ASSERT_MY_PARENT_ID, "{h1}")]
 #[case(ASSERT_MY_PUZZLEHASH, "{h2}")]
 #[case(CREATE_COIN, "{h2} (42 (({h1})")]
 #[case(AGG_SIG_UNSAFE, "{pubkey} ({msg1}")]
 #[case(AGG_SIG_ME, "{pubkey} ({msg1}")]
+#[case(AGG_SIG_PARENT, "{pubkey} ({msg1}")]
+#[case(AGG_SIG_PUZZLE, "{pubkey} ({msg1}")]
+#[case(AGG_SIG_AMOUNT, "{pubkey} ({msg1}")]
+#[case(AGG_SIG_PUZZLE_AMOUNT, "{pubkey} ({msg1}")]
+#[case(AGG_SIG_PARENT_PUZZLE, "{pubkey} ({msg1}")]
+#[case(AGG_SIG_PARENT_AMOUNT, "{pubkey} ({msg1}")]
 #[case(ASSERT_CONCURRENT_SPEND, "{coin12}")]
 #[case(ASSERT_CONCURRENT_PUZZLE, "{h2}")]
 fn test_extra_arg_mempool(#[case] condition: ConditionOpcode, #[case] arg: &str) {
     // extra args are disallowed in mempool mode
     assert_eq!(
         cond_test_flag(
             &format!(
                 "((({{h1}} ({{h2}} (123 ((({} ({} ( 1337 )))))",
                 condition as u8, arg
             ),
-            STRICT_ARGS_COUNT | ENABLE_ASSERT_BEFORE
+            STRICT_ARGS_COUNT | ENABLE_ASSERT_BEFORE | ENABLE_SOFTFORK_CONDITION
         )
         .unwrap_err()
         .1,
         ErrorCode::InvalidCondition
     );
 }
 
@@ -1889,22 +1972,28 @@
 #[case(ASSERT_MY_BIRTH_HEIGHT)]
 #[case(ASSERT_MY_COIN_ID)]
 #[case(ASSERT_MY_PARENT_ID)]
 #[case(ASSERT_MY_PUZZLEHASH)]
 #[case(CREATE_COIN)]
 #[case(AGG_SIG_UNSAFE)]
 #[case(AGG_SIG_ME)]
+#[case(AGG_SIG_PARENT)]
+#[case(AGG_SIG_PUZZLE)]
+#[case(AGG_SIG_AMOUNT)]
+#[case(AGG_SIG_PUZZLE_AMOUNT)]
+#[case(AGG_SIG_PARENT_PUZZLE)]
+#[case(AGG_SIG_PARENT_AMOUNT)]
 #[case(ASSERT_CONCURRENT_SPEND)]
 #[case(ASSERT_CONCURRENT_PUZZLE)]
 fn test_missing_arg(#[case] condition: ConditionOpcode) {
     // extra args are disallowed in mempool mode
     assert_eq!(
         cond_test_flag(
             &format!("((({{h1}} ({{h2}} (123 ((({} )))))", condition as u8),
-            ENABLE_ASSERT_BEFORE
+            ENABLE_ASSERT_BEFORE | ENABLE_SOFTFORK_CONDITION
         )
         .unwrap_err()
         .1,
         ErrorCode::InvalidCondition
     );
 }
 
@@ -2275,15 +2364,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
-        assert_eq!(c.puzzle_hash, H2.into());
+        assert_eq!(c.puzzle_hash, H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(c.hint, a.null());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2298,15 +2387,15 @@
     assert_eq!(conds.removal_amount, 0xffffffffffffffff);
     assert_eq!(conds.addition_amount, 0xffffffffffffffff);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 0xffffffffffffffff));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
-        assert_eq!(c.puzzle_hash, H2.into());
+        assert_eq!(c.puzzle_hash, H2);
         assert_eq!(c.amount, 0xffffffffffffffff_u64);
         assert_eq!(c.hint, a.null());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2364,15 +2453,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
-        assert!(c.puzzle_hash == H2.into());
+        assert!(c.puzzle_hash == H2);
         assert!(c.amount == 42_u64);
         assert!(a.atom(c.hint) == H1.to_vec());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2387,15 +2476,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
-        assert!(c.puzzle_hash == H2.into());
+        assert!(c.puzzle_hash == H2);
         assert!(c.amount == 42_u64);
         assert!(a.atom(c.hint) == H1.to_vec());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2408,15 +2497,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
-        assert!(c.puzzle_hash == H2.into());
+        assert!(c.puzzle_hash == H2);
         assert!(c.amount == 42_u64);
         assert!(a.atom(c.hint) == H1.to_vec());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2430,15 +2519,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
-        assert_eq!(c.puzzle_hash, H2.into());
+        assert_eq!(c.puzzle_hash, H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(c.hint, a.null());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2451,15 +2540,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
-        assert_eq!(c.puzzle_hash, H2.into());
+        assert_eq!(c.puzzle_hash, H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(c.hint, a.null());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2485,15 +2574,15 @@
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
 
     for c in &spend.create_coin {
-        assert!(c.puzzle_hash == H2.into());
+        assert!(c.puzzle_hash == H2);
         assert!(c.amount == 42_u64);
         assert!(a.atom(c.hint) == MSG1.to_vec());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2507,15 +2596,15 @@
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
 
     for c in &spend.create_coin {
-        assert_eq!(c.puzzle_hash, H2.into());
+        assert_eq!(c.puzzle_hash, H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(c.hint, a.null());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2530,15 +2619,15 @@
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
 
     for c in &spend.create_coin {
-        assert_eq!(c.puzzle_hash, H2.into());
+        assert_eq!(c.puzzle_hash, H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(a.atom(c.hint), H1.to_vec());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2552,15 +2641,15 @@
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 42);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.create_coin.len(), 1);
     for c in &spend.create_coin {
-        assert_eq!(c.puzzle_hash, H2.into());
+        assert_eq!(c.puzzle_hash, H2);
         assert_eq!(c.amount, 42_u64);
         assert_eq!(c.hint, a.null());
     }
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
@@ -2643,103 +2732,178 @@
         cond_test("((({h1} ({h2} (123 (((51 ({h2} (42 (({h1})) ((51 ({h2} (42 ) ))))")
             .unwrap_err()
             .1,
         ErrorCode::DuplicateOutput
     );
 }
 
-#[test]
-fn test_single_agg_sig_me() {
-    // AGG_SIG_ME
-    let (a, conds) = cond_test("((({h1} ({h2} (123 (((50 ({pubkey} ({msg1} )))))").unwrap();
+#[cfg(test)]
+fn agg_sig_vec(c: ConditionOpcode, s: &Spend) -> &[(NodePtr, NodePtr)] {
+    match c {
+        AGG_SIG_ME => &s.agg_sig_me,
+        AGG_SIG_PARENT => &s.agg_sig_parent,
+        AGG_SIG_PUZZLE => &s.agg_sig_puzzle,
+        AGG_SIG_AMOUNT => &s.agg_sig_amount,
+        AGG_SIG_PUZZLE_AMOUNT => &s.agg_sig_puzzle_amount,
+        AGG_SIG_PARENT_AMOUNT => &s.agg_sig_parent_amount,
+        AGG_SIG_PARENT_PUZZLE => &s.agg_sig_parent_puzzle,
+        _ => {
+            panic!("unexpected");
+        }
+    }
+}
+
+#[cfg(test)]
+#[rstest]
+#[case(AGG_SIG_ME)]
+#[case(AGG_SIG_PARENT)]
+#[case(AGG_SIG_PUZZLE)]
+#[case(AGG_SIG_AMOUNT)]
+#[case(AGG_SIG_PUZZLE_AMOUNT)]
+#[case(AGG_SIG_PARENT_PUZZLE)]
+#[case(AGG_SIG_PARENT_AMOUNT)]
+fn test_single_agg_sig_me(#[case] condition: ConditionOpcode) {
+    let (a, conds) = cond_test_flag(
+        &format!(
+            "((({{h1}} ({{h2}} (123 ((({} ({{pubkey}} ({{msg1}} )))))",
+            condition
+        ),
+        ENABLE_SOFTFORK_CONDITION,
+    )
+    .unwrap();
 
     assert_eq!(conds.cost, AGG_SIG_COST);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
-    assert_eq!(spend.agg_sig_me.len(), 1);
-    for c in &spend.agg_sig_me {
+
+    let agg_sigs = agg_sig_vec(condition, &spend);
+    assert_eq!(agg_sigs.len(), 1);
+    for c in agg_sigs {
         assert_eq!(a.atom(c.0), PUBKEY);
         assert_eq!(a.atom(c.1), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
-#[test]
-fn test_duplicate_agg_sig_me() {
-    // AGG_SIG_ME
+#[cfg(test)]
+#[rstest]
+#[case(AGG_SIG_ME)]
+#[case(AGG_SIG_PARENT)]
+#[case(AGG_SIG_PUZZLE)]
+#[case(AGG_SIG_AMOUNT)]
+#[case(AGG_SIG_PUZZLE_AMOUNT)]
+#[case(AGG_SIG_PARENT_PUZZLE)]
+#[case(AGG_SIG_PARENT_AMOUNT)]
+fn test_duplicate_agg_sig(#[case] condition: ConditionOpcode) {
     // we cannot deduplicate AGG_SIG conditions. Their signatures will be
     // aggregated, and so must all copies of the public keys
     let (a, conds) =
-        cond_test("((({h1} ({h2} (123 (((50 ({pubkey} ({msg1} ) ((50 ({pubkey} ({msg1} ) ))))")
+        cond_test_flag(&format!("((({{h1}} ({{h2}} (123 ((({} ({{pubkey}} ({{msg1}} ) (({} ({{pubkey}} ({{msg1}} ) ))))", condition as u8, condition as u8),
+            ENABLE_SOFTFORK_CONDITION)
             .unwrap();
 
     assert_eq!(conds.cost, AGG_SIG_COST * 2);
     assert_eq!(conds.spends.len(), 1);
     assert_eq!(conds.removal_amount, 123);
     assert_eq!(conds.addition_amount, 0);
     let spend = &conds.spends[0];
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
-    assert_eq!(spend.agg_sig_me.len(), 2);
-    for c in &spend.agg_sig_me {
+
+    let agg_sigs = agg_sig_vec(condition, &spend);
+    assert_eq!(agg_sigs.len(), 2);
+    for c in agg_sigs {
         assert_eq!(a.atom(c.0), PUBKEY);
         assert_eq!(a.atom(c.1), MSG1);
     }
     assert_eq!(spend.flags, 0);
 }
 
-#[test]
-fn test_agg_sig_me_invalid_pubkey() {
-    // AGG_SIG_ME
+#[cfg(test)]
+#[rstest]
+#[case(AGG_SIG_ME)]
+#[case(AGG_SIG_PARENT)]
+#[case(AGG_SIG_PUZZLE)]
+#[case(AGG_SIG_AMOUNT)]
+#[case(AGG_SIG_PUZZLE_AMOUNT)]
+#[case(AGG_SIG_PARENT_PUZZLE)]
+#[case(AGG_SIG_PARENT_AMOUNT)]
+fn test_agg_sig_invalid_pubkey(#[case] condition: ConditionOpcode) {
     assert_eq!(
-        cond_test("((({h1} ({h2} (123 (((50 ({h2} ({msg1} )))))")
-            .unwrap_err()
-            .1,
+        cond_test_flag(
+            &format!(
+                "((({{h1}} ({{h2}} (123 ((({} ({{h2}} ({{msg1}} )))))",
+                condition as u8
+            ),
+            ENABLE_SOFTFORK_CONDITION
+        )
+        .unwrap_err()
+        .1,
         ErrorCode::InvalidPubkey
     );
 }
 
-#[test]
-fn test_agg_sig_me_invalid_msg() {
-    // AGG_SIG_ME
+#[cfg(test)]
+#[rstest]
+#[case(AGG_SIG_ME)]
+#[case(AGG_SIG_PARENT)]
+#[case(AGG_SIG_PUZZLE)]
+#[case(AGG_SIG_AMOUNT)]
+#[case(AGG_SIG_PUZZLE_AMOUNT)]
+#[case(AGG_SIG_PARENT_PUZZLE)]
+#[case(AGG_SIG_PARENT_AMOUNT)]
+fn test_agg_sig_invalid_msg(#[case] condition: ConditionOpcode) {
     assert_eq!(
-        cond_test("((({h1} ({h2} (123 (((50 ({pubkey} ({longmsg} )))))")
-            .unwrap_err()
-            .1,
+        cond_test_flag(
+            &format!(
+                "((({{h1}} ({{h2}} (123 ((({} ({{pubkey}} ({{longmsg}} )))))",
+                condition as u8
+            ),
+            ENABLE_SOFTFORK_CONDITION
+        )
+        .unwrap_err()
+        .1,
         ErrorCode::InvalidMessage
     );
 }
 
-#[test]
-fn test_agg_sig_me_exceed_cost() {
-    // AGG_SIG_ME
+#[cfg(test)]
+#[rstest]
+#[case(AGG_SIG_ME)]
+#[case(AGG_SIG_PARENT)]
+#[case(AGG_SIG_PUZZLE)]
+#[case(AGG_SIG_AMOUNT)]
+#[case(AGG_SIG_PUZZLE_AMOUNT)]
+#[case(AGG_SIG_PARENT_PUZZLE)]
+#[case(AGG_SIG_PARENT_AMOUNT)]
+fn test_agg_sig_exceed_cost(#[case] condition: ConditionOpcode) {
     // ensure that we terminate parsing conditions once they exceed the max cost
     assert_eq!(
         cond_test_cb(
             "((({h1} ({h2} (123 ({} )))",
-            0,
-            Some(Box::new(|a: &mut Allocator| -> NodePtr {
+            ENABLE_SOFTFORK_CONDITION,
+            Some(Box::new(move |a: &mut Allocator| -> NodePtr {
                 let mut rest: NodePtr = a.null();
 
                 for _i in 0..9167 {
-                    // this builds one AGG_SIG_ME condition
+                    // this builds one AGG_SIG_* condition
                     // borrow-rules prevent this from being succint
                     let aggsig = a.null();
                     let val = a.new_atom(MSG1).unwrap();
                     let aggsig = a.new_pair(val, aggsig).unwrap();
                     let val = a.new_atom(PUBKEY).unwrap();
                     let aggsig = a.new_pair(val, aggsig).unwrap();
-                    let val = a.new_atom(&u64_to_bytes(AGG_SIG_ME as u64)).unwrap();
+                    let val = a.new_atom(&u64_to_bytes(condition as u64)).unwrap();
                     let aggsig = a.new_pair(val, aggsig).unwrap();
 
-                    // add the AGG_SIG_ME condition to the list (called rest)
+                    // add the condition to the list (called rest)
                     rest = a.new_pair(aggsig, rest).unwrap();
                 }
                 rest
             }))
         )
         .unwrap_err()
         .1,
@@ -2775,14 +2939,58 @@
         cond_test_flag("((({h1} ({h2} (123 (((49 ({pubkey} ({msg1} (456 )))))", 0)
             .unwrap_err()
             .1,
         ErrorCode::InvalidCondition
     );
 }
 
+#[cfg(test)]
+#[rstest]
+#[case(AGG_SIG_PARENT)]
+#[case(AGG_SIG_PUZZLE)]
+#[case(AGG_SIG_AMOUNT)]
+#[case(AGG_SIG_PUZZLE_AMOUNT)]
+#[case(AGG_SIG_PARENT_PUZZLE)]
+#[case(AGG_SIG_PARENT_AMOUNT)]
+fn test_agg_sig_extra_arg(#[case] condition: ConditionOpcode) {
+    // extra args are ignored in consensus mode
+    let (a, conds) = cond_test_flag(
+        &format!(
+            "((({{h1}} ({{h2}} (123 ((({} ({{pubkey}} ({{msg1}} ( 1337 ) ))))",
+            condition as u8
+        ),
+        ENABLE_SOFTFORK_CONDITION,
+    )
+    .unwrap();
+
+    assert_eq!(conds.cost, 1200000);
+    assert_eq!(conds.spends.len(), 1);
+    let spend = &conds.spends[0];
+    assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
+    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert!((spend.flags & ELIGIBLE_FOR_DEDUP) == 0);
+
+    let agg_sigs = agg_sig_vec(condition, &spend);
+    assert_eq!(agg_sigs.len(), 1);
+
+    // but not in mempool mode
+    assert_eq!(
+        cond_test_flag(
+            &format!(
+                "((({{h1}} ({{h2}} (123 ((({} ({{pubkey}} ({{msg1}} ( 1337 ) ))))",
+                condition as u8
+            ),
+            MEMPOOL_MODE | ENABLE_SOFTFORK_CONDITION,
+        )
+        .unwrap_err()
+        .1,
+        ErrorCode::InvalidCondition
+    );
+}
+
 #[test]
 fn test_agg_sig_me_extra_arg() {
     // AGG_SIG_ME
     // extra args are disallowed in non-mempool mode
     assert_eq!(
         cond_test_flag("((({h1} ({h2} (123 (((50 ({pubkey} ({msg1} (456 )))))", 0)
             .unwrap_err()
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/gen/flags.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/gen/flags.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/gen/opcodes.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/gen/opcodes.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 use crate::gen::flags::ENABLE_SOFTFORK_CONDITION;
 use clvmr::allocator::{Allocator, NodePtr, SExp};
 use clvmr::cost::Cost;
 
 pub type ConditionOpcode = u16;
 
 // AGG_SIG is ascii "1"
+pub const AGG_SIG_PARENT: ConditionOpcode = 43;
+pub const AGG_SIG_PUZZLE: ConditionOpcode = 44;
+pub const AGG_SIG_AMOUNT: ConditionOpcode = 45;
+pub const AGG_SIG_PUZZLE_AMOUNT: ConditionOpcode = 46;
+pub const AGG_SIG_PARENT_AMOUNT: ConditionOpcode = 47;
+pub const AGG_SIG_PARENT_PUZZLE: ConditionOpcode = 48;
 pub const AGG_SIG_UNSAFE: ConditionOpcode = 49;
 pub const AGG_SIG_ME: ConditionOpcode = 50;
 
 // the conditions below reserve coin amounts and have to be accounted for in
 // output totals
 pub const CREATE_COIN: ConditionOpcode = 51;
 pub const RESERVE_FEE: ConditionOpcode = 52;
@@ -130,15 +136,26 @@
             | ASSERT_MY_AMOUNT
             | ASSERT_SECONDS_RELATIVE
             | ASSERT_SECONDS_ABSOLUTE
             | ASSERT_HEIGHT_RELATIVE
             | ASSERT_HEIGHT_ABSOLUTE
             | REMARK => Some(b0),
             _ => {
-                if (flags & ENABLE_SOFTFORK_CONDITION) != 0 && b0 == SOFTFORK {
+                if (flags & ENABLE_SOFTFORK_CONDITION) != 0
+                    && [
+                        SOFTFORK,
+                        AGG_SIG_PARENT,
+                        AGG_SIG_PUZZLE,
+                        AGG_SIG_AMOUNT,
+                        AGG_SIG_PUZZLE_AMOUNT,
+                        AGG_SIG_PARENT_AMOUNT,
+                        AGG_SIG_PARENT_PUZZLE,
+                    ]
+                    .contains(&b0)
+                {
                     Some(b0)
                 } else if (flags & ENABLE_ASSERT_BEFORE) != 0 {
                     match b0 {
                         ASSERT_BEFORE_SECONDS_RELATIVE
                         | ASSERT_BEFORE_SECONDS_ABSOLUTE
                         | ASSERT_BEFORE_HEIGHT_RELATIVE
                         | ASSERT_BEFORE_HEIGHT_ABSOLUTE
@@ -227,16 +244,22 @@
 }
 
 #[cfg(test)]
 #[rstest]
 #[case(&[AGG_SIG_UNSAFE as u8], Some(AGG_SIG_UNSAFE), Some(AGG_SIG_UNSAFE))]
 #[case(&[AGG_SIG_ME as u8], Some(AGG_SIG_ME), Some(AGG_SIG_ME))]
 #[case(&[CREATE_COIN as u8], Some(CREATE_COIN), Some(CREATE_COIN))]
-// the SOFTOFORK condition is only recognized when the flag is set
+// the SOFTOFORK and new AGG_SIG_* condition is only recognized when the flag is set
 #[case(&[SOFTFORK as u8], None, Some(SOFTFORK))]
+#[case(&[AGG_SIG_PARENT as u8], None, Some(AGG_SIG_PARENT))]
+#[case(&[AGG_SIG_PUZZLE as u8], None, Some(AGG_SIG_PUZZLE))]
+#[case(&[AGG_SIG_AMOUNT as u8], None, Some(AGG_SIG_AMOUNT))]
+#[case(&[AGG_SIG_PUZZLE_AMOUNT as u8], None, Some(AGG_SIG_PUZZLE_AMOUNT))]
+#[case(&[AGG_SIG_PARENT_AMOUNT as u8], None, Some(AGG_SIG_PARENT_AMOUNT))]
+#[case(&[AGG_SIG_PARENT_PUZZLE as u8], None, Some(AGG_SIG_PARENT_PUZZLE))]
 #[case(&[ASSERT_EPHEMERAL as u8], None, None)]
 #[case(&[ASSERT_BEFORE_SECONDS_RELATIVE as u8], None, None)]
 fn test_parse_opcode_softfork(
     #[case] input: &[u8],
     #[case] expected: Option<ConditionOpcode>,
     #[case] expected2: Option<ConditionOpcode>,
 ) {
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/gen/run_puzzle.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/gen/run_puzzle.rs`

 * *Files 12% similar despite different names*

```diff
@@ -60,14 +60,20 @@
         seconds_relative: None,
         before_height_relative: None,
         before_seconds_relative: None,
         birth_height: None,
         birth_seconds: None,
         create_coin: HashSet::new(),
         agg_sig_me: Vec::new(),
+        agg_sig_parent: Vec::new(),
+        agg_sig_puzzle: Vec::new(),
+        agg_sig_amount: Vec::new(),
+        agg_sig_puzzle_amount: Vec::new(),
+        agg_sig_parent_amount: Vec::new(),
+        agg_sig_parent_puzzle: Vec::new(),
         // assume it's eligible until we see an agg-sig condition
         flags: ELIGIBLE_FOR_DEDUP,
     };
 
     let mut cost_left = max_cost - clvm_cost;
 
     parse_conditions(
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/gen/sanitize_int.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/gen/sanitize_int.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/gen/test_generators.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/gen/test_generators.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use super::conditions::{NewCoin, Spend, SpendBundleConditions};
-use super::run_block_generator::run_block_generator;
+use super::run_block_generator::{run_block_generator, run_block_generator2};
 use crate::allocator::make_allocator;
 use crate::gen::flags::{ALLOW_BACKREFS, MEMPOOL_MODE};
 use chia_protocol::{Bytes, Bytes48};
 use clvmr::Allocator;
 use std::iter::zip;
 use std::string::String;
 use text_diff::diff;
@@ -99,18 +99,59 @@
 
     ret += &format!("cost: {}\n", c.cost);
     ret += &format!("removal_amount: {}\n", c.removal_amount);
     ret += &format!("addition_amount: {}\n", c.addition_amount);
     ret
 }
 
+fn print_diff(output: &str, expected: &str) {
+    println!("\x1b[102m \x1b[0m - output from test");
+    println!("\x1b[101m \x1b[0m - expected output");
+    for diff in diff(expected, &output, "\n").1 {
+        match diff {
+            Difference::Same(s) => {
+                let lines: Vec<&str> = s.split("\n").collect();
+                if lines.len() <= 6 {
+                    for l in &lines {
+                        println!(" {l}");
+                    }
+                } else {
+                    for l in &lines[0..3] {
+                        println!(" {l}");
+                    }
+                    println!(" ...");
+                    for l in &lines[lines.len() - 3..] {
+                        println!(" {l}");
+                    }
+                }
+            }
+            Difference::Rem(s) => {
+                println!("\x1b[91m");
+                for l in s.split("\n") {
+                    println!("-{l}");
+                }
+                println!("\x1b[0m");
+            }
+            Difference::Add(s) => {
+                println!("\x1b[92m");
+                for l in s.split("\n") {
+                    println!("+{l}");
+                }
+                println!("\x1b[0m");
+            }
+        }
+    }
+}
+
 #[cfg(test)]
 #[rstest]
+#[case("block-225758")]
 #[case("assert-puzzle-announce-fail")]
 #[case("block-834752")]
+#[case("block-834752-compressed")]
 #[case("block-834760")]
 #[case("block-834761")]
 #[case("block-834765")]
 #[case("block-834766")]
 #[case("block-834768")]
 #[case("create-coin-different-amounts")]
 #[case("create-coin-hint-duplicate-outputs")]
@@ -140,73 +181,68 @@
 #[case("many-large-ints-negative")]
 #[case("many-large-ints")]
 #[case("max-height")]
 #[case("multiple-reserve-fee")]
 #[case("negative-reserve-fee")]
 #[case("recursion-pairs")]
 #[case("unknown-condition")]
-fn run_generator(#[case] filename: &str) {
+fn run_generator(#[case] name: &str) {
     use std::fs::read_to_string;
 
-    let filename = format!("generator-tests/{filename}.txt");
+    let filename = format!("generator-tests/{name}.txt");
     println!("file: {filename}");
     let test_file = read_to_string(filename).expect("test file not found");
     let (generator, expected) = test_file.split_once("\n").expect("invalid test file");
     let generator = hex::decode(generator).expect("invalid hex encoded generator");
 
     let expected = match expected.split_once("STRICT:\n") {
         Some((c, m)) => [c, m],
         None => [expected, expected],
     };
 
-    for (flags, expected) in zip(&[0, MEMPOOL_MODE, ALLOW_BACKREFS], expected) {
+    let mut block_refs = Vec::<Vec<u8>>::new();
+
+    let filename = format!("generator-tests/{name}.env");
+    if let Ok(env_hex) = std::fs::read_to_string(&filename) {
+        println!("block-ref file: {filename}");
+        block_refs.push(hex::decode(env_hex).expect("hex decode env-file"));
+    }
+
+    for (flags, expected) in zip(&[ALLOW_BACKREFS, ALLOW_BACKREFS | MEMPOOL_MODE], expected) {
         println!("flags: {:x}", flags);
         let mut a = make_allocator(*flags);
-        let output =
-            match run_block_generator(&mut a, &generator, &[] as &[&[u8]], 11000000000, *flags) {
-                Ok(conditions) => print_conditions(&mut a, &conditions),
+        let (expected_cost, output) =
+            match run_block_generator(&mut a, &generator, &block_refs, 11000000000, *flags) {
+                Ok(conditions) => (conditions.cost, print_conditions(&a, &conditions)),
+                Err(code) => (0, format!("FAILED: {}\n", u32::from(code.1))),
+            };
+
+        let output_hard_fork =
+            match run_block_generator2(&mut a, &generator, &block_refs, 11000000000, *flags) {
+                Ok(mut conditions) => {
+                    // in the hard fork, the cost of running the genrator +
+                    // puzzles should never be higher than before the hard-fork
+                    // but it's likely less.
+                    assert!(conditions.cost <= expected_cost);
+                    assert!(conditions.cost > 0);
+                    // update the cost we print here, just to be compatible with
+                    // the test cases we have. We've already ensured the cost is
+                    // lower
+                    conditions.cost = expected_cost;
+                    print_conditions(&a, &conditions)
+                }
                 Err(code) => {
                     format!("FAILED: {}\n", u32::from(code.1))
                 }
             };
 
+        if output != output_hard_fork {
+            print_diff(&output, &output_hard_fork);
+            panic!("run_block_generator2 produced a different result!");
+        }
+
         if output != expected {
-            println!("\x1b[102m \x1b[0m - output from test");
-            println!("\x1b[101m \x1b[0m - expected output");
-            for diff in diff(expected, &output, "\n").1 {
-                match diff {
-                    Difference::Same(s) => {
-                        let lines: Vec<&str> = s.split("\n").collect();
-                        if lines.len() <= 6 {
-                            for l in &lines {
-                                println!(" {l}");
-                            }
-                        } else {
-                            for l in &lines[0..3] {
-                                println!(" {l}");
-                            }
-                            println!(" ...");
-                            for l in &lines[lines.len() - 3..] {
-                                println!(" {l}");
-                            }
-                        }
-                    }
-                    Difference::Rem(s) => {
-                        println!("\x1b[91m");
-                        for l in s.split("\n") {
-                            println!("-{l}");
-                        }
-                        println!("\x1b[0m");
-                    }
-                    Difference::Add(s) => {
-                        println!("\x1b[92m");
-                        for l in s.split("\n") {
-                            println!("+{l}");
-                        }
-                        println!("\x1b[0m");
-                    }
-                }
-            }
+            print_diff(&output, &expected);
             panic!("mismatching generator output");
         }
     }
 }
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/gen/validation_error.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/gen/validation_error.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/generator_rom.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/generator_rom.rs`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,17 @@
     04ffff02ff0affff04ff02ffff04ff09ff80808080ffff02ff16ffff04ff02ff
     ff04ff0dff8080808080ff8080ff0180ff02ffff03ffff07ff0580ffff01ff0b
     ffff0102ffff02ff1effff04ff02ffff04ff09ff80808080ffff02ff1effff04
     ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff0180
     80"
 );
 
+// the CLVM deserializer from:
+// https://github.com/Chia-Network/chia-blockchain/blob/main/chia/wallet/puzzles/chialisp_deserialisation.clsp.hex
+pub const CLVM_DESERIALIZER: [u8; 471] = hex!(
+"
+ff02ffff01ff05ffff02ff3effff04ff02ffff04ff05ff8080808080ffff04ffff01ffffff81ff7fff81df81bfffffff02ffff03ffff09ff0bffff01818080ffff01ff04ff80ffff04ff05ff808080ffff01ff02ffff03ffff0aff0bff1880ffff01ff02ff1affff04ff02ffff04ffff02ffff03ffff0aff0bff1c80ffff01ff02ffff03ffff0aff0bff1480ffff01ff0880ffff01ff04ffff0effff18ffff011fff0b80ffff0cff05ff80ffff01018080ffff04ffff0cff05ffff010180ff80808080ff0180ffff01ff04ffff18ffff013fff0b80ffff04ff05ff80808080ff0180ff80808080ffff01ff04ff0bffff04ff05ff80808080ff018080ff0180ff04ffff0cff15ff80ff0980ffff04ffff0cff15ff0980ff808080ffff04ffff04ff05ff1380ffff04ff2bff808080ffff02ff16ffff04ff02ffff04ff09ffff04ffff02ff3effff04ff02ffff04ff15ff80808080ff8080808080ff02ffff03ffff09ffff0cff05ff80ffff010180ff1080ffff01ff02ff2effff04ff02ffff04ffff02ff3effff04ff02ffff04ffff0cff05ffff010180ff80808080ff80808080ffff01ff02ff12ffff04ff02ffff04ffff0cff05ffff010180ffff04ffff0cff05ff80ffff010180ff808080808080ff0180ff018080"
+);
+
 // constant from the main chia blockchain:
 // https://github.com/Chia-Network/chia-blockchain/blob/main/chia/consensus/default_constants.py
 pub const COST_PER_BYTE: u64 = 12000;
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia/src/merkle_set.rs` & `chia_rs-0.2.9/local_dependencies/chia/src/merkle_set.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/tests/generate-programs.py` & `chia_rs-0.2.9/local_dependencies/chia/tests/generate-programs.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/tests/run-programs.py` & `chia_rs-0.2.9/local_dependencies/chia/tests/run-programs.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/tests/run.py` & `chia_rs-0.2.9/local_dependencies/chia/tests/run.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/tests/run_gen.py` & `chia_rs-0.2.9/local_dependencies/chia/tests/run_gen.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 #!/usr/bin/env python3
 
-from chia_rs import run_block_generator
+from chia_rs import run_block_generator, SpendBundleConditions, run_block_generator2
 from time import time
 import sys
-from typing import Optional
+from time import perf_counter
+from typing import Optional, Tuple
 
-def run_gen(fn: str, flags: int = 0, args: Optional[str] = None):
+def run_gen(fn: str, flags: int = 0, args: Optional[str] = None, version: int = 1) -> Tuple[Optional[int], Optional[SpendBundleConditions], float]:
 
     # constants from the main chia blockchain:
     # https://github.com/Chia-Network/chia-blockchain/blob/main/chia/consensus/default_constants.py
     max_cost = 11000000000
     cost_per_byte = 12000
 
     generator = bytes.fromhex(open(fn, "r").read().split('\n')[0])
 
     # add the block program arguments
     block_refs = []
     if args and args != "":
-        with open(args, "r") as f:
-            block_refs = [bytes.fromhex(f.read())]
+        try:
+            with open(args, "r") as f:
+                block_refs = [bytes.fromhex(f.read())]
+            print("using ", args)
+        except OSError as e:
+            pass
 
+    block_runner = run_block_generator if version == 1 else run_block_generator2
+
+    start_time = perf_counter()
     try:
-        return run_block_generator(generator, block_refs, max_cost, flags)
+        ret = block_runner(generator, block_refs, max_cost, flags)
+        run_time = perf_counter() - start_time
+        return ret + (run_time, )
     except Exception as e:
         # GENERATOR_RUNTIME_ERROR
-        return (117, None)
+        run_time = perf_counter() - start_time
+        return (117, None, run_time)
 
 
 def print_spend_bundle_conditions(result) -> str:
     ret = ""
     if result.reserve_fee > 0:
         ret += f"RESERVE_FEE: {result.reserve_fee}\n"
     if result.height_absolute > 0:
@@ -64,19 +75,17 @@
     ret += f"removal_amount: {result.removal_amount}\n"
     ret += f"addition_amount: {result.addition_amount}\n"
     return ret
 
 
 if __name__ == "__main__":
     try:
-        start_time = time()
-        error_code, result = run_gen(sys.argv[1],
+        error_code, result, run_time = run_gen(sys.argv[1],
             0 if len(sys.argv) < 3 else int(sys.argv[2]),
             None if len(sys.argv) < 4 else sys.argv[3])
-        run_time = time() - start_time
         if error_code is not None:
             print(f"Validation Error: {error_code}")
             print(f"run-time: {run_time:.2f}s")
             sys.exit(1)
         start_time = time()
         print("Spend bundle:")
         print(print_spend_bundle_conditions(result))
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia/tests/test_coin.py` & `chia_rs-0.2.9/local_dependencies/chia/tests/test_coin.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/tests/test_run_block_generator.py` & `chia_rs-0.2.9/local_dependencies/chia/tests/test_run_block_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,52 @@
-from chia_rs import run_block_generator
+from chia_rs import run_block_generator, run_block_generator2
 from chia_rs import MEMPOOL_MODE
+from run_gen import print_spend_bundle_conditions
 import pytest
 
 def test_run_block_generator_cost() -> None:
 
-    generator = bytes.fromhex(open("generator-tests/block-834768.txt", "r").read().split("\n")[0])
     # the total cost of this generator is 635805370
-    err, conds = run_block_generator(generator, [], 635805370, 0)
+    original_consensus_cost = 635805370
+    # once the hard fork activates, the cost will be lower, because you no
+    # longer pay the cost of the generator ROM
+    hard_fork_consensus_cost = 596498808
+
+    generator = bytes.fromhex(open("generator-tests/block-834768.txt", "r").read().split("\n")[0])
+    err, conds = run_block_generator(generator, [], original_consensus_cost, 0)
     assert err is None
     assert conds is not None
 
+    err2, conds2 = run_block_generator2(generator, [], hard_fork_consensus_cost, 0)
+    assert err2 is None
+    assert conds2 is not None
+
+    output1 = print_spend_bundle_conditions(conds)
+    output2 = print_spend_bundle_conditions(conds2)
+    for l1, l2 in zip(output1.split("\n"), output2.split("\n")):
+        # the cost is supposed to differ, don't compare that
+        if "cost:" in l1 and "cost: " in l2:
+            continue
+        assert l1 == l2
+
     # we exceed the cost limit by 1
-    err, conds = run_block_generator(generator, [], 635805370 - 1, 0)
+    err, conds = run_block_generator(generator, [], original_consensus_cost - 1, 0)
+    # BLOCK_COST_EXCEEDS_MAX = 23
+    assert err == 23
+    assert conds is None
+
+    err, conds = run_block_generator2(generator, [], hard_fork_consensus_cost - 1, 0)
     # BLOCK_COST_EXCEEDS_MAX = 23
     assert err == 23
     assert conds is None
 
     # the byte cost alone exceeds the limit by 1
     err, conds = run_block_generator(generator, [], len(generator) * 12000 - 1, 0)
     # BLOCK_COST_EXCEEDS_MAX = 23
     assert err == 23
     assert conds is None
+
+    # the byte cost alone exceeds the limit by 1
+    err, conds = run_block_generator2(generator, [], len(generator) * 12000 - 1, 0)
+    # BLOCK_COST_EXCEEDS_MAX = 23
+    assert err == 23
+    assert conds is None
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia/tests/test_run_puzzle.py` & `chia_rs-0.2.9/local_dependencies/chia/tests/test_run_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia/tests/test_tree_hash.py` & `chia_rs-0.2.9/local_dependencies/chia/tests/test_tree_hash.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/Cargo.toml` & `chia_rs-0.2.9/local_dependencies/chia-protocol/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 homepage = "https://github.com/Chia-Network/chia_rs/chia-protocol/"
 repository = "https://github.com/Chia-Network/chia_rs/chia-protocol/"
 
 [features]
 py-bindings = ["dep:pyo3", "dep:chia_py_streamable_macro"]
 
 [dependencies]
-pyo3 = { version = "=0.15.1", features = ["extension-module", "multiple-pymethods"], optional = true }
-sha2 = "=0.9.9"
-hex = "=0.4.3"
-chia_streamable_macro = { version = "=0.2.4", path = "../chia_streamable_macro" }
-chia_py_streamable_macro = { path = "../chia_py_streamable_macro", version = "=0.1.3", optional = true }
-clvmr = "=0.2.6"
+pyo3 = { version = "0.19.0", features = ["extension-module", "multiple-pymethods"], optional = true }
+sha2 = "0.9.9"
+hex = "0.4.3"
+chia_streamable_macro = { version = "0.2.4", path = "../chia_streamable_macro" }
+chia_py_streamable_macro = { version = "0.1.3", path = "../chia_py_streamable_macro", optional = true }
+clvmr = "0.2.7"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/bls.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/bls.rs`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 #[cfg(feature = "py-bindings")]
 use crate::to_json_dict::ToJsonDict;
 #[cfg(feature = "py-bindings")]
 use chia_py_streamable_macro::PyStreamable;
 #[cfg(feature = "py-bindings")]
 use pyo3::prelude::*;
 
-#[cfg_attr(feature = "py-bindings", pyclass, derive(PyStreamable))]
+#[cfg_attr(feature = "py-bindings", pyclass(frozen), derive(PyStreamable))]
 #[derive(Streamable, Hash, Debug, Clone, Eq, PartialEq)]
 pub struct G1Element(Bytes48);
 
-#[cfg_attr(feature = "py-bindings", pyclass, derive(PyStreamable))]
+#[cfg_attr(feature = "py-bindings", pyclass(frozen), derive(PyStreamable))]
 #[derive(Streamable, Hash, Debug, Clone, Eq, PartialEq)]
 pub struct G2Element(Bytes96);
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/chia_error.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/chia_error.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/chia_protocol.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/chia_protocol.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/classgroup.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/classgroup.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin_spend.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/coin_spend.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin_state.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/coin_state.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/fee_estimate.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/fee_estimate.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/foliage.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/foliage.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/from_json_dict.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/from_json_dict.rs`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         if buf.len() != N {
             return Err(PyValueError::new_err(format!(
                 "invalid length {} expected {}",
                 buf.len(),
                 N
             )));
         }
-        Ok(buf.try_into()?)
+        Ok((&buf).try_into()?)
     }
 }
 
 impl FromJsonDict for Bytes {
     fn from_json_dict(o: &PyAny) -> PyResult<Self> {
         let s: String = o.extract()?;
         if !s.starts_with("0x") {
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/fullblock.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/fullblock.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/header_block.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/header_block.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/lib.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/pool_target.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/pool_target.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/program.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/program.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/proof_of_space.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/proof_of_space.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/reward_chain_block.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/reward_chain_block.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/slots.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/slots.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/spend_bundle.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/spend_bundle.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/streamable.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/streamable.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/to_json_dict.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/to_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/vdf.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/vdf.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/wallet_protocol.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/wallet_protocol.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia-protocol/src/weight_proof.rs` & `chia_rs-0.2.9/local_dependencies/chia-protocol/src/weight_proof.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/local_dependencies/chia_py_streamable_macro/src/lib.rs` & `chia_rs-0.2.9/local_dependencies/chia_py_streamable_macro/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,16 @@
         }
         _ => {
             panic!("Streamable only support struct");
         }
     };
 
     let mut py_protocol = quote! {
-        #[pyproto]
-        impl pyo3::class::basic::PyObjectProtocol for #ident {
+        #[pymethods]
+        impl #ident {
             fn __str__(&self) -> PyResult<String> {
                 Ok(format!("{:?}", self))
             }
 
             fn __repr__(&self) -> PyResult<String> {
                 Ok(format!("{:?}", self))
             }
@@ -93,32 +93,27 @@
             }
 
             py_protocol.extend( quote! {
                 #[pymethods]
                 impl #ident {
                     #[allow(too_many_arguments)]
                     #[new]
+                    #[pyo3(signature = (#(#fnames),*))]
                     fn new ( #(#fnames : #ftypes),* ) -> #ident {
                         #ident { #(#fnames),* }
                     }
 
                     pub fn to_json_dict(&self, py: Python) -> PyResult<PyObject> {
                         ToJsonDict::to_json_dict(self, py)
                     }
 
                     #[staticmethod]
                     pub fn from_json_dict(o: &pyo3::PyAny) -> PyResult<Self> {
                         <Self as FromJsonDict>::from_json_dict(o)
                     }
-
-                    #(#[getter]
-                        fn #fnames(&self, py: Python) -> PyResult<#ftypes> {
-                            Ok(self.#fnames.clone())
-                        }
-                    )*
                 }
 
                 impl ToJsonDict for #ident {
                     fn to_json_dict(&self, py: Python) -> PyResult<PyObject> {
                         let ret = pyo3::types::PyDict::new(py);
                         #(ret.set_item(stringify!(#fnames), self.#fnames.to_json_dict(py)?)?);*;
                         Ok(ret.into())
```

### Comparing `chia_rs-0.2.8/local_dependencies/chia_streamable_macro/src/lib.rs` & `chia_rs-0.2.9/local_dependencies/chia_streamable_macro/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/Cargo.toml` & `chia_rs-0.2.9/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "chia_rs"
-version = "0.2.8"
+version = "0.2.9"
 authors = ["Richard Kiss <him@richardkiss.com>"]
 edition = "2021"
 license = "Apache-2.0"
 description = "Code useful for implementing chia consensus."
 homepage = "https://github.com/Chia-Network/chia_rs/"
 repository = "https://github.com/Chia-Network/chia_rs/"
 readme = "README.md"
 
 [lib]
 name = "chia_rs"
 crate-type = ["cdylib"]
 path = "src/lib.rs"
 
 [dependencies]
+clvmr = "=0.2.7"
+hex = "=0.4.3"
+pyo3 = { version = "=0.19.0", features = ["extension-module", "multiple-pymethods"] }
 chia = { path = "local_dependencies/chia", features = ["py-bindings"] }
 chia-protocol = { path = "local_dependencies/chia-protocol", features = ["py-bindings"]  }
-clvmr = "=0.2.6"
-pyo3 = { version = "=0.15.1", features = ["extension-module", "multiple-pymethods"] }
-chia_py_streamable_macro = { version= "0.1.3", path = "local_dependencies/chia_py_streamable_macro" }
-chia_streamable_macro = { version = "0.2.4", path = "local_dependencies/chia_streamable_macro" }
-hex = "=0.4.3"
+chia_py_streamable_macro = { path = "local_dependencies/chia_py_streamable_macro" }
+chia_streamable_macro = { path = "local_dependencies/chia_streamable_macro" }
```

### Comparing `chia_rs-0.2.8/chia_rs.pyi` & `chia_rs-0.2.9/chia_rs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 #
 
 from typing import List, Optional, Sequence, Tuple
 from chia.types.blockchain_format.sized_bytes import bytes32
 
 ReadableBuffer = Union[bytes, bytearray, memoryview]
 
+def solution_generator(spends: Sequence[Tuple[Coin, bytes, bytes]]) -> bytes: ...
+def solution_generator_backrefs(spends: Sequence[Tuple[Coin, bytes, bytes]]) -> bytes: ...
+
 def compute_merkle_set_root(items: Sequence[bytes]) -> bytes: ...
 
-def run_generator(
-    program: bytes, args: bytes, max_cost: int, flags: int
+def run_block_generator(
+    program: ReadableBuffer, args: List[ReadableBuffer], max_cost: int, flags: int
 ) -> Tuple[Optional[int], Optional[SpendBundleConditions]]: ...
 
-def run_block_generator(
-    program: bytes, args: List[bytes], max_cost: int, flags: int
+def run_block_generator2(
+    program: ReadableBuffer, args: List[ReadableBuffer], max_cost: int, flags: int
 ) -> Tuple[Optional[int], Optional[SpendBundleConditions]]: ...
 
 def run_puzzle(
     puzzle: bytes, solution: bytes, parent_id: bytes32, amount: int, max_cost: int, flags: int
 ) -> SpendBundleConditions: ...
 
 COND_ARGS_NIL: int = ...
@@ -47,42 +50,58 @@
     program: bytes, args: bytes, max_cost: int, flags: int
 ) -> Pair[int, LazyNode]: ...
 
 class LazyNode:
     def pair() -> Optional[Tuple[LazyNode, LazyNode]]: ...
     def atom() -> bytes: ...
 
-def serialized_length(program: bytes) -> int: ...
+def serialized_length(program: ReadableBuffer) -> int: ...
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
-def get_puzzle_and_solution_for_coin(program: bytes, args: bytes, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
+def get_puzzle_and_solution_for_coin(program: ReadableBuffer, args: ReadableBuffer, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 
 class Spend:
     coin_id: bytes
+    parent_id: bytes
     puzzle_hash: bytes
+    coin_amount: int
     height_relative: Optional[int]
     seconds_relative: Optional[int]
     before_height_relative: Optional[int]
     before_seconds_relative: Optional[int]
     birth_height: Optional[int]
     birth_seconds: Optional[int]
     create_coin: List[Tuple[bytes, int, Optional[bytes]]]
     agg_sig_me: List[Tuple[bytes, bytes]]
+    agg_sig_parent: List[Tuple[bytes, bytes]]
+    agg_sig_puzzle: List[Tuple[bytes, bytes]]
+    agg_sig_amount: List[Tuple[bytes, bytes]]
+    agg_sig_puzzle_amount: List[Tuple[bytes, bytes]]
+    agg_sig_parent_amount: List[Tuple[bytes, bytes]]
+    agg_sig_parent_puzzle: List[Tuple[bytes, bytes]]
     flags: int
     def __init__(
         self,
         coin_id: bytes,
+        parent_id: bytes,
         puzzle_hash: bytes,
+        coin_amount: int,
         height_relative: Optional[int],
         seconds_relative: Optional[int],
         before_height_relative: Optional[int],
         before_seconds_relative: Optional[int],
         birth_height: Optional[int],
         birth_seconds: Optional[int],
         create_coin: Sequence[Tuple[bytes, int, Optional[bytes]]],
         agg_sig_me: Sequence[Tuple[bytes, bytes]],
+        agg_sig_parent: Sequence[Tuple[bytes, bytes]],
+        agg_sig_puzzle: Sequence[Tuple[bytes, bytes]],
+        agg_sig_amount: Sequence[Tuple[bytes, bytes]],
+        agg_sig_puzzle_amount: Sequence[Tuple[bytes, bytes]],
+        agg_sig_parent_amount: Sequence[Tuple[bytes, bytes]],
+        agg_sig_parent_puzzle: Sequence[Tuple[bytes, bytes]],
         flags: int
     ) -> None: ...
     def __hash__(self) -> int: ...
     def __str__(self) -> str: ...
     def __repr__(self) -> str: ...
     def __richcmp__(self) -> Any: ...
     def __deepcopy__(self) -> Spend: ...
```

### Comparing `chia_rs-0.2.8/generate_type_stubs.py` & `chia_rs-0.2.9/generate_type_stubs.py`

 * *Files 7% similar despite different names*

```diff
@@ -148,22 +148,25 @@
 #
 
 from typing import List, Optional, Sequence, Tuple
 from chia.types.blockchain_format.sized_bytes import bytes32
 
 ReadableBuffer = Union[bytes, bytearray, memoryview]
 
+def solution_generator(spends: Sequence[Tuple[Coin, bytes, bytes]]) -> bytes: ...
+def solution_generator_backrefs(spends: Sequence[Tuple[Coin, bytes, bytes]]) -> bytes: ...
+
 def compute_merkle_set_root(items: Sequence[bytes]) -> bytes: ...
 
-def run_generator(
-    program: bytes, args: bytes, max_cost: int, flags: int
+def run_block_generator(
+    program: ReadableBuffer, args: List[ReadableBuffer], max_cost: int, flags: int
 ) -> Tuple[Optional[int], Optional[SpendBundleConditions]]: ...
 
-def run_block_generator(
-    program: bytes, args: List[bytes], max_cost: int, flags: int
+def run_block_generator2(
+    program: ReadableBuffer, args: List[ReadableBuffer], max_cost: int, flags: int
 ) -> Tuple[Optional[int], Optional[SpendBundleConditions]]: ...
 
 def run_puzzle(
     puzzle: bytes, solution: bytes, parent_id: bytes32, amount: int, max_cost: int, flags: int
 ) -> SpendBundleConditions: ...
 
 COND_ARGS_NIL: int = ...
@@ -191,32 +194,40 @@
     program: bytes, args: bytes, max_cost: int, flags: int
 ) -> Pair[int, LazyNode]: ...
 
 class LazyNode:
     def pair() -> Optional[Tuple[LazyNode, LazyNode]]: ...
     def atom() -> bytes: ...
 
-def serialized_length(program: bytes) -> int: ...
+def serialized_length(program: ReadableBuffer) -> int: ...
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
-def get_puzzle_and_solution_for_coin(program: bytes, args: bytes, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
+def get_puzzle_and_solution_for_coin(program: ReadableBuffer, args: ReadableBuffer, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 """
     )
 
     print_class(f, "Spend",
         [
             "coin_id: bytes",
+            "parent_id: bytes",
             "puzzle_hash: bytes",
+            "coin_amount: int",
             "height_relative: Optional[int]",
             "seconds_relative: Optional[int]",
             "before_height_relative: Optional[int]",
             "before_seconds_relative: Optional[int]",
             "birth_height: Optional[int]",
             "birth_seconds: Optional[int]",
             "create_coin: List[Tuple[bytes, int, Optional[bytes]]]",
             "agg_sig_me: List[Tuple[bytes, bytes]]",
+            "agg_sig_parent: List[Tuple[bytes, bytes]]",
+            "agg_sig_puzzle: List[Tuple[bytes, bytes]]",
+            "agg_sig_amount: List[Tuple[bytes, bytes]]",
+            "agg_sig_puzzle_amount: List[Tuple[bytes, bytes]]",
+            "agg_sig_parent_amount: List[Tuple[bytes, bytes]]",
+            "agg_sig_parent_puzzle: List[Tuple[bytes, bytes]]",
             "flags: int",
         ],
     )
 
     print_class(f, "SpendBundleConditions",
         [
             "spends: List[Spend]",
```

### Comparing `chia_rs-0.2.8/src/adapt_response.rs` & `chia_rs-0.2.9/src/adapt_response.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/src/api.rs` & `chia_rs-0.2.9/src/api.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 use crate::compression;
 use crate::run_generator::{
-    convert_spend_bundle_conds, PySpend, PySpendBundleConditions,
-    __pyo3_get_function_run_block_generator, __pyo3_get_function_run_generator,
+    convert_spend_bundle_conds, run_block_generator, run_block_generator2, PySpend,
+    PySpendBundleConditions,
 };
 use chia::allocator::make_allocator;
 use chia::gen::flags::{
     AGG_SIG_ARGS, ALLOW_BACKREFS, COND_ARGS_NIL, ENABLE_ASSERT_BEFORE, ENABLE_SOFTFORK_CONDITION,
     LIMIT_ANNOUNCES, LIMIT_OBJECTS, MEMPOOL_MODE, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL,
     NO_UNKNOWN_CONDS, STRICT_ARGS_COUNT,
 };
 use chia::gen::run_puzzle::run_puzzle as native_run_puzzle;
+use chia::gen::solution_generator::solution_generator as native_solution_generator;
+use chia::gen::solution_generator::solution_generator_backrefs as native_solution_generator_backrefs;
 use chia::merkle_set::compute_merkle_set_root as compute_merkle_root_impl;
 use chia_protocol::Bytes32;
 use chia_protocol::FullBlock;
 use chia_protocol::G1Element;
 use chia_protocol::G2Element;
 use chia_protocol::{
     ChallengeBlockInfo, ChallengeChainSubSlot, ClassgroupElement, Coin, CoinSpend, CoinState,
@@ -31,23 +33,24 @@
     TransactionsInfo, VDFInfo, VDFProof,
 };
 use clvmr::serde::tree_hash_from_stream;
 use clvmr::{
     ENABLE_BLS_OPS, ENABLE_BLS_OPS_OUTSIDE_GUARD, ENABLE_FIXED_DIV, ENABLE_SECP_OPS, LIMIT_HEAP,
     NO_UNKNOWN_OPS,
 };
+use pyo3::buffer::PyBuffer;
 use pyo3::prelude::*;
+use pyo3::types::PyAny;
 use pyo3::types::PyBytes;
 use pyo3::types::PyModule;
+use pyo3::types::PyTuple;
 use pyo3::{wrap_pyfunction, PyResult, Python};
 use std::convert::TryInto;
 
-use crate::run_program::{
-    __pyo3_get_function_run_chia_program, __pyo3_get_function_serialized_length,
-};
+use crate::run_program::{run_chia_program, serialized_length};
 
 use crate::adapt_response::eval_err_to_pyresult;
 use chia::gen::get_puzzle_and_solution::get_puzzle_and_solution_for_coin as parse_puzzle_solution;
 use chia::gen::validation_error::ValidationErr;
 use clvmr::allocator::NodePtr;
 use clvmr::cost::Cost;
 use clvmr::reduction::EvalErr;
@@ -66,37 +69,48 @@
     for b in values {
         buffer.push(b.as_bytes().try_into()?);
     }
     Ok(PyBytes::new(py, &compute_merkle_root_impl(&mut buffer)))
 }
 
 #[pyfunction]
-pub fn tree_hash(py: Python, blob: pyo3::buffer::PyBuffer<u8>) -> PyResult<&PyBytes> {
+pub fn tree_hash(py: Python, blob: PyBuffer<u8>) -> PyResult<&PyBytes> {
     if !blob.is_c_contiguous() {
         panic!("tree_hash() must be called with a contiguous buffer");
     }
     let slice =
         unsafe { std::slice::from_raw_parts(blob.buf_ptr() as *const u8, blob.len_bytes()) };
     let mut input = std::io::Cursor::<&[u8]>::new(slice);
     Ok(PyBytes::new(py, &tree_hash_from_stream(&mut input)?))
 }
 
 #[pyfunction]
 pub fn get_puzzle_and_solution_for_coin<'py>(
     py: Python<'py>,
-    program: &[u8],
-    args: &[u8],
+    program: PyBuffer<u8>,
+    args: PyBuffer<u8>,
     max_cost: Cost,
     find_parent: Bytes32,
     find_amount: u64,
     find_ph: Bytes32,
     flags: u32,
 ) -> PyResult<(&'py PyBytes, &'py PyBytes)> {
     let mut allocator = make_allocator(LIMIT_HEAP);
 
+    if !program.is_c_contiguous() {
+        panic!("program must be contiguous");
+    }
+    let program =
+        unsafe { std::slice::from_raw_parts(program.buf_ptr() as *const u8, program.len_bytes()) };
+
+    if !args.is_c_contiguous() {
+        panic!("args must be contiguous");
+    }
+    let args = unsafe { std::slice::from_raw_parts(args.buf_ptr() as *const u8, args.len_bytes()) };
+
     let deserialize = if (flags & ALLOW_BACKREFS) != 0 {
         node_from_bytes_backrefs
     } else {
         node_from_bytes
     };
     let program = deserialize(&mut allocator, program)?;
     let args = deserialize(&mut allocator, args)?;
@@ -135,20 +149,49 @@
     flags: u32,
 ) -> PyResult<PySpendBundleConditions> {
     let mut a = make_allocator(LIMIT_HEAP);
     let conds = native_run_puzzle(&mut a, puzzle, solution, parent_id, amount, max_cost, flags)?;
     Ok(convert_spend_bundle_conds(&a, conds))
 }
 
+fn convert_list_of_tuples(spends: &PyAny) -> PyResult<Vec<(Coin, &[u8], &[u8])>> {
+    let mut native_spends = Vec::<(Coin, &[u8], &[u8])>::new();
+    for s in spends.iter()? {
+        let tuple = s?.downcast::<PyTuple>()?;
+        let coin = tuple.get_item(0)?.extract::<Coin>()?;
+        let puzzle = tuple.get_item(1)?.extract::<&[u8]>()?;
+        let solution = tuple.get_item(2)?.extract::<&[u8]>()?;
+        native_spends.push((coin, puzzle, solution));
+    }
+    Ok(native_spends)
+}
+
+#[pyfunction]
+fn solution_generator<'p>(py: Python<'p>, spends: &PyAny) -> PyResult<&'p PyBytes> {
+    let spends = convert_list_of_tuples(spends)?;
+    Ok(PyBytes::new(py, &native_solution_generator(spends)?))
+}
+
+#[pyfunction]
+fn solution_generator_backrefs<'p>(py: Python<'p>, spends: &PyAny) -> PyResult<&'p PyBytes> {
+    let spends = convert_list_of_tuples(spends)?;
+    Ok(PyBytes::new(
+        py,
+        &native_solution_generator_backrefs(spends)?,
+    ))
+}
+
 #[pymodule]
 pub fn chia_rs(py: Python, m: &PyModule) -> PyResult<()> {
     // generator functions
-    m.add_function(wrap_pyfunction!(run_generator, m)?)?;
     m.add_function(wrap_pyfunction!(run_block_generator, m)?)?;
+    m.add_function(wrap_pyfunction!(run_block_generator2, m)?)?;
     m.add_function(wrap_pyfunction!(run_puzzle, m)?)?;
+    m.add_function(wrap_pyfunction!(solution_generator, m)?)?;
+    m.add_function(wrap_pyfunction!(solution_generator_backrefs, m)?)?;
     m.add_class::<PySpendBundleConditions>()?;
     m.add(
         "ELIGIBLE_FOR_DEDUP",
         chia::gen::conditions::ELIGIBLE_FOR_DEDUP,
     )?;
     m.add_class::<PySpend>()?;
```

### Comparing `chia_rs-0.2.8/src/compression.rs` & `chia_rs-0.2.9/src/compression.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.8/src/run_generator.rs` & `chia_rs-0.2.9/src/run_generator.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,54 @@
-use super::adapt_response::eval_err_to_pyresult;
 use chia_protocol::from_json_dict::FromJsonDict;
 use chia_protocol::to_json_dict::ToJsonDict;
 
 use chia::allocator::make_allocator;
-use chia::gen::conditions::{parse_spends, Spend, SpendBundleConditions};
+use chia::gen::conditions::{Spend, SpendBundleConditions};
 use chia::gen::run_block_generator::run_block_generator as native_run_block_generator;
-use chia::gen::validation_error::{ErrorCode, ValidationErr};
+use chia::gen::run_block_generator::run_block_generator2 as native_run_block_generator2;
+use chia::gen::validation_error::ValidationErr;
 use chia_protocol::bytes::{Bytes, Bytes32, Bytes48};
 
-use clvmr::allocator::Allocator;
-use clvmr::chia_dialect::ChiaDialect;
+use clvmr::allocator::{Allocator, NodePtr};
 use clvmr::cost::Cost;
-use clvmr::reduction::{EvalErr, Reduction};
-use clvmr::run_program::run_program;
-use clvmr::serde::node_from_bytes;
 
+use pyo3::buffer::PyBuffer;
 use pyo3::prelude::*;
 use pyo3::types::PyList;
 
 use chia_protocol::chia_error;
 use chia_protocol::streamable::Streamable;
 use chia_py_streamable_macro::PyStreamable;
 use chia_streamable_macro::Streamable;
 
-#[pyclass(name = "Spend")]
+#[pyclass(name = "Spend", get_all, frozen)]
 #[derive(Streamable, PyStreamable, Hash, Debug, Clone, Eq, PartialEq)]
 pub struct PySpend {
     pub coin_id: Bytes32,
+    pub parent_id: Bytes32,
     pub puzzle_hash: Bytes32,
+    pub coin_amount: u64,
     pub height_relative: Option<u32>,
     pub seconds_relative: Option<u64>,
     pub before_height_relative: Option<u32>,
     pub before_seconds_relative: Option<u64>,
     pub birth_height: Option<u32>,
     pub birth_seconds: Option<u64>,
     pub create_coin: Vec<(Bytes32, u64, Option<Bytes>)>,
     pub agg_sig_me: Vec<(Bytes48, Bytes)>,
+    pub agg_sig_parent: Vec<(Bytes48, Bytes)>,
+    pub agg_sig_puzzle: Vec<(Bytes48, Bytes)>,
+    pub agg_sig_amount: Vec<(Bytes48, Bytes)>,
+    pub agg_sig_puzzle_amount: Vec<(Bytes48, Bytes)>,
+    pub agg_sig_parent_amount: Vec<(Bytes48, Bytes)>,
+    pub agg_sig_parent_puzzle: Vec<(Bytes48, Bytes)>,
     pub flags: u32,
 }
 
-#[pyclass(name = "SpendBundleConditions")]
+#[pyclass(name = "SpendBundleConditions", get_all, frozen)]
 #[derive(Streamable, PyStreamable, Hash, Debug, Clone, Eq, PartialEq)]
 pub struct PySpendBundleConditions {
     pub spends: Vec<PySpend>,
     pub reserve_fee: u64,
     // the highest height/time conditions (i.e. most strict)
     pub height_absolute: u32,
     pub seconds_absolute: u64,
@@ -57,19 +62,23 @@
     pub cost: u64,
     // the sum of all values of all spent coins
     pub removal_amount: u128,
     // the sum of all amounts of CREATE_COIN conditions
     pub addition_amount: u128,
 }
 
-fn convert_spend(a: &Allocator, spend: Spend) -> PySpend {
-    let mut agg_sigs = Vec::<(Bytes48, Bytes)>::new();
-    for (pk, msg) in spend.agg_sig_me {
-        agg_sigs.push((a.atom(pk).into(), a.atom(msg).into()));
+fn convert_agg_sigs(a: &Allocator, agg_sigs: &[(NodePtr, NodePtr)]) -> Vec<(Bytes48, Bytes)> {
+    let mut ret = Vec::<(Bytes48, Bytes)>::new();
+    for (pk, msg) in agg_sigs {
+        ret.push((a.atom(*pk).into(), a.atom(*msg).into()));
     }
+    ret
+}
+
+fn convert_spend(a: &Allocator, spend: Spend) -> PySpend {
     let mut create_coin =
         Vec::<(Bytes32, u64, Option<Bytes>)>::with_capacity(spend.create_coin.len());
     for c in spend.create_coin {
         create_coin.push((
             c.puzzle_hash,
             c.amount,
             if c.hint != a.null() {
@@ -78,23 +87,31 @@
                 None
             },
         ));
     }
 
     PySpend {
         coin_id: *spend.coin_id,
+        parent_id: a.atom(spend.parent_id).into(),
         puzzle_hash: a.atom(spend.puzzle_hash).into(),
+        coin_amount: spend.coin_amount,
         height_relative: spend.height_relative,
         seconds_relative: spend.seconds_relative,
         before_height_relative: spend.before_height_relative,
         before_seconds_relative: spend.before_seconds_relative,
         birth_height: spend.birth_height,
         birth_seconds: spend.birth_seconds,
         create_coin,
-        agg_sig_me: agg_sigs,
+        agg_sig_me: convert_agg_sigs(a, &spend.agg_sig_me),
+        agg_sig_parent: convert_agg_sigs(a, &spend.agg_sig_parent),
+        agg_sig_puzzle: convert_agg_sigs(a, &spend.agg_sig_puzzle),
+        agg_sig_amount: convert_agg_sigs(a, &spend.agg_sig_amount),
+        agg_sig_puzzle_amount: convert_agg_sigs(a, &spend.agg_sig_puzzle_amount),
+        agg_sig_parent_amount: convert_agg_sigs(a, &spend.agg_sig_parent_amount),
+        agg_sig_parent_puzzle: convert_agg_sigs(a, &spend.agg_sig_parent_puzzle),
         flags: spend.flags,
     }
 }
 
 pub fn convert_spend_bundle_conds(
     a: &Allocator,
     sb: SpendBundleConditions,
@@ -119,79 +136,86 @@
         agg_sig_unsafe: agg_sigs,
         cost: sb.cost,
         removal_amount: sb.removal_amount,
         addition_amount: sb.addition_amount,
     }
 }
 
-// returns the cost of running the CLVM program along with conditions and the list of
-// spends
 #[pyfunction]
-pub fn run_generator(
-    py: Python,
-    program: &[u8],
-    args: &[u8],
+pub fn run_block_generator(
+    _py: Python,
+    program: PyBuffer<u8>,
+    block_refs: &PyList,
     max_cost: Cost,
     flags: u32,
 ) -> PyResult<(Option<u32>, Option<PySpendBundleConditions>)> {
     let mut allocator = make_allocator(flags);
-    let program = node_from_bytes(&mut allocator, program)?;
-    let args = node_from_bytes(&mut allocator, args)?;
-    let dialect = &ChiaDialect::new(flags);
-
-    let r = py.allow_threads(
-        || -> Result<(Option<ErrorCode>, Option<SpendBundleConditions>), EvalErr> {
-            let Reduction(cost, node) =
-                run_program(&mut allocator, dialect, program, args, max_cost)?;
-            // we pass in what's left of max_cost here, to fail early in case the
-            // cost of a condition brings us over the cost limit
-            match parse_spends(&allocator, node, max_cost - cost, flags) {
-                Err(ValidationErr(_, c)) => Ok((Some(c), None)),
-                Ok(mut spend_bundle_conds) => {
-                    // the cost is only the cost of conditions, add the
-                    // cost of running the CLVM program here as well
-                    spend_bundle_conds.cost += cost;
-                    Ok((None, Some(spend_bundle_conds)))
-                }
-            }
-        },
-    );
 
-    match r {
-        Ok((None, Some(spend_bundle_conds))) => {
+    let mut refs = Vec::<&[u8]>::new();
+    for g in block_refs {
+        let buf = g.extract::<PyBuffer<u8>>()?;
+
+        if !buf.is_c_contiguous() {
+            panic!("block_refs buffers must be contiguous");
+        }
+        let slice =
+            unsafe { std::slice::from_raw_parts(buf.buf_ptr() as *const u8, buf.len_bytes()) };
+        refs.push(slice);
+    }
+
+    if !program.is_c_contiguous() {
+        panic!("program buffer must be contiguous");
+    }
+    let program =
+        unsafe { std::slice::from_raw_parts(program.buf_ptr() as *const u8, program.len_bytes()) };
+
+    match native_run_block_generator(&mut allocator, program, &refs, max_cost, flags) {
+        Ok(spend_bundle_conds) => {
             // everything was successful
             Ok((
                 None,
                 Some(convert_spend_bundle_conds(&allocator, spend_bundle_conds)),
             ))
         }
-        Ok((error_code, _)) => {
+        Err(ValidationErr(_, error_code)) => {
             // a validation error occurred
-            Ok((error_code.map(|x| x.into()), None))
+            Ok((Some(error_code.into()), None))
         }
-        Err(eval_err) => eval_err_to_pyresult(py, eval_err, allocator),
     }
 }
 
 #[pyfunction]
-pub fn run_block_generator(
+pub fn run_block_generator2(
     _py: Python,
-    program: &[u8],
+    program: PyBuffer<u8>,
     block_refs: &PyList,
     max_cost: Cost,
     flags: u32,
 ) -> PyResult<(Option<u32>, Option<PySpendBundleConditions>)> {
     let mut allocator = make_allocator(flags);
 
-    let mut refs = Vec::<Vec<u8>>::new();
+    let mut refs = Vec::<&[u8]>::new();
     for g in block_refs {
-        refs.push(g.extract::<Vec<u8>>()?);
+        let buf = g.extract::<PyBuffer<u8>>()?;
+
+        if !buf.is_c_contiguous() {
+            panic!("block_refs buffers must be contiguous");
+        }
+        let slice =
+            unsafe { std::slice::from_raw_parts(buf.buf_ptr() as *const u8, buf.len_bytes()) };
+        refs.push(slice);
     }
 
-    match native_run_block_generator(&mut allocator, program, &refs, max_cost, flags) {
+    if !program.is_c_contiguous() {
+        panic!("program buffer must be contiguous");
+    }
+    let program =
+        unsafe { std::slice::from_raw_parts(program.buf_ptr() as *const u8, program.len_bytes()) };
+
+    match native_run_block_generator2(&mut allocator, program, &refs, max_cost, flags) {
         Ok(spend_bundle_conds) => {
             // everything was successful
             Ok((
                 None,
                 Some(convert_spend_bundle_conds(&allocator, spend_bundle_conds)),
             ))
         }
```

### Comparing `chia_rs-0.2.8/src/run_program.rs` & `chia_rs-0.2.9/src/run_program.rs`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 use chia::gen::flags::ALLOW_BACKREFS;
 use clvmr::allocator::{Allocator, NodePtr, SExp};
 use clvmr::chia_dialect::ChiaDialect;
 use clvmr::cost::Cost;
 use clvmr::reduction::Response;
 use clvmr::run_program::run_program;
 use clvmr::serde::{node_from_bytes, node_from_bytes_backrefs, serialized_length_from_bytes};
+use pyo3::buffer::PyBuffer;
 use pyo3::prelude::*;
 use pyo3::types::{PyBytes, PyTuple};
 use std::rc::Rc;
 
-#[pyclass(subclass, unsendable)]
+#[pyclass(subclass, unsendable, frozen)]
 #[derive(Clone)]
 pub struct LazyNode {
     allocator: Rc<Allocator>,
     node: NodePtr,
 }
 
 impl ToPyObject for LazyNode {
@@ -57,15 +58,20 @@
             node: n,
         }
     }
 }
 
 #[allow(clippy::borrow_deref_ref)]
 #[pyfunction]
-pub fn serialized_length(program: &[u8]) -> PyResult<u64> {
+pub fn serialized_length(program: PyBuffer<u8>) -> PyResult<u64> {
+    if !program.is_c_contiguous() {
+        panic!("program must be contiguous");
+    }
+    let program =
+        unsafe { std::slice::from_raw_parts(program.buf_ptr() as *const u8, program.len_bytes()) };
     Ok(serialized_length_from_bytes(program)?)
 }
 
 #[allow(clippy::borrow_deref_ref)]
 #[pyfunction]
 pub fn run_chia_program(
     py: Python,
```

### Comparing `chia_rs-0.2.8/Cargo.lock` & `chia_rs-0.2.9/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chia"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "chia-protocol",
  "clvm-utils",
  "clvmr",
  "hex",
  "hex-literal",
  "pyo3",
@@ -104,23 +104,23 @@
  "hex",
  "pyo3",
  "sha2 0.9.9",
 ]
 
 [[package]]
 name = "chia_py_streamable_macro"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "chia_rs"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "chia",
  "chia-protocol",
  "chia_py_streamable_macro",
  "chia_streamable_macro",
  "clvmr",
  "hex",
@@ -128,29 +128,29 @@
 ]
 
 [[package]]
 name = "chia_streamable_macro"
 version = "0.2.4"
 dependencies = [
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "clvm-utils"
 version = "0.2.7"
 dependencies = [
  "clvmr",
 ]
 
 [[package]]
 name = "clvmr"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83afaa6d5081706f202d31ed08ddb2425c902ca968d9832429bcdf9474ca6c9f"
+checksum = "c2890f01537f1be43d2767ae71bbba0d0b3543dbb1ee892092d0ed4d913227fc"
 dependencies = [
  "bls12_381",
  "getrandom",
  "group",
  "hex",
  "k256",
  "lazy_static",
@@ -159,23 +159,23 @@
  "num-traits",
  "p256",
  "sha2 0.9.9",
 ]
 
 [[package]]
 name = "const-oid"
-version = "0.9.2"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "520fbf3c07483f94e3e3ca9d0cfd913d7718ef2483d2cfd91c0d9e91474ab913"
+checksum = "795bc6e66a8e340f075fcf6227e417a2dc976b92b91f3cdc778bb858778b6747"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
+checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crypto-bigint"
 version = "0.5.2"
@@ -195,28 +195,18 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
-name = "ctor"
-version = "0.1.26"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
-dependencies = [
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
 name = "der"
-version = "0.7.6"
+version = "0.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56acb310e15652100da43d130af8d97b509e95af61aab1c5a7939ef24337ee17"
+checksum = "0c7ed52955ce76b1554f509074bb357d3fb8ac9b51288a65a3fd480d1dfba946"
 dependencies = [
  "const-oid",
  "pem-rfc7468",
  "zeroize",
 ]
 
 [[package]]
@@ -312,25 +302,14 @@
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "ghost"
-version = "0.1.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.18",
-]
-
-[[package]]
 name = "group"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0f9ef7462f7c099f518d754361858f86d8a07af53ba9af0fe635bbccb151a63"
 dependencies = [
  "ff",
  "rand_core",
@@ -356,65 +335,23 @@
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest 0.10.7",
 ]
 
 [[package]]
 name = "indoc"
-version = "0.3.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "47741a8bc60fb26eb8d6e0238bbb26d8575ff623fdc97b1a2c00c050b9684ed8"
-dependencies = [
- "indoc-impl",
- "proc-macro-hack",
-]
-
-[[package]]
-name = "indoc-impl"
-version = "0.3.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce046d161f000fffde5f432a0d034d0341dc152643b2598ed5bfce44c4f3a8f0"
-dependencies = [
- "proc-macro-hack",
- "proc-macro2",
- "quote",
- "syn 1.0.109",
- "unindent",
-]
-
-[[package]]
-name = "instant"
-version = "0.1.12"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
-dependencies = [
- "cfg-if",
-]
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "inventory"
-version = "0.1.11"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0eb5160c60ba1e809707918ee329adb99d222888155835c6feedba19f6c3fd4"
-dependencies = [
- "ctor",
- "ghost",
- "inventory-impl",
-]
-
-[[package]]
-name = "inventory-impl"
-version = "0.1.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e41b53715c6f0c4be49510bb82dee2c1e51c8586d885abe65396e82ed518548"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
+checksum = "c38a87a1e0e2752433cd4b26019a469112a25fb43b30f5ee9b3b898925c5a0f9"
 
 [[package]]
 name = "js-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
@@ -439,17 +376,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
@@ -460,14 +397,23 @@
 [[package]]
 name = "log"
 version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "num-bigint"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
 dependencies = [
  "autocfg",
  "num-integer",
@@ -524,54 +470,33 @@
 checksum = "81fec4625e73cf41ef4bb6846cafa6d44736525f442ba45e407c4a000a13996f"
 dependencies = [
  "group",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.11.2"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
+checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
- "instant",
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.8.6"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
- "instant",
  "libc",
  "redox_syscall",
  "smallvec",
- "winapi",
-]
-
-[[package]]
-name = "paste"
-version = "0.1.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45ca20c77d80be666aef2b45486da86238fabe33e38306bd3118fe4af33fa880"
-dependencies = [
- "paste-impl",
- "proc-macro-hack",
-]
-
-[[package]]
-name = "paste-impl"
-version = "0.1.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d95a7db200b97ef370c8e6de0088252f7e0dfff7d047a28528e47456c0fc98b6"
-dependencies = [
- "proc-macro-hack",
+ "windows-targets",
 ]
 
 [[package]]
 name = "pem-rfc7468"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88b39c9bfcfc231068454382784bb460aae594343fb030d46e9f50a645418412"
@@ -595,82 +520,88 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c2fcef82c0ec6eefcc179b978446c399b3cdf73c392c35604e399eee6df1ee3"
 dependencies = [
  "elliptic-curve",
 ]
 
 [[package]]
-name = "proc-macro-hack"
-version = "0.5.20+deprecated"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
-
-[[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.15.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7cf01dbf1c05af0a14c7779ed6f3aa9deac9c3419606ac9de537a2d649005720"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
+ "memoffset",
  "parking_lot",
- "paste",
  "pyo3-build-config",
+ "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.15.2"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "779239fc40b8e18bc8416d3a37d280ca9b9fb04bda54b98037bb6748595c2410"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
+name = "pyo3-ffi"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+dependencies = [
+ "libc",
+ "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.15.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67701eb32b1f9a9722b4bc54b548ff9d7ebfded011c12daece7b9063be1fd755"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
+ "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.15.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f44f09e825ee49a105f2c7b23ebee50886a9aee0746f4dd5a704138a64b0218a"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
- "pyo3-build-config",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -684,17 +615,17 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rfc6979"
 version = "0.4.0"
@@ -757,17 +688,17 @@
 dependencies = [
  "digest 0.10.7",
  "rand_core",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "spki"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d1e996ef02c474957d681f1b05213dfb0abab947b446a62d37770b23500184a"
 dependencies = [
@@ -790,40 +721,46 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "15e3fc8c0c74267e2df136e5e5fb656a464158aa57624053375eb9c8c6e25ae2"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
+name = "target-lexicon"
+version = "0.12.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
+
+[[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -856,15 +793,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -878,46 +815,81 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
-name = "winapi"
-version = "0.3.9"
+name = "windows-targets"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
```

