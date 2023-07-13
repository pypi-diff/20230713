# Comparing `tmp/zen_engine-0.6.1.tar.gz` & `tmp/zen_engine-0.7.0.tar.gz`

## Comparing `zen_engine-0.6.1.tar` & `zen_engine-0.7.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 zen_engine-0.6.1/local_dependencies/zen-expression/Cargo.toml
--rw-r--r--   0     1001      123     2347 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/README.md
--rw-r--r--   0     1001      123      625 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/benches/isolate.rs
--rw-r--r--   0     1001      123    93335 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/benches/lexer.rs
--rw-r--r--   0     1001      123    93602 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/benches/standard.rs
--rw-r--r--   0     1001      123      867 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/benches/unary.rs
--rw-r--r--   0     1001      123      970 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/ast.rs
--rw-r--r--   0     1001      123    18474 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/compiler.rs
--rw-r--r--   0     1001      123     1479 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/helpers.rs
--rw-r--r--   0     1001      123     6819 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/isolate.rs
--rw-r--r--   0     1001      123      769 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/codes.rs
--rw-r--r--   0     1001      123     2035 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/cursor.rs
--rw-r--r--   0     1001      123      404 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/error.rs
--rw-r--r--   0     1001      123     6311 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/lexer.rs
--rw-r--r--   0     1001      123       88 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/mod.rs
--rw-r--r--   0     1001      123      273 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/token.rs
--rw-r--r--   0     1001      123      203 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lib.rs
--rw-r--r--   0     1001      123     3950 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/opcodes.rs
--rw-r--r--   0     1001      123      922 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/definitions.rs
--rw-r--r--   0     1001      123      638 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/error.rs
--rw-r--r--   0     1001      123     4684 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/iter.rs
--rw-r--r--   0     1001      123      131 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/mod.rs
--rw-r--r--   0     1001      123     4073 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/standard/constants.rs
--rw-r--r--   0     1001      123    13361 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/standard/mod.rs
--rw-r--r--   0     1001      123     2506 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/unary/constants.rs
--rw-r--r--   0     1001      123     9209 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/unary/mod.rs
--rw-r--r--   0     1001      123    45084 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/vm.rs
--rw-r--r--   0     1001      123    20080 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/tests/isolate.rs
--rw-r--r--   0     1001      123    11822 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/tests/lexer.rs
--rw-r--r--   0     1001      123     9097 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/tests/standard.rs
--rw-r--r--   0     1001      123     5185 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/tests/unary.rs
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.6.1/local_dependencies/zen-engine/Cargo.toml
--rw-r--r--   0     1001      123     4305 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/README.md
--rw-r--r--   0     1001      123     1558 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/benches/engine.rs
--rw-r--r--   0     1001      123     2031 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/decision.rs
--rw-r--r--   0     1001      123     2605 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/engine.rs
--rw-r--r--   0     1001      123      972 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/error.rs
--rw-r--r--   0     1001      123     1651 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/decision.rs
--rw-r--r--   0     1001      123     2136 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/expression/mod.rs
--rw-r--r--   0     1001      123     1097 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/mod.rs
--rw-r--r--   0     1001      123     3046 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/script.rs
--rw-r--r--   0     1001      123     6485 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
--rw-r--r--   0     1001      123      528 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
--rw-r--r--   0     1001      123     1747 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/vm.rs
--rw-r--r--   0     1001      123    11347 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/graph.rs
--rw-r--r--   0     1001      123      115 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/mod.rs
--rw-r--r--   0     1001      123      745 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/node.rs
--rw-r--r--   0     1001      123      807 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/table/mod.rs
--rw-r--r--   0     1001      123     4940 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/table/zen.rs
--rw-r--r--   0     1001      123     4796 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/lib.rs
--rw-r--r--   0     1001      123      715 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/closure.rs
--rw-r--r--   0     1001      123     2449 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/filesystem.rs
--rw-r--r--   0     1001      123     1245 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/memory.rs
--rw-r--r--   0     1001      123      892 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/mod.rs
--rw-r--r--   0     1001      123      466 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/noop.rs
--rw-r--r--   0     1001      123     3152 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/model/mod.rs
--rw-r--r--   0     1001      123     9076 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/util/json_map.rs
--rw-r--r--   0     1001      123       25 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/util/mod.rs
--rw-r--r--   0     1001      123     2081 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/tests/decision.rs
--rw-r--r--   0     1001      123     4759 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/tests/engine.rs
--rw-r--r--   0     1001      123     1381 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/tests/model.rs
--rw-r--r--   0     1001      123      884 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/tests/support/mod.rs
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.6.1/Cargo.toml
--rw-r--r--   0     1001      123      135 2023-06-02 14:18:17.000000 zen_engine-0.6.1/.bumpversion.cfg
--rw-r--r--   0     1001      123      691 2023-06-02 14:18:17.000000 zen_engine-0.6.1/.gitignore
--rw-r--r--   0     1001      123     1057 2023-06-02 14:18:17.000000 zen_engine-0.6.1/LICENSE
--rw-r--r--   0     1001      123     5965 2023-06-02 14:18:17.000000 zen_engine-0.6.1/README.md
--rw-r--r--   0     1001      123     1578 2023-06-02 14:18:17.000000 zen_engine-0.6.1/index.py
--rw-r--r--   0     1001      123      966 2023-06-02 14:18:17.000000 zen_engine-0.6.1/pyproject.toml
--rw-r--r--   0     1001      123     1429 2023-06-02 14:18:17.000000 zen_engine-0.6.1/src/decision.rs
--rw-r--r--   0     1001      123     3012 2023-06-02 14:18:17.000000 zen_engine-0.6.1/src/engine.rs
--rw-r--r--   0     1001      123      335 2023-06-02 14:18:17.000000 zen_engine-0.6.1/src/lib.rs
--rw-r--r--   0     1001      123     1188 2023-06-02 14:18:17.000000 zen_engine-0.6.1/src/loader.rs
--rw-r--r--   0     1001      123     1122 2023-06-02 14:18:17.000000 zen_engine-0.6.1/src/value.rs
--rw-r--r--   0     1001      123    48962 2023-06-02 14:20:03.000000 zen_engine-0.6.1/Cargo.lock
--rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 zen_engine-0.7.0/local_dependencies/zen-expression/Cargo.toml
+-rw-r--r--   0     1001      123     2347 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/README.md
+-rw-r--r--   0     1001      123      625 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/benches/isolate.rs
+-rw-r--r--   0     1001      123    93335 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/benches/lexer.rs
+-rw-r--r--   0     1001      123    93602 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/benches/standard.rs
+-rw-r--r--   0     1001      123      867 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/benches/unary.rs
+-rw-r--r--   0     1001      123      970 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/ast.rs
+-rw-r--r--   0     1001      123    19250 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/compiler.rs
+-rw-r--r--   0     1001      123     1479 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/helpers.rs
+-rw-r--r--   0     1001      123     6819 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/isolate.rs
+-rw-r--r--   0     1001      123      769 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/codes.rs
+-rw-r--r--   0     1001      123     2035 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/cursor.rs
+-rw-r--r--   0     1001      123      404 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/error.rs
+-rw-r--r--   0     1001      123     6311 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/lexer.rs
+-rw-r--r--   0     1001      123       88 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/mod.rs
+-rw-r--r--   0     1001      123      273 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/token.rs
+-rw-r--r--   0     1001      123      203 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lib.rs
+-rw-r--r--   0     1001      123     4010 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/opcodes.rs
+-rw-r--r--   0     1001      123      922 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/definitions.rs
+-rw-r--r--   0     1001      123      638 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/error.rs
+-rw-r--r--   0     1001      123     5318 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/iter.rs
+-rw-r--r--   0     1001      123      131 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/mod.rs
+-rw-r--r--   0     1001      123     4286 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/standard/constants.rs
+-rw-r--r--   0     1001      123    14060 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/standard/mod.rs
+-rw-r--r--   0     1001      123     2604 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/unary/constants.rs
+-rw-r--r--   0     1001      123     9905 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/unary/mod.rs
+-rw-r--r--   0     1001      123    51034 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/vm.rs
+-rw-r--r--   0     1001      123    22433 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/tests/isolate.rs
+-rw-r--r--   0     1001      123    11822 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/tests/lexer.rs
+-rw-r--r--   0     1001      123     9097 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/tests/standard.rs
+-rw-r--r--   0     1001      123     5185 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/tests/unary.rs
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.7.0/local_dependencies/zen-engine/Cargo.toml
+-rw-r--r--   0     1001      123     4305 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/README.md
+-rw-r--r--   0     1001      123     1558 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/benches/engine.rs
+-rw-r--r--   0     1001      123     2031 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/decision.rs
+-rw-r--r--   0     1001      123     2605 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/engine.rs
+-rw-r--r--   0     1001      123      972 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/error.rs
+-rw-r--r--   0     1001      123     1651 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/decision.rs
+-rw-r--r--   0     1001      123     2136 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/expression/mod.rs
+-rw-r--r--   0     1001      123     1097 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/mod.rs
+-rw-r--r--   0     1001      123     3046 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/script.rs
+-rw-r--r--   0     1001      123     6485 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
+-rw-r--r--   0     1001      123      528 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
+-rw-r--r--   0     1001      123     1747 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/vm.rs
+-rw-r--r--   0     1001      123    11347 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/graph.rs
+-rw-r--r--   0     1001      123      115 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/mod.rs
+-rw-r--r--   0     1001      123      745 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/node.rs
+-rw-r--r--   0     1001      123      807 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/table/mod.rs
+-rw-r--r--   0     1001      123     4940 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/table/zen.rs
+-rw-r--r--   0     1001      123     4796 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/lib.rs
+-rw-r--r--   0     1001      123      715 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/closure.rs
+-rw-r--r--   0     1001      123     2449 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/filesystem.rs
+-rw-r--r--   0     1001      123     1245 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/memory.rs
+-rw-r--r--   0     1001      123      892 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/mod.rs
+-rw-r--r--   0     1001      123      466 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/noop.rs
+-rw-r--r--   0     1001      123     3152 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/model/mod.rs
+-rw-r--r--   0     1001      123     9076 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/util/json_map.rs
+-rw-r--r--   0     1001      123       25 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/util/mod.rs
+-rw-r--r--   0     1001      123     2081 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/tests/decision.rs
+-rw-r--r--   0     1001      123     4759 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/tests/engine.rs
+-rw-r--r--   0     1001      123     1381 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/tests/model.rs
+-rw-r--r--   0     1001      123      884 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/tests/support/mod.rs
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.7.0/Cargo.toml
+-rw-r--r--   0     1001      123      135 2023-07-13 09:18:18.000000 zen_engine-0.7.0/.bumpversion.cfg
+-rw-r--r--   0     1001      123      691 2023-07-13 09:18:18.000000 zen_engine-0.7.0/.gitignore
+-rw-r--r--   0     1001      123     1057 2023-07-13 09:18:18.000000 zen_engine-0.7.0/LICENSE
+-rw-r--r--   0     1001      123     5965 2023-07-13 09:18:18.000000 zen_engine-0.7.0/README.md
+-rw-r--r--   0     1001      123     1578 2023-07-13 09:18:18.000000 zen_engine-0.7.0/index.py
+-rw-r--r--   0     1001      123      966 2023-07-13 09:18:18.000000 zen_engine-0.7.0/pyproject.toml
+-rw-r--r--   0     1001      123     1429 2023-07-13 09:18:18.000000 zen_engine-0.7.0/src/decision.rs
+-rw-r--r--   0     1001      123     3012 2023-07-13 09:18:18.000000 zen_engine-0.7.0/src/engine.rs
+-rw-r--r--   0     1001      123      335 2023-07-13 09:18:18.000000 zen_engine-0.7.0/src/lib.rs
+-rw-r--r--   0     1001      123     1188 2023-07-13 09:18:18.000000 zen_engine-0.7.0/src/loader.rs
+-rw-r--r--   0     1001      123     1122 2023-07-13 09:18:18.000000 zen_engine-0.7.0/src/value.rs
+-rw-r--r--   0     1001      123    48278 2023-07-13 09:18:27.000000 zen_engine-0.7.0/Cargo.lock
+-rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.7.0/PKG-INFO
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/Cargo.toml` & `zen_engine-0.7.0/local_dependencies/zen-expression/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 bumpalo = "3.13.0"
 chrono = "0.4.26"
 hashbrown = { version = "0.13.2", features = ["bumpalo"] }
 humantime = "2.1.0"
 fastrand = "1.9.0"
 once_cell = "1.17.2"
 phf = { version = "0.11.1", features = ["macros"] }
