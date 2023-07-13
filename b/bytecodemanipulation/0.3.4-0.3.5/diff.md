# Comparing `tmp/bytecodemanipulation-0.3.4.tar.gz` & `tmp/bytecodemanipulation-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecodemanipulation-0.3.4.tar", last modified: Wed Jul  5 11:00:12 2023, max compression
+gzip compressed data, was "bytecodemanipulation-0.3.5.tar", last modified: Thu Jul 13 14:49:46 2023, max compression
```

## Comparing `bytecodemanipulation-0.3.4.tar` & `bytecodemanipulation-0.3.5.tar`

### file list

```diff
@@ -1,165 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.484822 bytecodemanipulation-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-05 11:00:12.484822 bytecodemanipulation-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.452822 bytecodemanipulation-0.3.4/bytecodemanipulation/
--rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/Emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/Mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/MutableFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/MutableFunctionHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27037 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/Optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/Specialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/TypeEnforcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/annotated_std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.452822 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/
--rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/AbstractBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21487 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/syntax_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.456822 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/CommonUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.456822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.456822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/builtin_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.460822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.468822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AssertAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15500 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    27035 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    20630 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/RawAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.468822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/ExceptionInstructionCodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/LocationInformationHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/assembly_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.476822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    22437 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/specialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.476822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/assembly_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.480822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/specialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.480822 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_12/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/mixin_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.484822 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/CacheEntryCreation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/CodeObjectBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/ExceptionTable.py
--rw-r--r--   0 runner    (1001) docker     (123)    25709 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/Instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/OpcodeReplacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/Opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/optimise_self.py
--rw-r--r--   0 runner    (1001) docker     (123)    17702 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/optimiser_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/bytecodemanipulation/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.452822 bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-05 11:00:12.000000 bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-05 11:00:12.000000 bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:00:12.000000 bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 11:00:12.000000 bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 11:00:12.484822 bytecodemanipulation-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-05 11:00:05.000000 bytecodemanipulation-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:00:12.484822 bytecodemanipulation-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    58018 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_Assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_InlineSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_Mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_MutableFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_Operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_Optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_Specializations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_StandardLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-05 10:59:55.000000 bytecodemanipulation-0.3.4/tests/test_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.669877 bytecodemanipulation-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-13 14:49:46.669877 bytecodemanipulation-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.649875 bytecodemanipulation-0.3.5/bytecodemanipulation/
+-rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/Emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19904 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/MutableFunctionHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27037 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/Specialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/TypeEnforcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/annotated_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.653875 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/AbstractBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/Emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23045 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/syntax_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.653875 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/util/CommonUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/util/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/util/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.653875 bytecodemanipulation-0.3.5/bytecodemanipulation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.653875 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/builtin_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.653875 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.657876 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30740 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21386 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/RawAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.661876 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/ExceptionInstructionCodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/LocationInformationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.661876 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24122 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/specialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.661876 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.665876 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/specialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.665876 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_12/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/mixin_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.665876 bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/
+-rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/CacheEntryCreation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/CodeObjectBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/ExceptionTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25709 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/Instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/OpcodeReplacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/Opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/optimise_self.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17702 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/optimiser_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/bytecodemanipulation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.649875 bytecodemanipulation-0.3.5/bytecodemanipulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-13 14:49:46.000000 bytecodemanipulation-0.3.5/bytecodemanipulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-07-13 14:49:46.000000 bytecodemanipulation-0.3.5/bytecodemanipulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:49:46.000000 bytecodemanipulation-0.3.5/bytecodemanipulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 14:49:46.000000 bytecodemanipulation-0.3.5/bytecodemanipulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:49:46.669877 bytecodemanipulation-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-13 14:49:39.000000 bytecodemanipulation-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:49:46.669877 bytecodemanipulation-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    62653 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_Assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_AttributeAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_CompoundExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_ConstantAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_InlineSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_Operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_Specializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_StandardLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-13 14:49:28.000000 bytecodemanipulation-0.3.5/tests/test_issues.py
```

### Comparing `bytecodemanipulation-0.3.4/LICENSE` & `bytecodemanipulation-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/PKG-INFO` & `bytecodemanipulation-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecodemanipulation
-Version: 0.3.4
+Version: 0.3.5
 Summary: High level python bytecode manipulation
 Home-page: https://github.com/uuk0/PyBytecodeManipulator
 Author: uuk
 Author-email: uuk1301@gmail.com
 Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `bytecodemanipulation-0.3.4/README.md` & `bytecodemanipulation-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/Emulator.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/Emulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     continue_stack = []
 
     max_stack_size = mutable.calculate_max_stack_size()
 
     while True:
         print(instruction)
         print(stack)
+
         target = OPCODE_FUNCS[instruction.opcode]
 
         if target is None:
             raise UnknownOpcodeError(instruction)
 
         try:
             instruction, mutable = target(
@@ -133,15 +134,15 @@
         except YieldValue:
             raise RuntimeError("YIELD outside GENERATOR")
 
         if len(stack) > max_stack_size:
             raise StackSizeIssue(f"{len(stack)} > {max_stack_size}")
 
 
-OPCODE_FUNCS: typing.List[typing.Callable | None] = [None] * 256
+OPCODE_FUNCS: typing.List[typing.Callable | None] = [None] * 512
 
 
 def execution(opcode: int):
     def target(
         func: typing.Callable[
             [MutableFunction, Instruction, list, list, list, list, list],
             typing.Tuple[Instruction, MutableFunction],
@@ -177,14 +178,45 @@
     call_stack: list,
     exception_handle_stack: list,
 ) -> typing.Tuple[Instruction, MutableFunction]:
     stack.pop(-1)
     return instr.next_instruction, func
 
 
+@execution(Opcodes.DUP_TOP)
+def dup_top(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
+    stack.append(stack[-1])
+    return instr.next_instruction, func
+
+
+@execution(Opcodes.ROT_TWO)
+def rot_two(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
+    a = stack.pop(-1)
+    b = stack.pop(-1)
+    stack.append(a)
+    stack.append(b)
+    return instr.next_instruction, func
+
+
 @execution(Opcodes.JUMP_ABSOLUTE)
 @execution(Opcodes.JUMP_FORWARD)
 def jump_unconditional(
     func: MutableFunction,
     instr: Instruction,
     stack: list,
     local: list,
@@ -351,16 +383,20 @@
 
     if hasattr(target, "__self__") and hasattr(target, "__code__"):
         args.insert(0, target.__self__)
 
     try:
         mutable = MutableFunction(target)
     except AttributeError:
-        stack.append(target(*args))
-        return instr.next_instruction, func
+        try:
+            stack.append(target(*args))
+            return instr.next_instruction, func
+        except Exception as e:
+            print(target, args)
+            raise e from None
 
     if mutable.code_flags & CO_GENERATOR:
         stack.append(EmulatorGeneratorContainer(mutable, args))
         return instr.next_instruction, func
 
     call_stack.append(
         (
@@ -562,17 +598,30 @@
     local: list,
     free_vars: list,
     call_stack: list,
     exception_handle_stack: list,
 ) -> typing.Tuple[Instruction, MutableFunction]:
     op = ("<", "<=", "==", "!=", ">", ">=")[instr.arg]
     a, b = stack.pop(-2), stack.pop(-1)
-
     stack.append(eval(f"a {op} b", {"a": a, "b": b}))
+    return instr.next_instruction, func
+
 
+@execution(Opcodes.COMPARE_EQ)
+def compare_eq_op(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
+    a, b = stack.pop(-2), stack.pop(-1)
+    stack.append(a == b)
     return instr.next_instruction, func
 
 
 @execution(Opcodes.BINARY_SUBSCR)
 def binary_subscr(
     func: MutableFunction,
     instr: Instruction,
@@ -679,14 +728,78 @@
     a, b = stack.pop(-2), stack.pop(-1)
     a *= b
     stack.append(a)
 
     return instr.next_instruction, func
 
 
+@execution(Opcodes.BINARY_FLOOR_DIVIDE)
+def binary_subtract(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
+    stack.append(stack.pop(-2) // stack.pop(-1))
+
+    return instr.next_instruction, func
+
+
+@execution(Opcodes.INPLACE_FLOOR_DIVIDE)
+def binary_subtract(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
+    a, b = stack.pop(-2), stack.pop(-1)
+    a //= b
+    stack.append(a)
+
+    return instr.next_instruction, func
+
+
+@execution(Opcodes.BINARY_TRUE_DIVIDE)
+def binary_subtract(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
+    stack.append(stack.pop(-2) / stack.pop(-1))
+
+    return instr.next_instruction, func
+
+
+@execution(Opcodes.INPLACE_TRUE_DIVIDE)
+def binary_subtract(
+    func: MutableFunction,
+    instr: Instruction,
+    stack: list,
+    local: list,
+    free_vars: list,
+    call_stack: list,
+    exception_handle_stack: list,
+) -> typing.Tuple[Instruction, MutableFunction]:
+    a, b = stack.pop(-2), stack.pop(-1)
+    a /= b
+    stack.append(a)
+
+    return instr.next_instruction, func
+
+
 @execution(Opcodes.SETUP_FINALLY)
 def setup_finally(
     func: MutableFunction,
     instr: Instruction,
     stack: list,
     local: list,
     free_vars: list,
@@ -761,14 +874,17 @@
     stack: list,
     local: list,
     free_vars: list,
     call_stack: list,
     exception_handle_stack: list,
 ) -> typing.Tuple[Instruction, MutableFunction]:
 
+    if not stack:
+        raise StackSizeIssue("StackUnderflow: could not get TOS for FOR_ITER opcode")
+
     iterator = stack[-1]
 
     try:
         stack.append(next(iterator))
     except StopIteration:
         stack.pop(-1)
         return typing.cast(Instruction, instr.arg_value), func
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/Mixin.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/Mixin.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/MutableFunction.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/MutableFunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import simplejson
 
 from bytecodemanipulation.opcodes.AbstractOpcodeTransformerStage import ArgRealValueSetter
 from bytecodemanipulation.opcodes.AbstractOpcodeTransformerStage import ExtendedArgInserter
 from bytecodemanipulation.opcodes.AbstractOpcodeTransformerStage import InstructionAssembler
 from bytecodemanipulation.opcodes.AbstractOpcodeTransformerStage import JumpArgAssembler
 from bytecodemanipulation.opcodes.AbstractOpcodeTransformerStage import LinearStreamGenerator
+from bytecodemanipulation.opcodes.AbstractOpcodeTransformerStage import ForIterTransformer
 from bytecodemanipulation.opcodes.CodeObjectBuilder import CodeObjectBuilder
 from bytecodemanipulation.opcodes.ExceptionTable import ExceptionTable
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.opcodes.AbstractOpcodeTransformerStage import AbstractOpcodeTransformerStage, InstructionDecoder
 import bytecodemanipulation.data_loader
 from bytecodemanipulation.opcodes.OpcodeReplacer import IntermediateToRawOpcodeTransform
 from bytecodemanipulation.opcodes.OpcodeReplacer import RawToIntermediateOpcodeTransform
@@ -33,14 +34,15 @@
 
         INSTRUCTION_DECODING_PIPE += [
             ExceptionInstructionDecoder,
             LocationInformationDecoder,
         ]
 
     INSTRUCTION_ENCODING_PIPE: typing.List[typing.Type[AbstractOpcodeTransformerStage]] = [
+        ForIterTransformer,  # todo: how can we remove this hack?
         IntermediateToRawOpcodeTransform,
     ]
 
     if sys.version_info[1] == 10:
         from bytecodemanipulation.data.v3_10.ExceptionInstructionCodec import ExceptionInstructionEncoder
 
         INSTRUCTION_ENCODING_PIPE += [
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/MutableFunctionHelpers.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/MutableFunctionHelpers.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/Optimiser.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/Optimiser.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/Specialization.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/Specialization.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/AbstractBase.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/AbstractBase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import copy
 import types
 import typing
 from abc import ABC
 
+from bytecodemanipulation.assembler.syntax_errors import TraceInfo
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class ParsingScope:
@@ -43,21 +45,29 @@
         self.labels: typing.Set["IIdentifierAccessor"] = set()
         self.global_scope = {}
         self.scope_path: typing.List[str] = []
         self._name_counter = 1
         self.globals_dict = {}
         self.module_file: str = None
         self.last_base_token: AbstractToken = None
-        self.macro_parameter_namespace: typing.Dict[str] = {}
+        self.macro_parameter_namespace_stack: typing.List[typing.Dict[str]] = [{}]
         self.filled_locals = set()
 
         self.current_macro_assembly = None
 
+        self.may_get_trace_info = False
+
         self.closure_locals: typing.Set[str] = set()
 
+    def get_trace_info(self) -> TraceInfo:
+        if not self.may_get_trace_info:
+            raise RuntimeError("Cannot get trace info")
+
+        return TraceInfo()
+
     def scope_name_generator(self, suffix="") -> str:
         name = f"%INTERNAL:{self._name_counter}"
         self._name_counter += 1
 
         if suffix:
             name += "/" + suffix
 
@@ -122,15 +132,15 @@
     ):
         instance = ParsingScope()
         if copy_labels:
             instance.labels = self.labels
         instance.global_scope = self.global_scope
         instance.scope_path = self.scope_path.copy()
         instance.module_file = self.module_file
-        instance.macro_parameter_namespace = self.macro_parameter_namespace.copy()
+        instance.macro_parameter_namespace_stack = [e.copy() for e in self.macro_parameter_namespace_stack]
 
         if sub_scope_name is not None:
             if isinstance(sub_scope_name, str):
                 instance.scope_path.append(sub_scope_name)
             else:
                 instance.scope_path += sub_scope_name
 
@@ -154,14 +164,37 @@
             scope = scope.setdefault(e, {})
 
         if name[-1] in scope and not override_existing:
             raise ValueError(f"name '{name[-1]}' does already exists in the scope!")
 
         scope[name[-1]] = data
 
+    def lookup_macro_parameter(self, name: str, start: int = 0):
+        for space in reversed(self.macro_parameter_namespace_stack[:-start] if start != 0 else self.macro_parameter_namespace_stack):
+            if name in space:
+                return space[name]
+
+        raise KeyError(name)
+
+    def lookup_macro_parameter_with_level(self, name: str, start: int = 0) -> typing.Tuple[typing.Any, int]:
+        for i, space in enumerate(list(reversed(self.macro_parameter_namespace_stack[:-start] if start != 0 else self.macro_parameter_namespace_stack))):
+            if name in space:
+                return space[name], i
+
+        raise KeyError(name)
+
+    def set_macro_arg_value(self, key: str, value: typing.Any):
+        self.macro_parameter_namespace_stack[-1][key] = value
+
+    def push_macro_param_stack(self):
+        self.macro_parameter_namespace_stack.append({})
+
+    def pop_macro_param_stack(self):
+        self.macro_parameter_namespace_stack.pop(-1)
+
 
 class IAssemblyStructureVisitable(ABC):
     def visit_parts(
         self,
         visitor: typing.Callable[
             ["IAssemblyStructureVisitable", tuple, list], typing.Any
         ],
@@ -213,17 +246,19 @@
     PREFIX: str | None = None
     IS_STATIC = False
 
     def __init__(
         self,
         name: "IIdentifierAccessor | str",
         token: AbstractToken | typing.List[AbstractToken] = None,
+        trace_info: TraceInfo = None,
     ):
-        self.name = name
+        self.name = name if not isinstance(name, str) else StaticIdentifier(name)
         self.token = token
+        self.trace_info: TraceInfo = trace_info
 
     def __eq__(self, other):
         return type(self) == type(other) and self.name == other.name
 
     def __repr__(self):
         return f"{self.PREFIX}{self.name}"
 
@@ -259,14 +294,15 @@
     def __init__(
         self,
         macro_name: typing.Union[str, "IIdentifierAccessor"],
         token: typing.List[AbstractToken] = None,
     ):
         self.macro_name = macro_name
         self.token = token
+        self.trace_info: TraceInfo = None
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
         return self.token
 
     def __hash__(self):
         return hash(self.macro_name)
 
@@ -276,66 +312,74 @@
         return False
 
     def __repr__(self):
         return f"&{self.macro_name}"
 
     def __call__(self, scope: ParsingScope):
         from bytecodemanipulation.assembler.syntax_errors import (
-            throw_positioned_error,
+            PropagatingCompilerException,
         )
+
+        if scope is None:
+            raise SyntaxError("no scope provided")
+
+        try:
+            value = scope.lookup_macro_parameter(self.token[1].text)
+        except KeyError:
+            raise PropagatingCompilerException(
+                f"Could not find name '{self.token[1].text}' in macro parameter space"
+            ).add_trace_level(self.trace_info.with_token(self.token[1])) from None
+
+        return self._check_value(scope, value)
+
+    def _check_value(self, scope, value, level=1):
+        from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
         from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
             ConstantAccessExpression,
         )
         from bytecodemanipulation.data.shared.expressions.DerefAccessExpression import (
             DerefAccessExpression,
         )
         from bytecodemanipulation.data.shared.expressions.GlobalAccessExpression import (
             GlobalAccessExpression,
         )
         from bytecodemanipulation.data.shared.expressions.LocalAccessExpression import (
             LocalAccessExpression,
         )
-
-        if scope is None:
-            raise SyntaxError("no scope provided")
-
-        if self.token[1].text not in scope.macro_parameter_namespace:
-            raise throw_positioned_error(
-                scope,
-                self.token,
-                "Could not find name in macro parameter space",
-            )
-
-        value = scope.macro_parameter_namespace[self.token[1].text]
-
         if isinstance(value, ConstantAccessExpression):
             if not isinstance(value.value, str):
-                raise throw_positioned_error(
-                    scope,
-                    self.token,
-                    f"Expected 'string' for name de-referencing, got {value}",
-                )
+                raise PropagatingCompilerException(
+                    f"Expected 'string' for name de-referencing, got '{value}'"
+                ).add_trace_level(self.trace_info.with_token(self.token[0]))
 
             return value.value
 
         if isinstance(
             value,
             (
                 GlobalAccessExpression,
                 LocalAccessExpression,
                 DerefAccessExpression,
             ),
         ):
             return value.get_name(scope)
 
-        raise throw_positioned_error(
-            scope,
-            self.token,
-            f"Expected <static evaluated expression> for getting the name for storing, got {value}",
-        )
+        from bytecodemanipulation.data.shared.expressions.MacroParameterAcessExpression import MacroParameterAccessExpression
+
+        if isinstance(value, MacroParameterAccessExpression):
+            new_value = scope.lookup_macro_parameter(value.name(scope), start=level)
+
+            if value != new_value:
+                return self._check_value(scope, new_value, level=level+1)
+
+            print("WARN: got some value from macro namespace")
+
+        raise PropagatingCompilerException(
+            f"Expected <static evaluated expression> for getting the name for storing, got '{value}'"
+        ).add_trace_level(self.trace_info.with_token(self.token[0])) from None
 
 
 class StaticIdentifier(IIdentifierAccessor):
     def __init__(self, name: str, token: AbstractToken = None):
         self.name = name
         self.token = token
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Emitter.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/Emitter.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.assembler.Parser import (
     Parser as AssemblyParser,
 )
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel, ParsingScope
 from bytecodemanipulation.assembler import target as assembly_targets
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 
 
 def _visit_for_stack_effect(
     ins: Instruction,
     eff_a: typing.Tuple[int, int] | None,
     eff_b: typing.Tuple[int, int] | None,
 ) -> typing.Tuple[int, int]:
@@ -24,15 +25,15 @@
 
     eff = 0
     max_size = 0
 
     if eff_b is not None:
         max_size = eff_b[1]
 
-    if eff_a is not None:
+    if eff_a is not None and not ins.has_unconditional_jump():
         eff += eff_a[0]
 
         max_size = max(max_size, eff, eff_a[0])
 
     push, pop, *_ = ins.get_stack_affect()
 
     eff += push - pop
@@ -42,15 +43,15 @@
     return eff, max_size
 
 
 GLOBAL_SCOPE_CACHE: typing.Dict[str, dict] = {}
 
 
 def apply_inline_assemblies(
-    target: MutableFunction | typing.Callable, store_at_target: bool = None
+    target: MutableFunction | typing.Callable, store_at_target: bool = None, unwrap_exceptions=True,
 ):
     """
     Processes all assembly() calls, label() calls and jump() calls in 'target'
     """
     if not isinstance(target, MutableFunction):
         target = MutableFunction(target)
         if store_at_target is None:
@@ -150,37 +151,48 @@
     target.walk_instructions(visit)
 
     if target.target.__module__ in GLOBAL_SCOPE_CACHE:
         scope.global_scope = GLOBAL_SCOPE_CACHE[target.target.__module__]
     else:
         GLOBAL_SCOPE_CACHE[target.target.__module__] = scope.global_scope
 
-    assemblies = [
-        AssemblyParser(
-            Lexer(code).add_line_offset(instr.source_location[0] + 1).lex(),
-            scope.scope_path.clear() or scope,
-        ).parse()
-        for code, instr in insertion_points
-    ]
+    assemblies = []
+
+    for code, instr in insertion_points:
+        try:
+            scope.may_get_trace_info = True
+            assemblies.append(AssemblyParser(
+                Lexer(code, module_file=target.target.__globals__["__file__"]).add_line_offset(instr.source_location[0]).lex(),
+                scope.scope_path.clear() or scope,
+                module_file=target.target.__globals__["__file__"],
+            ).parse())
+            scope.may_get_trace_info = False
+        except PropagatingCompilerException as e:
+            if not unwrap_exceptions:
+                raise e
+
+            e.print_exception()
+            raise e.underlying_exception(*e.args) from None
 
     for asm in assemblies:
         asm_labels = asm.collect_label_info(scope)
         labels.update({StaticIdentifier(e) for e in asm_labels})
 
     scope.labels |= labels
 
     max_stack_effects = []
 
     # for asm in assemblies:
     #     asm.fill_scope_complete(scope)
 
     scope.scope_path.clear()
+    scope.may_get_trace_info = False
 
     for (_, instr), asm in zip(insertion_points, assemblies):
-        _create_fragment_bytecode(asm, instr, label_targets, max_stack_effects, scope, target)
+        _create_fragment_bytecode(asm, instr, label_targets, max_stack_effects, scope, target, unwrap_exceptions=unwrap_exceptions)
 
     target.walk_instructions(visit)
 
     pending: typing.List[Instruction] = []
 
     def resolve_special_code(ins: Instruction):
         # print(ins)
@@ -208,56 +220,63 @@
 
     if store_at_target:
         target.reassign_to_function()
 
     return target
 
 
-def _create_fragment_bytecode(asm, insertion_point: Instruction, label_targets: typing.Dict[str, Instruction], max_stack_effects: typing.List, scope: ParsingScope, target: MutableFunction):
-    bytecode = asm.create_bytecode(target, scope)
+def _create_fragment_bytecode(asm, insertion_point: Instruction, label_targets: typing.Dict[str, Instruction], max_stack_effects: typing.List, scope: ParsingScope, target: MutableFunction, unwrap_exceptions=False):
+    try:
+        bytecode = asm.create_bytecode(target, scope)
+    except PropagatingCompilerException as e:
+        if not unwrap_exceptions:
+            raise e
+
+        e.print_exception()
+        raise e.underlying_exception(*e.args) from None
 
     if bytecode:
         # link the instructions to each other
         for i, ins in enumerate(bytecode[:-1]):
             ins.next_instruction = bytecode[i + 1]
 
-        try:
-            stack_effect, max_stack_effect = bytecode[0].apply_value_visitor(
-                _visit_for_stack_effect
-            )
-        except RuntimeError:
-            stack_effect = 0
-            max_stack_effect = 0
+    #     try:
+    #         stack_effect, max_stack_effect = bytecode[0].apply_value_visitor(
+    #             _visit_for_stack_effect
+    #         )
+    #     except RuntimeError:
+    #         stack_effect = 0
+    #         max_stack_effect = 0
 
     else:
         max_stack_effects.append(0)
         return
 
-    if (
-        stack_effect != 0
-        and not (
-            bytecode[-1].has_unconditional_jump() or bytecode[-1].has_stop_flow()
-        )
-    ):
-        # print(asm)
-
-        total = 0
-
-        for e in enumerate(bytecode):
-            add, subtract, _ = e[1].get_stack_affect()
-            total += add - subtract
-            print(*e, total)
-
-        print(stack_effect)
-
-        raise RuntimeError(
-            f"Inline assembly code mustn't change overall stack size at exit, got a delta of {stack_effect}!"
-        )
+    # if (
+    #     stack_effect != 0
+    #     and not (
+    #         bytecode[-1].has_unconditional_jump() or bytecode[-1].has_stop_flow()
+    #     )
+    # ):
+    #     # print(asm)
+    #
+    #     total = 0
+    #
+    #     for e in enumerate(bytecode):
+    #         add, subtract, _ = e[1].get_stack_affect()
+    #         total += add - subtract
+    #         print(*e, total)
+    #
+    #     print(stack_effect)
+    #
+    #     raise RuntimeError(
+    #         f"Inline assembly code mustn't change overall stack size at exit, got a delta of {stack_effect}!"
+    #     )
 
-    max_stack_effects.append(max_stack_effect)
+    # max_stack_effects.append(max_stack_effect)
 
     for i, ins in enumerate(bytecode[:-1]):
         if not ins.has_stop_flow() and not ins.has_unconditional_jump():
             ins.next_instruction = bytecode[i + 1]
 
     bytecode[-1].next_instruction = following_instr = insertion_point.next_instruction
 
@@ -273,37 +292,54 @@
             ins.change_opcode(Opcodes.NOP)
             ins.next_instruction = (
                 bytecode[i + 1] if i < len(bytecode) - 1 else following_instr
             )
 
 
 def execute_module_in_instance(
-    asm_code: str, module: types.ModuleType, file: str = None
+    asm_code: str, module: types.ModuleType, file: str = None, unwrap_exceptions=True,
 ):
     scope = ParsingScope()
 
     try:
         scope.module_file = file or module.__file__
     except AttributeError:
         pass
 
     if module.__name__ in GLOBAL_SCOPE_CACHE:
         scope.global_scope = GLOBAL_SCOPE_CACHE[module.__name__]
     else:
         GLOBAL_SCOPE_CACHE[module.__name__] = scope.global_scope
 
-    asm = AssemblyParser(asm_code, scope).parse()
+    try:
+        scope.may_get_trace_info = True
+        asm = AssemblyParser(asm_code, scope, module_file=module.__file__).parse()
+        scope.may_get_trace_info = False
+    except PropagatingCompilerException as e:
+        if not unwrap_exceptions:
+            raise e
+
+        e.print_exception()
+        raise e.underlying_exception(*e.args) from None
+
     scope.labels = asm.get_labels(scope)
     # asm.fill_scope_complete(scope)
     scope.scope_path.clear()
     create_function = lambda m: None
     target = MutableFunction(create_function)
     target.argument_names[0] = "$module$"
 
-    bytecode = asm.create_bytecode(target, scope)
+    try:
+        bytecode = asm.create_bytecode(target, scope)
+    except PropagatingCompilerException as e:
+        if not unwrap_exceptions:
+            raise e
+
+        e.print_exception()
+        raise e.underlying_exception(*e.args) from None
 
     if bytecode is None:
         return
 
     label_targets = {}
     for ins in bytecode:
         if ins.opcode == Opcodes.BYTECODE_LABEL:
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Lexer.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/Lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             return token
 
         if char in string.digits or (
             char == "-" and self.try_inspect_multi(2)[1] in string.digits
         ):
             text = ""
             if self.try_consume("-"):
-                text += "."
+                text += "-"
             text += self.consume_while(string.digits + "_")
 
             if self.try_inspect() == ".":
                 remaining = self.consume(".") + self.consume_while(string.digits + "_")
 
                 if self.try_inspect() and self.try_inspect() in string.ascii_letters:
                     return [
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/Parser.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/OpAssembly.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,625 +1,611 @@
 import typing
-from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
+import abc
+import typing
+from collections import namedtuple
+
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
-from bytecodemanipulation.assembler.AbstractBase import (
-    IIdentifierAccessor,
-    MacroExpandedIdentifier,
-    StaticIdentifier,
-)
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import _syntax_wrapper
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.assembler.Lexer import SpecialToken
+from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException, TraceInfo
+from bytecodemanipulation.assembler.util.parser import AbstractExpression
+from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.data.shared.expressions.AttributeAccessExpression import (
-    AttributeAccessExpression,
-)
-from bytecodemanipulation.data.shared.instructions.CallAssembly import (
-    AbstractCallAssembly,
-)
-from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
-    CompoundExpression,
-)
-from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
-    ConstantAccessExpression,
-)
-from bytecodemanipulation.data.shared.expressions.DerefAccessExpression import (
-    DerefAccessExpression,
-)
-from bytecodemanipulation.data.shared.expressions.DiscardValueExpression import (
-    DiscardValueExpression,
-)
-from bytecodemanipulation.data.shared.expressions.DynamicAccessExpression import (
-    DynamicAttributeAccessExpression,
-)
-from bytecodemanipulation.data.shared.expressions.GlobalAccessExpression import (
-    GlobalAccessExpression,
-)
-from bytecodemanipulation.data.shared.expressions.GlobalStaticAccessExpression import (
-    GlobalStaticAccessExpression,
-)
-from bytecodemanipulation.data.shared.expressions.LocalAccessExpression import (
-    LocalAccessExpression,
-)
-from bytecodemanipulation.data.shared.instructions.MacroAssembly import MacroAssembly
-from bytecodemanipulation.data.shared.expressions.MacroParameterAcessExpression import (
-    MacroParameterAccessExpression,
-)
-from bytecodemanipulation.data.shared.expressions.ModuleAccessExpression import (
-    ModuleAccessExpression,
-)
-from bytecodemanipulation.data.shared.expressions.StaticAttributeAcccessExpression import (
-    StaticAttributeAccessExpression,
-)
-from bytecodemanipulation.data.shared.expressions.SubscriptionAccessExpression import (
-    SubscriptionAccessExpression,
-)
-from bytecodemanipulation.data.shared.expressions.TopOfStackAccessExpression import (
-    TopOfStackAccessExpression,
-)
-from bytecodemanipulation.data.shared.instructions.OpAssembly import AbstractOpAssembly
-
+from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Instruction import Instruction
+from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 
-from bytecodemanipulation.assembler.Lexer import (
-    Lexer,
-    SpecialToken,
-    StringLiteralToken,
-)
 
-try:
-    from code_parser.lexers.common import (
-        AbstractToken,
-        CommentToken,
-        IdentifierToken,
-        BinaryOperatorToken,
-        IntegerToken,
-        FloatToken,
-        BracketToken,
-    )
-    from code_parser.parsers.common import (
-        AbstractParser,
-        AbstractExpression,
-        NumericExpression,
-        BracketExpression,
-        BinaryExpression,
-        IdentifierExpression,
-    )
-    import code_parser.parsers.common as parser_file
-
-except ImportError:
-    from bytecodemanipulation.assembler.util.tokenizer import (
-        AbstractToken,
-        CommentToken,
-        IdentifierToken,
-        BinaryOperatorToken,
-        IntegerToken,
-        FloatToken,
-        BracketToken,
-    )
-    from bytecodemanipulation.assembler.util.parser import (
-        AbstractParser,
-        AbstractExpression,
-        NumericExpression,
-        BracketExpression,
-        BinaryExpression,
-        IdentifierExpression,
-    )
-    import bytecodemanipulation.assembler.util.parser as parser_file
-
-
-def create_instruction(token: AbstractToken, *args, **kwargs) -> Instruction:
-    instr = Instruction(*args, **kwargs)
-
-    if token is not None:
-        instr.source_location = token.line, token.column, token.span
-
-    return instr
-
-
-Instruction.create_with_token = create_instruction
-
-parser_file.raise_syntax_error = _syntax_wrapper
-
-
-class Parser(AbstractParser):
-    INSTRUCTIONS: typing.Dict[str, typing.Type[AbstractAssemblyInstruction]] = {}
-
-    T = typing.TypeVar(
-        "T", typing.Type[AbstractAssemblyInstruction], AbstractAssemblyInstruction
-    )
+if typing.TYPE_CHECKING:
+    from bytecodemanipulation.assembler.Parser import Parser
 
-    @classmethod
-    def register(cls, instr: T) -> T:
-        cls.INSTRUCTIONS[instr.NAME] = instr
-        return instr
 
-    def __init__(
+class AbstractOperator(abc.ABC):
+    def emit_bytecodes(
         self,
-        tokens_or_str: str | typing.List[AbstractToken],
-        scope: ParsingScope = None,
-        initial_line_offset=0,
-    ):
-        super().__init__(
-            tokens_or_str
-            if isinstance(tokens_or_str, list)
-            else Lexer(tokens_or_str, initial_line_offset=initial_line_offset).lex()
-        )
-        self.scope = scope or ParsingScope()
+        function: MutableFunction,
+        scope: ParsingScope,
+        *parameters: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
+    ) -> typing.List[Instruction]:
+        raise NotImplementedError
 
-    def parse(self, scope: ParsingScope = None) -> CompoundExpression:
-        """
-        Starts parsing the text, and returns the CompoundExpression holding everything
-
-        :param scope: the scope to use
-        """
-        self.scope = scope or self.scope
-        return self.parse_while_predicate(
-            lambda: not self.is_empty(), scope=scope or self.scope
-        )
+    def evaluate_static_value(self, scope: ParsingScope, *parameters: AbstractSourceExpression):
+        raise NotImplementedError
 
-    def parse_body(
-        self, namespace_part: str | list | None = None, scope: ParsingScope = None
-    ) -> CompoundExpression:
-        """
-        Parses the body of an expression, containing a list of assembly instructions
-
-        :param namespace_part: a suffix for the scope namespace
-        :param scope: optional, the scope to use
-        :return: the CompoundExpression representing the body
-        :raises: SyntaxError: if EOF is reached before finalizing, or '}' was not found at the end to end the body
-        """
-        scope = scope or self.scope
-
-        if namespace_part is not None:
-            if isinstance(namespace_part, str):
-                scope.scope_path.append(namespace_part)
-            else:
-                scope.scope_path += namespace_part
 
-        if not self.try_consume(SpecialToken("{")):
-            raise throw_positioned_error(
-                scope, self.try_inspect(), "expected '{'"
-            )
+OperatorArgValue = namedtuple("OperatorArgValue", "index")
 
-        body = self.parse_while_predicate(
-            lambda: not self.try_consume(SpecialToken("}")),
-            eof_error="Expected '}', got EOF",
-            scope=scope,
-        )
 
-        if namespace_part:
-            if isinstance(namespace_part, str):
-                if self.scope.scope_path.pop(-1) != namespace_part:
-                    raise RuntimeError
+class OpcodeBaseOperator(AbstractOperator):
+    def __init__(
+        self,
+        *opcodes: int
+        | str
+        | typing.Tuple[int | str, int]
+        | typing.Tuple[
+            int | str,
+            typing.Callable[
+                [MutableFunction, ParsingScope, typing.List[AbstractSourceExpression]],
+                typing.Any,
+            ],
+        ]
+        | OperatorArgValue,
+        static_eval: typing.Callable[[ParsingScope, typing.List[AbstractSourceExpression]], typing.Any] = None
+    ):
+        self.opcodes = opcodes
+        self.static_eval = static_eval
+
+    def emit_bytecodes(
+        self,
+        function: MutableFunction,
+        scope: ParsingScope,
+        *parameters: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
+    ) -> typing.List[Instruction]:
+        bytecode = []
+        if not any(isinstance(param, OperatorArgValue) for param in self.opcodes):
+            for param in parameters:
+                bytecode += param.emit_bytecodes(function, scope)
+
+        for opcode in self.opcodes:
+            if isinstance(opcode, (int, str)):
+                bytecode.append(Instruction(opcode))
+            elif isinstance(opcode, tuple):
+                if isinstance(opcode[1], typing.Callable):
+                    bytecode.append(
+                        Instruction(
+                            function,
+                            -1,
+                            opcode[0],
+                            arg=opcode[1](function, scope, list(parameters)),
+                        )
+                    )
+                else:
+                    bytecode.append(Instruction(opcode[0], arg=opcode[1]))
+            elif isinstance(opcode, OperatorArgValue):
+                bytecode += parameters[opcode.index].emit_bytecodes(function, scope)
+            elif hasattr(opcode, "emit_bytecodes"):
+                bytecode += opcode.emit_bytecodes(function, scope)
             else:
-                if self.scope.scope_path[-len(namespace_part) :] != namespace_part:
-                    raise RuntimeError
+                raise ValueError(opcode)
 
-                del self.scope.scope_path[-len(namespace_part) :]
+        return bytecode
 
-        return body
+    def evaluate_static_value(self, scope: ParsingScope, *parameters: AbstractSourceExpression):
+        if not self.static_eval:
+            raise NotImplementedError
 
-    def parse_while_predicate(
-        self,
-        predicate: typing.Callable[[], bool],
-        eof_error: str = None,
-        scope: ParsingScope = None,
-    ) -> CompoundExpression:
-        root = CompoundExpression()
-
-        while predicate():
-            if self.try_consume(CommentToken):
-                continue
-
-            if not (instr_token := self.try_consume(IdentifierToken)):
-                raise throw_positioned_error(
-                    scope, self.try_inspect(), "expected identifier"
-                )
+        return self.static_eval(scope, list(parameters))
 
-            if scope:
-                scope.last_base_token = instr_token
 
-            if instr_token.text not in self.INSTRUCTIONS:
-                if not (instr := self.try_parse_custom_assembly(instr_token, scope)):
-                    raise throw_positioned_error(
-                        scope,
-                        instr_token,
-                        "expected <assembly instruction name> or <assembly macro name>",
-                    )
-            else:
-                instr = self.INSTRUCTIONS[instr_token.text].consume(self, scope)
+class AbstractOpAssembly(
+    AbstractAssemblyInstruction, AbstractAccessExpression, abc.ABC
+):
+    """
+    OP ... [-> <target>]
+    - <expr> +|-|*|/|//|**|%|&|"|"|^|>>|<<|@|is|!is|in|!in|<|<=|==|!=|>|>=|xor|!xor|:=|isinstance|issubclass|hasattr|getattr <expr>
+    - -|+|~|not|! <expr>
+    """
 
-            root.add_child(instr)
+    NAME = "OP"
 
-            instr.fill_scope(self.scope)
+    BINARY_OPS: typing.Dict[str, AbstractOperator] = {}
+    SINGLE_OPS: typing.Dict[str, AbstractOperator] = {}
+    PREFIX_OPERATORS: typing.Dict[
+        str, typing.Tuple[AbstractOperator, int | None, bool | None, bool | None]
+    ] = {}
 
-            while self.try_consume(CommentToken):
-                pass
+    @classmethod
+    def register_prefix_operator(
+        cls,
+        name: str,
+        operator: AbstractOperator,
+        arg_count: int = None,
+        include_brackets: bool = None,
+        has_coma_sep: bool = None,
+    ):
+        if arg_count is None:
+            if include_brackets is False:
+                raise ValueError(
+                    "If 'include_brackets' is False, 'arg_count' must be set"
+                )
 
-            if self.is_empty():
-                break
+            include_brackets = True
 
-            if self.try_consume(SpecialToken(";")):
-                continue
+        cls.PREFIX_OPERATORS[name] = operator, arg_count, include_brackets, has_coma_sep
 
-            if not (expr := self.try_inspect()):
-                continue
+    class IOperation(IAssemblyStructureVisitable, abc.ABC):
+        def copy(self):
+            raise NotImplementedError
+
+        def emit_bytecodes(
+            self, function: MutableFunction, scope: ParsingScope
+        ) -> typing.List[Instruction]:
+            raise NotImplementedError
+
+        def __eq__(self, other):
+            raise NotImplementedError
+
+        def __repr__(self):
+            raise NotImplementedError
+
+        def evaluate_static_value(self, scope: ParsingScope):
+            raise NotImplementedError
+
+    class SingleOperation(IOperation):
+        def __init__(
+            self,
+            operator: str,
+            operator_token: typing.List[AbstractToken],
+            expression: AbstractSourceExpression,
+            base: typing.Type["AbstractOpAssembly"] = None,
+            trace_info: TraceInfo = None,
+        ):
+            self.operator = operator
+            self.operator_token = operator_token
+            self.expression = expression
+            self.base = base
+            self.trace_info: TraceInfo = trace_info
+
+        def __eq__(self, other):
+            return (
+                type(self) == type(other)
+                and self.operator == other.operator
+                and self.expression == other.expression
+            )
 
-            if self[-1].line != expr.line:
-                continue
+        def __repr__(self):
+            return f"{self.operator} {self.expression}"
 
-            if not predicate():
-                if eof_error and self.try_inspect() is None:
-                    print(self.try_inspect())
-                    print(repr(root))
-                    raise throw_positioned_error(scope, self[-1], eof_error)
+        def copy(self):
+            return type(self)(
+                self.operator, self.operator_token, self.expression.copy(), self.base
+            )
 
-                break
+        def emit_bytecodes(
+            self, function: MutableFunction, scope: ParsingScope
+        ) -> typing.List[Instruction]:
+            try:
+                return self.base.SINGLE_OPS[self.operator].emit_bytecodes(
+                    function, scope, self.expression, trace_info=self.trace_info,
+                )
+            except PropagatingCompilerException as e:
+                raise e.add_trace_level(self.trace_info)
 
-            print(self[-1].line, self[-1], expr.line)
+        def evaluate_static_value(self, scope: ParsingScope):
+            return self.base.SINGLE_OPS[self.operator].evaluate_static_value(scope, self.expression)
 
-            raise throw_positioned_error(
-                scope,
-                self.try_inspect(),
-                "Expected <newline> or ';' after assembly instruction",
+        def visit_parts(
+            self,
+            visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any],
+            parents: list,
+        ):
+            return visitor(
+                self,
+                (
+                    self.expression.visit_parts(visitor, parents + [self]),
+                    parents,
+                ),
             )
 
-        return root
+        def visit_assembly_instructions(
+            self,
+            visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any],
+        ):
+            pass
 
-    def try_parse_custom_assembly(
-        self, base_token: IdentifierToken, scope: ParsingScope
-    ):
-        self.cursor -= 1
-        self.save()
-        self.cursor += 1
-
-        name = [base_token.text]
-
-        while self.try_consume(SpecialToken(":")):
-            name.append(self.consume(IdentifierToken).text)
-
-        target = self.scope.lookup_namespace(name, create=False, include_prefixes=True)
-
-        if isinstance(target, MacroAssembly.MacroOverloadPage):
-            for macro in typing.cast(
-                MacroAssembly.MacroOverloadPage, target
-            ).assemblies:
-                if macro.allow_assembly_instr:
-                    self.rollback()
-                    # print(name)
-                    return AbstractCallAssembly.IMPLEMENTATION.consume_macro_call(
-                        self, scope
-                    )
+    class BinaryOperation(IOperation):
+        def __init__(
+            self,
+            lhs: AbstractSourceExpression,
+            operator: str,
+            operator_token: typing.List[AbstractToken],
+            rhs: AbstractSourceExpression,
+            base: typing.Type["AbstractOpAssembly"] = None,
+            trace_info: TraceInfo = None,
+        ):
+            self.base = base
+            self.lhs = lhs
+            self.operator = operator
+            self.operator_token = operator_token
+            self.rhs = rhs
+            self.trace_info: TraceInfo = trace_info
+
+        def __eq__(self, other):
+            return (
+                type(self) == type(other)
+                and self.lhs == other.lhs
+                and self.operator == other.operator
+                and self.rhs == other.rhs
+            )
 
-        self.rollback()
+        def __repr__(self):
+            return f"{self.lhs} {self.operator} {self.rhs}"
 
-    def try_consume_access_to_value(
-        self,
-        allow_tos=True,
-        allow_primitives=False,
-        allow_op=True,
-        allow_advanced_access=True,
-        allow_calls=True,
-        scope=None,
-    ) -> AbstractAccessExpression | None:
-        """
-        Consumes an access to a value, for read or write access
+        def copy(self):
+            return type(self)(
+                self.lhs.copy(),
+                self.operator,
+                self.operator_token,
+                self.rhs.copy(),
+                self.base,
+            )
 
-        todo: add an option to force write compatibility
-        todo: make it extendable
+        def emit_bytecodes(
+            self, function: MutableFunction, scope: ParsingScope
+        ) -> typing.List[Instruction]:
+            try:
+                return self.base.BINARY_OPS[self.operator].emit_bytecodes(
+                    function, scope, self.lhs, self.rhs, trace_info=self.trace_info,
+                )
+            except PropagatingCompilerException as e:
+                raise e.add_trace_level(self.trace_info)
 
-        :param allow_tos: if TOS (%) is allowed
-        :param allow_primitives: if primitives are allowed, e.g. numeric literals
-        :param allow_op: if operations are allowed, starting with OP
-        :param allow_advanced_access: if expressions like @global[$index].attribute are allowed
-        :param scope: the parsing scope instance
-        :param allow_calls: if True, calls will be allowed as expressions
-        """
-        start_token = self.try_inspect()
+        def evaluate_static_value(self, scope: ParsingScope):
+            return self.base.BINARY_OPS[self.operator].evaluate_static_value(scope, self.lhs, self.rhs)
 
-        if start_token is None:
-            return
+        def visit_parts(
+            self,
+            visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any],
+            parents: list,
+        ):
+            return visitor(
+                self,
+                (
+                    self.lhs.visit_parts(visitor, parents + [self]),
+                    self.rhs.visit_parts(visitor, parents + [self]),
+                ),
+                parents,
+            )
 
-        if allow_primitives:
-            if string := self.try_consume(StringLiteralToken):
-                return ConstantAccessExpression(string.text, string)
-
-            if integer := self.try_consume(IntegerToken):
-                return ConstantAccessExpression(
-                    int(integer.text)
-                    if "." not in integer.text
-                    else float(integer.text),
-                    integer,
-                )
+        def visit_assembly_instructions(
+            self,
+            visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any],
+        ):
+            pass
 
-            if isinstance(start_token, IdentifierToken):
-                if start_token.text == "None":
-                    return ConstantAccessExpression(None, start_token)
-                elif start_token.text == "True":
-                    return ConstantAccessExpression(True, start_token)
-                elif start_token.text == "False":
-                    return ConstantAccessExpression(False, start_token)
+    class PrefixOperator(IOperation):
+        def __init__(
+            self,
+            operator: str,
+            operator_token: typing.List[AbstractToken],
+            args: typing.List[AbstractSourceExpression],
+            base: typing.Type["AbstractOpAssembly"] = None,
+            trace_info: TraceInfo = None,
+        ):
+            self.base = base
+            self.operator = operator
+            self.operator_token = operator_token
+            self.args = args
+            self.trace_info: TraceInfo = trace_info
+
+        def __eq__(self, other):
+            return (
+                type(self) == type(other)
+                and self.args == other.args
+                and self.operator == other.operator
+            )
 
-        if not isinstance(start_token, (SpecialToken, IdentifierToken)):
-            return
+        def __repr__(self):
+            return f"{self.operator} {repr(self.args)[1:-1]}"
 
-        if start_token.text == "@":
-            self.consume(SpecialToken("@"), err_arg=scope)
+        def copy(self):
+            return type(self)(
+                self.operator, self.operator_token, [arg.copy() for arg in self.args]
+            )
 
-            if self.try_consume(SpecialToken("!")):
-                expr = GlobalStaticAccessExpression(
-                    self.parse_identifier_like(scope), start_token
-                )
-            else:
-                expr = GlobalAccessExpression(
-                    self.parse_identifier_like(scope), start_token
+        def emit_bytecodes(
+            self, function: MutableFunction, scope: ParsingScope
+        ) -> typing.List[Instruction]:
+            try:
+                return self.base.PREFIX_OPERATORS[self.operator][0].emit_bytecodes(
+                    function, scope, *self.args, trace_info=self.trace_info,
                 )
+            except PropagatingCompilerException as e:
+                raise e.add_trace_level(self.trace_info)
 
-        elif start_token.text == "$":
-            self.consume(SpecialToken("$"), err_arg=scope)
+        def evaluate_static_value(self, scope: ParsingScope):
+            return self.base.PREFIX_OPERATORS[self.operator][0].evaluate_static_value(scope, *self.args)
 
-            prefix = ""
+        def visit_parts(
+            self,
+            visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any],
+            parents: list,
+        ):
+            return visitor(
+                self,
+                tuple(
+                    [arg.visit_parts(visitor, parents + [self]) for arg in self.args]
+                ),
+                parents,
+            )
 
-            while self.try_consume(SpecialToken("|")):
-                prefix += "|"
+        def visit_assembly_instructions(
+            self,
+            visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any],
+        ):
+            pass
 
-            if prefix == "":
-                while self.try_consume(SpecialToken(":")):
-                    prefix += ":"
-
-            elif error := self.try_consume(SpecialToken(":")):
-                raise throw_positioned_error(
-                    scope,
-                    error,
-                    "Cannot parse '|' and ':' for <local variable name>",
-                )
+    MAX_TOKENS_FOR_OPERATORS = 3
 
-            expr = LocalAccessExpression(self.parse_identifier_like(scope), start_token, prefix=prefix)
+    @classmethod
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractOpAssembly":
+        if expr := cls.try_consume_binary(parser, scope):
+            return cls(expr, cls.try_consume_arrow(parser, scope))
+
+        if expr := cls.try_consume_single(parser, scope):
+            return cls(expr, cls.try_consume_arrow(parser, scope))
+
+        if expr := cls.try_consume_prefix(parser, scope):
+            return cls(expr, cls.try_consume_arrow(parser, scope))
+
+        raise PropagatingCompilerException(
+            "expected <operator> or <expression> <operator>..."
+        ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
-        elif start_token.text == "§":
-            self.consume(SpecialToken("§"), err_arg=scope)
+    @classmethod
+    def try_consume_operator_name(
+        cls, parser: "Parser", scope: ParsingScope, source: typing.Dict[str, typing.Any]
+    ) -> typing.List[AbstractToken] | None:
+        for count in range(cls.MAX_TOKENS_FOR_OPERATORS - 1, 0, -1):
+            operator = parser[0:count]
 
-            identifier = self.try_parse_identifier_like()
+            if operator and "".join(map(lambda e: e.text, operator)) in source:
+                if not parser.try_consume_multi(operator):
+                    raise RuntimeError
 
-            if identifier is None:
-                raise throw_positioned_error(
-                    scope,
-                    [start_token, self[0]],
-                    "Expected <identifier-like> after '§' for cell-var reference",
-                )
+                return operator
 
-            expr = DerefAccessExpression(identifier, start_token)
+    @classmethod
+    def try_consume_arrow(
+        cls, parser: "Parser", scope: ParsingScope
+    ) -> AbstractAccessExpression | None:
+        if parser.try_consume(SpecialToken("-")):
+            if not parser.try_consume(SpecialToken(">")):
+                raise PropagatingCompilerException(
+                    "expected '>' after '-' to complete '->'"
+                ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
-        elif start_token.text == "&":
-            self.consume(SpecialToken("&"), err_arg=scope)
-            expr = MacroParameterAccessExpression(
-                self.parse_identifier_like(scope), start_token
-            )
+            return parser.try_consume_access_to_value(scope=scope)
 
-        elif start_token.text == "%" and allow_tos:
-            self.consume(SpecialToken("%"), err_arg=scope)
+    @classmethod
+    def try_consume_single(
+        cls, parser: "Parser", scope: ParsingScope
+    ) -> typing.Optional[IOperation]:
+        operator_tokens = cls.try_consume_operator_name(parser, scope, cls.SINGLE_OPS)
 
-            offset = self.try_consume(IntegerToken)
+        if operator_tokens is None:
+            return
 
-            if offset is not None:
-                return TopOfStackAccessExpression(start_token, int(offset.text))
+        expression = parser.try_parse_data_source(
+            allow_primitives=True, include_bracket=False, scope=scope,
+        )
 
-            expr = TopOfStackAccessExpression(start_token)
+        if expression is None:
+            parser.rollback()
+            return
 
-        elif start_token.text == "~":
-            self.consume(SpecialToken("~"), err_arg=scope)
-            expr = ModuleAccessExpression(
-                self.parse_identifier_like(scope), start_token
-            )
+        return cls.SingleOperation(
+            "".join(map(lambda e: e.text, operator_tokens)),
+            operator_tokens,
+            expression,
+            base=cls,
+            trace_info=scope.get_trace_info().with_token(list(expression.get_tokens()), operator_tokens),
+        )
 
-        elif start_token.text == "\\":
-            self.consume(SpecialToken("\\"), err_arg=scope)
-            expr = DiscardValueExpression()
-
-        elif (
-            start_token.text == "OP"
-            and allow_op
-            and "OP" in self.INSTRUCTIONS
-            and AbstractOpAssembly.IMPLEMENTATION is not None
-        ):
-            self.consume(start_token, err_arg=scope)
+    @classmethod
+    def try_consume_binary(
+        cls, parser: "Parser", scope: ParsingScope
+    ) -> typing.Optional[IOperation]:
+        parser.save()
 
-            if not (opening := self.try_consume(SpecialToken("("))):
-                raise throw_positioned_error(
-                    scope,
-                    self[-1:1],
-                    "expected '(' after OP when used in expressions",
-                )
+        lhs = parser.try_parse_data_source(allow_primitives=True, include_bracket=False, scope=scope)
 
-            expr = AbstractOpAssembly.IMPLEMENTATION.consume(self, scope)
+        if lhs is None:
+            parser.rollback()
+            return
 
-            if not self.try_consume(SpecialToken(")")):
-                raise throw_positioned_error(
-                    scope,
-                    [opening, self[0]],
-                    "expected ')' after operation",
-                )
+        operator_tokens = cls.try_consume_operator_name(parser, scope, cls.BINARY_OPS)
 
-        else:
+        if operator_tokens is None:
+            parser.rollback()
             return
 
-        if allow_advanced_access:
-            while True:
-                if self.try_consume(SpecialToken("[")):
-                    # Consume either an Integer or a expression
-                    if not (
-                        index := self.try_consume_access_to_value(
-                            allow_primitives=True,
-                            allow_tos=allow_tos,
-                            allow_op=allow_op,
-                            scope=scope,
-                        )
-                    ):
-                        raise throw_positioned_error(
-                            scope,
-                            self.try_inspect() or self[-1],
-                            "expected <expression>"
-                            + (
-                                ""
-                                if not isinstance(self.try_inspect(), IdentifierToken)
-                                else " (did you forget a prefix?)"
-                            ),
-                        )
+        rhs = parser.try_parse_data_source(allow_primitives=True, include_bracket=False, scope=scope)
 
-                    if not self.try_consume(SpecialToken("]")):
-                        raise throw_positioned_error(
-                            scope, self.try_inspect() or self[-1], "expected ']''"
-                        )
+        if rhs is None:
+            print("rhs is invalid")
+            parser.rollback()
+            return
 
-                    expr = SubscriptionAccessExpression(
-                        expr,
-                        index,
-                    )
+        parser.discard_save()
 
-                elif self.try_consume(SpecialToken(".")):
-                    if opening_bracket := self.try_consume(SpecialToken("(")):
-                        if not (
-                            index := self.try_consume_access_to_value(
-                                allow_primitives=True,
-                                allow_tos=allow_tos,
-                                allow_op=allow_op,
-                                scope=scope,
-                                allow_calls=allow_calls,
-                            )
-                        ):
-                            raise throw_positioned_error(
-                                scope,
-                                self.try_inspect() or self[-1],
-                                "expected <expression>"
-                                + (
-                                    ""
-                                    if not isinstance(
-                                        self.try_inspect(), IdentifierToken
-                                    )
-                                    else " (did you forget a prefix?)"
-                                ),
-                            )
-
-                        if not self.try_consume(SpecialToken(")")):
-                            raise throw_positioned_error(
-                                scope,
-                                [opening_bracket, self.try_inspect()],
-                                "expected ')'",
-                            )
-
-                        expr = DynamicAttributeAccessExpression(expr, index)
-
-                    elif self.try_consume(SpecialToken("!")):
-                        name = self.parse_identifier_like(scope)
-                        expr = StaticAttributeAccessExpression(expr, name)
-
-                    else:
-                        name = self.parse_identifier_like(scope)
-                        expr = AttributeAccessExpression(expr, name)
-
-                elif self.try_inspect() == SpecialToken("(") and allow_calls:
-                    expr = AbstractCallAssembly.IMPLEMENTATION.construct_from_partial(
-                        expr, self, scope
-                    )
+        return cls.BinaryOperation(
+            lhs,
+            "".join(map(lambda e: e.text, operator_tokens)),
+            operator_tokens,
+            rhs,
+            base=cls,
+            trace_info=scope.get_trace_info().with_token(
+                list(lhs.get_tokens()), list(rhs.get_tokens()), operator_tokens
+            ),
+        )
 
-                else:
-                    break
+    @classmethod
+    def try_consume_prefix(
+        cls, parser: "Parser", scope: ParsingScope
+    ) -> typing.Optional[IOperation]:
+        operator_tokens = cls.try_consume_operator_name(
+            parser, scope, cls.PREFIX_OPERATORS
+        )
 
-        return expr
+        if operator_tokens is None:
+            return
 
-    def try_parse_data_source(
-        self,
-        allow_tos=True,
-        allow_primitives=False,
-        include_bracket=True,
-        allow_op=True,
-        allow_calls=True,
-        scope=None,
-    ) -> AbstractSourceExpression | None:
-        self.save()
+        operator = "".join(map(lambda e: e.text, operator_tokens))
+        operator_def, arg_count, has_brackets, has_coma_sep = cls.PREFIX_OPERATORS[
+            operator
+        ]
+
+        bracket = parser.try_consume(SpecialToken("("))
+
+        if bracket is None and has_brackets is True:
+            raise PropagatingCompilerException("expected '('").add_trace_level(scope.get_trace_info().with_token(parser[0]))
+        elif bracket is not None and has_brackets is False:
+            raise PropagatingCompilerException("did not expect '('").add_trace_level(scope.get_trace_info().with_token(parser[0], operator_tokens))
+
+        args = []
+
+        if arg_count is not None:
+            for _ in range(arg_count):
+                expr = parser.try_consume_access_to_value(
+                    scope=scope,
+                    allow_calls=True,
+                    allow_tos=True,
+                    allow_primitives=True,
+                    allow_op=True,
+                    allow_advanced_access=True,
+                )
 
-        if include_bracket and not self.try_consume(SpecialToken("(")):
-            self.rollback()
-            return
+                if expr is None:
+                    raise PropagatingCompilerException(
+                        "expected <expression>"
+                    ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
+
+                args.append(expr)
+
+                coma = parser.try_consume(SpecialToken(","))
+
+                if coma is None and has_coma_sep is True:
+                    raise PropagatingCompilerException(
+                        "expected ','"
+                    ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
+
+                elif coma is not None and has_coma_sep is False:
+                    raise PropagatingCompilerException(
+                        "did not expect ','"
+                    ).add_trace_level(scope.get_trace_info().with_token(coma))
+        else:
+            while not parser.try_inspect() == SpecialToken(")"):
+                expr = parser.try_consume_access_to_value(
+                    scope=scope,
+                    allow_calls=True,
+                    allow_tos=True,
+                    allow_primitives=True,
+                    allow_op=True,
+                    allow_advanced_access=True,
+                )
 
-        if access := self.try_consume_access_to_value(
-            allow_tos=allow_tos,
-            allow_primitives=allow_primitives,
-            allow_op=allow_op,
-            allow_calls=allow_calls,
-            scope=scope,
-        ):
-            self.discard_save()
-            if include_bracket:
-                self.consume(SpecialToken(")"))
-            return access
-
-        if allow_primitives:
-            if string := self.try_consume(StringLiteralToken):
-                return ConstantAccessExpression(string.text, string)
-
-            if integer := self.try_consume(IntegerToken):
-                return ConstantAccessExpression(int(integer.text), integer)
-
-            if boolean := self.try_consume(
-                (IdentifierToken("True"), IdentifierToken("False"))
-            ):
-                return ConstantAccessExpression(boolean.text == "True", boolean)
-
-        # print("failed", self.try_inspect())
-
-        self.rollback()
-
-    def try_parse_identifier_like(self) -> IIdentifierAccessor | None:
-        if expr := self.try_consume_multi([SpecialToken("&"), IdentifierToken]):
-            return MacroExpandedIdentifier(expr[1].text, expr)
-
-        if expr := self.try_consume(IdentifierToken):
-            return StaticIdentifier(expr.text, expr)
-
-    def parse_identifier_like(self, scope: ParsingScope) -> IIdentifierAccessor:
-        identifier = self.try_parse_identifier_like()
-
-        if identifier is None:
-            raise throw_positioned_error(
-                scope,
-                self[0],
-                "expected <identifier> or &<identifier>",
-            )
+                if expr is None:
+                    raise PropagatingCompilerException(
+                        "expected <expression>"
+                    ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
+
+                args.append(expr)
+
+                coma = parser.try_consume(SpecialToken(","))
+
+                if (
+                    coma is None
+                    and has_coma_sep is True
+                    and parser[0] != SpecialToken(")")
+                ):
+                    raise PropagatingCompilerException(
+                        "expected ','"
+                    ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
+
+                elif coma is not None and has_coma_sep is False:
+                    raise PropagatingCompilerException(
+                        "did not expect ','"
+                    ).add_trace_level(scope.get_trace_info().with_token(coma))
 
-        return identifier
+        if bracket and not parser.try_consume(SpecialToken(")")):
+            raise PropagatingCompilerException("expected ')'").add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
-    def try_parse_jump_target(self) -> typing.List[IIdentifierAccessor] | None:
-        self.save()
-        tokens = []
+        return cls.PrefixOperator(operator, operator_tokens, args, base=cls, trace_info=scope.get_trace_info())
 
-        if not (t := self.try_parse_identifier_like()):
-            return
+    def __init__(
+        self, operation: IOperation, target: AbstractAccessExpression | None = None
+    ):
+        if operation is None:
+            raise ValueError("operation cannot be null!")
 
-        tokens.append(t)
+        self.operation = operation
+        self.target = target
 
-        while self.try_consume(SpecialToken(":")):
-            t = self.try_parse_identifier_like()
+    def copy(self) -> "AbstractOpAssembly":
+        return type(self)(
+            self.operation.copy(), self.target.copy() if self.target else None
+        )
 
-            if t is None:
-                self.rollback()
-                return
+    def __eq__(self, other):
+        return (
+            type(self) == type(other)
+            and self.operation == other.operation
+            and self.target == other.target
+        )
 
-            tokens.append(t)
+    def __repr__(self):
+        return f"OP({self.operation}{', ' + repr(self.target) if self.target else ''})"
 
-        self.discard_save()
-        return tokens
+    def emit_bytecodes(
+        self, function: MutableFunction, scope: ParsingScope
+    ) -> typing.List[Instruction]:
+        return self.operation.emit_bytecodes(function, scope) + (
+            []
+            if self.target is None
+            else self.target.emit_store_bytecodes(function, scope)
+        )
 
-    def parse_jump_target(self, scope: ParsingScope) -> typing.List[IIdentifierAccessor]:
-        tokens = self.try_parse_jump_target()
+    def emit_store_bytecodes(
+        self, function: MutableFunction, scope: ParsingScope
+    ) -> typing.List[Instruction]:
+        raise RuntimeError(f"cannot assign to an '{self.operation}' operator!")
 
-        if tokens is None:
-            raise throw_positioned_error(
-                scope,
-                self[0],
-                "expected <identifier-like>[{':' <identifier like>}] for jump target"
-            )
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        return self.operation.evaluate_static_value(scope)
 
-        return tokens
+    def visit_parts(
+        self,
+        visitor: typing.Callable[
+            [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
+            typing.Any,
+        ],
+        parents: list,
+    ):
+        return visitor(
+            self,
+            (
+                self.operation.visit_parts(visitor, parents + [self]),
+                self.target.visit_parts(
+                    visitor,
+                    parents + [self],
+                )
+                if self.target
+                else None,
+            ),
+            parents,
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/hook.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/hook.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import types
 
 import typing
 
 from bytecodemanipulation.assembler import Emitter
 
 
+LET_PROPAGATE_EXCEPTIONS_THROUGH = False
+
+
 class ASMFileFinder(importlib.machinery.SourceFileLoader):
     """
     .pyasm file importer
     so the Emitter is bound to module-level parsing if only the .pyasm file is provided
     """
 
     MODULE_CACHE: typing.Dict[str, types.ModuleType] = {}
@@ -39,15 +42,17 @@
             return self.MODULE_CACHE[module.__name__]
 
         self.MODULE_CACHE[module.__name__] = module
 
         with open(self.path, encoding="utf-8") as fid:
             asm_code = fid.read()
 
-        Emitter.execute_module_in_instance(asm_code, module, self.path)
+        module.__file__ = self.path
+
+        Emitter.execute_module_in_instance(asm_code, module, self.path, unwrap_exceptions=not LET_PROPAGATE_EXCEPTIONS_THROUGH)
 
         return module
 
 
 def hook():
     if ASMFileFinder not in sys.meta_path:
         sys.meta_path.append(ASMFileFinder)
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/target.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,29 +101,29 @@
             mutable.reassign_to_function()
 
         return function
 
     return annotation
 
 
-def configurate_makro_parameter(name: str | int, config_pattern: typing.Type):
+def configurate_macro_parameter(name: str | int, config_pattern: typing.Type):
     """
     Configures the type of parameter of a @make_macro annotated function
 
     :param name: the name of the parameter, or the index
     :param config_pattern: the type of parameter
     """
 
     def annotation(function):
         return function
 
     return annotation
 
 
-def apply_operations(target: typing.Callable):
+def apply_operations(target: typing.Callable, unwrap_exceptions=True):
     from bytecodemanipulation.MutableFunction import MutableFunction
     from bytecodemanipulation.assembler.Emitter import apply_inline_assemblies
 
     mutable = MutableFunction(target)
-    apply_inline_assemblies(mutable)
+    apply_inline_assemblies(mutable, unwrap_exceptions=unwrap_exceptions)
     mutable.reassign_to_function()
     return target
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/parser.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/util/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+import traceback
 import typing
 from bytecodemanipulation.assembler.util.tokenizer import (
     AbstractToken,
     IntegerToken,
     BinaryOperatorToken,
     BracketToken,
     IdentifierToken,
@@ -273,16 +274,16 @@
         :raises SyntaxError: if it failed to parse the token (either invalid type or end of stream)
         """
         token: AbstractToken = self.inspect()
 
         if expected:
             if isinstance(expected, AbstractToken):
                 if token != expected:
-                    raise_syntax_error(token, f"Expected {expected}", err_arg)
-                    raise SyntaxError
+                    traceback.print_stack()
+                    raise raise_syntax_error(token, f"Expected {expected}", err_arg)
 
             elif isinstance(expected, list):
                 for element in expected:
                     if isinstance(element, AbstractToken):
                         if token == element:
                             break
                     else:
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/assembler/util/tokenizer.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/assembler/util/tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import typing
 from collections import namedtuple
 
 from .CommonUtil import AbstractCursorStateItem
 
 
 class AbstractToken(abc.ABC):
-    __slots__ = ("text", "line", "column", "span")
+    __slots__ = ("text", "line", "column", "span", "module_file")
 
     def __init__(self, text: str):
         self.text = text
         self.line: int | None = None
         self.column: int | None = None
         self.span: int | None = None
+        self.module_file: str | None = None
 
     def __eq__(self, other):
         return type(other) == type(self) and self.text == other.text
 
     def __repr__(self):
         return f"{type(self).__name__}({repr(self.text)})"
 
@@ -99,20 +100,21 @@
 
     Contains handling code for a linear tokenizer,
     and functions for collecting text easily.
     """
 
     INCLUDE_LINE_INFO = True
 
-    def __init__(self, text: str, initial_line_offset=0):
+    def __init__(self, text: str, initial_line_offset=0, module_file: str | None = None):
         super().__init__()
         self.text = text
         self.old_line_number = 1
         self.old_column_number = 0
         self._line_offset = initial_line_offset
+        self.module_file = module_file
 
     def add_line_offset(self, offset: int):
         self._line_offset += offset
         return self
 
     def is_empty(self) -> bool:
         """
@@ -281,14 +283,15 @@
                     )
 
                 for r in result if isinstance(result, list) else (result,):
                     newline_count = partial[:whitespace_count].count("\n")
                     r.line = self.old_line_number + self._line_offset
                     r.column = self.old_column_number - newline_count
                     r.span = self.cursor - old_cursor
+                    r.module_file = self.module_file
 
                     # print(
                     #     f"parsed string '{repr(partial)[1:-1]}' (line: {r.line}, column: {r.column}, span: {r.span})"
                     # )
 
                     self.old_column_number += r.span
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/builtin_spec.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/builtin_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,19 @@
                     "Random.randrange() missing 1 required positional argument: 'start'"
                 )
             )
         elif (
             container.method_call_descriptor.lookup_method_instr.arg_value
             == random.Random.randrange
         ):
-            pass
+            container.replace_with_raise_exception(
+                TypeError(
+                    "Random.randrange() missing 1 required positional argument: 'start'"
+                )
+            )
         else:
             raise NotImplementedError
     else:
         if container.method_call_descriptor.lookup_method_instr.arg_value == range:
             container.replace_with_raise_exception(
                 TypeError(f"range expected at most 3 arguments, got {len(sources)}")
             )
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 from bytecodemanipulation.assembler.AbstractBase import (
     IIdentifierAccessor,
     StaticIdentifier,
 )
 
 
 class AttributeAccessExpression(AbstractAccessExpression):
-    def __init__(self, root: AbstractAccessExpression, name: IIdentifierAccessor | str):
+    def __init__(self, root: AbstractAccessExpression, name: IIdentifierAccessor | str, trace_info=None):
         self.root = root
         self.name = name if not isinstance(name, str) else StaticIdentifier(name)
+        self.trace_info = trace_info
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.root == other.root
             and self.name == other.name
         )
@@ -56,18 +57,12 @@
     ):
         return visitor(
             self, (self.root.visit_parts(visitor, parents + [self]),), parents
         )
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
         return (
-            list(self.root.get_tokens()) + list(self.name.get_tokens()) + [self.token]
+            list(self.root.get_tokens()) + list(self.name.get_tokens())
         )
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
-        base = self.root.evaluate_static_value(scope)
-        name = self.name(scope)
-
-        if not hasattr(base, name):
-            raise NotImplementedError
-
-        return getattr(base, name)
+        raise NotImplementedError
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/CompoundExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/CompoundExpression.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 )
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class CompoundExpression(AbstractExpression, IAssemblyStructureVisitable):
-    def __init__(self, children: typing.List[AbstractExpression] = None):
+    def __init__(self, children: typing.List[AbstractExpression] | AbstractExpression = None):
+        if isinstance(children, AbstractExpression):
+            children = [children]
+
         self.children = children or []
 
     def __eq__(self, other):
         return type(self) == type(other) and self.children == other.children
 
     def __repr__(self):
         return f"Compound({repr(self.children)[1:-1]})"
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import copy
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class ConstantAccessExpression(AbstractAccessExpression):
     IS_STATIC = True
 
-    def __init__(self, value, token: AbstractToken = None):
+    def __init__(self, value, token: AbstractToken = None, trace_info=None):
         self.value = value
         self.token = token
+        self.trace_info = trace_info
 
     def __eq__(self, other):
         return isinstance(other, type(self)) and self.value == other.value
 
     def __repr__(self):
         return f"CONSTANT({repr(self.value)})"
 
@@ -29,16 +30,16 @@
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return [Instruction("LOAD_CONST", self.value)]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        raise throw_positioned_error(
-            scope, self.token, f"Cannot assign to a constant: {self}"
-        )
+        raise PropagatingCompilerException(
+            f"Cannot assign to a constant: {self}"
+        ).add_trace_level(self.trace_info.with_token(self.token))
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
         return (self.token,)
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
         return self.value
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class DerefAccessExpression(AbstractAccessExpression):
-    PREFIX = "§"
+class GlobalAccessExpression(AbstractAccessExpression):
+    PREFIX = "@"
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value.isdigit():
             value = int(value)
 
         return [
             Instruction.create_with_token(
-                self.token, Opcodes.LOAD_DEREF, value
+                self.token, Opcodes.LOAD_GLOBAL, value
             )
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value.isdigit():
             value = int(value)
 
         return [
             Instruction.create_with_token(
-                self.token, Opcodes.STORE_DEREF, value
+                self.token, Opcodes.STORE_GLOBAL, value
             )
         ]
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
         raise NotImplementedError  # todo: implement in some cases
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class DynamicAttributeAccessExpression(AbstractAccessExpression):
     def __init__(
-        self, root: AbstractAccessExpression, name_expr: AbstractSourceExpression
+        self, root: AbstractAccessExpression, name_expr: AbstractSourceExpression, trace_info=None,
     ):
         self.root = root
         self.name_expr = name_expr
+        self.trace_info = trace_info
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.root == other.root
             and self.name_expr == other.name_expr
         )
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import typing
-
-from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
+from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.data.shared.instructions.IfAssembly import AbstractIFAssembly
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class GlobalAccessExpression(AbstractAccessExpression):
-    PREFIX = "@"
-
-    def emit_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        value = self.get_name(scope)
-
-        if value.isdigit():
-            value = int(value)
-
-        return [
-            Instruction.create_with_token(
-                self.token, Opcodes.LOAD_GLOBAL, value
+@Parser.register
+class IFAssembly(AbstractIFAssembly):
+    def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
+
+        if self.label_name is None:
+            end = Instruction("NOP")
+        else:
+            end = Instruction(
+                function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text + "_END"
             )
-        ]
-
-    def emit_store_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        value = self.get_name(scope)
 
-        if value.isdigit():
-            value = int(value)
-
-        return [
-            Instruction.create_with_token(
-                self.token, Opcodes.STORE_GLOBAL, value
+        return (
+            (
+                []
+                if self.label_name is None
+                else [
+                    Instruction(
+                        function,
+                        -1,
+                        Opcodes.BYTECODE_LABEL,
+                        self.label_name.text + "_HEAD",
+                    )
+                ]
             )
-        ]
-
-    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
-        raise NotImplementedError  # todo: implement in some cases
-
-    def get_tokens(self) -> typing.Iterable[AbstractToken]:
-        return (self.token,)
+            + self.source.emit_bytecodes(function, scope)
+            + [Instruction("POP_JUMP_IF_FALSE", end)]
+            + (
+                []
+                if self.label_name is None
+                else [
+                    Instruction(
+                        function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text
+                    )
+                ]
+            )
+            + self.body.emit_bytecodes(function, scope)
+            + [end]
+        )
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import builtins
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class GlobalStaticAccessExpression(AbstractAccessExpression):
@@ -33,16 +33,13 @@
     ) -> typing.List[Instruction]:
         raise RuntimeError("Cannot assign to a constant global")
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
         if self.get_name(scope) in scope.globals_dict:
             return scope.globals_dict[self.get_name(scope)]
 
-        raise throw_positioned_error(
-            scope,
-            self.token,
-            f"Name {self.get_name(scope)} not found!",
-            NameError,
-        )
+        raise PropagatingCompilerException(
+            f"Name {self.get_name(scope)} not found!"
+        ).add_trace_level(scope.get_trace_info().with_token(self.token))
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
         return (self.token,)
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,17 +13,19 @@
     PREFIX = "$"
 
     def __init__(
         self,
         name: "IIdentifierAccessor | str",
         token: AbstractToken | typing.List[AbstractToken] = None,
         prefix="",
+        trace_info=None,
     ):
         super(LocalAccessExpression, self).__init__(name, token)
         self.prefix = prefix
+        self.trace_info = trace_info
 
     def __repr__(self):
         return f"{self.PREFIX}{self.prefix}{self.name}"
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
@@ -51,8 +53,8 @@
             Instruction.create_with_token(self.token, Opcodes.STORE_FAST, self.prefix + value)
         ]
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
         raise NotImplementedError  # todo: implement in some cases
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
-        return (self.token,)
+        return (self.token,) + tuple(self.name.get_tokens())
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/StoreAssembly.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,84 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
+from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
+    AbstractAssemblyInstruction,
+)
+from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
+from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
+from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
-from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
+from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class MacroParameterAccessExpression(AbstractAccessExpression):
-    PREFIX = "&"
+@Parser.register
+class StoreAssembly(AbstractAssemblyInstruction):
+    # STORE <access> [(expression)]
+    NAME = "STORE"
+
+    @classmethod
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "StoreAssembly":
+        access = parser.try_consume_access_to_value(
+            allow_tos=False, scope=scope, allow_calls=False
+        )
+
+        if access is None:
+            raise PropagatingCompilerException(
+                "expected <expression> after STORE"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
+
+        source = parser.try_parse_data_source(scope=scope)
+
+        return cls(access, source)
+
+    def __init__(
+        self,
+        access_token: AbstractAccessExpression,
+        source: AbstractSourceExpression | None = None,
+    ):
+        self.access_token = access_token
+        self.source = source
+
+    def __eq__(self, other):
+        return (
+            type(self) == type(other)
+            and self.access_token == other.access_token
+            and self.source == other.source
+        )
+
+    def __repr__(self):
+        return f"STORE({self.access_token}, {self.source})"
+
+    def copy(self) -> "StoreAssembly":
+        return StoreAssembly(
+            self.access_token, self.source.copy() if self.source else None
+        )
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        value = self.get_name(scope)
-
-        if value not in scope.macro_parameter_namespace:
-            raise throw_positioned_error(
-                scope, self.token, "Name not found in macro var space"
-            )
-
-        if scope.macro_parameter_namespace[value] != self and hasattr(
-            scope.macro_parameter_namespace[value], "emit_bytecodes"
-        ):
-            instructions = scope.macro_parameter_namespace[value].emit_bytecodes(
-                function, scope
-            )
-
-            for instr in instructions:
-                if instr.has_local():
-                    instr.change_arg_value(":" + instr.arg_value)
-
-            return instructions
-
-        return [
-            Instruction.create_with_token(
-                self.token, Opcodes.MACRO_LOAD_PARAMETER, value
-            )
-        ]
-
-    def emit_store_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        value = self.get_name(scope)
-
-        if value not in scope.macro_parameter_namespace:
-            raise throw_positioned_error(
-                scope, self.token, "Name not found in macro var space"
-            )
-
-        if scope.macro_parameter_namespace[value] != self and hasattr(
-            scope.macro_parameter_namespace[value], "emit_bytecodes"
-        ):
-            instructions = scope.macro_parameter_namespace[value].emit_store_bytecodes(
-                function, scope
-            )
-
-            for instr in instructions:
-                if instr.has_local():
-                    instr.change_arg_value(":" + instr.arg_value)
-
-            return instructions
-
-        return [
-            Instruction.create_with_token(
-                self.token, Opcodes.MACRO_STORE_PARAMETER, value
-            )
-        ]
-
-    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
-        name = self.name(scope)
-
-        if name not in scope.macro_parameter_namespace:
-            raise NotImplementedError
-
-        return scope.macro_parameter_namespace[name].evaluate_static_value(scope)
-
-    def get_tokens(self) -> typing.Iterable[AbstractToken]:
-        return (self.token,)
+        return (
+            [] if self.source is None else self.source.emit_bytecodes(function, scope)
+        ) + self.access_token.emit_store_bytecodes(function, scope)
+
+    def visit_parts(
+        self,
+        visitor: typing.Callable[
+            [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
+            typing.Any,
+        ],
+        parents: list,
+    ):
+        return visitor(
+            self,
+            (
+                self.access_token.visit_parts(visitor, parents + [self]),
+                self.source.visit_parts(visitor, parents + [self])
+                if self.source is not None
+                else None,
+            ),
+            parents,
+        )
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import sys
 import types
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 root = __file__
@@ -44,15 +45,21 @@
             return module
 
         return cls._CACHE[module_name]
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        value = self._cached_lookup(self.get_name(scope))
+        try:
+            value = self._cached_lookup(self.get_name(scope))
+        except (ModuleNotFoundError, ImportError) as e:
+            raise PropagatingCompilerException(
+                f"expected <module>, got '{self.name(scope)}'"
+            ).add_trace_level(scope.get_trace_info().with_token(self.token), "\n".join(map(str, e.args))) from None
+
         return [
             Instruction.create_with_token(
                 self.token, Opcodes.LOAD_CONST, value
             )
         ]
 
     def emit_store_bytecodes(
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 class StaticAttributeAccessExpression(AbstractAccessExpression):
     IS_STATIC = True
 
     def __init__(
         self,
         root: AbstractAccessExpression,
         name: typing.Union["IIdentifierAccessor", str],
+        trace_info=None,
     ):
         self.root = root
         self.name = name if not isinstance(name, str) else StaticIdentifier(name)
+        self.trace_info = trace_info
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.root == other.root
             and self.name == other.name
         )
@@ -71,8 +73,8 @@
 
         if not hasattr(base, self.name(scope)):
             raise NotImplementedError
 
         return getattr(base, self.name(scope))
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
-        return list(self.root.get_tokens()) + [self.token]
+        return list(self.root.get_tokens())
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 
 class SubscriptionAccessExpression(AbstractAccessExpression):
     def __init__(
         self,
         base_expr: "AbstractAccessExpression",
         index_expr: AbstractAccessExpression | IntegerToken,
         token=None,
+        trace_info=None,
     ):
         self.base_expr = base_expr
         self.index_expr = index_expr
         self.token = token
+        self.trace_info = trace_info
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.base_expr == other.base_expr
             and self.index_expr == self.index_expr
         )
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AssertAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/AssertAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC
 
 from bytecodemanipulation.assembler.AbstractBase import (
     ParsingScope,
     AbstractSourceExpression,
 )
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.Parser import Parser
 
 
 class AbstractAssertAssembly(AbstractAssemblyInstruction, ABC):
@@ -16,17 +16,17 @@
     NAME = "ASSERT"
 
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractAssertAssembly":
         target = parser.try_consume_access_to_value(scope=scope, allow_primitives=True)
 
         if target is None:
-            raise throw_positioned_error(
-                scope, parser[0], "expected <expression>"
-            )
+            raise PropagatingCompilerException(
+                "expected <expression> after ASSERT"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         return cls(
             target,
             parser.try_consume_access_to_value(scope=scope, allow_primitives=True),
         )
 
     def __init__(
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import sys
 import typing
 import warnings
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import print_positional_warning
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException, TraceInfo
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
@@ -23,32 +23,35 @@
     NAME = "ASSERT_STATIC"
 
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractAssertAssembly":
         target = parser.try_consume_access_to_value(scope=scope, allow_primitives=True)
 
         if target is None:
-            raise throw_positioned_error(
-                scope, parser[0], "expected <expression>"
-            )
+            raise PropagatingCompilerException(
+                "expected <expression>"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         return cls(
             target,
             parser.try_consume_access_to_value(scope=scope, allow_primitives=True),
             base_token=scope.last_base_token,
+            trace_info=scope.get_trace_info(),
         )
 
     def __init__(
         self, source: AbstractSourceExpression,
         text: AbstractSourceExpression = None,
         base_token: AbstractToken = None,
+        trace_info: TraceInfo = None,
     ):
         self.source = source
         self.text = text
         self.base_token = base_token
+        self.trace_info = trace_info
 
     def __repr__(self):
         return f"ASSERT({self.source}, {self.text})"
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
@@ -62,38 +65,31 @@
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         try:
             value = self.source.evaluate_static_value(scope)
         except NotImplementedError:
             print("<target>:", self.source)
+            print(scope.macro_parameter_namespace_stack)
 
-            raise throw_positioned_error(
-                scope,
-                self.base_token or list(self.source.get_tokens()),
-                "Expected <static evaluate-able at 'expression'>",
-            ) from None
+            raise PropagatingCompilerException(
+                f"Expected <static evaluate-able> at 'expression', got '{type(self.source).__name__}' as type"
+            ).add_trace_level(self.trace_info.with_token(self.base_token, list(self.source.get_tokens()))) from None
 
         if not value:
             try:
                 message = (
                     "expected <true-ish value>"
                     if self.text is None
                     else self.text.evaluate_static_value(scope)
                 )
             except NotImplementedError:
-                print_positional_warning(
-                    scope,
-                    list(self.source.get_tokens()),
-                    f"<message> could not be evaluated (got syntax element: {self.text})",
-                )
+                print(f"SyntaxWarning: <message> could not be evaluated (got syntax element: {self.text})", file=sys.stderr)
+                self.trace_info.with_token(list(self.source.get_tokens())).print_stack(sys.stderr)
 
                 message = "expected <true-ish value> (message not arrival)"
 
-            raise throw_positioned_error(
-                scope,
-                list(self.source.get_tokens()),
-                f"assertion failed: {message}",
-                AssertionError,
-            )
+            raise PropagatingCompilerException(
+                "assertion failed: " + message
+            ).add_trace_level(self.trace_info.with_token(list(self.source.get_tokens()))).set_underlying_exception(AssertionError)
 
         return []
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/CallAssembly.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.data.shared.expressions.MacroAccessExpression import (
     MacroAccessExpression,
 )
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException, TraceInfo
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 
 
 if typing.TYPE_CHECKING:
     from bytecodemanipulation.assembler.Parser import Parser
 
 
@@ -172,58 +172,47 @@
                 call_target = parser.try_parse_data_source(
                     include_bracket=False, scope=scope, allow_calls=False
                 )
 
                 if isinstance(call_target, AbstractCallAssembly):
                     # should not be reachable
 
-                    raise throw_positioned_error(
-                        scope,
-                        list(call_target.get_tokens()),
-                        "Must be not <call assembly> (internal error)",
-                        RuntimeError,
-                    )
+                    raise PropagatingCompilerException(
+                        "Must not be <call assembly> (internal error)"
+                    ).add_trace_level(scope.get_trace_info().with_token(list(call_target.get_tokens())))
 
             else:
                 name = [parser.consume(IdentifierToken, err_arg=scope)]
 
                 while expr := parser.try_consume(SpecialToken(":")):
                     # todo: allow identifier-like
                     part = parser.try_consume(IdentifierToken)
 
                     if part is None:
-                        raise throw_positioned_error(
-                            scope,
-                            [expr, parser[0]],
-                            "<identifier> expected after '.'",
-                        )
+                        raise PropagatingCompilerException(
+                            "<identifier> expected after '.'"
+                        ).add_trace_level(scope.get_trace_info().with_token(expr, parser[0]))
 
                     name.append(part)
 
                 call_target = MacroAccessExpression(name)
 
         if call_target is None:
             # should be unreachable
 
-            raise throw_positioned_error(
-                scope,
-                parser.try_inspect(),
+            raise PropagatingCompilerException(
                 "expected <expression> to be called (did you forget the prefix?)"
-                if not is_macro
-                else "expected <macro name>",
-            )
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         args: typing.List[AbstractCallAssembly.IArg] = []
 
         if not (opening_bracket := parser.try_consume(SpecialToken("("))):
-            raise throw_positioned_error(
-                scope,
-                parser[0],
-                "Expected '(' after <call target>",
-            )
+            raise PropagatingCompilerException(
+                "Expected '(' after <call target>"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0], list(call_target.get_tokens())))
 
         has_seen_keyword_arg = False
 
         while not (bracket := parser.try_consume(SpecialToken(")"))):
             parser.save()
 
             identifier = parser.try_parse_identifier_like()
@@ -238,15 +227,15 @@
                 key = identifier
 
                 parser.consume(SpecialToken("="))
 
                 is_dynamic = is_partial and bool(parser.try_consume(SpecialToken("?")))
 
                 expr = parser.try_parse_data_source(
-                    allow_primitives=True, include_bracket=False
+                    allow_primitives=True, include_bracket=False, scope=scope
                 )
 
                 args.append(AbstractCallAssembly.KwArg(key, expr, is_dynamic))
 
                 has_seen_keyword_arg = True
 
             elif parser[0].text == "*" and not is_macro:
@@ -258,53 +247,47 @@
                     )
                     args.append(AbstractCallAssembly.KwArgStar(expr))
                     has_seen_keyword_arg = True
 
                 elif not has_seen_keyword_arg:
                     parser.consume(SpecialToken("*"))
                     expr = parser.try_parse_data_source(
-                        allow_primitives=True, include_bracket=False
+                        allow_primitives=True, include_bracket=False, scope=scope
                     )
                     args.append(AbstractCallAssembly.StarArg(expr))
 
                 else:
-                    raise throw_positioned_error(
-                        scope,
-                        parser.try_inspect(),
-                        "*<arg> only allowed before keyword arguments!",
-                    )
+                    raise PropagatingCompilerException(
+                        "*<arg> only allowed before keyword arguments!"
+                    ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
             elif not has_seen_keyword_arg:
                 if is_macro and ((inner_opening_bracket := parser[0]) == SpecialToken("[")):
                     parser.consume(SpecialToken("["))
 
                     to_be_stored_at = []
 
                     while not parser.try_inspect() == SpecialToken("]"):
                         parser.try_consume(SpecialToken("$"))
                         base = parser.try_parse_identifier_like()
 
                         if base is None:
-                            raise throw_positioned_error(
-                                scope,
-                                [inner_opening_bracket, parser[0]],
-                                "Expected <expression> after ','",
-                            )
+                            raise PropagatingCompilerException(
+                                "Expected <expression> after ','"
+                            ).add_trace_level(scope.get_trace_info().with_token(inner_opening_bracket, parser[0]))
 
                         to_be_stored_at.append(base)
 
                         if not parser.try_consume(SpecialToken(",")):
                             break
 
                     if not parser.try_consume(SpecialToken("]")):
-                        raise throw_positioned_error(
-                            scope,
-                            [inner_opening_bracket, parser[0]],
-                            "Expected ']' closing '['",
-                        )
+                        raise PropagatingCompilerException(
+                            "Expected ']' closing '['"
+                        ).add_trace_level(scope.get_trace_info().with_token(inner_opening_bracket, parser[0]))
 
                     expr = parser.parse_body(scope=scope)
                     expr.to_be_stored_at = to_be_stored_at
                     is_dynamic = False
 
                 # todo: maybe parse here also partial variable names
                 elif is_macro and parser[0] == SpecialToken("{"):
@@ -313,78 +296,72 @@
                     is_dynamic = False
 
                 else:
                     is_dynamic = is_partial and bool(
                         parser.try_consume(SpecialToken("?"))
                     )
 
-                    expr = parser.try_consume_access_to_value(allow_primitives=True)
+                    expr = parser.try_consume_access_to_value(allow_primitives=True, scope=scope)
 
                     if expr is None:
                         if parser[0] == SpecialToken(")"):
                             break
 
-                        raise throw_positioned_error(
-                            scope, parser[0], "<expression> expected"
-                        )
+                        raise PropagatingCompilerException(
+                            "Expected <expression>"
+                        ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
                 args.append(AbstractCallAssembly.Arg(expr, is_dynamic))
 
             else:
-                raise throw_positioned_error(
-                    scope,
-                    parser.try_inspect(),
-                    "pure <arg> only allowed before keyword arguments",
-                )
+                raise PropagatingCompilerException(
+                    "pure <arg> only allowed before keyword arguments"
+                ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
             if not parser.try_consume(SpecialToken(",")):
                 break
 
         if bracket is None and not parser.try_consume(SpecialToken(")")):
-            raise throw_positioned_error(
-                scope,
-                [opening_bracket, parser[0]],
-                "expected ')' matching '('",
-            )
+            raise PropagatingCompilerException(
+                "Expected ')' matching '('"
+            ).add_trace_level(scope.get_trace_info().with_token(opening_bracket, parser[0]))
 
         if allow_target and (arrow_0 := parser.try_consume(SpecialToken("-"))):
 
             if not (arrow_1 := parser.try_consume(SpecialToken(">"))):
-                raise throw_positioned_error(
-                    scope,
-                    [arrow_0, parser[0]],
-                    "expected '>' after '-' to fill out <target> expression",
-                )
+                raise PropagatingCompilerException(
+                    "Expected '>' after '-' to fill out <target> expression"
+                ).add_trace_level(scope.get_trace_info().with_token(arrow_0, parser[0]))
 
             target = parser.try_consume_access_to_value(scope=scope)
 
             if target is None:
-                raise throw_positioned_error(
-                    scope,
-                    [arrow_0, arrow_1],
-                    "expected <target> expression after '->'",
-                )
+                raise PropagatingCompilerException(
+                    "expected <target> expression after '->'"
+                ).add_trace_level(scope.get_trace_info().with_token(arrow_0, arrow_1))
         else:
             target = None
 
-        return cls(call_target, args, target, is_partial, is_macro)
+        return cls(call_target, args, target, is_partial, is_macro, trace_info=scope.get_trace_info().with_token(list(call_target.get_tokens())))
 
     def __init__(
         self,
         call_target: AbstractSourceExpression,
         args: typing.List["AbstractCallAssembly.IArg"],
         target: AbstractAccessExpression | None = None,
         is_partial: bool = False,
         is_macro: bool = False,
+        trace_info: typing.Optional[TraceInfo] = None,
     ):
         self.call_target = call_target
         self.args = args
         self.target = target
         self.is_partial = is_partial
         self.is_macro = is_macro
+        self.trace_info = trace_info
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/WhileAssembly.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,133 +1,112 @@
 import abc
-
 import typing
 
+from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
+from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
-from bytecodemanipulation.assembler.AbstractBase import (
-    ParsingScope,
-    IAssemblyStructureVisitable,
-    AbstractExpression,
-)
+from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
-from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
-    ConstantAccessExpression,
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
+from bytecodemanipulation.assembler.util.parser import AbstractExpression
+from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
+    CompoundExpression,
 )
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
-    CompoundExpression,
-)
 
 
-class AbstractClassDefinitionAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # CLASS <name> '<' <exposed namespace> '>' ['(' [<parent> {',' <parent>}] ')'] '{' ... '}'
-    NAME = "CLASS"
+class AbstractWhileAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # # WHILE <expression> ['\'' <label name> '\''] '{' <body> '}'
+    NAME = "WHILE"
 
     @classmethod
-    def consume(
-        cls, parser: "Parser", scope: ParsingScope
-    ) -> "AbstractClassDefinitionAssembly":
-        name = parser.parse_identifier_like(scope)
-
-        if name is None:
-            raise throw_positioned_error(
-                scope,
-                parser[0],
-                "Expected <identifier like>"
-            )
-
-        namespace = None
-
-        if opening_bracket := parser.try_consume(SpecialToken("<")):
-            # todo: maybe use try_parse_identifier_like() instead
-            namespace_f = parser.try_consume(IdentifierToken)
-
-            if namespace_f is None:
-                raise throw_positioned_error(
-                    scope,
-                    parser[0],
-                    "<name> expected",
-                )
-
-            namespace = [namespace_f.text]
-
-            while parser.try_consume(SpecialToken(":")):
-                p = parser.try_consume(IdentifierToken)
-
-                if p is None:
-                    raise throw_positioned_error(
-                        scope,
-                        [namespace_f, parser[0]],
-                        "<name> expected after ':' to complete namespace name",
-                    )
-
-                namespace.append(p.text)
-
-            if parser.try_consume(SpecialToken(">")) is None:
-                raise throw_positioned_error(
-                    scope,
-                    [opening_bracket, parser[0]],
-                    "expected '>' to close namespace declaration",
-                )
-
-        parents = []
-
-        if opening_bracket := parser.try_consume(SpecialToken("(")):
-            if parent := parser.try_consume_access_to_value():
-                parents.append(parent)
-
-                while parser.try_consume(SpecialToken(",")):
-                    if parser[0] == SpecialToken(")"):
-                        break
-
-                    parent = parser.try_consume_access_to_value()
-                    if parent is None:
-                        raise throw_positioned_error(
-                            scope,
-                            parser[0],
-                            "Expected <expression> for parent",
-                        )
-
-                    parents.append(parent)
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractWhileAssembly":
+        condition = parser.try_parse_data_source(
+            allow_primitives=True, include_bracket=False, scope=scope
+        )
+
+        if condition is None:
+            raise PropagatingCompilerException(
+                "expected <expression> after WHILE for condition"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
+
+        if parser.try_consume(SpecialToken("'")):
+            label_name = parser.parse_jump_target(scope)
+
+            if not parser.try_consume(SpecialToken("'")):
+                raise PropagatingCompilerException(
+                    "expected ' closing <label name>"
+                ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
-            if not parser.try_consume(SpecialToken(")")):
-                raise throw_positioned_error(scope, [opening_bracket, parser[0]], "Expected ')'")
+        else:
+            label_name = None
 
-        if not parents:
-            parents = [ConstantAccessExpression(object)]
+        body = parser.parse_body(scope=scope)
 
-        code_block = parser.parse_body(scope=scope, namespace_part=namespace)
         return cls(
-            name,
-            parents,
-            code_block,
+            condition,
+            body,
+            label_name,
         )
 
     def __init__(
-        self, name: IIdentifierAccessor, parents, code_block: CompoundExpression
+        self,
+        source: AbstractSourceExpression,
+        body: CompoundExpression,
+        label_name: typing.List[IIdentifierAccessor] | str | None = None,
     ):
-        self.name = name
-        self.parents = parents
-        self.code_block = code_block
-
-    def __repr__(self):
-        return f"ClassAssembly::'{self.name}'({','.join(map(repr, self.parents))}){{{self.code_block}}}"
+        self.source = source
+        self.body = body
+        self.label_name = (
+            label_name
+            if not isinstance(label_name, str)
+            else [StaticIdentifier(e) for e in label_name.split(":")]
+        ) if label_name is not None else None
 
     def copy(self):
-        return AbstractClassDefinitionAssembly(
-            self.name,
-            [parent.copy() for parent in self.parents],
-            self.code_block.copy(),
-        )
+        return type(self)(self.source.copy(), self.body.copy(), self.label_name.copy())
 
     def __eq__(self, other):
         return (
-            isinstance(other, type(self))
-            and self.name == other.name
-            and self.parents == other.parents
-            and self.code_block == other.code_block
+            type(self) == type(other)
+            and self.source == other.source
+            and self.body == other.body
+            and self.label_name == other.label_name
+        )
+
+    def __repr__(self):
+        c = "'"
+        return f"WHILE({self.source}{'' if self.label_name is None else ', label='+c+repr(self.label_name)+c}) -> {{{self.body}}}"
+
+    def visit_parts(
+        self,
+        visitor: typing.Callable[
+            [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
+            typing.Any,
+        ],
+        parents: list,
+    ):
+        return visitor(
+            self, (self.source.visit_parts(visitor), self.body.visit_parts(visitor))
         )
+
+    def visit_assembly_instructions(
+        self, visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any]
+    ):
+        return visitor(self, (self.body.visit_assembly_instructions(visitor),))
+
+    def get_labels(self, scope: ParsingScope):
+        name = ":".join(e(scope) for e in self.label_name)
+
+        return (
+            set()
+            if self.label_name is None
+            else {
+                name,
+                name + ":END",
+                name + ":INNER",
+            }
+        ) | self.body.get_labels(scope)
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 import itertools
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Instruction import Instruction
@@ -42,72 +42,72 @@
             ]
             return bytecode
 
     @classmethod
     def consume(
         cls, parser: "Parser", scope: ParsingScope
     ) -> "AbstractForEachAssembly":
-        initial = parser.try_consume_access_to_value()
+        initial = parser.try_consume_access_to_value(scope=scope)
         if initial is None:
-            raise throw_positioned_error(
-                scope, parser[0], "initial <expression> expected"
-            )
+            raise PropagatingCompilerException(
+                "expected <expression> after FOREACH"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         variables = [initial]
 
-        while parser.try_consume(SpecialToken(",")):
+        while separator := parser.try_consume(SpecialToken(",")):
 
-            expr = parser.try_consume_access_to_value()
+            expr = parser.try_consume_access_to_value(scope=scope)
 
             if expr is None:
-                raise throw_positioned_error(
-                    scope, parser[0], "further <expression> expected after ','"
-                )
+                raise PropagatingCompilerException(
+                    "expected <expression> after ','"
+                ).add_trace_level(scope.get_trace_info().with_token(separator, parser[0]))
 
             variables.append(expr)
 
         if not parser.try_consume(IdentifierToken("IN")):
-            raise throw_positioned_error(scope, parser[0], "'IN' expected")
+            raise PropagatingCompilerException(
+                "expected 'IN' after FOREACH and <expression>..."
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
-        source = parser.try_consume_access_to_value()
+        source = parser.try_consume_access_to_value(scope=scope)
         if not source:
-            raise throw_positioned_error(
-                scope, parser[0], "base iterator <expression> expected"
-            )
+            raise PropagatingCompilerException(
+                "expected <expression> after 'IN'"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         sources = [source]
 
         multi = None
-        while parser.try_consume(SpecialToken(",")) or (
+        while separator := (parser.try_consume(SpecialToken(",")) or (
             multi := parser.try_consume(SpecialToken("*"))
-        ):
-            source = parser.try_consume_access_to_value()
+        )):
+            source = parser.try_consume_access_to_value(scope=scope)
             if not source:
-                raise throw_positioned_error(
-                    scope, parser[0], f"further iterator <expression> expected after '{'*' if multi else ','}'"
-                )
+                raise PropagatingCompilerException(
+                    f"expected <expression> after '{separator.text}' and <expression>..."
+                ).add_trace_level(scope.get_trace_info().with_token(separator, parser[0]))
 
             if multi:
                 s = sources[-1]
 
                 if isinstance(s, cls.ForEachMultiplier):
                     s.items.append(source)
                 else:
                     sources[-1] = cls.ForEachMultiplier(s, source)
 
                 multi = None
             else:
                 sources.append(source)
 
         if len(variables) != len(sources):
-            raise throw_positioned_error(
-                scope,
-                scope.last_base_token,
+            raise PropagatingCompilerException(
                 f"Number of Variables ({len(variables)}) must equal number of Sources ({len(sources)})",
-            )
+            ).add_trace_level(scope.get_trace_info().with_token(scope.last_base_token))
 
         body = parser.parse_body(scope=scope)
         return cls(
             variables,
             sources,
             body,
             typing.cast(IdentifierToken, scope.last_base_token),
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException, TraceInfo
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.data.shared.instructions.CallAssembly import (
     AbstractCallAssembly,
 )
@@ -35,19 +35,17 @@
             prefix += "|"
 
         if prefix == "":
             while parser.try_consume(SpecialToken(":")):
                 prefix += ":"
 
         elif error := parser.try_consume(SpecialToken(":")):
-            raise throw_positioned_error(
-                scope,
-                error,
-                "Cannot parse '|' and ':' as inter-fix for <function name>",
-            )
+            raise PropagatingCompilerException(
+                "Cannot parser '|' and ':' as inter-fix for <function name>",
+            ).add_trace_level(scope.get_trace_info().with_token(error))
 
         func_name = parser.parse_identifier_like(scope)
 
         bound_variables: typing.List[typing.Tuple[IIdentifierAccessor, bool]] = []
         args = []
 
         if parser.try_consume(SpecialToken("<")):
@@ -65,51 +63,45 @@
                         break
 
                     bound_variables.append((expr, is_static))
 
             parser.consume(SpecialToken(">"), err_arg=scope)
 
         if (opening_bracket := parser.try_consume(SpecialToken("("))) is None:
-            raise throw_positioned_error(
-                scope,
-                parser[0],
-                "expected '(' after <identifier>"
-            )
+            raise PropagatingCompilerException(
+                f"expected '(' after <{'identifier' if not bound_variables else 'bound variables'}>"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         while parser.try_inspect() != SpecialToken(")"):
             arg = None
 
             star = parser.try_consume(SpecialToken("*"))
             star_star = parser.try_consume(SpecialToken("*"))
             identifier = parser.try_parse_identifier_like()
 
             if not identifier:
                 if star:
-                    raise throw_positioned_error(
-                        scope,
-                        [star, star_star],
+                    raise PropagatingCompilerException(
                         "Expected <identifier> after '*'"
                         if not star_star
-                        else "Expected <identifier> after '**'",
-                    )
+                        else "Expected <identifier> after '**'"
+                    ).add_trace_level(scope.get_trace_info().with_token(star, star_star))
 
                 break
 
             if not star:
                 if equal_sign := parser.try_consume(SpecialToken("=")):
                     default_value = parser.try_parse_data_source(
-                        allow_primitives=True, include_bracket=False, allow_op=True
+                        allow_primitives=True, include_bracket=False, allow_op=True, scope=scope
                     )
 
                     if default_value is None:
-                        raise throw_positioned_error(
-                            scope,
-                            [identifier, equal_sign, parser[0]],
-                            "expected <expression>",
-                        )
+                        raise PropagatingCompilerException(
+                            "expected <expression> after '='"
+                        ).add_trace_level(scope.get_trace_info().with_token(list(identifier.get_tokens()), equal_sign, parser[0]))
 
                     arg = AbstractCallAssembly.KwArg(identifier, default_value, token=identifier)
 
             if not arg:
                 if star_star:
                     arg = AbstractCallAssembly.KwArgStar(identifier, token=identifier)
 
@@ -121,75 +113,68 @@
 
             args.append(arg)
 
             if not parser.try_consume(SpecialToken(",")):
                 break
 
         if not parser.try_consume(SpecialToken(")")):
-            raise throw_positioned_error(
-                scope,
-                [opening_bracket, parser[0]],
-                "expected ')' matching '(' in function definition",
-            )
+            raise PropagatingCompilerException(
+                "expected ')' matching '(' in function definition"
+            ).add_trace_level(scope.get_trace_info().with_token(opening_bracket, parser[0]))
 
         if expr := parser.try_consume(SpecialToken("<")):
             if bound_variables:
-                raise throw_positioned_error(
-                    scope,
-                    expr,
-                    "got '<' after '(' ... ')' expression, where a '{' ... '}' (code block) was expected"
-                )
-
-            raise throw_positioned_error(
-                scope,
-                expr,
-                "Respect ordering (got 'args' before 'captured'): DEF ['name'] ['captured'] ('args') [-> 'target'] { code }",
-            )
+                raise PropagatingCompilerException(
+                    "got '<' after '('... ')' expression, where a '{'... '}' (code block) was expected"
+                ).add_trace_level(scope.get_trace_info().with_token(expr))
+
+            raise PropagatingCompilerException(
+                "Respect ordering (got '<' before 'args'): DEF ['name'] ['captured'] ('args') [-> 'target'] { 'code' }"
+            ).add_trace_level(scope.get_trace_info().with_token(expr))
 
         if (arrow_0 := parser.try_consume(SpecialToken("-"))) and (arrow_1 := parser.try_consume(
             SpecialToken(">")
         )):
             target = parser.try_consume_access_to_value(scope=scope)
 
             if target is None:
-                raise throw_positioned_error(
-                    scope,
-                    [arrow_0, arrow_1, parser[0]],
+                raise PropagatingCompilerException(
                     "expected <expression> after '->' as target"
-                )
+                ).add_trace_level(scope.get_trace_info().with_token(arrow_0, arrow_1, parser[0]))
 
         elif arrow_0:
-            raise throw_positioned_error(
-                scope,
-                [arrow_0, parser[0]],
-                "expected '>' after '-' to complete <target> expression",
-            )
+            raise PropagatingCompilerException(
+                "expected '>' after '-' to complete <target> expression"
+            ).add_trace_level(scope.get_trace_info().with_token(arrow_0, parser[0]))
 
         else:
             target = None
 
-        body = parser.parse_body(scope=scope)
+        try:
+            body = parser.parse_body(scope=scope)
+        except PropagatingCompilerException as e:
+            e.add_trace_level(scope.get_trace_info().with_token(list(func_name.get_tokens())), message=f"during parsing function definition {func_name(scope)}")
+            raise e
 
         if expr := parser.try_consume(SpecialToken("-")):
-            raise throw_positioned_error(
-                scope,
-                expr,
-                "Respect ordering (got 'code' before 'target'): DEF ['name'] ['captured'] ('args') [-> 'target'] { code }",
-            )
+            raise PropagatingCompilerException(
+                "Respect ordering (got '-' before 'args'): DEF ['name'] ['captured'] ('args') [-> 'target'] { 'code' }"
+            ).add_trace_level(scope.get_trace_info().with_token(expr))
 
-        return cls(func_name, bound_variables, args, body, target, prefix=prefix)
+        return cls(func_name, bound_variables, args, body, target, prefix=prefix, trace_info=scope.get_trace_info().with_token(list(func_name.get_tokens())))
 
     def __init__(
         self,
         func_name: IIdentifierAccessor | str | None,
         bound_variables: typing.List[typing.Tuple[IIdentifierAccessor, bool] | str],
         args: typing.List[AbstractCallAssembly.IArg],
         body: CompoundExpression,
         target: AbstractAccessExpression | None = None,
         prefix="",
+        trace_info: TraceInfo = None,
     ):
         self.func_name = (
             func_name if not isinstance(func_name, str) else StaticIdentifier(func_name)
         )
         self.bound_variables: typing.List[typing.Tuple[IIdentifierAccessor, bool]] = []
         # var if isinstance(var, IdentifierToken) else IdentifierToken(var) for var in bound_variables]
 
@@ -214,14 +199,15 @@
             else:
                 raise ValueError(element)
 
         self.args = args
         self.body = body
         self.target = target
         self.prefix = prefix
+        self.trace_info = trace_info
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/IfAssembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
@@ -25,25 +25,25 @@
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractIFAssembly":
         source = parser.try_parse_data_source(
             allow_primitives=True, include_bracket=False, scope=scope
         )
 
         if source is None:
-            raise throw_positioned_error(
-                scope, parser.try_inspect(), "expected <expression>"
-            )
+            raise PropagatingCompilerException(
+                "expected <expression> after IF"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         if parser.try_consume(SpecialToken("'")):
             label_name = parser.parse_jump_target(scope)
 
             if not parser.try_consume(SpecialToken("'")):
-                raise throw_positioned_error(
-                    scope, parser.try_inspect(), "expected ' after label name declaration"
-                )
+                raise PropagatingCompilerException(
+                    "expected ' after label name declaration"
+                ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         else:
             label_name = None
 
         body = parser.parse_body(scope=scope)
 
         return cls(
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/JumpAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,26 +27,26 @@
         label_target = parser.parse_jump_target(scope)
 
         if has_quotes:
             parser.consume(SpecialToken("'"))
 
         if parser.try_consume(IdentifierToken("IF")):
             condition = parser.try_parse_data_source(
-                allow_primitives=True, include_bracket=False, allow_op=True
+                allow_primitives=True, include_bracket=False, allow_op=True, scope=scope
             )
 
         elif parser.try_consume(SpecialToken("(")):
             parser.save()
             condition = parser.try_parse_data_source(
-                allow_primitives=True, include_bracket=False, allow_op=True
+                allow_primitives=True, include_bracket=False, allow_op=True, scope=scope
             )
 
             if condition is None or not parser.try_consume(SpecialToken(")")):
                 parser.rollback()
-                condition = AbstractOpAssembly.IMPLEMENTATION.consume(parser, None)
+                condition = AbstractOpAssembly.IMPLEMENTATION.consume(parser, scope)
                 parser.consume(SpecialToken(")"))
             else:
                 parser.discard_save()
 
         else:
             condition = None
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LabelAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/LabelAssembly.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
@@ -19,17 +19,17 @@
     NAME = "LABEL"
 
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "LabelAssembly":
         name = parser.try_parse_jump_target()
 
         if name is None:
-            raise throw_positioned_error(
-                scope, parser[0], "expected <identifier like>"
-            )
+            raise PropagatingCompilerException(
+                "expected <identifier like>"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         return cls(name)
 
     def __init__(self, name: typing.List[IIdentifierAccessor] | str):
         self.name = name if not isinstance(name, str) else [StaticIdentifier(e) for e in name.split(":")]
 
     def __repr__(self):
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/LoadAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class LoadAssembly(AbstractAssemblyInstruction):
@@ -22,25 +22,23 @@
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "LoadAssembly":
         access_expr = parser.try_consume_access_to_value(
             allow_tos=False, allow_primitives=True, scope=scope
         )
 
         if access_expr is None:
-            raise throw_positioned_error(
-                scope, parser.try_inspect(), "expected <expression>"
-            )
+            raise PropagatingCompilerException(
+                "expected <expression> after LOAD"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         if parser.try_consume(SpecialToken("-")):
             if not parser.try_consume(SpecialToken(">")):
-                raise throw_positioned_error(
-                    scope,
-                    parser[-1:1] + [scope.last_base_token],
-                    "expected '>' after '-' to complete '->'",
-                )
+                raise PropagatingCompilerException(
+                    "expected '>' after '-' to complete '->'"
+                ).add_trace_level(scope.get_trace_info().with_token(parser[-1:1], scope.last_base_token))
 
             target = parser.try_consume_access_to_value(scope=scope)
         else:
             target = None
 
         return cls(access_expr, target)
 
@@ -61,15 +59,15 @@
 
     def __repr__(self):
         return (
             f"LOAD({self.access_expr}{', ' + repr(self.target) if self.target else ''})"
         )
 
     def copy(self) -> "LoadAssembly":
-        return LoadAssembly(self.access_expr, self.target)
+        return LoadAssembly(self.access_expr.copy(), self.target.copy() if self.target else None)
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return self.access_expr.emit_bytecodes(function, scope) + (
             self.target.emit_store_bytecodes(function, scope) if self.target else []
         )
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
     ConstantAccessExpression,
 )
 from bytecodemanipulation.data.shared.expressions.GlobalAccessExpression import (
     GlobalAccessExpression,
 )
@@ -33,21 +33,21 @@
             else ConstantAccessExpression(value)
         )
         self.target = target
 
     @classmethod
     def consume(cls, parser: "Parser", scope) -> "AbstractLoadConstAssembly":
         value = parser.try_parse_data_source(
-            allow_primitives=True, include_bracket=False
+            allow_primitives=True, include_bracket=False, scope=scope
         )
 
         if not isinstance(value, (ConstantAccessExpression, GlobalAccessExpression)):
-            raise throw_positioned_error(
-                scope, parser.try_inspect(), "expected <constant epxression>"
-            )
+            raise PropagatingCompilerException(
+                "expected <constant epxression>"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         if parser.try_consume_multi(
             [
                 SpecialToken("-"),
                 SpecialToken(">"),
             ]
         ):
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
@@ -34,35 +34,34 @@
         )
         self.target = target
 
     @classmethod
     def consume(cls, parser: "Parser", scope) -> "AbstractLoadGlobalAssembly":
         parser.try_consume(SpecialToken("@"))
 
-        name = parser.try_consume([IdentifierToken, IntegerToken])
+        # todo: make parse_identifier_like()
+        name = parser.try_consume(IdentifierToken)
 
         if name is None:
-            raise throw_positioned_error(
-                scope, parser.try_inspect(), "expected <name> or <integer>"
-            )
+            raise PropagatingCompilerException(
+                "expected <name>"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
         if parser.try_consume(SpecialToken("-")):
             if not parser.try_consume(SpecialToken(">")):
-                raise throw_positioned_error(
-                    scope,
-                    parser[-1:1] + [scope.last_base_token],
-                    "expected '>' after '-'",
-                )
+                raise PropagatingCompilerException(
+                    "expected '>' after '-'"
+                ).add_trace_level(scope.get_trace_info().with_token(parser[-1:1], scope.last_base_token))
 
             target = parser.try_consume_access_to_value(scope=scope)
 
             if target is None:
-                raise throw_positioned_error(
-                    scope, parser.try_inspect(), "expected <expression>"
-                )
+                raise PropagatingCompilerException(
+                    "expected <expression> after '->'"
+                ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
         else:
             target = None
 
         return cls(name, target)
 
     def __eq__(self, other):
         return (
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/MacroAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import traceback
 import typing
 from abc import ABC
 
 from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
+from bytecodemanipulation.data.shared.expressions.MacroParameterAcessExpression import MacroParameterAccessExpression
 from bytecodemanipulation.MutableFunctionHelpers import capture_local
 
 from bytecodemanipulation.MutableFunctionHelpers import outer_return
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import SpecialToken
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException, TraceInfo
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
@@ -68,14 +69,15 @@
         Parser.register(cls)
 
     class AbstractDataType(ABC):
         IDENTIFIER: str = None
 
         def is_match(
             self,
+            scope: ParsingScope,
             arg: "MacroAssembly.MacroArg",
             arg_accessor: AbstractAccessExpression | CompoundExpression,
         ) -> bool:
             raise NotImplementedError
 
         def emit_for_arg(
             self,
@@ -94,45 +96,54 @@
             raise RuntimeError
 
     class AnyDataType(AbstractDataType):
         IDENTIFIER = "ANY"
 
         def is_match(
             self,
+            scope: ParsingScope,
             arg: "MacroAssembly.MacroArg",
             arg_accessor: AbstractAccessExpression | CompoundExpression,
         ) -> bool:
             return True
 
     class CodeBlockDataType(AbstractDataType):
         IDENTIFIER = "CODE_BLOCK"
 
         def __init__(self, count=0):
             self.count = count
 
         def is_match(
             self,
+            scope: ParsingScope,
             arg: "MacroAssembly.MacroArg",
-            arg_accessor: AbstractAccessExpression | CompoundExpression,
+            arg_accessor: AbstractAccessExpression | CompoundExpression | MacroParameterAccessExpression,
         ) -> bool:
+            if isinstance(arg_accessor, MacroParameterAccessExpression):
+                arg_accessor = scope.lookup_macro_parameter(arg_accessor.name(scope))
+
             return isinstance(arg_accessor, CompoundExpression)
 
     class VariableDataType(AbstractDataType):
         IDENTIFIER = "VARIABLE"
         VALID_ACCESSOR_TYPES = [
             GlobalAccessExpression,
             LocalAccessExpression,
             DerefAccessExpression,
         ]
 
         def is_match(
             self,
+            scope: ParsingScope,
             arg: "MacroAssembly.MacroArg",
             arg_accessor: AbstractAccessExpression | CompoundExpression,
         ) -> bool:
+            if isinstance(arg_accessor, MacroParameterAccessExpression):
+                arg_accessor = scope.lookup_macro_parameter(arg_accessor.name(scope))
+
             return isinstance(arg_accessor, tuple(self.VALID_ACCESSOR_TYPES))
 
         def emit_for_arg_store(
             self,
             arg: AbstractAccessExpression,
             function: MutableFunction,
             scope: ParsingScope,
@@ -143,14 +154,15 @@
         IDENTIFIER = "VARIABLE_ARG"
 
         def __init__(self, sub_type: typing.Optional["MacroAssembly.AbstractDataType"]):
             self.sub_type = sub_type
 
         def is_match(
             self,
+            scope: ParsingScope,
             arg: "MacroAssembly.MacroArg",
             arg_accessor: AbstractAccessExpression | CompoundExpression,
         ) -> bool:
             return self.sub_type is None or self.sub_type.is_match(arg, arg_accessor)
 
         def emit_for_arg(
             self,
@@ -174,34 +186,42 @@
             self.is_static = is_static
             self.index = -1
             self.data_type_annotation: MacroAssembly.AbstractDataType = None
 
         def copy(self):
             return type(self)(self.name, self.is_static)
 
+        def __repr__(self):
+            return f"MACRO_ARG('{self.name.text}', is_static={self.is_static}, type={self.data_type_annotation})"
+
         def is_match(
-            self, arg_accessor: AbstractAccessExpression | CompoundExpression
+            self, scope: ParsingScope, arg_accessor: AbstractAccessExpression | CompoundExpression
         ) -> bool:
             if self.data_type_annotation is None:
                 return True
 
             if isinstance(self.data_type_annotation, MacroAssembly.AbstractDataType):
-                return self.data_type_annotation.is_match(self, arg_accessor)
+                return self.data_type_annotation.is_match(scope, self, arg_accessor)
 
             return False
 
     class MacroOverloadPage:
         def __init__(
             self,
             name: typing.List[str],
             name_token: typing.List[IdentifierToken] = None,
         ):
             self.name = name
             self.name_token = name_token
             self.assemblies: typing.List[MacroAssembly] = []
+            self.trace_info: TraceInfo = None
+
+        def set_trace_info(self, trace_info: TraceInfo):
+            self.trace_info = trace_info
+            return self
 
         def add_assembly(self, assembly: "MacroAssembly"):
             self.assemblies.append(assembly)
             return self
 
         def __repr__(self) -> str:
             return f"MACRO_OVERLOAD({'::'.join(self.name)}, [{', '.join(map(repr, self.assemblies))}])"
@@ -218,15 +238,15 @@
                         e.data_type_annotation, MacroAssembly.VariableArgCountDataType
                     )
                     for e in macro.args
                 )
 
                 if (
                     len(macro.args) == len(args)
-                    and all(arg.is_match(param) for arg, param in zip(macro.args, args))
+                    and all(arg.is_match(scope, param) for arg, param in zip(macro.args, args))
                     and not has_star_args
                 ):
                     return macro, args
 
                 if has_star_args:
                     error = False
                     prefix = []
@@ -273,84 +293,101 @@
                     if error:
                         continue
 
                     # And now collect the args in between
                     for arg in (
                         args[star_index : i + 1] if i != -1 else args[star_index:]
                     ):
-                        if not macro.args[star_index].is_match(arg):
+                        if not macro.args[star_index].is_match(scope, arg):
                             error = True
                             break
 
                         inner.append(arg)
 
                     if error:
                         continue
 
                     args[:] = prefix + [inner] + postfix
                     return macro, args
 
-            raise throw_positioned_error(
-                scope,
-                self.name_token,
-                f"Could not find overloaded variant of {':'.join(self.name)} with args {args}!",
-                NameError,
-            )
+            print(args)
+
+            for decl in self.assemblies:
+                print(decl.args)
+
+            raise PropagatingCompilerException(
+                f"Could not find overloaded variant of '{':'.join(self.name)}' with args {args}!"
+            ).add_trace_level(self.trace_info.with_token(self.name_token)).set_underlying_exception(NameError)
 
         def add_definition(self, macro: "MacroAssembly", override=False):
             # todo: do a safety check!
             self.assemblies.append(macro)
 
     @classmethod
     def _try_parse_arg_data_type(cls, parser: "Parser", scope: ParsingScope) -> AbstractDataType | None:
         if identifier := parser.try_inspect(IdentifierToken):
             if identifier.text == "CODE_BLOCK":
                 parser.consume(identifier)
 
-                count = 0
                 if opening_bracket := parser.try_consume(SpecialToken("[")):
                     if not (expr := parser.try_consume(IntegerToken)) or not expr.text.isdigit() or (count := int(expr.text)) < 0:
-                        raise throw_positioned_error(
-                            scope,
-                            [opening_bracket, parser[0]],
-                            "expected <integer> after '[' to declare count",
-                        )
+                        raise PropagatingCompilerException(
+                            "expected <positive integer> after '[' to declare count"
+                        ).add_trace_level(scope.get_trace_info().with_token(opening_bracket, parser[0]))
 
                     if not parser.try_consume(SpecialToken("]")):
-                        raise throw_positioned_error(
-                            scope,
-                            [opening_bracket, parser[0]],
-                            "expected ']' closing '[' in CODE_BLOCK",
-                        )
+                        raise PropagatingCompilerException(
+                            "expected ']' closing '[' after <count> in CODE_BLOCK"
+                        ).add_trace_level(scope.get_trace_info().with_token(opening_bracket, parser[0]))
+
+                    inst = cls.CodeBlockDataType(int(expr.text))
+                    return inst
 
-                inst = cls.CodeBlockDataType(count=count)
+                inst = cls.CodeBlockDataType()
                 return inst
 
             elif identifier.text == "VARIABLE_ARG":
                 parser.consume(identifier)
                 # todo: add check that it is the only * arg
                 if parser.try_consume(SpecialToken("[")):
                     inner_type = cls._try_parse_arg_data_type(parser, scope)
                     if inner_type is None:
-                        return
+                        raise PropagatingCompilerException(
+                            "expected <inner type>"
+                        ).add_trace_level(scope.get_trace_info().with_token(identifier, parser[0]))
+
+                    if not parser.try_consume(SpecialToken("]")):
+                        raise PropagatingCompilerException(
+                            "expected ']' closing '[' after <inner type>"
+                        ).add_trace_level(scope.get_trace_info().with_token(identifier, parser[0]))
 
                     inst = cls.VariableArgCountDataType(inner_type)
-                    parser.consume(SpecialToken("]"))
                 else:
                     inst = cls.VariableArgCountDataType(None)
 
                 return inst
 
             elif identifier.text == "VARIABLE":
                 parser.consume(identifier)
-                inst = cls.VariableDataType()
-                return inst
+
+                if parser[0] == SpecialToken("["):
+                    raise PropagatingCompilerException(
+                        "did not expect '[' after 'VARIABLE' in macro type declaration"
+                    ).add_trace_level(scope.get_trace_info().with_token(identifier, parser[0]))
+
+                return cls.VariableDataType()
 
             elif identifier.text == "ANY":
                 parser.consume(identifier)
+
+                if parser[0] == SpecialToken("["):
+                    raise PropagatingCompilerException(
+                        "did not expect '[' after 'ANY' in macro type declaration"
+                    ).add_trace_level(scope.get_trace_info().with_token(identifier, parser[0]))
+
                 return cls.AnyDataType()
 
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "MacroAssembly":
         allow_assembly_instr = bool(parser.try_consume(IdentifierToken("ASSEMBLY")))
 
         name = [parser.consume(IdentifierToken)]
@@ -377,53 +414,64 @@
                 if data_type is not None:
                     arg.data_type_annotation = data_type
                     parser.discard_save()
                 else:
                     parser.rollback()
 
                 if not parser.try_consume(SpecialToken(",")):
-                    parser.consume(SpecialToken(")"), err_arg=scope)
+                    if not parser.try_consume(SpecialToken(")")):
+                        raise PropagatingCompilerException(
+                            "Expected ',' for continue or ')' closing MACRO declaration"
+                        ).add_trace_level(scope.get_trace_info().with_token(parser[0], name))
+
                     break
 
         if parser.try_consume(SpecialToken("-")):
             parser.consume(SpecialToken(">"), err_arg=scope)
 
             return_type = cls._try_parse_arg_data_type(parser, scope)
         else:
             return_type = None
 
-        body = parser.parse_body(scope=scope)
+        try:
+            body = parser.parse_body(scope=scope)
+        except PropagatingCompilerException as e:
+            e.add_trace_level(scope.get_trace_info().with_token(name))
+            raise e
 
         return cls(
             name,
             args,
             body,
             allow_assembly_instr,
             scope_path=scope.scope_path.copy(),
             module_path=scope.module_file,
             return_type=return_type,
+            trace_info=scope.get_trace_info().with_token(name),
         )
 
     def __init__(
         self,
         name: typing.List[IdentifierToken],
         args: typing.List[MacroArg],
         body: CompoundExpression,
         allow_assembly_instr=False,
         scope_path: typing.List[str] = None,
         module_path: str = None,
         return_type=None,
+        trace_info: TraceInfo = None,
     ):
         self.name = name
         self.args = args
         self.body = body
         self.allow_assembly_instr = allow_assembly_instr
         self.scope_path = scope_path or []
         self.module_path = module_path
         self.return_type = return_type
+        self.trace_info: TraceInfo = trace_info
 
     def __repr__(self):
         return f"MACRO:{'ASSEMBLY' if self.allow_assembly_instr else ''}:'{':'.join(map(lambda e: e.text, self.name))}'({', '.join(map(repr, self.args))}) {{{repr(self.body)}}}"
 
     def __eq__(self, other):
         return (
             type(self) is type(other)
@@ -457,146 +505,166 @@
         if len(args) != len(self.args):
             raise RuntimeError("Argument count must be equal!")
 
         scope = scope.copy()
         scope.scope_path = self.scope_path
         scope.module_file = self.module_path
         scope.current_macro_assembly = self
+        scope.push_macro_param_stack()
 
         bytecode = []
 
         for arg_decl, arg_code in zip(self.args, args):
             if isinstance(arg_decl.data_type_annotation, MacroAssembly.CodeBlockDataType):
                 if isinstance(arg_code, CompoundExpression) and hasattr(arg_code, "to_be_stored_at"):
                     if len(arg_code.to_be_stored_at) != arg_decl.data_type_annotation.count:
-                        raise throw_positioned_error(
-                            scope,
-                            arg_decl.name,
+                        raise PropagatingCompilerException(
                             f"Expected {arg_decl.data_type_annotation.count} dynamic name entries, got {len(arg_code.to_be_stored_at)}"
-                        )
+                        ).add_trace_level(self.trace_info.with_token(arg_decl.name))
 
             if arg_decl.is_static:
-                scope.macro_parameter_namespace[arg_decl.name.text] = arg_decl.name.text
+                scope.set_macro_arg_value(arg_decl.name.text, arg_decl.name.text)
             else:
-                scope.macro_parameter_namespace[arg_decl.name.text] = arg_code
+                scope.set_macro_arg_value(arg_decl.name.text, arg_code)
 
-        inner_bytecode = self.body.emit_bytecodes(function, scope)
+        try:
+            inner_bytecode = self.body.emit_bytecodes(function, scope)
+        except PropagatingCompilerException as e:
+            e.add_trace_level(self.trace_info)
+            raise e
 
         arg_names: typing.List[str | None] = []
         arg_decl_lookup: typing.Dict[str, MacroAssembly.MacroArg] = {}
         for i, (arg_decl, arg_code) in enumerate(zip(self.args, args)):
             arg_decl_lookup[arg_decl.name.text] = arg_decl
             if arg_decl.is_static:
                 if arg_decl.data_type_annotation is not None:
                     arg_names.append(var_name := scope.scope_name_generator(f"arg_{i}"))
-                    bytecode += arg_decl.data_type_annotation.emit_for_arg(
-                        arg_code, function, scope
-                    )
+                    try:
+                        bytecode += arg_decl.data_type_annotation.emit_for_arg(
+                            arg_code, function, scope
+                        )
+                    except PropagatingCompilerException as e:
+                        e.add_trace_level(self.trace_info.with_token(arg_decl.name), f"during emitting arg lookup for static argument with type annotationwith index {arg_decl.index} and name '{arg_decl.name.text}'")
+                        raise e
+
                     bytecode.append(
                         Instruction(
                             Opcodes.STORE_FAST,
                             var_name,
                         )
                     )
 
                 else:
                     arg_names.append(var_name := scope.scope_name_generator(f"arg_{i}"))
-                    bytecode += arg_code.emit_bytecodes(function, scope)
+                    try:
+                        bytecode += arg_code.emit_bytecodes(function, scope)
+                    except PropagatingCompilerException as e:
+                        e.add_trace_level(self.trace_info.with_token(arg_decl.name), f"during emitting arg lookup for static argument with index {arg_decl.index} and name '{arg_decl.name.text}'")
+                        raise e
+
                     bytecode.append(
                         Instruction(
                             Opcodes.STORE_FAST,
                             var_name,
                         )
                     )
 
             else:
                 arg_names.append(None)
 
-        local_prefix = scope.scope_name_generator("macro_local")
-        end_target = scope.scope_name_generator("macro_end")
+        local_prefix = scope.scope_name_generator("macro_local~"+":".join(map(lambda e: e.text, self.name)))
+        end_target = scope.scope_name_generator("macro_end~"+":".join(map(lambda e: e.text, self.name)))
         requires_none_load = (
             self.return_type is not None
             and not inner_bytecode[-1].has_unconditional_jump()
             and inner_bytecode[-1].opcode != Opcodes.RETURN_VALUE
         )
 
         for instr in inner_bytecode:
             bytecode.append(instr)
 
             if instr.opcode in (
                 Opcodes.MACRO_LOAD_PARAMETER,
                 Opcodes.MACRO_PARAMETER_EXPANSION,
             ):
                 if instr.arg_value not in arg_decl_lookup:
-                    raise throw_positioned_error(
-                        scope,
-                        self.name,
-                        f"macro name {instr.arg_value} not found in scope",
-                    )
+                    raise PropagatingCompilerException(
+                        f"macro name {instr.arg_value} not found in scope"
+                    ).add_trace_level(self.trace_info.with_token(self.name))
 
                 arg_decl: MacroAssembly.MacroArg = arg_decl_lookup[instr.arg_value]
 
                 if arg_decl.data_type_annotation is not None:
                     if arg_decl.is_static:
                         instr.change_opcode(
                             Opcodes.LOAD_FAST, arg_names[arg_decl.index]
                         )
 
                     else:
                         instr.change_opcode(Opcodes.NOP)
-                        instructions = arg_decl.data_type_annotation.emit_for_arg(
-                            args[arg_decl.index], function, scope
-                        )
+                        try:
+                            instructions = arg_decl.data_type_annotation.emit_for_arg(
+                                args[arg_decl.index], function, scope
+                            )
+                        except PropagatingCompilerException as e:
+                            e.add_trace_level(self.trace_info.with_token(arg_decl.name), f"during emitting arg lookup for dynamic argument with type annotation with index {arg_decl.index} and name '{arg_decl.name.text}'")
+                            raise e
+
                         instr.insert_after(instructions)
                         bytecode += instructions
 
                 else:
                     if arg_decl.is_static:
                         instr.change_opcode(
                             Opcodes.LOAD_FAST, arg_names[arg_decl.index]
                         )
 
                     else:
                         instr.change_opcode(Opcodes.NOP)
-                        instructions = args[arg_decl.index].emit_bytecodes(
-                            function, scope
-                        )
+                        try:
+                            instructions = args[arg_decl.index].emit_bytecodes(
+                                function, scope
+                            )
+                        except PropagatingCompilerException as e:
+                            e.add_trace_level(self.trace_info.with_token(arg_decl.name), f"during emitting arg lookup for dynamic argument with index {arg_decl.index} and name '{arg_decl.name.text}'")
+                            raise e
+
                         instr.insert_after(instructions)
                         bytecode += instructions
 
             elif instr.opcode == Opcodes.MACRO_STORE_PARAMETER:
                 if instr.arg_value not in arg_decl_lookup:
-                    raise throw_positioned_error(
-                        scope,
-                        self.name,
-                        f"macro name {instr.arg_value} not found in scope",
-                    )
+                    raise PropagatingCompilerException(
+                        f"macro name {instr.arg_value} not found in scope"
+                    ).add_trace_level(self.trace_info.with_token(self.name))
 
                 arg_decl = arg_decl_lookup[instr.arg_value]
 
                 if arg_decl.is_static:
                     instr.change_opcode(Opcodes.STORE_FAST, arg_names[arg_decl.index])
                 else:
                     if arg_decl.data_type_annotation is not None:
-                        instructions = arg_decl.data_type_annotation.emit_for_arg_store(
-                            args[arg_decl.index], function, scope
-                        )
+                        try:
+                            instructions = arg_decl.data_type_annotation.emit_for_arg_store(
+                                args[arg_decl.index], function, scope
+                            )
+                        except PropagatingCompilerException as e:
+                            e.add_trace_level(self.trace_info.with_token(arg_decl.name), f"during emitting store arg lookup for dynamic argument with index {arg_decl.index} and name '{arg_decl.name.text}'")
+                            raise e
 
                         if instructions is not None:
                             instr.change_opcode(Opcodes.NOP)
                             instr.insert_after(instructions)
                             bytecode += instructions
                             continue
 
-                    raise throw_positioned_error(
-                        scope,
-                        self.name,
-                        f"Tried to override non-static MACRO parameter '{instr.arg_value}'; This is not allowed as the parameter will be evaluated on each access!",
-                        RuntimeError,
-                    )
+                    raise PropagatingCompilerException(
+                        f"Tried to override non-static MACRO parameter '{instr.arg_value}'; This is not allowed as the parameter will be evaluated on each access!"
+                    ).add_trace_level(self.trace_info.with_token(self.name)).set_underlying_exception(RuntimeError)
 
             elif instr.has_local() and instr.arg_value.startswith(":"):
                 instr.change_arg_value(
                     instr.arg_value.removeprefix(":")
                 )
 
             elif instr.has_local():
@@ -606,48 +674,31 @@
                 if self.return_type is None:
                     raise SyntaxError(
                         "'MACRO_RETURN' only allowed in assembly if return type declared!"
                     )
 
                 instr.change_opcode(Opcodes.JUMP_ABSOLUTE, JumpToLabel(end_target))
 
+        scope.pop_macro_param_stack()
+
         if requires_none_load:
             bytecode.append(Instruction(Opcodes.LOAD_CONST, None))
 
         bytecode.append(Instruction(Opcodes.BYTECODE_LABEL, end_target))
 
-        # handle = Instruction(Opcodes.NOP)
-        # handle.insert_after(
-        #     [
-        #         Instruction(Opcodes.POP_TOP),
-        #         Instruction(Opcodes.ROT_TWO),  # TOS would be the exception
-        #         Instruction(Opcodes.POP_TOP),
-        #         Instruction(Opcodes.LOAD_CONST, _manipulate_stack_trace),
-        #         Instruction(Opcodes.ROT_TWO),
-        #         Instruction(Opcodes.LOAD_CONST, scope.module_file),
-        #         Instruction(Opcodes.LOAD_CONST, "".join(map(lambda e: e.text, self.name))),
-        #         Instruction(Opcodes.LOAD_CONST, 0),  # todo: load position info (line)
-        #         Instruction(Opcodes.LOAD_CONST, 0),  # todo: load position info (column)
-        #         Instruction(Opcodes.LOAD_CONST, 0),  # todo: load position info (span)
-        #         Instruction(Opcodes.CALL_FUNCTION, arg=6),
-        #         Instruction(Opcodes.RAISE_VARARGS, arg=0),
-        #     ]
-        # )
-        # function.exception_table.add_handle(handle, inner_bytecode)
-
         return bytecode
 
     def fill_scope(self, scope: ParsingScope):
         name = scope.scope_path + list(map(lambda e: e.text, self.name))
         namespace = name[:-1]
         inner_name = name[-1]
         namespace_level = scope.lookup_namespace(namespace)
 
         if inner_name not in namespace_level:
-            page = self.MacroOverloadPage(name, self.name)
+            page = self.MacroOverloadPage(name, self.name).set_trace_info(scope.get_trace_info())
             namespace_level[inner_name] = page
         elif not isinstance(namespace_level[inner_name], self.MacroOverloadPage):
             raise RuntimeError(
                 f"Expected <empty> or MacroOverloadPage, got {namespace_level[inner_name]}"
             )
         else:
             page = namespace_level[inner_name]
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import traceback
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException, TraceInfo
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
@@ -45,25 +47,28 @@
         else:
             target = None
 
         return cls(
             name,
             target,
             is_relative_target,
+            trace_info=scope.get_trace_info().with_token(name),
         )
 
     def __init__(
         self,
         name: typing.List[IdentifierToken],
         target: typing.List[IdentifierToken] = None,
         is_relative_target: bool = False,
+        trace_info: TraceInfo = None
     ):
         self.name = name
         self.target = target
         self.is_relative_target = is_relative_target
+        self.trace_info = trace_info
 
     def __repr__(self):
         return f"MACRO_IMPORT('{'.'.join(map(lambda e: e.text, self.name))}'{'' if self.target is None else ('.' if self.is_relative_target else '') + '.'.join(map(lambda e: e.text, self.target))})"
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
@@ -78,28 +83,41 @@
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return []
 
     def fill_scope(self, scope: ParsingScope):
         from bytecodemanipulation.assembler.Emitter import GLOBAL_SCOPE_CACHE
+        import bytecodemanipulation.assembler.hook
 
         if self.target is None:
             namespace = scope.scope_path
         elif self.is_relative_target:
             namespace = scope.scope_path + [e.text for e in self.target]
         else:
             namespace = [e.text for e in self.target]
 
         scope_entry = scope.lookup_namespace(namespace)
 
         module = ".".join(map(lambda e: e.text, self.name))
 
         if module not in GLOBAL_SCOPE_CACHE:
-            __import__(module)
+            prev = bytecodemanipulation.assembler.hook.LET_PROPAGATE_EXCEPTIONS_THROUGH
+            bytecodemanipulation.assembler.hook.LET_PROPAGATE_EXCEPTIONS_THROUGH = True
+
+            try:
+                __import__(module)
+            except PropagatingCompilerException as e:
+                e.add_trace_level(self.trace_info)
+                raise e
+            except Exception as e:
+                traceback.print_exc()
+                raise PropagatingCompilerException("MACRO_IMPORT failed due to the normal import failing", *e.args).set_underlying_exception(type(e)).add_trace_level(self.trace_info) from None
+
+            bytecodemanipulation.assembler.hook.LET_PROPAGATE_EXCEPTIONS_THROUGH = prev
 
         if not scope_entry:
             scope_entry.update(GLOBAL_SCOPE_CACHE[module])
 
         else:
             tasks = [(scope_entry, GLOBAL_SCOPE_CACHE[module])]
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,170 +1,187 @@
+import functools
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.Lexer import SpecialToken
+from bytecodemanipulation.data.shared.instructions.CallAssembly import (
+    AbstractCallAssembly,
+)
+from bytecodemanipulation.data.shared.expressions.MacroAccessExpression import (
+    MacroAccessExpression,
+)
+from bytecodemanipulation.data.shared.instructions.MacroAssembly import MacroAssembly
 from bytecodemanipulation.assembler.Parser import Parser
+from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
-from bytecodemanipulation.data.shared.expressions.CompoundExpression import CompoundExpression
-from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
-    AbstractAssemblyInstruction,
-)
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class MacroPasteAssembly(AbstractAssemblyInstruction):
-    # MACRO_PASTE <macro param name> ['[' <access> {',' <access>} ']'] ['->' <target>]
-    NAME = "MACRO_PASTE"
-
-    @classmethod
-    def register(cls):
-        Parser.register(cls)
-
-    @classmethod
-    def consume(cls, parser: "Parser", scope) -> "MacroPasteAssembly":
-        # Parse an optional § infront of the name
-        parser.try_consume(SpecialToken("&"))
-
-        name = parser.consume(IdentifierToken)
-
-        dynamic_names: typing.List[typing.Tuple[AbstractAccessExpression, bool]] = []
-        if opening_bracket := parser.try_consume(SpecialToken("[")):
-            while parser.try_inspect() != SpecialToken("]"):
-                is_static = bool(parser.try_consume(SpecialToken("!")))
-                base = parser.try_consume_access_to_value(scope=scope)
-
-                if base is None:
-                    raise throw_positioned_error(
-                        scope,
-                        [opening_bracket, parser[0]],
-                        "Expected <expression> after ',' for dynamic name access",
-                    )
-
-                dynamic_names.append((base, is_static))
+@Parser.register
+class CallAssembly(AbstractCallAssembly):
+    def emit_bytecodes(
+        self, function: MutableFunction, scope: ParsingScope
+    ) -> typing.List[Instruction]:
+        if self.is_macro:
+            return self.emit_macro_bytecode(function, scope)
 
-                if not parser.try_consume(SpecialToken(",")):
-                    break
+        has_seen_star = False
+        has_seen_star_star = False
+        has_seen_kw_arg = False
+
+        for arg in self.args:
+            if isinstance(arg, CallAssembly.KwArg):
+                has_seen_kw_arg = True
+
+            elif isinstance(arg, CallAssembly.KwArgStar):
+                has_seen_star_star = True
+
+            elif isinstance(arg, CallAssembly.StarArg):
+                has_seen_star = True
+
+        if not has_seen_kw_arg and not has_seen_star and not has_seen_star_star:
+            if self.is_partial:
+                bytecode = [
+                    Instruction(Opcodes.LOAD_CONST, functools.partial)
+                ]
+                extra_args = 1
+            else:
+                bytecode = []
+                extra_args = 0
+
+            bytecode += self.call_target.emit_bytecodes(function, scope)
+
+            for arg in self.args:
+                bytecode += arg.source.emit_bytecodes(function, scope)
+
+            bytecode += [
+                Instruction(
+                    Opcodes.CALL_FUNCTION, arg=len(self.args) + extra_args
+                ),
+            ]
+
+        elif has_seen_kw_arg and not has_seen_star and not has_seen_star_star:
+            if self.is_partial:
+                bytecode = [
+                    Instruction(Opcodes.LOAD_CONST, functools.partial)
+                ]
+                extra_args = 1
+            else:
+                bytecode = []
+                extra_args = 0
+
+            bytecode += self.call_target.emit_bytecodes(function, scope)
+
+            kw_arg_keys = []
+
+            for arg in reversed(self.args):
+                bytecode += arg.source.emit_bytecodes(function, scope)
+
+                if isinstance(arg, CallAssembly.KwArg):
+                    kw_arg_keys.append(arg.key.text)
+
+                kw_const = tuple(reversed(kw_arg_keys))
+
+                bytecode += [
+                    Instruction("LOAD_CONST", kw_const),
+                    Instruction(
+                        function,
+                        -1,
+                        "CALL_FUNCTION_KW",
+                        arg=len(self.args) + extra_args,
+                    ),
+                ]
 
-            if not parser.try_consume(SpecialToken("]")):
-                raise throw_positioned_error(
-                    scope,
-                    [opening_bracket, parser[0]],
-                    "expected ']' to close '[' closing dynamic names",
-                )
-
-        if parser.try_consume_multi([SpecialToken("-"), SpecialToken(">")]):
-            target = parser.try_consume_access_to_value(
-                allow_primitives=False, scope=scope
-            )
         else:
-            target = None
+            bytecode = self.call_target.emit_bytecodes(function, scope)
 
-        return cls(name, target, dynamic_names=dynamic_names)
+            bytecode += [Instruction("BUILD_LIST", arg=0)]
 
-    def __init__(self, name: IdentifierToken, target: AbstractAccessExpression = None, dynamic_names: typing.List[typing.Tuple[AbstractAccessExpression, bool]] = None):
-        self.name = name
-        self.target = target
-        self.dynamic_names = dynamic_names or []
-
-    def __repr__(self):
-        return f"MACRO_PASTE({self.name.text}{repr(self.dynamic_names)[1:-1]}{'' if self.target is None else '-> '+repr(self.target)})"
-
-    def __eq__(self, other):
-        return (
-            type(self) == type(other)
-            and self.name == other.name
-            and self.target == other.target
-            and self.dynamic_names == other.dynamic_names
-        )
+            if self.is_partial:
+                bytecode += [
+                    Instruction(Opcodes.LOAD_CONST, functools.partial),
+                    Instruction("LIST_APPEND"),
+                ]
+
+            i = -1
+            for i, arg in enumerate(self.args):
+                bytecode += arg.source.emit_bytecodes(function, scope)
+
+                if isinstance(arg, CallAssembly.Arg):
+                    bytecode += [Instruction("LIST_APPEND", arg=1)]
+                elif isinstance(arg, CallAssembly.StarArg):
+                    bytecode += [Instruction("LIST_EXTEND", arg=1)]
+                else:
+                    break
 
-    def copy(self) -> "MacroPasteAssembly":
-        return type(self)(self.name, self.target.copy() if self.target else None, [(e[0].copy(), e[1]) for e in self.dynamic_names])
+            bytecode += [
+                Instruction("LIST_TO_TUPLE"),
+            ]
+
+            if has_seen_kw_arg or has_seen_star_star:
+                bytecode += [Instruction("BUILD_MAP", arg=0)]
+
+                for arg in self.args[i + 1 :]:
+                    if isinstance(arg, CallAssembly.KwArg):
+                        bytecode += (
+                            [Instruction("LOAD_CONST", arg.key.text)]
+                            + arg.source.emit_bytecodes(function, scope)
+                            + [
+                                Instruction("BUILD_MAP", arg=1),
+                                Instruction("DICT_MERGE", arg=1),
+                            ]
+                        )
+                    else:
+                        bytecode += arg.source.emit_bytecodes(function, scope) + [
+                            Instruction("DICT_MERGE", arg=1)
+                        ]
+
+            bytecode += [
+                Instruction(
+                    function,
+                    -1,
+                    "CALL_FUNCTION_EX",
+                    arg=int(has_seen_kw_arg or has_seen_star_star),
+                ),
+            ]
+
+        if self.target:
+            bytecode += self.target.emit_store_bytecodes(function, scope)
+
+        return bytecode
+
+    def emit_macro_bytecode(self, function: MutableFunction, scope: ParsingScope):
+        access = typing.cast(MacroAccessExpression, self.call_target)
+        name = access.name
+
+        macro_declaration = scope.lookup_name_in_scope(name[0].text)
+
+        if macro_declaration is None:
+            raise throw_positioned_error(
+                scope,
+                typing.cast(MacroAccessExpression, self.call_target).name,
+                f"Macro '{':'.join(map(lambda e: e.text, name))}' not found!",
+                NameError,
+            )
 
-    def emit_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        if self.name.text in scope.macro_parameter_namespace and hasattr(
-            scope.macro_parameter_namespace[self.name.text], "emit_bytecodes"
-        ):
-            body: CompoundExpression = scope.macro_parameter_namespace[self.name.text]
-            instructions = body.emit_bytecodes(
-                function, scope
+        if len(name) > 1:
+            for e in name[1:]:
+                macro_declaration = macro_declaration[e.text]
+
+        if not isinstance(macro_declaration, MacroAssembly.MacroOverloadPage):
+            raise RuntimeError(
+                f"Expected Macro Declaration for '{':'.join(map(lambda e: e.text, name))}', got {macro_declaration}"
             )
 
-            sources = [e(scope) for e in getattr(body, "to_be_stored_at", [])]
+        macro, args = macro_declaration.lookup([arg.source for arg in self.args], scope)
 
-            if len(sources) != len(self.dynamic_names):
-                raise throw_positioned_error(
-                    scope,
-                    self.name,
-                    f"Expected exactly {len(sources)} paramters at MACRO_PASTE, but got {len(self.dynamic_names)}",
-                )
-
-            result = []
-            special_names = []
-
-            for i, (code, is_static) in enumerate(self.dynamic_names):
-                if is_static:
-                    label_name = scope.scope_name_generator(f"dynamic_name_{i}")
-
-                    result += code.emit_bytecodes(function, scope)
-                    result += [
-                        Instruction(Opcodes.STORE_FAST, label_name)
-                    ]
-                    special_names.append(label_name)
-                else:
-                    special_names.append(None)
+        if self.target is not None and macro.return_type is None:
+            raise RuntimeError(
+                f"Expected <return type> declaration at macro if using '->' in call"
+            )
 
-            for instr in instructions:
-                if instr.has_local():
-                    local: str = typing.cast(str, instr.arg_value)
-
-                    if local in sources:
-                        index = sources.index(local)
-                        code, is_static = self.dynamic_names[index]
-
-                        if instr.opcode == Opcodes.LOAD_FAST:
-                            if is_static:
-                                result += [
-                                    Instruction(Opcodes.LOAD_FAST, special_names[index]),
-                                ]
-                            else:
-                                result += code.emit_bytecodes(function, scope)
-
-                        elif instr.opcode == Opcodes.STORE_FAST:
-                            if is_static:
-                                raise throw_positioned_error(
-                                    scope,
-                                    self.name,  # todo: use outer call entry
-                                    f"arg {index+1} is marked as static, but it was tried to write to",
-                                )
-
-                            result += code.emit_store_bytecodes(function, scope)
-                        else:
-                            result.append(instr)
-
-                    elif local.startswith("|"):
-                        instr.change_arg_value(local[1:])
-                        result.append(instr)
-                    else:
-                        instr.change_arg_value(":" + local)
-                        result.append(instr)
-                else:
-                    result.append(instr)
+        bytecode = macro.emit_call_bytecode(function, scope, args)
 
-            return result + (
-                []
-                if self.target is None
-                else self.target.emit_store_bytecodes(function, scope)
-            )
+        if self.target:
+            bytecode += self.target.emit_bytecodes(function, scope)
 
-        return [
-            Instruction(Opcodes.MACRO_PARAMETER_EXPANSION, self.name.text)
-        ] + (
-            []
-            if self.target is None
-            else self.target.emit_store_bytecodes(function, scope)
-        )
+        return bytecode
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class MacroReturnAssembly(AbstractAssemblyInstruction):
     NAME = "MACRO_RETURN"
 
     @classmethod
     def consume(cls, parser: "Parser", scope) -> "MacroReturnAssembly":
         return cls(
             parser.try_parse_data_source(
-                allow_primitives=True, allow_op=True, include_bracket=False
+                allow_primitives=True, allow_op=True, include_bracket=False, scope=scope
             )
         )
 
     def __init__(self, expr: AbstractSourceExpression | None = None):
         self.expr = expr
 
     def visit_parts(
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,68 @@
+import abc
 import typing
 
+from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import SpecialToken
+from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
+from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
-    CompoundExpression,
-)
-from bytecodemanipulation.opcodes.Instruction import Instruction
-from bytecodemanipulation.MutableFunction import MutableFunction
-
-
-if typing.TYPE_CHECKING:
-    from bytecodemanipulation.assembler.Parser import Parser
 
 
-class NamespaceAssembly(AbstractAssemblyInstruction):
-    # 'NAMESPACE' [{<namespace> ':'}] <name> '{' <code> '}'
-    NAME = "NAMESPACE"
-
-    @classmethod
-    def register(cls):
-        from bytecodemanipulation.assembler.Parser import Parser
+class AbstractStoreFastAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # STORE_FAST <name> [<source>]
+    NAME = "STORE_FAST"
 
-        Parser.register(cls)
+    def __init__(
+        self,
+        name_token: IdentifierToken | IntegerToken | str | int,
+        source: AbstractSourceExpression | None = None,
+    ):
+        self.name_token = (
+            name_token
+            if not isinstance(name_token, (str, int))
+            else (
+                IdentifierToken(name_token)
+                if isinstance(name_token, str)
+                else IntegerToken(str(name_token))
+            )
+        )
+        self.source = source
 
     @classmethod
-    def consume(cls, parser: "Parser", scope: ParsingScope) -> "NamespaceAssembly":
-        name = [parser.consume(IdentifierToken)]
-
-        while parser.try_consume(SpecialToken(":")):
-            name.append(parser.consume(IdentifierToken))
+    def consume(cls, parser: "Parser", scope) -> "AbstractStoreFastAssembly":
+        parser.try_consume(SpecialToken("$"))
+        name = parser.consume([IdentifierToken, IntegerToken])
 
-        assembly = parser.parse_body(namespace_part=[e.text for e in name], scope=scope)
+        source = parser.try_parse_data_source(scope=scope)
 
-        return cls(
-            name,
-            assembly,
-        )
-
-    def __init__(
-        self, name: typing.List[IdentifierToken], assembly: CompoundExpression
-    ):
-        self.name = name
-        self.assembly = assembly
-
-    def __repr__(self):
-        return (
-            f"NAMESPACE::'{':'.join(e.text for e in self.name)}'({repr(self.assembly)})"
-        )
+        return cls(name, source)
 
     def __eq__(self, other):
         return (
-            type(self) is type(other)
-            and self.name == other.name
-            and self.assembly == other.assembly
+            type(self) == type(other)
+            and self.name_token == other.name_token
+            and self.source == other.source
         )
 
-    def copy(self):
-        return type(self)(self.name, self.assembly.copy())
+    def __repr__(self):
+        return f"STORE_FAST({self.name_token}, source={self.source or 'TOS'})"
 
-    def emit_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        return self.assembly.emit_bytecodes(
-            function, scope.copy(sub_scope_name=[e.text for e in self.name])
-        )
+    def copy(self) -> "AbstractStoreFastAssembly":
+        return type(self)(self.name, self.source.copy() if self.source else None)
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self,
-            (
-                self.assembly.visit_parts(
-                    visitor,
-                    parents + [self],
-                ),
-            ),
-            parents,
+            self, (self.source.visit_parts(visitor) if self.target else None,)
         )
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     NAME = "RAISE"
 
     def __init__(self, source):
         self.source = source
 
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractRaiseAssembly":
-        return cls(parser.try_parse_data_source(include_bracket=False))
+        return cls(parser.try_parse_data_source(include_bracket=False, scope=scope))
 
     def __eq__(self, other):
         return type(self) == type(other) and self.source == other.source
 
     def __repr__(self):
         return f"RAISE({'TOS' if self.source is None else self.source})"
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/RawAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/RawAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,70 @@
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
-from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
-    AbstractAssemblyInstruction,
-)
-from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
-from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
-from bytecodemanipulation.assembler.util.parser import AbstractExpression
+from bytecodemanipulation.data.shared.instructions.ClassDefinitionAssembly import (
+    AbstractClassDefinitionAssembly,
+)
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
-class StoreAssembly(AbstractAssemblyInstruction):
-    # STORE <access> [(expression)]
-    NAME = "STORE"
-
-    @classmethod
-    def consume(cls, parser: "Parser", scope: ParsingScope) -> "StoreAssembly":
-        access = parser.try_consume_access_to_value(
-            allow_tos=False, scope=scope, allow_calls=False
-        )
-
-        if access is None:
-            raise throw_positioned_error(
-                scope, parser.try_inspect(), "expected <expression>"
-            )
-
-        source = parser.try_parse_data_source()
-
-        return cls(access, source)
-
-    def __init__(
-        self,
-        access_token: AbstractAccessExpression,
-        source: AbstractSourceExpression | None = None,
-    ):
-        self.access_token = access_token
-        self.source = source
-
-    def __eq__(self, other):
-        return (
-            type(self) == type(other)
-            and self.access_token == other.access_token
-            and self.source == other.source
-        )
-
-    def __repr__(self):
-        return f"STORE({self.access_token}, {self.source})"
-
-    def copy(self) -> "StoreAssembly":
-        return StoreAssembly(
-            self.access_token, self.source.copy() if self.source else None
-        )
-
+class ClassDefinitionAssembly(AbstractClassDefinitionAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        return (
-            [] if self.source is None else self.source.emit_bytecodes(function, scope)
-        ) + self.access_token.emit_store_bytecodes(function, scope)
-
-    def visit_parts(
-        self,
-        visitor: typing.Callable[
-            [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
-            typing.Any,
-        ],
-        parents: list,
-    ):
-        return visitor(
-            self,
-            (
-                self.access_token.visit_parts(visitor, parents + [self]),
-                self.source.visit_parts(visitor, parents + [self])
-                if self.source is not None
-                else None,
-            ),
-            parents,
-        )
+        inner_scope = scope.copy(sub_scope_name=self.name(scope), shared_locals=False)
+
+        target = MutableFunction(lambda: None)
+
+        inner_bytecode = [
+            Instruction(Opcodes.LOAD_NAME, "__name__"),
+            Instruction(Opcodes.STORE_NAME, "__module__"),
+            Instruction(Opcodes.LOAD_CONST, self.name(scope)),
+            Instruction(Opcodes.STORE_NAME, "__qualname__"),
+        ]
+
+        raw_inner_code = self.code_block.emit_bytecodes(target, inner_scope)
+
+        for instr in raw_inner_code:
+            if instr.opcode == Opcodes.LOAD_FAST:
+                instr.change_opcode(Opcodes.LOAD_NAME, arg_value=instr.arg_value)
+            elif instr.opcode == Opcodes.STORE_FAST:
+                instr.change_opcode(Opcodes.STORE_NAME, arg_value=instr.arg_value)
+            elif instr.opcode == Opcodes.DELETE_FAST:
+                instr.change_opcode(Opcodes.DELETE_NAME, arg_value=instr.arg_value)
+
+        inner_bytecode += raw_inner_code
+
+        if inner_bytecode:
+            inner_bytecode[-1].next_instruction = target.instruction_entry_point
+
+        for i, instr in enumerate(inner_bytecode[:-1]):
+            instr.next_instruction = inner_bytecode[i + 1]
+
+        target.instruction_entry_point = inner_bytecode[0]
+        target.reassign_to_function()
+
+        code_obj = target.target.__code__
+
+        bytecode = [
+            Instruction(Opcodes.LOAD_BUILD_CLASS),
+            Instruction(Opcodes.LOAD_CONST, code_obj),
+            Instruction(Opcodes.LOAD_CONST, self.name(scope)),
+            Instruction(Opcodes.MAKE_FUNCTION, arg=0),
+            Instruction(Opcodes.LOAD_CONST, self.name(scope)),
+        ]
+
+        for parent in self.parents:
+            bytecode += parent.emit_bytecodes(
+                function,
+                scope,
+            )
+
+        bytecode += [
+            Instruction(Opcodes.CALL_FUNCTION, arg=2 + len(self.parents)),
+            Instruction(Opcodes.STORE_FAST, self.name(scope)),
+        ]
+        return bytecode
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractStoreFastAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # STORE_FAST <name> [<source>]
-    NAME = "STORE_FAST"
+class AbstractStoreGlobalAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # STORE_GLOBAL <name> [<source>]
+    NAME = "STORE_GLOBAL"
 
     def __init__(
         self,
         name_token: IdentifierToken | IntegerToken | str | int,
         source: AbstractSourceExpression | None = None,
     ):
         self.name_token = (
@@ -30,39 +31,46 @@
                 if isinstance(name_token, str)
                 else IntegerToken(str(name_token))
             )
         )
         self.source = source
 
     @classmethod
-    def consume(cls, parser: "Parser", scope) -> "AbstractStoreFastAssembly":
-        parser.try_consume(SpecialToken("$"))
-        name = parser.consume([IdentifierToken, IntegerToken])
+    def consume(cls, parser: "Parser", scope) -> "AbstractStoreGlobalAssembly":
+        parser.try_consume(SpecialToken("@"))
 
-        source = parser.try_parse_data_source()
+        # todo: make parse_identifier_like()
+        name = parser.try_consume(IdentifierToken)
+
+        if name is None:
+            raise PropagatingCompilerException(
+                "expected <name>"
+            ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
+
+        source = parser.try_parse_data_source(scope=scope)
 
         return cls(name, source)
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.name_token == other.name_token
             and self.source == other.source
         )
 
     def __repr__(self):
-        return f"STORE_FAST({self.name_token}, source={self.source or 'TOS'})"
+        return f"STORE_GLOBAL({self.name_token}, source={self.source or 'TOS'})"
 
-    def copy(self) -> "AbstractStoreFastAssembly":
-        return type(self)(self.name, self.source.copy() if self.source else None)
+    def copy(self) -> "AbstractStoreGlobalAssembly":
+        return type(self)(self.name_token, self.source.copy() if self.source else None)
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self, (self.source.visit_parts(visitor) if self.target else None,)
+            self, (self.source.visit_parts(visitor, []) if self.source else None,)
         )
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/shared/instructions/YieldAssembly.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,92 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
-from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractStoreGlobalAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # STORE_GLOBAL <name> [<source>]
-    NAME = "STORE_GLOBAL"
+class AbstractYieldAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # YIELD [*] [<expr>] [-> <target>]
+    NAME = "YIELD"
 
     def __init__(
         self,
-        name_token: IdentifierToken | IntegerToken | str | int,
-        source: AbstractSourceExpression | None = None,
+        expr: AbstractSourceExpression | None = None,
+        is_star: bool = False,
+        target: AbstractSourceExpression | None = None,
     ):
-        self.name_token = (
-            name_token
-            if not isinstance(name_token, (str, int))
-            else (
-                IdentifierToken(name_token)
-                if isinstance(name_token, str)
-                else IntegerToken(str(name_token))
-            )
-        )
-        self.source = source
+        self.expr = expr
+        self.is_star = is_star
+        self.target = target
 
     @classmethod
-    def consume(cls, parser: "Parser", scope) -> "AbstractStoreGlobalAssembly":
-        parser.try_consume(SpecialToken("@"))
-        name = parser.try_consume([IdentifierToken, IntegerToken])
-
-        if name is None:
-            raise throw_positioned_error(
-                scope, parser.try_inspect(), "expected <name> or <integer>"
-            )
+    def consume(cls, parser: "Parser", scope) -> "AbstractYieldAssembly":
+        is_star = bool(parser.try_consume(SpecialToken("*")))
 
-        source = parser.try_parse_data_source()
+        expr = parser.try_parse_data_source(
+            allow_primitives=True, allow_op=True, include_bracket=False, scope=scope
+        )
 
-        return cls(name, source)
+        if parser.try_consume(SpecialToken("-")) and parser.try_consume(
+            SpecialToken(">")
+        ):
+            target = parser.try_parse_data_source(
+                allow_primitives=True, allow_op=True, include_bracket=False, scope=scope
+            )
 
-    def __eq__(self, other):
-        return (
-            type(self) == type(other)
-            and self.name_token == other.name_token
-            and self.source == other.source
-        )
+            if target is None:
+                raise PropagatingCompilerException(
+                    "expected <expression> after '->'"
+                ).add_trace_level(scope.get_trace_info().with_token(parser[0]))
 
-    def __repr__(self):
-        return f"STORE_GLOBAL({self.name_token}, source={self.source or 'TOS'})"
+        else:
+            target = None
 
-    def copy(self) -> "AbstractStoreGlobalAssembly":
-        return type(self)(self.name_token, self.source.copy() if self.source else None)
+        return cls(expr, is_star, target)
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self, (self.source.visit_parts(visitor, []) if self.source else None,)
+            self,
+            (
+                self.expr.visit_parts(visitor, parents + [self]) if self.expr else None,
+                self.target.visit_parts(
+                    visitor,
+                    parents + [self],
+                )
+                if self.target
+                else None,
+            ),
+            parents,
+        )
+
+    def __eq__(self, other):
+        return (
+            type(self) == type(other)
+            and self.expr == other.expr
+            and self.is_star == other.is_star
+            and self.target == other.target
+        )
+
+    def __repr__(self):
+        return f"YIELD{'' if not self.is_star else '*'}({self.expr if self.expr else ''}{(', ' if self.expr else '->') + repr(self.target) if self.target else ''})"
+
+    def copy(self) -> "AbstractYieldAssembly":
+        return type(self)(
+            self.expr.copy() if self.expr else None,
+            self.is_star,
+            self.target.copy() if self.target else None,
         )
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/ExceptionInstructionCodec.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/ExceptionInstructionCodec.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/LocationInformationHandler.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/LocationInformationHandler.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/assembly_instructions.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/assembly_instructions.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 )
 from bytecodemanipulation.data.shared.expressions.MacroAccessExpression import (
     MacroAccessExpression,
 )
 from bytecodemanipulation.data.shared.instructions.MacroAssembly import MacroAssembly
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class CallAssembly(AbstractCallAssembly):
@@ -148,20 +148,17 @@
     def emit_macro_bytecode(self, function: MutableFunction, scope: ParsingScope):
         access = typing.cast(MacroAccessExpression, self.call_target)
         name = access.name
 
         macro_declaration = scope.lookup_name_in_scope(name[0].text)
 
         if macro_declaration is None:
-            raise throw_positioned_error(
-                scope,
-                typing.cast(MacroAccessExpression, self.call_target).name,
-                f"Macro '{':'.join(map(lambda e: e.text, name))}' not found!",
-                NameError,
-            )
+            raise PropagatingCompilerException(
+                "Macro '{':'.join(map(lambda e: e.text, name))}' not found"
+            ).add_trace_level(self.trace_info.with_token(list(self.call_target.get_tokens()))).set_underlying_exception(NameError)
 
         if len(name) > 1:
             for e in name[1:]:
                 macro_declaration = macro_declaration[e.text]
 
         if not isinstance(macro_declaration, MacroAssembly.MacroOverloadPage):
             raise RuntimeError(
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.data.shared.instructions.ClassDefinitionAssembly import (
     AbstractClassDefinitionAssembly,
 )
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
@@ -22,15 +23,19 @@
         inner_bytecode = [
             Instruction(Opcodes.LOAD_NAME, "__name__"),
             Instruction(Opcodes.STORE_NAME, "__module__"),
             Instruction(Opcodes.LOAD_CONST, self.name(scope)),
             Instruction(Opcodes.STORE_NAME, "__qualname__"),
         ]
 
-        raw_inner_code = self.code_block.emit_bytecodes(target, inner_scope)
+        try:
+            raw_inner_code = self.code_block.emit_bytecodes(target, inner_scope)
+        except PropagatingCompilerException as e:
+            e.add_trace_level(self.trace_info, message=f"during emitting class '{self.name(scope)}'")
+            raise e
 
         for instr in raw_inner_code:
             if instr.opcode == Opcodes.LOAD_FAST:
                 instr.change_opcode(Opcodes.LOAD_NAME, arg_value=instr.arg_value)
             elif instr.opcode == Opcodes.STORE_FAST:
                 instr.change_opcode(Opcodes.STORE_NAME, arg_value=instr.arg_value)
             elif instr.opcode == Opcodes.DELETE_FAST:
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import functools
 import inspect
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import MacroExpandedIdentifier
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
-from bytecodemanipulation.data.shared.expressions.LocalAccessExpression import LocalAccessExpression
-from bytecodemanipulation.data.shared.expressions.MacroParameterAcessExpression import MacroParameterAccessExpression
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException
 from bytecodemanipulation.data.shared.instructions.FunctionDefinitionAssembly import (
     AbstractFunctionDefinitionAssembly,
 )
 from bytecodemanipulation.data.v3_10.instructions.CallAssembly import CallAssembly
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
@@ -62,15 +59,20 @@
         local_variable_buffer = scope.scope_name_generator("outer_locals")
 
         target.argument_count = len(self.args)
         if self.bound_variables:
             target.argument_names.insert(0, local_variable_buffer)
             target.argument_count += 1
 
-        inner_bytecode += self.body.emit_bytecodes(target, inner_scope)
+        try:
+            inner_bytecode += self.body.emit_bytecodes(target, inner_scope)
+        except PropagatingCompilerException as e:
+            e.add_trace_level(self.trace_info, message=f"during parsing function definition {self.func_name(scope)}")
+            raise e
+
         inner_bytecode[-1].next_instruction = target.instruction_entry_point
 
         for i, instr in enumerate(inner_bytecode[:-1]):
             instr.next_instruction = inner_bytecode[i + 1]
 
         def walk_label(instruction: Instruction):
             if instruction.opcode == Opcodes.BYTECODE_LABEL:
@@ -80,14 +82,16 @@
                     if instruction.next_instruction is not None
                     else instruction
                 )
                 instruction.change_opcode(Opcodes.NOP)
 
         inner_bytecode[0].apply_visitor(LambdaInstructionWalker(walk_label))
 
+        has_yield_statement = False
+
         def rewrite_outer_access(instruction: Instruction):
             if instruction.opcode == Opcodes.LOAD_DEREF and instruction.arg_value in scope.closure_locals:
                 instruction.insert_after([
                     Instruction(Opcodes.LOAD_FAST, local_variable_buffer),
                     Instruction(Opcodes.LOAD_CONST, instruction.arg_value),
                     Instruction(Opcodes.BINARY_SUBSCR),
                 ])
@@ -102,17 +106,23 @@
             elif instruction.opcode == Opcodes.DELETE_DEREF and instruction.arg_value in scope.closure_locals:
                 instruction.insert_after([
                     Instruction(Opcodes.LOAD_FAST, local_variable_buffer),
                     Instruction(Opcodes.LOAD_CONST, instruction.arg_value),
                     Instruction(Opcodes.DELETE_SUBSCR),
                 ])
                 instruction.change_opcode(Opcodes.NOP)
+            elif instruction.opcode in (Opcodes.YIELD_VALUE, Opcodes.YIELD_FROM):
+                nonlocal has_yield_statement
+                has_yield_statement = True
 
         inner_bytecode[0].apply_visitor(LambdaInstructionWalker(rewrite_outer_access))
 
+        if has_yield_statement:
+            target.code_flags |= inspect.CO_GENERATOR
+
         def resolve_jump_to_label(ins: Instruction):
             if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
                 ins.change_arg_value(label_targets[ins.arg_value.name])
 
         inner_bytecode[0].apply_visitor(LambdaInstructionWalker(resolve_jump_to_label))
 
         target.instruction_entry_point = inner_bytecode[0]
@@ -171,18 +181,16 @@
                 Instruction(Opcodes.LOAD_ATTR, "f_locals"),
                 Instruction(Opcodes.CALL_FUNCTION, arg=2),
             ]
 
         if self.target:
             bytecode += self.target.emit_store_bytecodes(function, scope)
         elif not self.func_name:
-            raise throw_positioned_error(
-                scope,
-                [],
-                "Expected either 'target' or <valid name>",
-            )
+            raise PropagatingCompilerException(
+                "Expected either 'target' or <valid name>"
+            ).add_trace_level(self.trace_info)
         else:
             bytecode += [
                 Instruction(Opcodes.STORE_FAST, self.prefix + self.func_name(scope)),
             ]
 
         return bytecode
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.syntax_errors import PropagatingCompilerException, TraceInfo
 from bytecodemanipulation.data.shared.instructions.OpAssembly import OpcodeBaseOperator
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.data.shared.instructions.OpAssembly import (
     AbstractOpAssembly,
     AbstractOperator,
@@ -19,14 +19,15 @@
 class NandOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         label_name = scope.scope_name_generator("and_skip_second")
 
         bytecode = lhs.emit_bytecodes(function, scope)
         bytecode += [
             Instruction(Opcodes.DUP_TOP),
             Instruction(
@@ -51,14 +52,15 @@
 class AndOperator(NandOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         return super().emit_bytecodes(function, scope, lhs, rhs) + [
             Instruction(Opcodes.UNARY_NOT, bool)
         ]
 
     def evaluate_static_value(self, scope: ParsingScope, lhs: AbstractSourceExpression, rhs: AbstractSourceExpression):
         if not lhs.evaluate_static_value(scope):
@@ -70,14 +72,15 @@
 class AndEvalOperator(NandOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         inner_label = scope.scope_name_generator("and_eval_swap_skip")
 
         return lhs.emit_bytecodes(function, scope) + rhs.emit_bytecodes(function, scope) + [
             Instruction(Opcodes.DUP_TOP),
             Instruction(Opcodes.POP_JUMP_IF_TRUE, JumpToLabel(inner_label)),
             Instruction(Opcodes.ROT_TWO),
@@ -95,14 +98,15 @@
 class NorOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         label_name = scope.scope_name_generator("or_skip_second")
 
         bytecode = lhs.emit_bytecodes(function, scope)
         bytecode += [
             Instruction(Opcodes.DUP_TOP),
             Instruction(
@@ -127,14 +131,15 @@
 class OrOperator(NorOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         return super().emit_bytecodes(function, scope, lhs, rhs) + [
             Instruction(Opcodes.UNARY_NOT, bool)
         ]
 
     def evaluate_static_value(self, scope: ParsingScope, lhs: AbstractSourceExpression, rhs: AbstractSourceExpression):
         if lhs.evaluate_static_value(scope):
@@ -146,14 +151,15 @@
 class OrEvalOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         inner_label = scope.scope_name_generator("or_eval_swap_skip")
 
         return lhs.emit_bytecodes(function, scope) + rhs.emit_bytecodes(function, scope) + [
             Instruction(Opcodes.DUP_TOP),
             Instruction(Opcodes.POP_JUMP_IF_FALSE, JumpToLabel(inner_label)),
             Instruction(Opcodes.ROT_TWO),
@@ -171,14 +177,15 @@
 class XOROperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope)
         bytecode += [
             Instruction(Opcodes.UNARY_NOT),
         ]
         bytecode += rhs.emit_bytecodes(function, scope)
         bytecode += [
@@ -197,14 +204,15 @@
 class XNOROperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope)
         bytecode += [
             Instruction(Opcodes.UNARY_NOT),
         ]
         bytecode += rhs.emit_bytecodes(function, scope)
         bytecode += [
@@ -223,14 +231,15 @@
 class WalrusOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         bytecode = rhs.emit_bytecodes(function, scope)
         bytecode += [
             Instruction(Opcodes.DUP_TOP),
         ]
         bytecode += lhs.emit_store_bytecodes(function, scope)
         return bytecode
@@ -239,14 +248,15 @@
 class InverseWalrusOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope)
         bytecode += [
             Instruction(Opcodes.DUP_TOP),
         ]
         bytecode += rhs.emit_store_bytecodes(function, scope)
         return bytecode
@@ -255,52 +265,67 @@
 class InstanceOfChecker(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope) + rhs.emit_bytecodes(
             function, scope
         )
         bytecode += [
             Instruction(Opcodes.LOAD_CONST, isinstance),
             Instruction(Opcodes.ROT_THREE),
             Instruction(Opcodes.CALL_FUNCTION, arg=2),
         ]
         return bytecode
 
+    def evaluate_static_value(self, scope: ParsingScope, lhs: AbstractSourceExpression, rhs: AbstractSourceExpression):
+        lhs = lhs.evaluate_static_value(scope)
+        rhs = rhs.evaluate_static_value(scope)
+
+        return isinstance(lhs, rhs)
+
 
 class SubclassOfChecker(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope) + rhs.emit_bytecodes(
             function, scope
         )
         bytecode += [
             Instruction(Opcodes.LOAD_CONST, issubclass),
             Instruction(Opcodes.ROT_THREE),
             Instruction(Opcodes.CALL_FUNCTION, arg=2),
         ]
         return bytecode
 
+    def evaluate_static_value(self, scope: ParsingScope, lhs: AbstractSourceExpression, rhs: AbstractSourceExpression):
+        lhs = lhs.evaluate_static_value(scope)
+        rhs = rhs.evaluate_static_value(scope)
+
+        return issubclass(lhs, rhs)
+
 
 class HasattrChecker(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope) + rhs.emit_bytecodes(
             function, scope
         )
         bytecode += [
             Instruction(Opcodes.LOAD_CONST, hasattr),
             Instruction(Opcodes.ROT_THREE),
@@ -310,15 +335,16 @@
 
 
 class SumOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
-        *parameters: AbstractSourceExpression
+        *parameters: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         if len(parameters) == 0:
             raise SyntaxError("expected at least one parameter")
 
         bytecode = parameters[0].emit_bytecodes(function, scope)
 
         for param in parameters[1:]:
@@ -340,15 +366,16 @@
 
 
 class ProdOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
-        *parameters: AbstractSourceExpression
+        *parameters: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         if len(parameters) == 0:
             raise SyntaxError("expected at least one parameter")
 
         bytecode = parameters[0].emit_bytecodes(function, scope)
 
         for param in parameters[1:]:
@@ -370,15 +397,16 @@
 
 
 class AvgOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
-        *parameters: AbstractSourceExpression
+        *parameters: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         if len(parameters) == 0:
             raise SyntaxError("expected at least one parameter")
 
         bytecode = parameters[0].emit_bytecodes(function, scope)
 
         for param in parameters[1:]:
@@ -404,15 +432,16 @@
 
 
 class AvgIOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
-        *parameters: AbstractSourceExpression
+        *parameters: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         if len(parameters) == 0:
             raise SyntaxError("expected at least one parameter")
 
         bytecode = parameters[0].emit_bytecodes(function, scope)
 
         for param in parameters[1:]:
@@ -439,14 +468,15 @@
 
 class TupleOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         *parameters: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         bytecode = []
 
         for param in parameters:
             bytecode += param.emit_bytecodes(
                 function,
                 scope,
@@ -469,14 +499,15 @@
 
 class ListOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         *parameters: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         bytecode = []
 
         for param in parameters:
             bytecode += param.emit_bytecodes(
                 function,
                 scope,
@@ -491,14 +522,15 @@
 
 class SetOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         *parameters: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         bytecode = []
 
         for param in parameters:
             bytecode += param.emit_bytecodes(
                 function,
                 scope,
@@ -513,21 +545,20 @@
 
 class DictOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         *parameters: AbstractSourceExpression,
+        trace_info: typing.Optional[TraceInfo] = None,
     ) -> typing.List[Instruction]:
         if len(parameters) % 2 != 0:
-            raise throw_positioned_error(
-                scope,
-                sum([list(param.get_tokens()) for param in parameters], []),
-                "expected even arg count for dict build",
-            )
+            raise PropagatingCompilerException(
+                "expected even arg count for dict build"
+            ).add_trace_level(trace_info.with_token(sum([list(param.get_tokens()) for param in parameters], [])))
 
         bytecode = []
 
         for param in parameters:
             bytecode += param.emit_bytecodes(
                 function,
                 scope,
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/assembly_instructions.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/assembly_instructions.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.IfAssembly import AbstractIFAssembly
+from bytecodemanipulation.data.shared.instructions.WhileAssembly import (
+    AbstractWhileAssembly,
+)
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
-class IFAssembly(AbstractIFAssembly):
+class WHILEAssembly(AbstractWhileAssembly):
     def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
-
         if self.label_name is None:
             end = Instruction("NOP")
         else:
             end = Instruction(
                 function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text + "_END"
             )
 
-        return (
-            (
-                []
-                if self.label_name is None
-                else [
-                    Instruction(
-                        function,
-                        -1,
-                        Opcodes.BYTECODE_LABEL,
-                        self.label_name.text + "_HEAD",
-                    )
-                ]
+        CONDITION = self.source.emit_bytecodes(function, scope)
+
+        if self.label_name:
+            CONDITION.insert(
+                0,
+                Instruction(Opcodes.BYTECODE_LABEL, self.label_name.text),
             )
-            + self.source.emit_bytecodes(function, scope)
-            + [Instruction("POP_JUMP_IF_FALSE", end)]
-            + (
-                []
-                if self.label_name is None
-                else [
-                    Instruction(
-                        function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text
-                    )
-                ]
+
+        HEAD = Instruction("POP_JUMP_IF_FALSE", end)
+
+        BODY = self.body.emit_bytecodes(function, scope)
+
+        if self.label_name:
+            BODY.insert(
+                0,
+                Instruction(
+                    function,
+                    -1,
+                    Opcodes.BYTECODE_LABEL,
+                    self.label_name.text + "_INNER",
+                ),
             )
-            + self.body.emit_bytecodes(function, scope)
-            + [end]
-        )
+
+        JUMP_BACK = Instruction("JUMP_ABSOLUTE", CONDITION[0])
+
+        return CONDITION + [HEAD] + BODY + [JUMP_BACK, end]
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/data_loader.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/data_loader.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/mixin_util.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/mixin_util.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py`

 * *Files 15% similar despite different names*

```diff
@@ -131,14 +131,68 @@
         pass
 
     @classmethod
     def get_new_metadata(cls, function: "MutableFunction", old_meta: typing.Any, metadata: typing.List[typing.Tuple["Instruction", typing.Any]]) -> typing.Any:
         return old_meta
 
 
+class ForIterTransformer(AbstractInstructionWalkerTransform):
+    """
+    This is a hack to make the strange FOR_ITER opcode work, by replacing it by a sequence of equal opcodes
+    """
+
+    class _ForIterDefault:
+        def __repr__(self):
+            return "FOR_ITER"
+
+    """
+    FOR_ITER<skip target> ->
+
+    DUP_TOP
+    LOAD_FAST ~next
+    ROT_TWO
+    LOAD_CONST <empty value>
+    CALL_METHOD 2
+    DUP_TOP
+    LOAD_CONST <empty value>
+    COMPARE_EQ
+    POP_JUMP_IF_FALSE <skip>
+    POP_TOP
+    POP_TOP
+    JUMP <target>
+    [continue]
+    """
+
+    DEFAULT_VALUE = _ForIterDefault()
+
+    @classmethod
+    def visit(cls, function: "MutableFunction", metadata: typing.Any, target: "Instruction") -> typing.Any:
+        if target.opcode == Opcodes.FOR_ITER:
+            section = [
+                Instruction(Opcodes.DUP_TOP),
+                Instruction(Opcodes.LOAD_CONST, next),
+                Instruction(Opcodes.ROT_TWO),
+                Instruction(Opcodes.LOAD_CONST, cls.DEFAULT_VALUE),
+                Instruction(Opcodes.CALL_FUNCTION, arg=2),
+                Instruction(Opcodes.DUP_TOP),
+                Instruction(Opcodes.LOAD_CONST, cls.DEFAULT_VALUE),
+                Instruction(Opcodes.COMPARE_EQ),
+                Instruction(Opcodes.POP_JUMP_IF_FALSE, arg_value=target.next_instruction),
+                Instruction(Opcodes.POP_TOP),
+                Instruction(Opcodes.POP_TOP),
+                Instruction(Opcodes.JUMP_FORWARD, arg_value=target.arg_value),
+            ]
+
+            for i, instr in enumerate(section[:-1]):
+                instr.next_instruction = section[i+1]
+
+            target.change_opcode(Opcodes.NOP)
+            target.next_instruction = section[0]
+
+
 class ArgRealValueSetter(AbstractInstructionWalkerTransform):
     @classmethod
     def visit(cls, function: "MutableFunction", builder: CodeObjectBuilder, target: "Instruction") -> typing.Any:
         if target.has_local():
             target.arg = builder.reserve_local_name(target.arg_value)
         elif target.has_name():
             target.arg = builder.reserve_name(target.arg_value)
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/CacheEntryCreation.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/CacheEntryCreation.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/CodeObjectBuilder.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/CodeObjectBuilder.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/ExceptionTable.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/ExceptionTable.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/Instruction.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/Instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -684,15 +684,15 @@
             Opcodes.UNARY_INVERT,
             Opcodes.UNARY_POSITIVE,
             Opcodes.STATIC_ATTRIBUTE_ACCESS,
         ):
             return 1, 1, None
 
         if self.opcode in (Opcodes.STORE_ATTR, Opcodes.STORE_SUBSCR):
-            return 2, 0, None
+            return 0, 2, None
 
         if self.opcode in (
             Opcodes.POP_TOP,
             Opcodes.POP_JUMP_IF_TRUE,
             Opcodes.POP_JUMP_IF_FALSE,
             Opcodes.STORE_FAST,
             Opcodes.STORE_NAME,
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/OpcodeReplacer.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/OpcodeReplacer.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/opcodes/Opcodes.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/opcodes/Opcodes.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/optimiser_util.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/optimiser_util.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation/util.py` & `bytecodemanipulation-0.3.5/bytecodemanipulation/util.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/PKG-INFO` & `bytecodemanipulation-0.3.5/bytecodemanipulation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecodemanipulation
-Version: 0.3.4
+Version: 0.3.5
 Summary: High level python bytecode manipulation
 Home-page: https://github.com/uuk0/PyBytecodeManipulator
 Author: uuk
 Author-email: uuk1301@gmail.com
 Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `bytecodemanipulation-0.3.4/bytecodemanipulation.egg-info/SOURCES.txt` & `bytecodemanipulation-0.3.5/bytecodemanipulation.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,18 @@
 bytecodemanipulation/opcodes/CodeObjectBuilder.py
 bytecodemanipulation/opcodes/ExceptionTable.py
 bytecodemanipulation/opcodes/Instruction.py
 bytecodemanipulation/opcodes/OpcodeReplacer.py
 bytecodemanipulation/opcodes/Opcodes.py
 bytecodemanipulation/opcodes/__init__.py
 tests/test_Assembly.py