+regex = "1.8.4"
 serde_json = { version = "1.0.96", features = ["arbitrary_precision"] }
 thiserror = "1.0.40"
 rust_decimal = { version = "1.29.1", features = ["maths-nopanic"] }
 rust_decimal_macros = "1.29.1"
 
 [[bench]]
 harness = false
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/README.md` & `zen_engine-0.7.0/local_dependencies/zen-expression/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/benches/isolate.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/benches/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/benches/lexer.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/benches/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/benches/standard.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/benches/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/benches/unary.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/benches/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/ast.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/ast.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/compiler.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/compiler.rs`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,24 @@
                     Ok(self.emit(Opcode::EndsWith))
                 }
                 "contains" => {
                     self.compile_argument(name, arguments, 0)?;
                     self.compile_argument(name, arguments, 1)?;
                     Ok(self.emit(Opcode::Contains))
                 }
+                "matches" => {
+                    self.compile_argument(name, arguments, 0)?;
+                    self.compile_argument(name, arguments, 1)?;
+                    Ok(self.emit(Opcode::Matches))
+                }
+                "extract" => {
+                    self.compile_argument(name, arguments, 0)?;
+                    self.compile_argument(name, arguments, 1)?;
+                    Ok(self.emit(Opcode::Extract))
+                }
                 "flatten" => {
                     self.compile_argument(name, arguments, 0)?;
                     Ok(self.emit(Opcode::Flatten))
                 }
                 "upper" => {
                     self.compile_argument(name, arguments, 0)?;
                     Ok(self.emit(Opcode::Uppercase))
@@ -337,14 +347,22 @@
                     self.compile_argument(name, arguments, 0)?;
                     Ok(self.emit(Opcode::Abs))
                 }
                 "avg" => {
                     self.compile_argument(name, arguments, 0)?;
                     Ok(self.emit(Opcode::Average))
                 }
+                "median" => {
+                    self.compile_argument(name, arguments, 0)?;
+                    Ok(self.emit(Opcode::Median))
+                }
+                "mode" => {
+                    self.compile_argument(name, arguments, 0)?;
+                    Ok(self.emit(Opcode::Mode))
+                }
                 "max" => {
                     self.compile_argument(name, arguments, 0)?;
                     Ok(self.emit(Opcode::Max))
                 }
                 "min" => {
                     self.compile_argument(name, arguments, 0)?;
                     Ok(self.emit(Opcode::Min))
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/helpers.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/isolate.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/codes.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/codes.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/cursor.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/cursor.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/lexer.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/opcodes.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/opcodes.rs`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,16 @@
     In,
     Less,
     More,
     LessOrEqual,
     MoreOrEqual,
     Abs,
     Average,