+tests/test_AssertAssembly.py
+tests/test_AttributeAccessExpression.py
+tests/test_CompoundExpression.py
+tests/test_ConstantAccessExpression.py
 tests/test_InlineSystem.py
 tests/test_Mixin.py
 tests/test_MutableFunction.py
 tests/test_Operators.py
 tests/test_Optimiser.py
 tests/test_Specializations.py
 tests/test_StandardLibrary.py
```

### Comparing `bytecodemanipulation-0.3.4/setup.py` & `bytecodemanipulation-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="bytecodemanipulation",
-    version="0.3.4",
+    version="0.3.5",
     author="uuk",
     author_email="uuk1301@gmail.com",
     description="High level python bytecode manipulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uuk0/PyBytecodeManipulator",
     project_urls={
```

### Comparing `bytecodemanipulation-0.3.4/tests/test_Assembly.py` & `bytecodemanipulation-0.3.5/tests/test_Assembly.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dis
 import functools
 import itertools
 import sys
 from unittest import TestCase
 
 import bytecodemanipulation.data_loader
+from bytecodemanipulation.Emulator import run_code
 from bytecodemanipulation.data.shared.instructions.LabelAssembly import LabelAssembly
 from bytecodemanipulation.data.shared.instructions.PythonCodeAssembly import (
     PythonCodeAssembly,
 )
 
 from bytecodemanipulation.data.shared.instructions.FunctionDefinitionAssembly import (
     AbstractFunctionDefinitionAssembly,
@@ -107,36 +108,41 @@
         )
 
         for a, b in zip(correct.children, to_check.children):
             self.assertEqual(a, b)
 
     def test_syntax_error(self):
         def test():
-            @apply_inline_assemblies
             def target():
                 assembly(
                     """
 LOAD 19 --> $test
     """
                 )
 
-        self.assertRaises(SyntaxError, test)
+            apply_inline_assemblies(target, unwrap_exceptions=False)
+
+        try:
+            test()
+        except PropagatingCompilerException as e:
+            self.assertEqual(e.underlying_exception, SyntaxError)
+            self.assertEqual(e.args, ("expected '>' after '-' to complete '->'",))
+        else:
+            self.fail()
 
     def test_load_global(self):
         expr = Parser(
-            "LOAD_GLOBAL test\nLOAD_GLOBAL 10\nLOAD_GLOBAL @test\nLOAD_GLOBAL @10\nLOAD_GLOBAL @hello -> $test"
+            "LOAD_GLOBAL test\nLOAD_GLOBAL @test\nLOAD_GLOBAL @hello -> $test"
         ).parse()
 
         self.assertEqualList(
             CompoundExpression(
                 [
                     AbstractLoadGlobalAssembly.IMPLEMENTATION("test"),
-                    AbstractLoadGlobalAssembly.IMPLEMENTATION(10),
                     AbstractLoadGlobalAssembly.IMPLEMENTATION("test"),
-                    AbstractLoadGlobalAssembly.IMPLEMENTATION(10),
                     AbstractLoadGlobalAssembly.IMPLEMENTATION(
                         "hello", LocalAccessExpression("test")
                     ),
                 ]
             ),
             expr,
         )
@@ -1844,47 +1850,14 @@
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(), 10)
 
 
 class TestAssert(TestCase):
-    def test_assert(self):
-        @apply_operations
-        def target(x):
-            assembly(
-                """
-ASSERT $x
-"""
-            )
-
-        dis.dis(target)
-
-        target(1)
-        self.assertRaises(AssertionError, lambda: target(0))
-
-    def test_assert_with_message(self):
-        @apply_operations
-        def target(x):
-            assembly(
-                """
-ASSERT $x \"Test Message\"
-"""
-            )
-
-        target(1)
-        self.assertRaises(AssertionError, lambda: target(0))
-
-        try:
-            target(0)
-        except AssertionError as e:
-            self.assertEqual(e.args, ("Test Message",))
-        else:
-            self.assertTrue(False)
-
     def test_assert_static(self):
         @apply_operations
         def target():
             assembly("ASSERT_STATIC 1")
 
         target()
 
@@ -1922,15 +1895,15 @@
     def test_assert_static_dynamic_expression(self):
         def target():
             assembly("ASSERT_STATIC $a")
 
         try:
             apply_operations(target)
         except SyntaxError as e:
-            self.assertEqual(e.args, ("Expected <static evaluate-able at 'expression'>",))
+            self.assertEqual(e.args, ("Expected <static evaluate-able> at 'expression', got 'LocalAccessExpression' as type",))
 
     def test_assert_static_macro_static_parameter(self):
         @apply_operations
         def target():
             assembly(
                 """
 MACRO test_assert_static_macro_static_parameter(a)
@@ -2051,7 +2024,185 @@
 ASSERT OP ($test == 0) "old implementation limitation lifted?"
 RETURN $result 
 """)
 
         dis.dis(target)
 
         self.assertEqual(target(), 10)