+    Median,
+    Mode,
     Min,
     Max,
     Round,
     Floor,
     Ceil,
     Sum,
     Random,
@@ -104,14 +106,16 @@
     },
     Contains,
     DateManipulation(&'a str),
     Uppercase,
     Lowercase,
     StartsWith,
     EndsWith,
+    Matches,
+    Extract,
     Slice,
     Array,
     Len,
     ParseDateTime,
     ParseTime,
     ParseDuration,
     IncrementIt,
@@ -128,15 +132,15 @@
     type Error = ();
 
     fn try_from(value: &Variable<'_>) -> Result<Self, Self::Error> {
         match value {
             Variable::Null => Ok(Value::Null),
             Variable::Bool(b) => Ok(Value::Bool(*b)),
             Variable::Number(n) => Ok(Value::Number(
-                Number::from_str(n.to_string().as_str()).map_err(|_| ())?,
+                Number::from_str(n.normalize().to_string().as_str()).map_err(|_| ())?,
             )),
             Variable::String(s) => Ok(Value::String(s.to_string())),
             Variable::Array(arr) => {
                 let mut v = Vec::<Value>::with_capacity(arr.len());
                 for i in *arr {
                     v.push(Value::try_from(*i)?)
                 }
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/definitions.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/definitions.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/error.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/iter.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/iter.rs`

 * *Files 8% similar despite different names*

```diff
@@ -13,33 +13,56 @@
 #[derive(Debug)]
 pub(crate) struct ParserIterator<'a, 'b> {
     tokens: &'a Vec<Token<'a>>,
     current: Cell<&'a Token<'a>>,
     position: Cell<usize>,
     bump: &'b Bump,
     is_done: Cell<bool>,
+    has_interval: bool,
 }
 
 impl<'a, 'b> ParserIterator<'a, 'b> {
     pub fn try_new(tokens: &'a Vec<Token<'a>>, bump: &'b Bump) -> Result<Self, ParserError> {
         let current = tokens.get(0).ok_or(ParserError::TokenOutOfBounds)?;
+        let has_interval = tokens
+            .iter()
+            .any(|t| t.kind == TokenKind::Operator && t.value == "..");
 
         Ok(Self {
             tokens,
             bump,
+            has_interval,
             current: Cell::new(current),
             position: Cell::new(0),
             is_done: Cell::new(false),
         })
     }
 
+    pub fn has_interval(&self) -> bool {
+        self.has_interval
+    }
+
     pub fn current(&self) -> &'a Token<'a> {
         self.current.get()
     }
 
+    pub fn position(&self) -> usize {
+        self.position.get()
+    }
+
+    pub fn set_position(&self, position: usize) -> ParserResult<()> {
+        let Some(token) = self.tokens.get(position) else {
+            return Err(ParserError::TokenOutOfBounds)
+        };
+
+        self.position.set(position);
+        self.current.set(token);
+        Ok(())
+    }
+
     pub fn is_done(&self) -> bool {
         self.is_done.get()
     }
 
     pub fn next(&self) -> ParserResult<()> {
         self.position.set(self.position.get() + 1);
 
@@ -62,14 +85,15 @@
 
     pub fn expect(&self, kind: TokenKind, values: TokenValues<'a>) -> Result<(), ParserError> {
         self.token_cmp(kind, values)?;
         self.next()?;
         Ok(())
     }
 
+    #[allow(dead_code)]
     pub fn lookup(&self, dx: usize, kind: TokenKind, values: TokenValues<'a>) -> bool {
         self.token_cmp_at_bool(self.position.get() + dx, kind, values)
     }
 
     pub fn lookup_back(&self, dx: usize, kind: TokenKind, values: TokenValues<'a>) -> bool {
         if self.position.get() < dx {
             return false;
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/standard/constants.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/standard/constants.rs`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
         "abs" => BuiltIn { arity: Arity::Single },
         "sum" => BuiltIn { arity: Arity::Single },
         "avg" => BuiltIn { arity: Arity::Single },
         "min" => BuiltIn { arity: Arity::Single },
         "max" => BuiltIn { arity: Arity::Single },
         "rand" => BuiltIn { arity: Arity::Single },
+        "median" => BuiltIn { arity: Arity::Single },
+        "mode" => BuiltIn { arity: Arity::Single },
 
         "floor" => BuiltIn { arity: Arity::Single },
         "ceil" => BuiltIn { arity: Arity::Single },
         "round" => BuiltIn { arity: Arity::Single },
 
         "dayOfWeek" => BuiltIn { arity: Arity::Single },
         "dayOfMonth" => BuiltIn { arity: Arity::Single },
@@ -40,14 +42,17 @@
         "seasonOfYear" => BuiltIn { arity: Arity::Single },
         "monthString" => BuiltIn { arity: Arity::Single },
         "weekdayString" => BuiltIn { arity: Arity::Single },
 
         "startsWith" => BuiltIn { arity: Arity::Dual },
         "endsWith" => BuiltIn { arity: Arity::Dual },
         "contains" => BuiltIn { arity: Arity::Dual },
+        "matches" => BuiltIn { arity: Arity::Dual },
+        "extract" => BuiltIn { arity: Arity::Dual },
+
         "all" => BuiltIn { arity: Arity::Closure },
         "some" => BuiltIn { arity: Arity::Closure },
         "none" => BuiltIn { arity: Arity::Closure },
         "filter" => BuiltIn { arity: Arity::Closure },
         "map" => BuiltIn { arity: Arity::Closure },
         "count" => BuiltIn { arity: Arity::Closure },
         "one" => BuiltIn { arity: Arity::Closure },
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/standard/mod.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/standard/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -174,29 +174,51 @@
             }
         }
 
         self.parse_postfix(node)
     }
 
     fn parse_interval(&self) -> ParserResult<Option<&'b Node<'b>>> {
-        if self.iterator.current().kind != TokenKind::Bracket {
+        // Performance optimisation: skip if expression does not contain an interval for faster evaluation
+        if !self.iterator.has_interval() {
             return Ok(None);
         }
 
-        if !self.iterator.lookup(2, TokenKind::Operator, Some(&[".."])) {
+        if self.iterator.current().kind != TokenKind::Bracket {
             return Ok(None);
         }
 
+        let initial_position = self.iterator.position();
         let left_bracket = self.iterator.current().value;
-        self.iterator.expect(TokenKind::Bracket, None)?;
-        let left = self.parse_primary_expression()?;
-        self.iterator.expect(TokenKind::Operator, Some(&[".."]))?;
-        let right = self.parse_primary_expression()?;
+        if let Err(_) = self.iterator.expect(TokenKind::Bracket, None) {
+            self.iterator.set_position(initial_position)?;
+            return Ok(None);
+        };
+
+        let Ok(left) = self.parse_primary_expression() else {
+            self.iterator.set_position(initial_position)?;
+            return Ok(None);
+        };
+
+        if let Err(_) = self.iterator.expect(TokenKind::Operator, Some(&[".."])) {
+            self.iterator.set_position(initial_position)?;
+            return Ok(None);
+        };
+
+        let Ok(right) = self.parse_primary_expression() else {
+            self.iterator.set_position(initial_position)?;
+            return Ok(None);
+        };
+
         let right_bracket = self.iterator.current().value;
-        self.iterator.expect(TokenKind::Bracket, None)?;
+
+        if let Err(_) = self.iterator.expect(TokenKind::Bracket, None) {
+            self.iterator.set_position(initial_position)?;
+            return Ok(None);
+        };
 
         let interval_node = self.iterator.node(Node::Interval {
             left_bracket: self.iterator.str_value(left_bracket),
             left,
             right,
             right_bracket: self.iterator.str_value(right_bracket),
         })?;
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/unary/constants.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/unary/constants.rs`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
     "abs" => BuiltIn { arity: Arity::Single },
     "sum" => BuiltIn { arity: Arity::Single },
     "avg" => BuiltIn { arity: Arity::Single },
     "min" => BuiltIn { arity: Arity::Single },
     "max" => BuiltIn { arity: Arity::Single },
     "rand" => BuiltIn { arity: Arity::Single },
+    "median" => BuiltIn { arity: Arity::Single },
+    "mode" => BuiltIn { arity: Arity::Single },
 
     "floor" => BuiltIn { arity: Arity::Single },
     "ceil" => BuiltIn { arity: Arity::Single },
     "round" => BuiltIn { arity: Arity::Single },
 
     "flatten" => BuiltIn { arity: Arity::Single },
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/unary/mod.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/unary/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -131,35 +131,57 @@
             }
         }
 
         Ok(node_left)
     }
 
     fn parse_interval(&self, node: &'b Node<'b>) -> ParserResult<Option<&'b Node<'b>>> {
-        let current_token = self.iterator.current();
-        if current_token.kind != TokenKind::Bracket {
+        // Performance optimisation: skip if expression does not contain an interval for faster evaluation
+        if !self.iterator.has_interval() {
             return Ok(None);
         }
 
-        if !self.iterator.lookup(2, TokenKind::Operator, Some(&[".."])) {
+        let current_token = self.iterator.current();
+        if current_token.kind != TokenKind::Bracket {
             return Ok(None);
         }
 
+        let initial_position = self.iterator.position();
         let should_wrap =
             !self
                 .iterator
                 .lookup_back(1, TokenKind::Operator, Some(&["not in", "in"]));
 
         let left_bracket = self.iterator.current().value;
-        self.iterator.expect(TokenKind::Bracket, None)?;
-        let left = self.parse_primary()?;
-        self.iterator.expect(TokenKind::Operator, Some(&[".."]))?;
-        let right = self.parse_primary()?;
+        if let Err(_) = self.iterator.expect(TokenKind::Bracket, None) {
+            self.iterator.set_position(initial_position)?;
+            return Ok(None);
+        }
+
+        let Ok(left) = self.parse_primary() else {
+            self.iterator.set_position(initial_position)?;
+            return Ok(None);
+        };
+
+        if let Err(_) = self.iterator.expect(TokenKind::Operator, Some(&[".."])) {
+            self.iterator.set_position(initial_position)?;
+            return Ok(None);
+        }
+
+        let Ok(right) = self.parse_primary() else {
+            self.iterator.set_position(initial_position)?;
+            return Ok(None);
+        };
+
         let right_bracket = self.iterator.current().value;
-        self.iterator.expect(TokenKind::Bracket, None)?;
+
+        if let Err(_) = self.iterator.expect(TokenKind::Bracket, None) {
+            self.iterator.set_position(initial_position)?;
+            return Ok(None);
+        }
 
         let interval_node = self.iterator.node(Node::Interval {
             left,
             left_bracket: self.iterator.str_value(left_bracket),
             right,
             right_bracket: self.iterator.str_value(right_bracket),
         })?;
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/src/vm.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/src/vm.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 use bumpalo::Bump;
 use chrono::NaiveDateTime;
 use chrono::{Datelike, Timelike};
+use regex::Regex;
 use rust_decimal::prelude::ToPrimitive;
 use rust_decimal::{Decimal, MathematicalOps};
+use rust_decimal_macros::dec;
+use std::collections::HashMap;
 use thiserror::Error;
 
 use crate::helpers::{date_time, time};
 use crate::opcodes::Variable::{Array, Bool, Int, Interval, Null, Number, Object, String};
 use crate::opcodes::{Opcode, Variable};
 use crate::vm::VMError::{OpcodeErr, OpcodeOutOfBounds, ParseDateTimeErr, StackOutOfBounds};
 
@@ -506,14 +509,109 @@
                             return Err(OpcodeErr {
                                 opcode: "Average".into(),
                                 message: "Unsupported type".into(),
                             })
                         }
                     }
                 }
+                Opcode::Median => {
+                    let Array(arr) = self.pop()? else {
+                        return Err(OpcodeErr {
+                            opcode: "Median".into(),
+                            message: "Unsupported type".into()
+                        })
+                    };
+
+                    let mut num_arr = arr
+                        .iter()
+                        .map(|n| match n {
+                            Number(num) => Ok(num),
+                            _ => Err(OpcodeErr {
+                                opcode: "Median".into(),
+                                message: "Unsupported type".into(),
+                            }),
+                        })
+                        .collect::<Result<Vec<_>, _>>()?;
+
+                    if num_arr.len() == 0 {
+                        return Err(OpcodeErr {
+                            opcode: "Median".into(),
+                            message: "Array is empty".into(),
+                        });
+                    }
+
+                    num_arr.sort();
+
+                    let center = num_arr.len() / 2;
+                    if num_arr.len() % 2 == 1 {
+                        let center_num = num_arr.get(center).ok_or_else(|| OpcodeErr {
+                            opcode: "Median".into(),
+                            message: "Array out of bounds".into(),
+                        })?;
+
+                        self.push(Number((*center_num).clone()));
+                    } else {
+                        let center_left = num_arr.get(center - 1).ok_or_else(|| OpcodeErr {
+                            opcode: "Median".into(),
+                            message: "Array out of bounds".into(),
+                        })?;
+
+                        let center_right = num_arr.get(center).ok_or_else(|| OpcodeErr {
+                            opcode: "Median".into(),
+                            message: "Array out of bounds".into(),
+                        })?;
+
+                        let median = ((**center_left) + (**center_right)) / dec!(2);
+                        self.push(Number(median));
+                    }
+                }
+                Opcode::Mode => {
+                    let Array(arr) = self.pop()? else {
+                        return Err(OpcodeErr {
+                            opcode: "Mode".into(),
+                            message: "Unsupported type".into()
+                        })
+                    };
+
+                    let num_arr = arr
+                        .iter()
+                        .map(|n| match n {
+                            Number(num) => Ok(num),
+                            _ => Err(OpcodeErr {
+                                opcode: "Mode".into(),
+                                message: "Unsupported type".into(),
+                            }),
+                        })
+                        .collect::<Result<Vec<_>, _>>()?;
+
+                    if num_arr.len() == 0 {
+                        return Err(OpcodeErr {
+                            opcode: "Mode".into(),
+                            message: "Array is empty".into(),
+                        });
+                    }
+
+                    let mut map = HashMap::new();
+                    num_arr.iter().for_each(|n| {
+                        let count = map.entry(**n).or_insert(0);
+                        *count += 1;
+                    });
+
+                    let maybe_mode = map
+                        .iter()
+                        .max_by_key(|&(_, count)| *count)
+                        .map(|(val, _)| val);
+
+                    let mode = maybe_mode.ok_or_else(|| OpcodeErr {
+                        opcode: "Mode".into(),
+                        message: "Failed to find most common element".into(),
+                    })?;
+
+                    self.push(Number(*mode));
+                }
                 Opcode::Min => {
                     let var = self.pop()?;
 
                     match var {
                         Array(arr) => {
                             let first_item = arr.get(0).ok_or_else(|| OpcodeErr {
                                 opcode: "Min".into(),
@@ -829,14 +927,64 @@
                             return Err(OpcodeErr {
                                 opcode: "EndsWith".into(),
                                 message: "Unsupported type".into(),
                             })
                         }
                     }
                 }
+                Opcode::Matches => {
+                    let b = self.pop()?;
+                    let a = self.pop()?;
+
+                    let (String(a), String(b)) = (a, b) else {
+                        return Err(OpcodeErr {
+                            opcode: "Matches".into(),
+                            message: "Unsupported type".into(),
+                        })
+                    };
+
+                    let regex = Regex::new(b).map_err(|_| OpcodeErr {
+                        opcode: "Matches".into(),
+                        message: "Invalid regular expression".into(),
+                    })?;
+
+                    self.push(Bool(regex.is_match(a)));
+                }
+                Opcode::Extract => {
+                    let b = self.pop()?;
+                    let a = self.pop()?;
+
+                    let (String(a), String(b)) = (a, b) else {
+                        return Err(OpcodeErr {
+                            opcode: "Matches".into(),
+                            message: "Unsupported type".into(),
+                        })
+                    };
+
+                    let regex = Regex::new(b).map_err(|_| OpcodeErr {
+                        opcode: "Matches".into(),
+                        message: "Invalid regular expression".into(),
+                    })?;
+
+                    let captures = regex
+                        .captures(a)
+                        .map(|capture| {
+                            capture
+                                .iter()
+                                .map(|c| c.map(|c| c.as_str()))
+                                .filter_map(|c| c)
+                                .map(|s| {
+                                    self.bump.alloc(String(self.bump.alloc_str(s))) as &Variable
+                                })
+                                .collect::<Vec<_>>()
+                        })
+                        .unwrap_or_default();
+
+                    self.push(Array(self.bump.alloc_slice_copy(captures.as_slice())));
+                }
                 Opcode::DateManipulation(operation) => {
                     let timestamp = self.pop()?;
 
                     let time = match timestamp {
                         String(a) => date_time(a)?,
                         Number(a) => NaiveDateTime::from_timestamp_opt(
                             a.to_i64().ok_or_else(|| OpcodeErr {
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/tests/isolate.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/tests/isolate.rs`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,22 @@
                     result: json!(false),
                 },
                 TestCase {
                     expr: r#"date("2022-04-04") > date("2022-03-04")"#,
                     result: json!(true),
                 },
                 TestCase {
+                    expr: r#"date("2022-04-04") in [date("2022-03-04")..date("2022-04-04")]"#,
+                    result: json!(true),
+                },
+                TestCase {
+                    expr: r#"date("2022-04-04") in [date("2022-03-04")..date("2022-04-04"))"#,
+                    result: json!(false),
+                },
+                TestCase {
                     expr: r#"time("2022-04-04T21:48:30Z") > time("2022-05-04 21:48:20")"#,
                     result: json!(true),
                 },
                 TestCase {
                     expr: r#"time("21:48:30") > time("2022-05-04T21:48:30+01:00")"#,
                     result: json!(true),
                 },
@@ -362,14 +370,26 @@
                     expr: r#"10 % 4"#,
                     result: json!(2),
                 },
                 TestCase {
                     expr: r#"true ? 10.0 == 10 : 1.0"#,
                     result: json!(true),
                 },
+                TestCase {
+                    expr: r#"median([1, 2, 3])"#,
+                    result: json!(2),
+                },
+                TestCase {
+                    expr: r#"median([1, 2, 3, 4])"#,
+                    result: json!(2.5),
+                },
+                TestCase {
+                    expr: r#"mode([1, 1, 2, 2, 2, 5, 6, 9])"#,
+                    result: json!(2),
+                },
             ]),
         },
         TestEnv {
             env: json!({}),
             cases: Vec::from([
                 TestCase {
                     expr: r#"223_000.48 - 120_000_00 / 100"#,
@@ -474,14 +494,35 @@
                 },
                 TestCase {
                     expr: r#"flatMap(nestedArray, #)"#,
                     result: json!([1, 2, 3, 4, 5, 6]),
                 },
             ]),
         },
+        TestEnv {
+            env: json!({}),
+            cases: Vec::from([
+                TestCase {
+                    expr: r#"extract("2022-02-01", "(\d{4})-(\d{2})-(\d{2})")"#,
+                    result: json!(["2022-02-01", "2022", "02", "01"]),
+                },
+                TestCase {
+                    expr: r#"all(["babble", "bebble", "bibble", "bobble", "bubble"], matches(#, "b[aeiou]bble"))"#,
+                    result: json!(true),
+                },
+                TestCase {
+                    expr: r#"none(["babble", "bebble", "bibble", "bobble", "bubble"], matches(#, "b[aeiou]bblo"))"#,
+                    result: json!(true),
+                },
+                TestCase {
+                    expr: r#"extract("foo.bar", "(\w+)\.(\w+)")"#,
+                    result: json!(["foo.bar", "foo", "bar"]),
+                },
+            ]),
+        },
     ]);
 
     let isolate = Isolate::default();
 
     for TestEnv { env, cases } in tests {
         isolate.inject_env(&env);
 
@@ -511,14 +552,34 @@
             cases: Vec::from([TestCase {
                 expr: r#"some($, # == "admin")"#,
                 result: json!(true),
             }]),
         },
         UnaryTestEnv {
             env: json!({
+                "input": "2023-01-02"
+            }),
+            reference: "date(input)",
+            cases: Vec::from([
+                TestCase {
+                    expr: r#"[date("2023-01-01")..date("2023-01-03")]"#,
+                    result: json!(true),
+                },
+                TestCase {
+                    expr: r#"[date("2023-02-01")..date("2023-01-03")]"#,
+                    result: json!(false),
+                },
+                TestCase {
+                    expr: r#"$ in [date("2023-01-01")..date("2023-01-03")]"#,
+                    result: json!(true),
+                },
+            ]),
+        },
+        UnaryTestEnv {
+            env: json!({
                 "customer": {
                     "groups": ["admin", "user"],
                     "purchaseAmounts": [100, 200, 400, 800]
                 }
             }),
             reference: "sum(filter(customer.purchaseAmounts, # < 300))",
             cases: Vec::from([
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/tests/lexer.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/tests/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/tests/standard.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/tests/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-expression/tests/unary.rs` & `zen_engine-0.7.0/local_dependencies/zen-expression/tests/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/Cargo.toml` & `zen_engine-0.7.0/local_dependencies/zen-engine/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 async-recursion = "1.0.4"
 anyhow = "1.0.71"
 thiserror = "1.0.40"
 async-trait = "0.1.68"
 bincode = { version = "2.0.0-rc.3", optional = true }
 serde_json = { version = "1.0.96", features = ["arbitrary_precision"] }
 serde = { version = "1.0.163", features = ["derive"] }
-serde_v8 = { version = "0.100.0" }
+serde_v8 = { version = "0.103.0" }
 once_cell = { version = "1.17.2" }
 futures = "0.3.28"
-v8 = { version = "0.73.0" }
+v8 = { version = "0.74.0" }
 zen-expression = { path = "../zen-expression", version = "0.5.2" }
 
 [features]
 bincode = ["dep:bincode"]
 
 [[bench]]
 harness = false
```

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/README.md` & `zen_engine-0.7.0/local_dependencies/zen-engine/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/benches/engine.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/benches/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/decision.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/engine.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/error.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/decision.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/expression/mod.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/expression/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/mod.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/script.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/script.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/scripts/internals.js` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/vm.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/vm.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/graph.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/graph.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/node.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/node.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/table/mod.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/table/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/table/zen.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/table/zen.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/lib.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/closure.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/closure.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/filesystem.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/filesystem.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/memory.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/memory.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/mod.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/model/mod.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/model/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/src/util/json_map.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/src/util/json_map.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/tests/decision.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/tests/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/tests/engine.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/tests/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/tests/model.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/tests/model.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/local_dependencies/zen-engine/tests/support/mod.rs` & `zen_engine-0.7.0/local_dependencies/zen-engine/tests/support/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/.gitignore` & `zen_engine-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/LICENSE` & `zen_engine-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/README.md` & `zen_engine-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/index.py` & `zen_engine-0.7.0/index.py`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/pyproject.toml` & `zen_engine-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/src/decision.rs` & `zen_engine-0.7.0/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/src/engine.rs` & `zen_engine-0.7.0/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/src/loader.rs` & `zen_engine-0.7.0/src/loader.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/src/value.rs` & `zen_engine-0.7.0/src/value.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.1/Cargo.lock` & `zen_engine-0.7.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
+name = "adler"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
 name = "ahash"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
 dependencies = [
  "getrandom",
  "once_cell",
@@ -23,17 +38,17 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
@@ -53,59 +68,74 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstyle"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
+checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
 
 [[package]]
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "arrayvec"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
+checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "async-recursion"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "a564d521dd56509c4c47480d00b80ee55f7e385ae48db5744c67ad50c92d2ebf"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "backtrace"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "bincode"
 version = "2.0.0-rc.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f11ea1a0346b94ef188834a65c068a03aec181c94896d481d7a0a40d85b0ce95"
 dependencies = [
  "bincode_derive",
  "serde",
@@ -124,17 +154,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.3.1"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6776fc96284a0bb647b615056fc496d1fe1644a7ab01829818a6d91cae888b84"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
 
 [[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
@@ -287,29 +317,28 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.1"
+version = "4.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4ed2379f8603fa2b7509891660e802b88c70a79a6427a70abb5968054de2c28"
+checksum = "1640e5cc7fb47dbb8338fd471b105e7ed6c3cb2aeb00c2e067127ffd3764a05d"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.1"
+version = "4.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72394f3339a76daf211e57d4bcb374410f3965dcc606dd0e03738c7888766980"
+checksum = "98c59138d527eeaf9b53f35a77fcc1fad9d883116070c63d5de1c7dc7b00c72b"
 dependencies = [
  "anstyle",
- "bitflags 1.3.2",
  "clap_lex",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -392,42 +421,42 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "ctor"
-version = "0.2.2"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1586fa608b1dab41f667475b4a41faec5ba680aee428bfa5de4ea520fdc6e901"
+checksum = "1f34ba9a9bcb8645379e9de8cb3ecfcf4d1c85ba66d90deb3259206fa5aa193b"
 dependencies = [
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
@@ -449,15 +478,15 @@
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -543,15 +572,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -578,24 +607,30 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
 name = "half"
 version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
 name = "hashbrown"
@@ -614,38 +649,29 @@
 dependencies = [
  "ahash 0.8.3",
  "bumpalo",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.56"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
@@ -672,97 +698,85 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "io-lifetimes"
-version = "1.0.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
-dependencies = [
- "hermit-abi 0.3.1",
- "libc",
- "windows-sys 0.48.0",
-]
-
-[[package]]
 name = "is-terminal"
-version = "0.4.7"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
- "hermit-abi 0.3.1",
- "io-lifetimes",
+ "hermit-abi",
  "rustix",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
 
 [[package]]
 name = "js-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
  "cfg-if",
  "winapi",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.8"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.18"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
@@ -772,21 +786,39 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
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
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
 name = "napi"
-version = "2.13.1"
+version = "2.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7f0a2e93526dd9c8c522d72a4d0c88678be8966fabe9fb8f2947fde6339b682"
+checksum = "0ede2d12cd6fce44da537a4be1f5510c73be2506c2e32dfaaafd1f36968f3a0e"
 dependencies = [
  "anyhow",
- "bitflags 2.3.1",
+ "bitflags 2.3.3",
  "ctor",
  "napi-derive",
  "napi-sys",
  "once_cell",
  "serde",
  "serde_json",
  "tokio",
@@ -865,27 +897,36 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
+name = "object"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "once_cell"
-version = "1.17.2"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
@@ -897,103 +938,103 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "phf"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
+checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
 dependencies = [
  "phf_macros",
  "phf_shared",
 ]
 
 [[package]]
 name = "phf_generator"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1181c94580fa345f50f19d738aaa39c0ed30a600d95cb2d3e23f94266f14fbf"
+checksum = "48e4cc64c2ad9ebe670cb8fd69dd50ae301650392e81c05f9bfcb2d5bdbc24b0"
 dependencies = [
  "phf_shared",
  "rand",
 ]
 
 [[package]]
 name = "phf_macros"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92aacdc5f16768709a569e913f7451034034178b05bdc8acda226659a3dccc66"
+checksum = "3444646e286606587e49f3bcf1679b8cef1dc2c5ecc29ddacaffc305180d464b"
 dependencies = [
  "phf_generator",
  "phf_shared",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "phf_shared"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
+checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "plotters"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2538b639e642295546c50fcd545198c9d64ee2a38620a628724a3b266d5fbf97"
+checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
 dependencies = [
  "num-traits",
  "plotters-backend",
  "plotters-svg",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "plotters-backend"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "193228616381fecdc1224c62e96946dfbc73ff4384fba576e052ff8c1bea8142"
+checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
 
 [[package]]
 name = "plotters-svg"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9a81d2759aae1dae668f783c308bc5c8ebd191ff4184aaa1b37f65a6ae5a56f"
+checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
@@ -1007,17 +1048,17 @@
 checksum = "1d6ea3c4595b96363c13943497db34af4460fb474a95c43f4446ad341b8c9785"
 dependencies = [
  "toml",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.59"
+version = "1.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
+checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.1.4"
@@ -1044,15 +1085,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "serde",
  "unindent",
 ]
@@ -1108,17 +1149,17 @@
 dependencies = [
  "pyo3",
  "serde",
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
@@ -1175,37 +1216,49 @@
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.3"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "rend"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "581008d2099240d37fb08d77ad713bcaec2c4d89d50b5b21a8bb1996bbab68ab"
 dependencies = [
@@ -1238,17 +1291,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "rust_decimal"
-version = "1.29.1"
+version = "1.30.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26bd36b60561ee1fb5ec2817f198b6fd09fa571c897a5e86d1487cfc2b096dfc"
+checksum = "d0446843641c69436765a35a5a77088e28c2e6a12da93e84aa3ab1cd4aa5a042"
 dependencies = [
  "arrayvec",
  "borsh",
  "bytecheck",
  "byteorder",
  "bytes",
  "num-traits",
@@ -1256,50 +1309,55 @@
  "rkyv",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "rust_decimal_macros"
-version = "1.29.1"
+version = "1.30.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e773fd3da1ed42472fdf3cfdb4972948a555bc3d73f5e0bdb99d17e7b54c687"
+checksum = "7ca5c398d85f83b9a44de754a2048625a8c5eafcf070da7b8f116b685e2f6608"
 dependencies = [
  "quote",
  "rust_decimal",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.19"
+version = "0.38.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
+checksum = "0a962918ea88d644592894bc6dc55acc6c0956488adcebbfb6e273506b7fd6e5"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.3.3",
  "errno",
- "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1322,57 +1380,57 @@
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
-version = "0.11.9"
+version = "0.11.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "416bda436f9aab92e02c8e10d49a15ddd339cea90b6e340fe51ed97abb548294"
+checksum = "5a16be4fe5320ade08736447e3198294a5ea9a6d44dde6f35f0a5e06859c427a"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "b5062a995d481b2308b6064e9af76011f2921c35f97b0468811ed9f6cd91dfed"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_v8"
-version = "0.100.0"
+version = "0.103.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e66031ca2e6c4b682cf0377633992f3c0ec3fda65701ff14fee99d6ff5eeeeb"
+checksum = "4af59e98cf3d92adb88b1f6df912d892a8ef84c29a23b8340028fb8b326eb078"
 dependencies = [
  "bytes",
  "derive_more",
  "num-bigint",
  "serde",
  "serde_bytes",
  "smallvec",
@@ -1399,70 +1457,70 @@
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
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
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
@@ -1495,50 +1553,50 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "num_cpus",
  "pin-project-lite",
  "tokio-macros",
- "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "toml"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unicode-segmentation"
 version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
@@ -1546,23 +1604,23 @@
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "uuid"
-version = "1.3.3"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
+checksum = "d023da39d1fde5a8a3fe1f3e01ca9632ada0a63e9797de55a879d6e2236277be"
 
 [[package]]
 name = "v8"
-version = "0.73.0"
+version = "0.74.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1bd3f04ba5065795dae6e3db668ff0b628920fbd2e39c1755e9b62d93660c3c"
+checksum = "7568bf38565bd5b350d96abbf3d09417e8c9dd74fbb38860e91b759e46f9009c"
 dependencies = [
  "bitflags 1.3.2",
  "fslock",
  "once_cell",
  "which",
 ]
 
@@ -1598,71 +1656,71 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
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
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
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
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "web-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "which"
@@ -1708,145 +1766,79 @@
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
-name = "windows-targets"
-version = "0.48.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
-dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
-]
-
-[[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
@@ -1885,14 +1877,15 @@
  "chrono",
  "criterion",
  "fastrand",
  "hashbrown 0.13.2",
  "humantime",
  "once_cell",
  "phf",
+ "regex",
  "rust_decimal",
  "rust_decimal_macros",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
@@ -1906,15 +1899,15 @@
  "napi-derive",
  "serde_json",
  "zen-engine",
 ]
 
 [[package]]
 name = "zen-python"
-version = "0.6.1"
+version = "0.7.0"
 dependencies = [
  "anyhow",
  "async-trait",
  "futures",
  "pyo3",
  "pythonize",
  "serde",
```

### Comparing `zen_engine-0.6.1/PKG-INFO` & `zen_engine-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-engine
-Version: 0.6.1
+Version: 0.7.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: bumpver; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
```