+
+    def test_change_after_create(self):
+        @apply_operations
+        def target():
+            assembly("""
+LOAD 0 -> $test            
+
+DEF func<test>()
+{
+    RETURN §test
+}
+
+LOAD 1 -> $test
+
+LOAD $func() -> $result
+# ASSERT OP ($test == 10)  # wont work as we currently cannot write back outside
+ASSERT OP ($test == 1) "old implementation limitation lifted?"
+RETURN $result 
+""")
+
+        dis.dis(target)
+
+        # todo: this is a limitation of the current implementation, we don't update the local variables
+        #    captured
+        # self.assertEqual(target(), 1)
+        self.assertEqual(target(), 0)
+
+
+class TestPropagateException(TestCase):
+    def test_class_add_info_to_exception(self):
+        def target():
+            def test():
+                assembly("""
+CLASS xy {
+    LOAD 10 -> 20
+}
+"""
+                )
+
+            apply_inline_assemblies(test, unwrap_exceptions=False)
+
+        try:
+            target()
+        except PropagatingCompilerException as e:
+            self.assertEqual(e.args, ("Expected <newline> or ';' after assembly instruction, got '20' (IntegerToken)",))
+            self.assertEqual(len(e.levels), 2)
+
+    def test_class_add_info_to_exception_emitting(self):
+        def target():
+            def test():
+                assembly("""
+CLASS xy {
+    ASSERT_STATIC $test
+}
+"""
+                         )
+
+            apply_inline_assemblies(test, unwrap_exceptions=False)
+
+        try:
+            target()
+        except PropagatingCompilerException as e:
+            self.assertEqual(e.args, ("Expected <static evaluate-able> at 'expression', got 'LocalAccessExpression' as type",))
+            self.assertEqual(len(e.levels), 2)
+
+    def test_function_add_info_to_exception(self):
+        def target():
+            def test():
+                assembly("""
+DEF xy() {
+    LOAD 10 -> 20
+}
+"""
+                         )
+
+            apply_inline_assemblies(test, unwrap_exceptions=False)
+
+        try:
+            target()
+        except PropagatingCompilerException as e:
+            self.assertEqual(e.args, ("Expected <newline> or ';' after assembly instruction, got '20' (IntegerToken)",))
+            self.assertEqual(len(e.levels), 2)
+
+    def test_function_add_info_to_exception_emitting(self):
+        def target():
+            def test():
+                assembly("""
+DEF xy() {
+    ASSERT_STATIC $test
+}
+"""
+                         )
+
+            apply_inline_assemblies(test, unwrap_exceptions=False)
+
+        try:
+            target()
+        except PropagatingCompilerException as e:
+            self.assertEqual(e.args, ("Expected <static evaluate-able> at 'expression', got 'LocalAccessExpression' as type",))
+            self.assertEqual(len(e.levels), 2)
+
+    def test_namespace_add_info_to_exception(self):
+        def target():
+            def test():
+                assembly("""
+NAMESPACE xy {
+    LOAD 10 -> 20
+}
+"""
+                         )
+
+            apply_inline_assemblies(test, unwrap_exceptions=False)
+
+        try:
+            target()
+        except PropagatingCompilerException as e:
+            self.assertEqual(e.args,
+                             ("Expected <newline> or ';' after assembly instruction, got '20' (IntegerToken)",))
+            self.assertEqual(len(e.levels), 2)
+
+    def test_namespace_add_info_to_exception_emitting(self):
+        def target():
+            def test():
+                assembly("""
+NAMESPACE xy {
+    ASSERT_STATIC $test
+}
+"""
+                         )
+
+            apply_inline_assemblies(test, unwrap_exceptions=False)
+
+        try:
+            target()
+        except PropagatingCompilerException as e:
+            self.assertEqual(e.args, (
+            "Expected <static evaluate-able> at 'expression', got 'LocalAccessExpression' as type",))
+            self.assertEqual(len(e.levels), 2)
+
+    def test_macro_decl_add_info_to_exception(self):
+        def target():
+            def test():
+                assembly("""
+MACRO xy_1() {
+    LOAD 10 -> 20
+}
+"""
+                         )
+
+            apply_inline_assemblies(test, unwrap_exceptions=False)
+
+        try:
+            target()
+        except PropagatingCompilerException as e:
+            self.assertEqual(e.args, ("Expected <newline> or ';' after assembly instruction, got '20' (IntegerToken)",))
+            self.assertEqual(len(e.levels), 2)
+            self.assertEqual(e.levels[0][0].tokens[0].text, "20")
+            self.assertEqual(e.levels[1][0].tokens[0].text, "xy_1")
+
+    def test_macro_decl_add_info_to_exception_emitting(self):
+        def target():
+            def test():
+                assembly("""
+MACRO xy_2() {
+    ASSERT_STATIC $test
+}
+"""
+                         )
+
+            apply_inline_assemblies(test, unwrap_exceptions=False)
+
+        try:
+            target()
+        except PropagatingCompilerException as e:
+            self.assertEqual(e.args, ("Expected <static evaluate-able> at 'expression', got LocalAccessExpression as type",))
+            self.assertEqual(len(e.levels), 2)
+            self.assertEqual(e.levels[0][0].tokens[0].text, "20")
+            self.assertEqual(e.levels[1][0].tokens[0].text, "xy_1")
```

### Comparing `bytecodemanipulation-0.3.4/tests/test_InlineSystem.py` & `bytecodemanipulation-0.3.5/tests/test_InlineSystem.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/tests/test_Mixin.py` & `bytecodemanipulation-0.3.5/tests/test_Mixin.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/tests/test_MutableFunction.py` & `bytecodemanipulation-0.3.5/tests/test_MutableFunction.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/tests/test_Operators.py` & `bytecodemanipulation-0.3.5/tests/test_Operators.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/tests/test_Optimiser.py` & `bytecodemanipulation-0.3.5/tests/test_Optimiser.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.4/tests/test_StandardLibrary.py` & `bytecodemanipulation-0.3.5/tests/test_StandardLibrary.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,27 @@
 import os.path
 import time
 from unittest import TestCase
 import dis
 
+from bytecodemanipulation.Emulator import run_code
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.assembler.target import *
 from bytecodemanipulation.assembler.Emitter import apply_inline_assemblies
 
 
 class StandardLibraryTest(TestCase):
     def setUp(self):
         import bytecodemanipulation.assembler.hook as hook
 
         hook.hook()
 
         def target():
-            assembly("""MACRO_IMPORT bytecodemanipulation.standard_library""")
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        target()
-
-    def test_macro_import(self):
-        def target():
-            assembly(
-                """CALL MACRO std:print("Hello World"); CALL MACRO std:print("Hello World", "World Hello!"); CALL MACRO std:print("hello", "world", "test", 123)"""
-            )
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-        target()
-
-    def test_macro_as_assembly(self):
-        def target():
-            assembly("""std:print("Hello World")""")
+            assembly("""
+MACRO_IMPORT bytecodemanipulation.standard_library""")
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         target()
 
@@ -101,26 +82,27 @@
             data = (0, 1, 2)
             stream = None
             output = None
             assembly(
                 """
 std:stream:initialize($stream)
 std:stream:extend($stream, $data)
-std:stream:to_list($stream, $output)
+std:stream:to_list($stream) -> $output
 """
             )
             return output
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(), [0, 1, 2])
 
     def test_stream_simple_reduce(self):
+        @apply_operations
         def target():
             data = (0, 1, 2)
             stream = None
             output = None
             assembly(
                 """
 std:stream:initialize($stream)
@@ -129,37 +111,93 @@
     OP $lhs + $rhs
 })
 STORE $output
 """
             )
             return output
 
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
         self.assertEqual(target(), 3)
 
+    def test_stream_simple_reduce_empty(self):
+        @apply_operations
+        def target():
+            data = tuple()
+            stream = None
+            output = None
+            assembly(
+                """
+std:stream:initialize($stream)
+std:stream:extend($stream, $data)
+std:stream:reduce($stream, [$lhs, $rhs] {
+    OP $lhs + $rhs
+})
+STORE $output
+"""
+            )
+            return output
+
+        dis.dis(target)
+
+        self.assertEqual(target(), -1)
+
+    def test_stream_simple_reduce_with_start(self):
+        @apply_operations
+        def target():
+            data = (0, 1, 2)
+            stream = None
+            output = None
+            assembly(
+                """
+std:stream:initialize($stream)
+std:stream:extend($stream, $data)
+std:stream:reduce($stream, [$lhs, $rhs] {
+    OP $lhs + $rhs
+}, 2)
+STORE $output
+"""
+            )
+            return output
+
+        self.assertEqual(target(), 5)
+
+    def test_stream_simple_reduce_with_start_empty(self):
+        @apply_operations
+        def target():
+            data = tuple()
+            stream = None
+            output = None
+            assembly(
+                """
+std:stream:initialize($stream)
+std:stream:extend($stream, $data)
+std:stream:reduce($stream, [$lhs, $rhs] {
+    OP $lhs + $rhs
+}, 2)
+STORE $output
+"""
+            )
+            return output
+
+        self.assertEqual(target(), 2)
+
     def test_stream_simple_filter(self):
 
         @apply_operations
         def target():
             data = (0, 1, 2)
             stream = None
             output = None
             assembly(
                 """
 std:stream:initialize($stream)
 std:stream:extend($stream, $data)
-std:print($stream)
 std:stream:filter($stream, [$var] {
     OP $var < 2 -> %
 })
-std:print($stream)
-std:stream:to_list($stream, $output)
+std:stream:to_list($stream) -> $output
 """
             )
             return output
 
         self.assertEqual(target(), [0, 1])
 
     def test_stream_simple_map(self):
@@ -171,21 +209,61 @@
             assembly(
                 """
 std:stream:initialize($stream)
 std:stream:extend($stream, $data)
 std:stream:map($stream, [$var] {
     OP $var + 1 -> $var
 })
-std:stream:to_list($stream, $output)
+std:stream:to_list($stream) -> $output
 """
             )
             return output
 
         self.assertEqual(target(), [1, 2, 3])
 
+    def test_stream_grouped(self):
+        @apply_operations
+        def target():
+            data = (0, 1, 2, 3)
+            stream = None
+            output = None
+            assembly(
+                """
+std:stream:initialize($stream)
+std:stream:extend($stream, $data)
+std:stream:grouped($stream, 2, [_] {})
+std:stream:to_list($stream) -> $output
+"""
+            )
+            return output
+
+        dis.dis(target)
+        # self.assertEqual(run_code(target), [1, 2, 3])
+        self.assertEqual(target(), [[0, 1], [2, 3]])
+
+    def test_stream_grouped_without_handle(self):
+        @apply_operations
+        def target():
+            data = (0, 1, 2, 3)
+            stream = None
+            output = None
+            assembly(
+                """
+std:stream:initialize($stream)
+std:stream:extend($stream, $data)
+std:stream:grouped($stream, 2)
+std:stream:to_list($stream) -> $output
+"""
+            )
+            return output
+
+        dis.dis(target)
+
+        self.assertEqual(target(), [[0, 1], [2, 3]])
+
     def test_comprehension_list(self):
         @apply_operations
         def target():
             l = [1, 2, 3, 4]
             assembly("""
 std:comprehension:list($l, [$value] { OP $value + 1 -> % }) -> %
 RETURN %""")
```

### Comparing `bytecodemanipulation-0.3.4/tests/test_issues.py` & `bytecodemanipulation-0.3.5/tests/test_issues.py`

 * *Files identical despite different names*

