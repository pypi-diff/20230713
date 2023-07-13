# Comparing `tmp/SwissArmyTransformer-0.4.0.tar.gz` & `tmp/SwissArmyTransformer-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-br8z1pgj/SwissArmyTransformer-0.4.0.tar", last modified: Wed Jul  5 09:26:21 2023, max compression
+gzip compressed data, was "SwissArmyTransformer-0.4.1.tar", last modified: Thu Jul 13 14:26:33 2023, max compression
```

## Comparing `SwissArmyTransformer-0.4.0.tar` & `SwissArmyTransformer-0.4.1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.874483 SwissArmyTransformer-0.4.0/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.4.0/LICENSE
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      191 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/MANIFEST.in
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9410 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/README.md
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.846483 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-07-05 09:26:21.000000 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4934 2023-07-05 09:26:21.000000 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-07-05 09:26:21.000000 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       90 2023-07-05 09:26:21.000000 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/requires.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-07-05 09:26:21.000000 SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/top_level.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       89 2023-06-28 07:19:19.000000 SwissArmyTransformer-0.4.0/requirements.txt
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.850483 SwissArmyTransformer-0.4.0/sat/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      433 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    25363 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/arguments.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.850483 SwissArmyTransformer-0.4.0/sat/data_utils/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/data_utils/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15565 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/data_utils/configure_data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2676 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/data_utils/datasets.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.4.0/sat/data_utils/hf_dataset.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/data_utils/samplers.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7129 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/data_utils/webds.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.850483 SwissArmyTransformer-0.4.0/sat/generation/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/generation/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9777 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/generation/autoregressive_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/generation/cuda2d_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/generation/magnify.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.854483 SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4025 2023-05-27 05:35:24.000000 SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/base_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7377 2023-05-15 19:45:51.000000 SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/beam_search_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.4.0/sat/generation/utils.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5187 2023-05-16 12:24:16.000000 SwissArmyTransformer-0.4.0/sat/helpers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.854483 SwissArmyTransformer-0.4.0/sat/model/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      214 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/model/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.854483 SwissArmyTransformer-0.4.0/sat/model/attention/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      110 2023-06-06 14:36:22.000000 SwissArmyTransformer-0.4.0/sat/model/attention/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3654 2023-06-07 06:54:10.000000 SwissArmyTransformer-0.4.0/sat/model/attention/memory_efficient_attention.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12760 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/base_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1731 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/cached_autoregressive_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5479 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/model/encoder_decoder_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.854483 SwissArmyTransformer-0.4.0/sat/model/finetune/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/adapter.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/ffadd.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/lora.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    13473 2023-06-01 06:34:25.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/lora2.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/mlp_head.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/finetune/prompt_tuning.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      391 2023-06-06 14:36:32.000000 SwissArmyTransformer-0.4.0/sat/model/mixins.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.854483 SwissArmyTransformer-0.4.0/sat/model/normalization/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       24 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/normalization/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      610 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/normalization/rms.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.858483 SwissArmyTransformer-0.4.0/sat/model/official/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      676 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/official/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1923 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/official/bert_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/cait_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     6378 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/official/chatglm2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    12890 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/model/official/chatglm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7294 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/model/official/clip_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9612 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/model/official/cuda2d_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/distill_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/dpr_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.4.0/sat/model/official/eva2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    13903 2023-06-06 13:57:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/glm130B_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.0/sat/model/official/glm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/gpt2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/gptneo_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4614 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/official/llama_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/mae_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/roberta_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/t5_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6254 2023-05-27 05:12:45.000000 SwissArmyTransformer-0.4.0/sat/model/official/vit_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/official/yolos_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.858483 SwissArmyTransformer-0.4.0/sat/model/position_embedding/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/position_embedding/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5402 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/model/position_embedding/rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2713 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/position_embedding/rotary_embeddings_original.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/position_embedding/sincos2d.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-05-16 18:46:06.000000 SwissArmyTransformer-0.4.0/sat/model/position_embedding/vision_rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      819 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/model/registry.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    28857 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/model/transformer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.858483 SwissArmyTransformer-0.4.0/sat/mpu/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2217 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/mpu/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/mpu/cross_entropy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/mpu/data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4926 2023-05-16 13:17:56.000000 SwissArmyTransformer-0.4.0/sat/mpu/initialize.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    18083 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/mpu/layers.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/mpu/mappings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1243 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/mpu/operation.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3924 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/mpu/utils.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.858483 SwissArmyTransformer-0.4.0/sat/ops/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1233 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.842483 SwissArmyTransformer-0.4.0/sat/ops/csrc/
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      947 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5595 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/multi_tensor_apply.cuh
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7076 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/multi_tensor_ema_adam.cu
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/ops/csrc/includes/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      336 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/csrc/includes/compat.h
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     6388 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/csrc/includes/type_shim.h
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    10712 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/fused_ema_adam.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/ops/layernorm.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/ops/local_attention_function.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      578 2023-06-07 05:52:48.000000 SwissArmyTransformer-0.4.0/sat/ops/memory_efficient_attention.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/ops/ops_builder/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1982 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/ops_builder/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    28554 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/ops_builder/builder.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      957 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.0/sat/ops/ops_builder/fused_ema_adam.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-06-05 05:26:26.000000 SwissArmyTransformer-0.4.0/sat/ops/scaled_mask_softmax.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/quantization/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       29 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.4.0/sat/quantization/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    18674 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.4.0/sat/quantization/kernels.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/resources/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/resources/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6754 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/resources/download.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3081 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/resources/urls.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/tokenization/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.4.0/sat/tokenization/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/templates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/unified_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.862483 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/api.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/vqvae_zc.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.842483 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.866483 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/chinese_sentencepiece/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/sat/tokenization/glm/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/glm/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/glm/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization_gpt2.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization_wordpiece.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/hf_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/sat/training/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.0/sat/training/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23899 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/training/deepspeed_training.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/training/deepspeed_zero0.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/training/deepspeed_zero1.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/sat/training/deepspeed_zero2.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.4.0/sat/training/learning_rates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    11576 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/training/model_io.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.4.0/sat/training/utils.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9348 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/sat/transformer_defaults.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-07-05 09:26:21.874483 SwissArmyTransformer-0.4.0/setup.cfg
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-07-05 09:23:25.000000 SwissArmyTransformer-0.4.0/setup.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-05 09:26:21.870483 SwissArmyTransformer-0.4.0/tests/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/tests/test_base_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.4.0/tests/test_inference.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.0/tests/test_list_info.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3104 2023-06-07 06:54:04.000000 SwissArmyTransformer-0.4.0/tests/test_mea.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      913 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.0/tests/test_model_parallel.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.0/tests/test_nested_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      611 2023-05-18 18:05:46.000000 SwissArmyTransformer-0.4.0/tests/test_speed.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.4.0/tests/test_train.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-17 07:43:42.000000 SwissArmyTransformer-0.4.0/tests/test_train_dp.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.0/tests/test_train_nested.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.417250 SwissArmyTransformer-0.4.1/
+-rw-rw-r--   0 dm        (2000) dm        (2000)    11338 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/LICENSE
+-rw-rw-r--   0 dm        (2000) dm        (2000)      191 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/MANIFEST.in
+-rw-rw-r--   0 dm        (2000) dm        (2000)     9893 2023-07-13 14:26:33.416622 SwissArmyTransformer-0.4.1/PKG-INFO
+-rw-rw-r--   0 dm        (2000) dm        (2000)     9521 2023-07-13 14:24:51.000000 SwissArmyTransformer-0.4.1/README.md
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.305028 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/
+-rw-rw-r--   0 dm        (2000) dm        (2000)     9893 2023-07-13 14:26:33.303612 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 dm        (2000) dm        (2000)     4934 2023-07-13 14:26:33.303909 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 dm        (2000) dm        (2000)        1 2023-07-13 14:26:33.304350 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 dm        (2000) dm        (2000)       90 2023-07-13 14:26:33.304731 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/requires.txt
+-rw-rw-r--   0 dm        (2000) dm        (2000)        4 2023-07-13 14:26:33.305118 SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/top_level.txt
+-rw-rw-r--   0 dm        (2000) dm        (2000)       89 2023-06-28 10:49:48.000000 SwissArmyTransformer-0.4.1/requirements.txt
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.306929 SwissArmyTransformer-0.4.1/sat/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      433 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/__init__.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    25746 2023-07-13 03:48:02.000000 SwissArmyTransformer-0.4.1/sat/arguments.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.310757 SwissArmyTransformer-0.4.1/sat/data_utils/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      288 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/data_utils/__init__.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    15633 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/data_utils/configure_data.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     2676 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/data_utils/datasets.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     1894 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/data_utils/hf_dataset.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     7028 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/data_utils/samplers.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     7129 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/data_utils/webds.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.313895 SwissArmyTransformer-0.4.1/sat/generation/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/__init__.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     9777 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/generation/autoregressive_sampling.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     3218 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/cuda2d_sampling.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     1709 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/magnify.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.316453 SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      161 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/__init__.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     4300 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/base_strategy.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     7659 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/beam_search_strategy.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     2270 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     3201 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/generation/utils.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     5187 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/helpers.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.319249 SwissArmyTransformer-0.4.1/sat/model/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      214 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/__init__.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.319954 SwissArmyTransformer-0.4.1/sat/model/attention/
+-rw-rw-r--   0 dm        (2000) dm        (2000)      110 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/attention/__init__.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     3654 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/attention/memory_efficient_attention.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    16317 2023-07-13 06:36:01.000000 SwissArmyTransformer-0.4.1/sat/model/base_model.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     1731 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/model/cached_autoregressive_model.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     5479 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/encoder_decoder_model.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.323231 SwissArmyTransformer-0.4.1/sat/model/finetune/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      187 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/__init__.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     2659 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/adapter.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     2019 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/ffadd.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     3879 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/lora.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)    12022 2023-07-13 06:36:01.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/lora2.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     1110 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/mlp_head.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     1611 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/model/finetune/prompt_tuning.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      391 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/mixins.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.323867 SwissArmyTransformer-0.4.1/sat/model/normalization/
+-rw-rw-r--   0 dm        (2000) dm        (2000)       24 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/model/normalization/__init__.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)      610 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/model/normalization/rms.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.339156 SwissArmyTransformer-0.4.1/sat/model/official/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      676 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/model/official/__init__.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     1923 2023-06-28 11:04:30.000000 SwissArmyTransformer-0.4.1/sat/model/official/bert_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)    10409 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/cait_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     7173 2023-07-13 14:01:04.000000 SwissArmyTransformer-0.4.1/sat/model/official/chatglm2_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)    11797 2023-07-13 14:01:05.000000 SwissArmyTransformer-0.4.1/sat/model/official/chatglm_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     7294 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/clip_model.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     9612 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/cuda2d_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     1310 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/distill_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     3942 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/dpr_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     7369 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/eva2_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)    13903 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/glm130B_model.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     3751 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/glm_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     3488 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/gpt2_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     4648 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/gptneo_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     5239 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/model/official/llama_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     8336 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/mae_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)      262 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/roberta_model.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    14715 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/t5_model.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     6254 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/vit_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     2969 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/official/yolos_model.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.342443 SwissArmyTransformer-0.4.1/sat/model/position_embedding/
+-rw-rw-r--   0 dm        (2000) dm        (2000)      296 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/position_embedding/__init__.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     5388 2023-07-13 07:20:14.000000 SwissArmyTransformer-0.4.1/sat/model/position_embedding/rotary_embeddings.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     2713 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/model/position_embedding/rotary_embeddings_original.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     4078 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/position_embedding/sincos2d.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     5021 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/model/position_embedding/vision_rotary_embeddings.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     1199 2023-07-13 06:36:01.000000 SwissArmyTransformer-0.4.1/sat/model/registry.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    29395 2023-07-13 12:51:21.000000 SwissArmyTransformer-0.4.1/sat/model/transformer.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.347753 SwissArmyTransformer-0.4.1/sat/mpu/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     2263 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/mpu/__init__.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     4716 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/mpu/cross_entropy.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     4018 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/mpu/data.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     6435 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/mpu/initialize.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    22165 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/mpu/layers.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     4136 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/mpu/mappings.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     3898 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/mpu/operation.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     3924 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/mpu/utils.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.350118 SwissArmyTransformer-0.4.1/sat/ops/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     1233 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/__init__.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.299962 SwissArmyTransformer-0.4.1/sat/ops/csrc/
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.351559 SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/
+-rw-rw-r--   0 dm        (2000) dm        (2000)      947 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp
+-rw-rw-r--   0 dm        (2000) dm        (2000)     5595 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/multi_tensor_apply.cuh
+-rw-rw-r--   0 dm        (2000) dm        (2000)     7076 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/multi_tensor_ema_adam.cu
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.352778 SwissArmyTransformer-0.4.1/sat/ops/csrc/includes/
+-rw-rw-r--   0 dm        (2000) dm        (2000)      336 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/csrc/includes/compat.h
+-rw-rw-r--   0 dm        (2000) dm        (2000)     6388 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/csrc/includes/type_shim.h
+-rw-rw-r--   0 dm        (2000) dm        (2000)    10712 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/fused_ema_adam.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     1159 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/layernorm.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     2067 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/local_attention_function.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)      578 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/memory_efficient_attention.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.354889 SwissArmyTransformer-0.4.1/sat/ops/ops_builder/
+-rw-rw-r--   0 dm        (2000) dm        (2000)     1982 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/ops_builder/__init__.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)    28554 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/ops_builder/builder.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)      957 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/ops_builder/fused_ema_adam.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)      389 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/ops/scaled_mask_softmax.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.355494 SwissArmyTransformer-0.4.1/sat/quantization/
+-rw-rw-r--   0 dm        (2000) dm        (2000)       29 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/quantization/__init__.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)    18674 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/quantization/kernels.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.357362 SwissArmyTransformer-0.4.1/sat/resources/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)       33 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/resources/__init__.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     6815 2023-07-11 08:40:38.000000 SwissArmyTransformer-0.4.1/sat/resources/download.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     3531 2023-07-13 06:36:01.000000 SwissArmyTransformer-0.4.1/sat/resources/urls.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.358024 SwissArmyTransformer-0.4.1/sat/tokenization/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     3810 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/__init__.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.361007 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      303 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/__init__.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     5092 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/sp_tokenizer.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     1767 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/templates.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     7095 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/unified_tokenizer.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.364101 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      167 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/__init__.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     7691 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/api.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    30392 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    12917 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/vqvae_zc.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     2453 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae_tokenizer.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.301044 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.369743 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/chinese_sentencepiece/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)  1021864 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
+-rwxrwxr-x   0 dm        (2000) dm        (2000)   723078 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.393180 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)   231508 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
+-rwxrwxr-x   0 dm        (2000) dm        (2000)   231508 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
+-rwxrwxr-x   0 dm        (2000) dm        (2000)   456318 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
+-rwxrwxr-x   0 dm        (2000) dm        (2000)  1042301 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
+-rwxrwxr-x   0 dm        (2000) dm        (2000)   456318 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
+-rwxrwxr-x   0 dm        (2000) dm        (2000)   898823 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.401770 SwissArmyTransformer-0.4.1/sat/tokenization/glm/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)       87 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/glm/__init__.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     3272 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/glm/sp_tokenizer.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    23223 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    13844 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization_gpt2.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)    14571 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization_wordpiece.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     3271 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/hf_tokenizer.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.404224 SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/
+-rw-rw-r--   0 dm        (2000) dm        (2000)       40 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/__init__.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     9661 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     2295 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/tokenizer.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.408078 SwissArmyTransformer-0.4.1/sat/training/
+-rwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/training/__init__.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    24074 2023-07-12 13:12:07.000000 SwissArmyTransformer-0.4.1/sat/training/deepspeed_training.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      392 2023-07-12 13:17:48.000000 SwissArmyTransformer-0.4.1/sat/training/deepspeed_zero0.json
+-rwxrwxr-x   0 dm        (2000) dm        (2000)      999 2023-07-12 13:17:55.000000 SwissArmyTransformer-0.4.1/sat/training/deepspeed_zero1.json
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     1151 2023-07-12 13:18:02.000000 SwissArmyTransformer-0.4.1/sat/training/deepspeed_zero2.json
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     3475 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/training/learning_rates.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)    11576 2023-07-05 08:12:32.000000 SwissArmyTransformer-0.4.1/sat/training/model_io.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     4488 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/sat/training/utils.py
+-rwxrwxr-x   0 dm        (2000) dm        (2000)     9663 2023-07-13 12:52:36.000000 SwissArmyTransformer-0.4.1/sat/transformer_defaults.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)       38 2023-07-13 14:26:33.417402 SwissArmyTransformer-0.4.1/setup.cfg
+-rw-rw-r--   0 dm        (2000) dm        (2000)      880 2023-07-13 14:21:56.000000 SwissArmyTransformer-0.4.1/setup.py
+drwxrwxr-x   0 dm        (2000) dm        (2000)        0 2023-07-13 14:26:33.415271 SwissArmyTransformer-0.4.1/tests/
+-rw-rw-r--   0 dm        (2000) dm        (2000)     2000 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_base_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     1530 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_inference.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)      290 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_list_info.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     3104 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_mea.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)      913 2023-06-28 16:44:01.000000 SwissArmyTransformer-0.4.1/tests/test_model_parallel.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     2134 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_nested_model.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)      611 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_speed.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     4078 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_train.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     4078 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_train_dp.py
+-rw-rw-r--   0 dm        (2000) dm        (2000)     4336 2023-06-28 10:46:39.000000 SwissArmyTransformer-0.4.1/tests/test_train_nested.py
```

### Comparing `SwissArmyTransformer-0.4.0/LICENSE` & `SwissArmyTransformer-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/PKG-INFO` & `SwissArmyTransformer-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.4.0
+Version: 0.4.1
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -174,15 +174,16 @@
         # ...
         return attention_results
 ```
 Here `attention_fn` is a hook function, replacing the default action by the new function. All available hooks are in [transformer_defaults.py](/sat/transformer_defaults.py). 
 Now we can use `add_mixin` to apply our change to all the transformers, such as BERT, Vit and CogView. See the tutorial for more details. 
 
 ## Tutorials 
-TO BE RELEASED SOON...
+* [How to use pretrained models collected in sat?](tutorials/model_usage)
+* [Why and how to train models in sat?](tutorials/training)
 
 # Citation
 Currently we don't have a paper, so you don't need to formally cite us!~ 
 
 If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/SwissArmyTransformer}` to mention us and recommend `SwissArmyTransformer` to others.
 
 The tutorial for contributing sat is on the way!
```

### Comparing `SwissArmyTransformer-0.4.0/README.md` & `SwissArmyTransformer-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,16 @@
         # ...
         return attention_results
 ```
 Here `attention_fn` is a hook function, replacing the default action by the new function. All available hooks are in [transformer_defaults.py](/sat/transformer_defaults.py). 
 Now we can use `add_mixin` to apply our change to all the transformers, such as BERT, Vit and CogView. See the tutorial for more details. 
 
 ## Tutorials 
-TO BE RELEASED SOON...
+* [How to use pretrained models collected in sat?](tutorials/model_usage)
+* [Why and how to train models in sat?](tutorials/training)
 
 # Citation
 Currently we don't have a paper, so you don't need to formally cite us!~ 
 
 If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/SwissArmyTransformer}` to mention us and recommend `SwissArmyTransformer` to others.
 
 The tutorial for contributing sat is on the way!
```

### Comparing `SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/PKG-INFO` & `SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.4.0
+Version: 0.4.1
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -174,15 +174,16 @@
         # ...
         return attention_results
 ```
 Here `attention_fn` is a hook function, replacing the default action by the new function. All available hooks are in [transformer_defaults.py](/sat/transformer_defaults.py). 
 Now we can use `add_mixin` to apply our change to all the transformers, such as BERT, Vit and CogView. See the tutorial for more details. 
 
 ## Tutorials 
-TO BE RELEASED SOON...
+* [How to use pretrained models collected in sat?](tutorials/model_usage)
+* [Why and how to train models in sat?](tutorials/training)
 
 # Citation
 Currently we don't have a paper, so you don't need to formally cite us!~ 
 
 If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/SwissArmyTransformer}` to mention us and recommend `SwissArmyTransformer` to others.
 
 The tutorial for contributing sat is on the way!
```

### Comparing `SwissArmyTransformer-0.4.0/SwissArmyTransformer.egg-info/SOURCES.txt` & `SwissArmyTransformer-0.4.1/SwissArmyTransformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/arguments.py` & `SwissArmyTransformer-0.4.1/sat/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,17 +369,19 @@
     if args.mode != 'inference': # training with deepspeed
         args.deepspeed = True
         if args.deepspeed_config is None: # not specified
             args.deepspeed_config = os.path.join(os.path.dirname(__file__), 'training', f'deepspeed_zero{args.zero_stage}.json')
             override_deepspeed_config = True
         else:
             override_deepspeed_config = False
-    if args.zero_stage > 0:
-        if args.rank == 0 and not args.fp16:
-            print_rank0('Automatically set fp16=True to use ZeRO.')     
+
+    assert not (args.fp16 and args.bf16), 'cannot specify both fp16 and bf16.'
+
+    if args.zero_stage > 0 and not args.fp16 and not args.bf16:
+        print_rank0('Automatically set fp16=True to use ZeRO.')     
         args.fp16 = True
         args.bf16 = False
 
     if args.deepspeed:
         if args.checkpoint_activations:
             args.deepspeed_activation_checkpointing = True
         else:
@@ -387,28 +389,35 @@
         if args.deepspeed_config is not None:
             with open(args.deepspeed_config) as file:
                 deepspeed_config = json.load(file)
             
         if override_deepspeed_config: # not specify deepspeed_config, use args
             if args.fp16:
                 deepspeed_config["fp16"]["enabled"] = True
+            elif args.bf16:
+                deepspeed_config["bf16"]["enabled"] = True
+                deepspeed_config["fp16"]["enabled"] = False
             else:
                 deepspeed_config["fp16"]["enabled"] = False
             deepspeed_config["train_micro_batch_size_per_gpu"] = args.batch_size
             deepspeed_config["gradient_accumulation_steps"] = args.gradient_accumulation_steps
             optimizer_params_config = deepspeed_config["optimizer"]["params"]
             optimizer_params_config["lr"] = args.lr
             optimizer_params_config["weight_decay"] = args.weight_decay
         else: # override args with values in deepspeed_config
             if args.rank == 0:
                 print_rank0('Will override arguments with manually specified deepspeed_config!')
             if "fp16" in deepspeed_config and deepspeed_config["fp16"]["enabled"]:
                 args.fp16 = True
             else:
                 args.fp16 = False
+            if "bf16" in deepspeed_config and deepspeed_config["bf16"]["enabled"]:
+                args.bf16 = True
+            else:
+                args.bf16 = False
             if "train_micro_batch_size_per_gpu" in deepspeed_config:
                 args.batch_size = deepspeed_config["train_micro_batch_size_per_gpu"]
             if "gradient_accumulation_steps" in deepspeed_config:
                 args.gradient_accumulation_steps = deepspeed_config["gradient_accumulation_steps"]
             else:
                 args.gradient_accumulation_steps = None
             if "optimizer" in deepspeed_config:
```

### Comparing `SwissArmyTransformer-0.4.0/sat/data_utils/configure_data.py` & `SwissArmyTransformer-0.4.1/sat/data_utils/configure_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         args.test_drop_number = 0
         return torch.utils.data.DataLoader(
             dataset,
             batch_size=batch_size//world_size,
             num_workers=args.num_workers,
             pin_memory=True,
             collate_fn=collate_fn,
-            prefetch_factor=args.prefetch_factor,
+            prefetch_factor=args.prefetch_factor if args.num_workers > 0 else None,
             )
 
     sampler = torch.utils.data.SequentialSampler(dataset)
     # drop_last = distributed
     drop_last = False # TODO will always drop last to keep the consistency.
     # or, how to avg in eval last batch?
 
@@ -87,15 +87,15 @@
         args.test_last_shape = last_shape
         args.test_drop_number = drop_number
     data_loader = torch.utils.data.DataLoader(dataset,
                                               batch_sampler=batch_sampler,
                                               num_workers=args.num_workers,
                                               pin_memory=True,
                                               collate_fn=collate_fn,
-                                              prefetch_factor=args.prefetch_factor,
+                                              prefetch_factor=args.prefetch_factor if args.num_workers > 0 else None,
                                               )
     return data_loader
 
 
 def make_dataset_full(path, split, args, create_dataset_function, 
         dataset_weights=None, random_mapping=True, is_train_data=False, **kwargs):
     """function to create datasets+tokenizers for common options"""
```

### Comparing `SwissArmyTransformer-0.4.0/sat/data_utils/datasets.py` & `SwissArmyTransformer-0.4.1/sat/data_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/data_utils/hf_dataset.py` & `SwissArmyTransformer-0.4.1/sat/data_utils/hf_dataset.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/data_utils/samplers.py` & `SwissArmyTransformer-0.4.1/sat/data_utils/samplers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/data_utils/webds.py` & `SwissArmyTransformer-0.4.1/sat/data_utils/webds.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/generation/autoregressive_sampling.py` & `SwissArmyTransformer-0.4.1/sat/generation/autoregressive_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/generation/cuda2d_sampling.py` & `SwissArmyTransformer-0.4.1/sat/generation/cuda2d_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/generation/magnify.py` & `SwissArmyTransformer-0.4.1/sat/generation/magnify.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/base_strategy.py` & `SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/base_strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # here put the import lib
 import os
 import sys
 import math
 import random
 import torch
 import torch.nn.functional as F
+from sat.mpu.initialize import get_model_parallel_world_size, get_model_parallel_src_rank, get_model_parallel_group
 
 def top_k_logits(logits, top_k=0, top_p=0.0, filter_value=-65504):
     # This function has been mostly taken from huggingface conversational ai code at
     # https://medium.com/huggingface/how-to-build-a-state-of-the-art-conversational-ai-with-transfer-learning-2d818ac26313
 
     if top_k > 0:
         # Remove all tokens with a probability less than the last token of the top-k
@@ -86,14 +87,16 @@
         logits = logits.float() / penalty_mat
 
         for invalid_slice in self.invalid_slices:
             logits[..., invalid_slice] = -65504
         logits = top_k_logits(logits, self.topk, self.top_p)
         probs = F.softmax(logits, dim=-1)  # float is essetial, due to a bug in Pytorch
         pred = torch.multinomial(probs, num_samples=1)
+        if get_model_parallel_world_size() > 1:
+            torch.distributed.broadcast(pred, get_model_parallel_src_rank(), group=get_model_parallel_group())
         if pred.numel() == 1 and pred.item() in self.end_tokens:
             self._is_done = True
         tokens = torch.cat((tokens, pred.view(tokens.shape[0], 1)), dim=1)
         return tokens, mems
 
     def finalize(self, tokens, mems):
         self._is_done = False
```

### Comparing `SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/beam_search_strategy.py` & `SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/beam_search_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 @Contact :   dm18@mails.tsinghua.edu.cn
 '''
 
 # here put the import lib
 import torch
 import torch.nn.functional as F
 from .base_strategy import top_k_logits
+from sat.mpu.initialize import get_model_parallel_world_size, get_model_parallel_src_rank, get_model_parallel_group
 
 class BeamSearchStrategy:
     def __init__(self, num_beams, length_penalty=1., 
                 temperature=1., top_k=0., top_p=0.0,
                 consider_end=True,
                 end_tokens=[], invalid_slices=[], no_repeat_ngram_size=0, 
                 min_tgt_length=0,
@@ -106,14 +107,16 @@
         next_token_scores = next_token_scores + prev_scores
         
         next_token_scores = next_token_scores.view(batch_size * vocab_size)
 
         probs = F.softmax(logits.view(batch_size * vocab_size), dim=0)
         next_tokens = torch.multinomial(probs, 
             num_samples=(max(1,len(self.end_tokens))+1) * self.num_beams) # [2*nb]
+        if get_model_parallel_world_size() > 1:
+            torch.distributed.broadcast(next_tokens, get_model_parallel_src_rank(), group=get_model_parallel_group())
         next_token_scores = next_token_scores[next_tokens]
         next_token_scores, _indices = torch.sort(next_token_scores, descending=True, dim=0)
         next_tokens = next_tokens[_indices]
 
         next_indices = torch.div(next_tokens, vocab_size, rounding_mode='trunc')
         next_tokens = next_tokens % vocab_size
```

### Comparing `SwissArmyTransformer-0.4.0/sat/generation/sampling_strategies/iterative_entfilter_strategy.py` & `SwissArmyTransformer-0.4.1/sat/generation/sampling_strategies/iterative_entfilter_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/generation/utils.py` & `SwissArmyTransformer-0.4.1/sat/generation/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/helpers.py` & `SwissArmyTransformer-0.4.1/sat/helpers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/attention/memory_efficient_attention.py` & `SwissArmyTransformer-0.4.1/sat/model/attention/memory_efficient_attention.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/base_model.py` & `SwissArmyTransformer-0.4.1/sat/model/base_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from sat.model.transformer import BaseTransformer, standard_attention
 from sat.arguments import update_args_with_file, overwrite_args_by_dict
 from sat.training.model_io import load_checkpoint
 from sat.helpers import print_rank0
 
 from sat.transformer_defaults import HOOKS_DEFAULT, ARGS_DEFAULT
 from sat.resources import auto_create
+from sat.mpu.initialize import get_node_rank, destroy_model_parallel, initialize_model_parallel
+from sat.mpu.operation import mp_split_model_rank0, mp_split_model_receive
 
 def non_conflict(func):
     '''mark a hook function as non-conflict,
     so that it can be compatible with any already defined hooks.
     e.g. PrefixTuningMixin.attention_fn
     '''
     func.non_conflict = True
@@ -177,15 +179,15 @@
 
     @classmethod
     def add_model_specific_args(cls, parser):
         # recorded in arguments.py: add_model_config_args
         return parser
 
     @classmethod
-    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, overwrite_args={}, **kwargs):
+    def from_pretrained_base(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, overwrite_args={}, **kwargs):
         '''Load a pretrained checkpoint of the current model.
             Args:
                 name: The identifier of the pretrained model.
                 args: NameSpace. will add the loaded args into it. None will create a new model-only one with defaults.
                 path: the parent folder of existing `name` model. Default: SAT_HOME.
                 url: the url of the model. Default: SAT_URL.
                 prefix: the prefix of the checkpoint. Default: ''.
@@ -204,14 +206,41 @@
         args = overwrite_args_by_dict(args, overwrite_args=overwrite_args)
         model = get_model(args, cls, **kwargs)
         if not build_only:
             load_checkpoint(model, args, load_path=model_path, prefix=prefix)
         return model, args
     
     @classmethod
+    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, overwrite_args={}, **kwargs):
+        if build_only or 'model_parallel_size' not in overwrite_args:
+            return cls.from_pretrained_base(name, args=args, home_path=home_path, url=url, prefix=prefix, build_only=build_only, overwrite_args=overwrite_args, **kwargs)
+        else:
+            new_model_parallel_size = overwrite_args['model_parallel_size']
+            model, model_args = cls.from_pretrained_base(name, args=args, home_path=home_path, url=url, prefix=prefix, build_only=True, overwrite_args=overwrite_args, **kwargs)
+            local_rank = get_node_rank()
+            world_size = torch.distributed.get_world_size()
+            assert world_size % new_model_parallel_size == 0, "world size should be a multiplier of new model_parallel_size."
+            destroy_model_parallel()
+            initialize_model_parallel(1)
+            if local_rank == 0:
+                args.use_gpu_initialization = False
+                args.device = 'cpu'
+                overwrite_args.pop('model_parallel_size')
+                model_full, args_ = cls.from_pretrained_base(name, args=args, home_path=home_path, url=url, prefix=prefix, build_only=False, overwrite_args=overwrite_args, **kwargs)
+            torch.distributed.barrier()
+            destroy_model_parallel()
+            initialize_model_parallel(new_model_parallel_size)
+            if local_rank == 0:
+                mp_split_model_rank0(model, model_full)
+                del model_full
+            else:
+                mp_split_model_receive(model)
+            return model, model_args
+    
+    @classmethod
     def list_avail_args(cls, print=True):
         '''List all available args of the current model.'''
         parser = argparse.ArgumentParser()
         from sat.arguments import add_model_config_args
         add_model_config_args(parser)
         # add args of the current model
         if hasattr(cls, 'add_model_specific_args'):
@@ -238,15 +267,15 @@
             else:
                 print_rank0(f'warning: Unknown arg {k} for class {cls.__name__}.', level='DEBUG')
                 setattr(args, k, v)
         return args
 
 class AutoModel():
     @classmethod
-    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, overwrite_args={}, **kwargs):
+    def from_pretrained_base(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, overwrite_args={}, **kwargs):
         '''Automatically find the class and instantiate it. Auto-download.
             Args:
                 name: The identifier of the pretrained model.
                 args: NameSpace. will add the loaded args into it.
                 path: the parent folder of existing `name` model. Default: SAT_HOME.
                 url: manually specified url for the `name` model.
         '''
@@ -271,14 +300,41 @@
                 if not hasattr(args, k):
                     setattr(args, k, v)
         model = get_model(args, model_cls, **kwargs)
         if not build_only:
             load_checkpoint(model, args, load_path=model_path, prefix=prefix)
         return model, args
     
+    @classmethod
+    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, overwrite_args={}, **kwargs):
+        if build_only or 'model_parallel_size' not in overwrite_args:
+            return cls.from_pretrained_base(name, args=args, home_path=home_path, url=url, prefix=prefix, build_only=build_only, overwrite_args=overwrite_args, **kwargs)
+        else:
+            new_model_parallel_size = overwrite_args['model_parallel_size']
+            model, model_args = cls.from_pretrained_base(name, args=args, home_path=home_path, url=url, prefix=prefix, build_only=True, overwrite_args=overwrite_args, **kwargs)
+            local_rank = get_node_rank()
+            world_size = torch.distributed.get_world_size()
+            assert world_size % new_model_parallel_size == 0, "world size should be a multiplier of new model_parallel_size."
+            destroy_model_parallel()
+            initialize_model_parallel(1)
+            if local_rank == 0:
+                args.use_gpu_initialization = False
+                args.device = 'cpu'
+                overwrite_args.pop('model_parallel_size')
+                model_full, args_ = cls.from_pretrained_base(name, args=args, home_path=home_path, url=url, prefix=prefix, build_only=False, overwrite_args=overwrite_args, **kwargs)
+            torch.distributed.barrier()
+            destroy_model_parallel()
+            initialize_model_parallel(new_model_parallel_size)
+            if local_rank == 0:
+                mp_split_model_rank0(model, model_full)
+                del model_full
+            else:
+                mp_split_model_receive(model)
+            return model, model_args
+    
 def get_model(args, model_cls, **kwargs):
     """Build the model."""
     import torch
     from sat.helpers import print_rank0,print_all
     from sat import mpu
 
     print_rank0(f'building {model_cls.__name__} model ...')
```

### Comparing `SwissArmyTransformer-0.4.0/sat/model/cached_autoregressive_model.py` & `SwissArmyTransformer-0.4.1/sat/model/cached_autoregressive_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/encoder_decoder_model.py` & `SwissArmyTransformer-0.4.1/sat/model/encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/finetune/adapter.py` & `SwissArmyTransformer-0.4.1/sat/model/finetune/adapter.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/finetune/ffadd.py` & `SwissArmyTransformer-0.4.1/sat/model/finetune/ffadd.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/finetune/lora.py` & `SwissArmyTransformer-0.4.1/sat/model/finetune/lora.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/finetune/mlp_head.py` & `SwissArmyTransformer-0.4.1/sat/model/finetune/mlp_head.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/finetune/prompt_tuning.py` & `SwissArmyTransformer-0.4.1/sat/model/finetune/prompt_tuning.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 # here put the import lib
 import os
 import sys
 import math
 import random
 import torch
 
-from sat.model.transformer import standard_attention
+from sat.transformer_defaults import attention_fn_default
 from sat.model.base_model import BaseModel, BaseMixin, non_conflict
 
 
 class PrefixTuningMixin(BaseMixin):
     def __init__(self, num_layers, hidden_size_per_attention_head, num_attention_heads, prefix_len):
         super().__init__()
         self.prefix = torch.nn.ParameterList([
             torch.nn.Parameter(torch.randn(2, num_attention_heads, prefix_len, hidden_size_per_attention_head)*0.01)
             for layer_id in range(num_layers)
         ])
         self.prefix_len = prefix_len
 
     @non_conflict
-    def attention_fn(self, q, k, v, mask, dropout_fn, old_impl=standard_attention, **kw_args):
+    def attention_fn(self, q, k, v, mask, dropout_fn, old_impl=attention_fn_default, **kw_args):
         prefix_k, prefix_v = self.prefix[kw_args['layer_id']]
 
         b, nh, seq_len, hidden_size = k.shape
         prefix_k = prefix_k.unsqueeze(0).expand(b, nh, -1, hidden_size)
         prefix_v = prefix_v.unsqueeze(0).expand(b, nh, -1, hidden_size)
 
         k = torch.cat((k, prefix_k), dim=2)
```

### Comparing `SwissArmyTransformer-0.4.0/sat/model/normalization/rms.py` & `SwissArmyTransformer-0.4.1/sat/model/normalization/rms.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/__init__.py` & `SwissArmyTransformer-0.4.1/sat/model/official/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/bert_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/bert_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/cait_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/cait_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/chatglm2_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/chatglm2_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import torch.nn.functional as F
 from sat.model.base_model import BaseMixin, BaseModel
 from sat.mpu.utils import split_tensor_along_last_dim
 
 from sat.model.normalization import RMSNorm
 from sat.transformer_defaults import attention_fn_default
 from sat.model.position_embedding.rotary_embeddings_original import RotaryEmbedding, apply_rotary_pos_emb
+from sat.mpu.layers import ColumnParallelLinear
 
 class ChatGLM2AttnMixin(BaseMixin):
     def __init__(self, hidden_size, num_heads, max_seq_len):
         super().__init__()
         rotary_dim = hidden_size // num_heads
         self.rotary_pos_emb = RotaryEmbedding(rotary_dim // 2, original_impl=True)
         self.max_seq_len = max_seq_len
@@ -57,15 +58,26 @@
         if self.training:
             output = self.output_dropout(output)
         return output
 
 class SwiGLUMixin(BaseMixin):
     def __init__(self, num_layers, in_features, hidden_features, bias=False):
         super().__init__()
-        self.w2 = nn.ModuleList([nn.Linear(in_features, hidden_features, bias=bias) for i in range(num_layers)])
+        self.w2 = nn.ModuleList([ColumnParallelLinear(
+            in_features,
+            hidden_features,
+            gather_output=False,
+            # init_method=init_method,
+            bias=bias,
+            # params_dtype=params_dtype,
+            module=self,
+            name="dense_h_to_4h_gate",
+            # skip_init=skip_init,
+            # device=device
+        ) for i in range(num_layers)])
 
     def mlp_forward(self, hidden_states, **kw_args):
         x = hidden_states
         origin = self.transformer.layers[kw_args['layer_id']].mlp
         x1 = origin.dense_h_to_4h(x)
         x2 = self.w2[kw_args['layer_id']](x)
         hidden = origin.activation_func(x1) * x2
@@ -83,32 +95,39 @@
         self.add_mixin("mlp", SwiGLUMixin(args.num_layers, args.hidden_size, args.inner_hidden_size, bias=args.use_bias))
 
     def position_embedding_forward(self, position_ids, output_cross_layer, **kw_args):
         return None
     
     def get_masks(self, input_ids, past_key_values, padding_mask=None):
         batch_size, seq_length = input_ids.shape
-        full_attention_mask = torch.ones(batch_size, seq_length, seq_length, device=input_ids.device)
+        full_attention_mask = torch.ones(batch_size, seq_length, seq_length, dtype=next(self.parameters()).dtype, device=input_ids.device)
         full_attention_mask.tril_()
         past_length = 0
         if past_key_values:
             past_length = past_key_values[0][0].shape[2]
         if past_length:
-            full_attention_mask = torch.cat((torch.ones(batch_size, seq_length, past_length,
+            full_attention_mask = torch.cat((torch.ones(batch_size, seq_length, past_length, dtype=next(self.parameters()).dtype,
                                                         device=input_ids.device), full_attention_mask), dim=-1)
         if padding_mask is not None:
             full_attention_mask = full_attention_mask * padding_mask.unsqueeze(1)
         if not past_length and padding_mask is not None:
             full_attention_mask -= padding_mask.unsqueeze(-1) - 1
         full_attention_mask = (full_attention_mask < 0.5).bool()
         full_attention_mask.unsqueeze_(1)
         return full_attention_mask
     
+    def get_position_ids(self, input_ids):
+        batch_size, seq_length = input_ids.shape
+        position_ids = torch.arange(seq_length, dtype=torch.long, device=input_ids.device).unsqueeze(0).repeat(batch_size, 1)
+        return position_ids
+    
     def forward(self, input_ids, position_ids=None, attention_mask=None, past_key_values=None, **kwargs):
-        if attention_mask.ndim == 4:
+        if position_ids is None:
+            position_ids = self.get_position_ids(input_ids)
+        if attention_mask is not None and attention_mask.ndim == 4:
             pass
         elif past_key_values is not None and input_ids.size(0) == 1:
             attention_mask = torch.tensor([[1]], dtype=torch.long, device=input_ids.device)
         else:
             attention_mask = self.get_masks(input_ids, past_key_values, padding_mask=attention_mask)
         if attention_mask is not None and attention_mask.dtype is torch.bool:
             attention_mask = ~attention_mask
```

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/chatglm_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/chatglm_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,78 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from sat.model.base_model import BaseMixin, BaseModel
 import math
 from sat import mpu
 from sat.mpu.utils import split_tensor_along_last_dim
+from sat.transformer_defaults import attention_fn_default
 
 @torch.jit.script
 def gelu_impl(x):
     """OpenAI's gelu implementation."""
     return 0.5 * x * (1.0 + torch.tanh(0.7978845608028654 * x *
                                        (1.0 + 0.044715 * x * x)))
 
 def gelu(x):
     return gelu_impl(x)
 
 from sat.model.position_embedding.rotary_embeddings import RotaryEmbedding, apply_rotary_pos_emb_index
+from sat.mpu.layers import ColumnParallelLinear
 
 class ChatGLMFinalMixin(BaseMixin):
     def __init__(self, vocab_size, hidden_size):
         super().__init__()
-        self.lm_head = nn.Linear(hidden_size, vocab_size, bias=False)
+        self.lm_head = ColumnParallelLinear(
+            hidden_size,
+            vocab_size,
+            gather_output=True,
+            # init_method=init_method,
+            bias=False,
+            # params_dtype=params_dtype,
+            module=self,
+            name="lm_head",
+            # skip_init=skip_init,
+            # device=device
+        )
 
     def final_forward(self, logits, **kwargs):
         return self.lm_head(logits)
 
 class ChatGLMAttnMixin(BaseMixin):
     def __init__(self, hidden_size, num_heads):
         super().__init__()
         self.rotary_emb = RotaryEmbedding(
             hidden_size // (num_heads * 2),
             base=10000,
             precision=torch.half,
             learnable=False,
         )
 
-    def attention_fn(self, query_layer, key_layer, value_layer, attention_mask,
-                        attention_dropout=None, log_attention_weights=None, scaling_attention_score=True, **kwargs):
-        # We disable the PB-relax-Attention and only changes the order of computation, because it is enough for most of training. 
-        # The implementation in the paper can be done very easily, if you really need it to train very deep transformers. 
-        query_key_layer_scaling_coeff = float(kwargs['layer_id'] + 1)
-        if scaling_attention_score:
-            query_layer = query_layer / (math.sqrt(query_layer.shape[-1]) * query_key_layer_scaling_coeff)
-        attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
-        dtype = attention_scores.dtype
-        if log_attention_weights is not None:
-            attention_scores += log_attention_weights
-
-        if not (attention_mask.shape[-2] == 1 and (attention_mask > 0).all()):
-            # if auto-regressive, skip
-            attention_scores = torch.mul(attention_scores, attention_mask) - \
-                            10000.0 * (1.0 - attention_mask)
-        attention_scores = attention_scores.float()
-        attention_scores = attention_scores * query_key_layer_scaling_coeff
-        attention_probs = F.softmax(attention_scores, dim=-1)
-        attention_probs = attention_probs.type(dtype)
-
-        if attention_dropout is not None:
-            if mpu.get_cuda_rng_tracker is not None:
-                with mpu.get_cuda_rng_tracker().fork():
-                    attention_probs = attention_dropout(attention_probs)
-            else:
-                attention_probs = attention_dropout(attention_probs)
-
-        context_layer = torch.matmul(attention_probs, value_layer)
-        return context_layer
-
     def attention_forward(self, hidden_states, mask, **kw_args):
         mixin_self = self
         position_ids = kw_args['position_ids']
         self = self.transformer.layers[kw_args['layer_id']].attention
-        attention_fn = self.hooks['attention_fn']
-
-        hidden_states = hidden_states.transpose(0, 1)
+        attention_fn = attention_fn_default
+        if 'attention_fn' in self.hooks:
+            attention_fn = self.hooks['attention_fn']
         mixed_raw_layer = self.query_key_value(hidden_states)
+        (mixed_query_layer,
+            mixed_key_layer,
+            mixed_value_layer) = split_tensor_along_last_dim(mixed_raw_layer, self.stride)
 
-        new_tensor_shape = mixed_raw_layer.size()[:-1] + (
-            self.num_attention_heads_per_partition,
-            3 * self.hidden_size_per_attention_head,
-        )
-        mixed_raw_layer = mixed_raw_layer.view(*new_tensor_shape)
+        dropout_fn = self.attention_dropout if self.training else None
 
-        # [seq_len, batch, num_attention_heads, hidden_size_per_attention_head]
-        (query_layer, key_layer, value_layer) = split_tensor_along_last_dim(mixed_raw_layer, 3)
+        query_layer = self._transpose_for_scores(mixed_query_layer)
+        key_layer = self._transpose_for_scores(mixed_key_layer)
+        value_layer = self._transpose_for_scores(mixed_value_layer)
+        
+        query_layer = query_layer.permute(2, 0, 1, 3)
+        key_layer = key_layer.permute(2, 0, 1, 3)
+        value_layer = value_layer.permute(2, 0, 1, 3)
 
         q1, q2 = query_layer.chunk(2, dim=(query_layer.ndim - 1))
         k1, k2 = key_layer.chunk(2, dim=(key_layer.ndim - 1))
         cos, sin = mixin_self.rotary_emb(q1, seq_len=position_ids.max() + 1)
         position_ids, block_position_ids = position_ids[:, 0, :].transpose(0, 1).contiguous(), \
             position_ids[:, 1, :].transpose(0, 1).contiguous()
         q1, k1 = apply_rotary_pos_emb_index(q1, k1, cos, sin, position_ids)
@@ -181,15 +167,15 @@
         super(ChatGLMModel, self).__init__(args, transformer=transformer, activation_func=gelu, **kwargs)
         self.add_mixin("chatglm-final", ChatGLMFinalMixin(args.vocab_size, args.hidden_size))
         self.add_mixin("chatglm-attn", ChatGLMAttnMixin(args.hidden_size, args.num_attention_heads))
         self.add_mixin("chatglm-layer", ChatGLMLayerMixin(args.num_layers))
         self.bos_token_id = args.bos_token_id
         self.mask_token_id = args.mask_token_id
         self.gmask_token_id = args.gmask_token_id
-        self.pad_token_id = 3
+        self.pad_token_id = args.pad_token_id
 
     def position_embedding_forward(self, position_ids, output_cross_layer, **kw_args):
         return None
     
     def forward(self, input_ids, position_ids=None, attention_mask=None, past_key_values=None, **kwargs):
         if attention_mask is None and position_ids is None:
             attention_mask, position_ids = self.get_inputs(input_ids, attention_mask=attention_mask, position_ids=position_ids, past_key_values=past_key_values, **kwargs)
@@ -230,15 +216,15 @@
         while l < len(seq) and seq[l] == self.pad_token_id:
             l += 1
         return l
     
     def get_masks(self, input_ids, device, **kwargs):
         batch_size, seq_length = input_ids.shape
         context_lengths = [seq.tolist().index(self.bos_token_id) for seq in input_ids]
-        attention_mask = torch.ones((batch_size, seq_length, seq_length), device=device)
+        attention_mask = torch.ones((batch_size, seq_length, seq_length), dtype=next(self.parameters()).dtype, device=device)
         attention_mask.tril_()
         for i, context_length in enumerate(context_lengths):
             attention_mask[i, :, :context_length] = 1
         pad_lengths = [self.get_pad_length(seq.tolist()) for seq in input_ids]
         for i, pad_length in enumerate(pad_lengths):
             attention_mask[i, :, :pad_length] = 0
             attention_mask[i, :pad_length, :] = 0
@@ -270,8 +256,9 @@
     
     @classmethod
     def add_model_specific_args(cls, parser):
         group = parser.add_argument_group('ChatGLM', 'ChatGLM Configurations')
         group.add_argument('--bos-token-id', type=int)
         group.add_argument('--mask-token-id', type=int)
         group.add_argument('--gmask-token-id', type=int)
-        return super().add_model_specific_args(parser)
+        group.add_argument('--pad-token-id', type=int)
+        return super().add_model_specific_args(parser)
```

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/clip_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/clip_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/cuda2d_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/cuda2d_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/distill_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/distill_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/dpr_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/dpr_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/eva2_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/eva2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/glm130B_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/glm130B_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/glm_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/glm_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/gpt2_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/gpt2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/gptneo_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/gptneo_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/llama_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/llama_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import torch.nn as nn
 
 from sat.model.official.gpt2_model import GPT2AttnMixin
 from sat.transformer_defaults import standard_attention
 from sat.mpu.utils import split_tensor_along_last_dim
 from sat.model.position_embedding.rotary_embeddings import RotaryEmbedding, rotate_half
 import torch.nn.functional as F
+from sat.mpu import ColumnParallelLinear
 
 def apply_rotary_pos_emb_index_bhs(q, k, cos, sin, position_id):
     # batch_size, num_head, seq_len, hidden_size
     cos, sin = F.embedding(position_id, cos.squeeze(1)).unsqueeze(1), \
                F.embedding(position_id, sin.squeeze(1)).unsqueeze(1)
     q, k = (q * cos) + (rotate_half(q) * sin), (k * cos) + (rotate_half(k) * sin)
     return q, k
@@ -56,26 +57,48 @@
             output = self.output_dropout(output)
         return output
 
 class LLaMAMlpMixin(BaseMixin):
     def __init__(self, num_layers, in_features, hidden_features):
         super().__init__()
         hidden_features = 4 * in_features if hidden_features is None else hidden_features
-        self.gate_proj = nn.ModuleList([nn.Linear(in_features, hidden_features, bias=False) for i in range(num_layers)])
+        self.gate_proj = nn.ModuleList([ColumnParallelLinear(
+            in_features,
+            hidden_features,
+            gather_output=False,
+            # init_method=init_method,
+            bias=False,
+            # params_dtype=params_dtype,
+            module=self,
+            name="dense_h_to_4h_gate",
+            # skip_init=skip_init,
+            # device=device
+        ) for i in range(num_layers)])
 
     def mlp_forward(self, hidden_states, **kw_args):
         origin = self.transformer.layers[kw_args['layer_id']].mlp
         hidden_states = origin.activation_func(self.gate_proj[kw_args['layer_id']](hidden_states)) * origin.dense_h_to_4h(hidden_states)
         hidden_states = origin.dense_4h_to_h(hidden_states)
         return hidden_states
 
 class LMMixin(BaseMixin):
     def __init__(self, vocab_size, hidden_size):
         super().__init__()
-        self.lm_head = nn.Linear(hidden_size, vocab_size, bias=False)
+        self.lm_head = ColumnParallelLinear(
+            hidden_size,
+            vocab_size,
+            gather_output=True,
+            # init_method=init_method,
+            bias=False,
+            # params_dtype=params_dtype,
+            module=self,
+            name="lm_head",
+            # skip_init=skip_init,
+            # device=device
+        )
 
     def final_forward(self, logits, **kwargs):
         return self.lm_head(logits)
 
 from sat.model.normalization import RMSNorm
 
 class LLaMAModel(BaseModel):
```

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/mae_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/mae_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/t5_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/t5_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/vit_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/vit_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/official/yolos_model.py` & `SwissArmyTransformer-0.4.1/sat/model/official/yolos_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/position_embedding/rotary_embeddings.py` & `SwissArmyTransformer-0.4.1/sat/model/position_embedding/rotary_embeddings.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,16 +34,16 @@
             emb = torch.cat((freqs, freqs), dim=-1).to(x.device)
             if self.precision == torch.bfloat16:
                 emb = emb.float()
 
             # [sx, 1 (b * np), hn]
             cos_cached = emb.cos()[:, None, :]
             sin_cached = emb.sin()[:, None, :]
-            cos_cached = cos_cached.to(self.precision)
-            sin_cached = sin_cached.to(self.precision)
+            cos_cached = cos_cached.to(x.dtype)
+            sin_cached = sin_cached.to(x.dtype)
             if self.learnable:
                 return cos_cached, sin_cached
             self.cos_cached, self.sin_cached = cos_cached, sin_cached
         return self.cos_cached[:seq_len, ...], self.sin_cached[:seq_len, ...]
 
 
 class RotaryPositionalEmbeddingFunction(torch.autograd.Function):
```

### Comparing `SwissArmyTransformer-0.4.0/sat/model/position_embedding/rotary_embeddings_original.py` & `SwissArmyTransformer-0.4.1/sat/model/position_embedding/rotary_embeddings_original.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/position_embedding/sincos2d.py` & `SwissArmyTransformer-0.4.1/sat/model/position_embedding/sincos2d.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/position_embedding/vision_rotary_embeddings.py` & `SwissArmyTransformer-0.4.1/sat/model/position_embedding/vision_rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/model/transformer.py` & `SwissArmyTransformer-0.4.1/sat/model/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self.hidden_size_per_partition = self.hidden_size_per_attention_head * self.num_attention_heads_per_partition
 
         # Strided linear layer.
         if num_multi_query_heads == 0:
             qkv_size = 3 * self.inner_hidden_size
             self.stride = 3
         else: # multi-query 
-            qkv_size = self.inner_hidden_size + self.hidden_size_per_attention_head * self.num_multi_query_heads_per_partition * 2 
+            qkv_size = self.inner_hidden_size + self.hidden_size_per_attention_head * self.num_multi_query_heads * 2 
             self.stride = [self.num_attention_heads_per_partition, self.num_multi_query_heads_per_partition, self.num_multi_query_heads_per_partition]
         self.query_key_value = ColumnParallelLinear(
             hidden_size,
             qkv_size,
             stride=self.stride,
             gather_output=False,
             init_method=init_method,
@@ -406,17 +406,20 @@
         self.layernorm_order = layernorm_order
         self.hooks = copy.copy(hooks)  # hooks will be updated each forward
         object.__setattr__(self, 'transformer', self) # to give the default hooks the same api as outer hooks
 
         # create embedding parameters
         self.embedding_dropout = torch.nn.Dropout(embedding_dropout_prob)
 
-        self.word_embeddings = VocabParallelEmbedding(
-            num_embeddings=vocab_size, embedding_dim=hidden_size, 
-            params_dtype=params_dtype, skip_init=skip_init, device=device)
+        if vocab_size < 1000:
+            self.word_embeddings = torch.nn.Embedding(vocab_size, hidden_size, dtype=params_dtype, device=device)
+        else:
+            self.word_embeddings = VocabParallelEmbedding(
+                num_embeddings=vocab_size, embedding_dim=hidden_size, 
+                params_dtype=params_dtype, skip_init=skip_init, device=device)
 
         self.position_embeddings = torch.nn.Embedding(max_sequence_length, hidden_size)
         torch.nn.init.normal_(self.position_embeddings.weight, mean=0.0, std=init_method_std)
 
         # create all layers
         if init_method is None:
             self.output_layer_init_method = scaled_init_method(init_method_std, num_layers)
@@ -462,17 +465,24 @@
     def forward(self, input_ids, position_ids, attention_mask, *,
                 output_hidden_states=False, **kw_args):
         # sanity check
         assert len(input_ids.shape) >= 2
         batch_size, query_length = input_ids.shape[:2]
 
         if attention_mask is None:
-            attention_mask = torch.ones(1, 1, device=input_ids.device).type_as(
+            # Definition: None means full attention
+            attention_mask = torch.ones(1, 1, device=input_ids.device)
+        elif isinstance(attention_mask, int) and (attention_mask < 0):
+            # Definition: -1 means lower triangular attention mask
+            attention_mask = torch.ones(query_length, query_length, 
+                                        device=input_ids.device).tril()
+            
+        attention_mask = attention_mask.type_as(
                 next(self.parameters())
-            )  # None means full attention
+            )
         assert len(attention_mask.shape) == 2 or \
                len(attention_mask.shape) == 4 and attention_mask.shape[1] == 1
 
         # initial output_cross_layer might be generated by word/position_embedding_forward
         output_cross_layer = {}
 
         # embedding part
@@ -517,15 +527,15 @@
                                 **kw_args, position_ids=position_ids, **output_cross_layer,
                                 output_this_layer=output_this_layer_obj,
                                 output_cross_layer=output_cross_layer_obj
                             )
                         else:
                             layer_ret = layer(
                                 x_, mask, layer_id=layer.layer_id,
-                                **kw_args, **output_cross_layer,
+                                **kw_args, position_ids=position_ids, **output_cross_layer,
                                 output_this_layer=output_this_layer_obj,
                                 output_cross_layer=output_cross_layer_obj
                             )
                         if isinstance(layer_ret, tuple):
                             layer_ret = layer_ret[0] # for legacy API
                         x_, output_this_layer, output_cross_layer = layer_ret, output_this_layer_obj, output_cross_layer_obj
                         if output_hidden_states:
```

### Comparing `SwissArmyTransformer-0.4.0/sat/mpu/__init__.py` & `SwissArmyTransformer-0.4.1/sat/mpu/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from .layers import VocabParallelEmbedding
 
 from .mappings import copy_to_model_parallel_region
 from .mappings import gather_from_model_parallel_region
 from .mappings import reduce_from_model_parallel_region
 from .mappings import scatter_to_model_parallel_region
 
-from .operation import mp_split_model
+from .operation import mp_split_model, mp_split_model_rank0, mp_split_model_receive
 
 try:
     import torch
     assert torch.cuda.is_available() # or set get_cuda_rng_tracker to None
     from deepspeed.runtime.activation_checkpointing.checkpointing import checkpoint, get_cuda_rng_tracker, model_parallel_cuda_manual_seed
 except Exception as e:
     from sat.helpers import print_rank0
```

### Comparing `SwissArmyTransformer-0.4.0/sat/mpu/cross_entropy.py` & `SwissArmyTransformer-0.4.1/sat/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/mpu/data.py` & `SwissArmyTransformer-0.4.1/sat/mpu/data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/mpu/initialize.py` & `SwissArmyTransformer-0.4.1/sat/mpu/initialize.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 from sat.helpers import print_rank0
 
 
 # Model parallel group that the current rank belongs to.
 _MODEL_PARALLEL_GROUP = None
 # Data parallel group that the current rank belongs to.
 _DATA_PARALLEL_GROUP = None
+# Node group that current rank belongs to.
+_NODE_GROUP = None
 
+import os
 
 def initialize_model_parallel(model_parallel_size_):
     """
     Initialize model data parallel groups.
 
     Arguments:
         model_parallel_size: number of GPUs used to parallelize model.
@@ -73,14 +76,28 @@
         'model parallel group is already initialized'
     for i in range(world_size // model_parallel_size):
         ranks = range(i * model_parallel_size,
                       (i + 1) * model_parallel_size)
         group = torch.distributed.new_group(ranks)
         if i == (rank // model_parallel_size):
             _MODEL_PARALLEL_GROUP = group
+    
+    local_world_size = os.environ.get('LOCAL_WORLD_SIZE', None)
+    if local_world_size is not None:
+        local_world_size = int(local_world_size)
+        # Build the node groups.
+        global _NODE_GROUP
+        assert _NODE_GROUP is None, \
+            'node group is already initialized'
+        for i in range(world_size // local_world_size):
+            ranks = range(i * local_world_size,
+                        (i + 1) * local_world_size)
+            group = torch.distributed.new_group(ranks)
+            if i == (rank // local_world_size):
+                _NODE_GROUP = group
 
 
 def model_parallel_is_initialized():
     """Check if model and data parallel groups are initialized."""
     if _MODEL_PARALLEL_GROUP is None or _DATA_PARALLEL_GROUP is None:
         return False
     return True
@@ -96,32 +113,57 @@
 def get_data_parallel_group():
     """Get the data parallel group the caller rank belongs to."""
     assert _DATA_PARALLEL_GROUP is not None, \
         'data parallel group is not initialized'
     return _DATA_PARALLEL_GROUP
 
 
+def get_node_group():
+    """Get the data parallel group the caller rank belongs to."""
+    assert _NODE_GROUP is not None, \
+        'node group is not initialized, please pass LOCAL_WORLD_SIZE environment variable.'
+    return _NODE_GROUP
+
+
 def get_model_parallel_world_size():
     """Return world size for the model parallel group."""
     return torch.distributed.get_world_size(group=get_model_parallel_group())
 
 
+def get_node_world_size():
+    """Return world size for the node group."""
+    return torch.distributed.get_world_size(group=get_node_group())
+
+
 def get_model_parallel_rank():
     """Return my rank for the model parallel group."""
     return torch.distributed.get_rank(group=get_model_parallel_group())
 
 
+def get_node_rank():
+    """Return my rank for the node group."""
+    return torch.distributed.get_rank(group=get_node_group())
+
+
 def get_model_parallel_src_rank():
     """Calculate the global rank corresponding to a local rank zero
     in the model parallel group."""
     global_rank = torch.distributed.get_rank()
     local_world_size = get_model_parallel_world_size()
     return (global_rank // local_world_size) * local_world_size
 
 
+def get_node_src_rank():
+    """Calculate the global rank corresponding to a local rank zero
+    in the node group."""
+    global_rank = torch.distributed.get_rank()
+    local_world_size = get_node_world_size()
+    return (global_rank // local_world_size) * local_world_size
+
+
 def get_data_parallel_world_size():
     """Return world size for the data parallel group."""
     return torch.distributed.get_world_size(group=get_data_parallel_group())
 
 
 def get_data_parallel_rank():
     """Return my rank for the data parallel group."""
@@ -130,7 +172,9 @@
 
 def destroy_model_parallel():
     """Set the groups to none."""
     global _MODEL_PARALLEL_GROUP
     _MODEL_PARALLEL_GROUP = None
     global _DATA_PARALLEL_GROUP
     _DATA_PARALLEL_GROUP = None
+    global _NODE_GROUP
+    _NODE_GROUP = None
```

### Comparing `SwissArmyTransformer-0.4.0/sat/mpu/layers.py` & `SwissArmyTransformer-0.4.1/sat/mpu/layers.py`

 * *Files 11% similar despite different names*

```diff
@@ -140,14 +140,32 @@
                                             self.vocab_start_index
         self.original_weight = self.weight
         self.weight = torch.nn.Parameter(torch.clone(
             self.weight[self.vocab_start_index:self.vocab_end_index],
             ).detach())
         del self.original_weight
 
+    def partition(self, new_model_parallel_size=None):
+        assert self.num_embeddings_per_partition == self.num_embeddings
+        if new_model_parallel_size is None:
+            new_model_parallel_size = get_model_parallel_world_size()
+        new_weights = []
+        for rank in range(new_model_parallel_size):
+            self.vocab_start_index, self.vocab_end_index = \
+                VocabUtility.vocab_range_from_global_vocab_size(
+                    self.num_embeddings, rank,
+                    new_model_parallel_size)
+            self.num_embeddings_per_partition = self.vocab_end_index - \
+                                                self.vocab_start_index
+            weight = torch.clone(
+                self.weight[self.vocab_start_index:self.vocab_end_index],
+                ).detach()
+            new_weights.append(weight)
+        return new_weights, []
+
 
 class ParallelEmbedding(torch.nn.Module):
     """Embedding parallelized in the embedding dimension.
 
     This is mainly adapted from torch.nn.Embedding and all the default
     values are kept.
     Arguments:
@@ -304,14 +322,56 @@
                     (strided_bias.shape[0]//mp_size)*(mp_rank+1)
                     ]
                 for strided_bias in strided_biases
             ], dim=0).contiguous().view(self.output_size_per_partition)
             self.bias = torch.nn.Parameter(new_bias)
             del self.original_bias
 
+    def partition(self, new_model_parallel_size=None):
+        assert self.output_size_per_partition == self.output_size
+        if new_model_parallel_size is None:
+            new_model_parallel_size = get_model_parallel_world_size()
+        output_size_per_partition = divide(self.output_size, new_model_parallel_size)
+        new_weights = []
+        new_biases = []
+        for rank in range(new_model_parallel_size):
+            mp_rank = rank
+            mp_size = new_model_parallel_size
+            # weight is arranged as [stride0...stride1...stride2] * [input_size], extract non-contiguous parts
+            strides = [1]*self.stride if isinstance(self.stride, int) else self.stride # int means equal number of qkv, or ratios
+            assert self.weight.shape[0] % sum(strides) == 0, 'cannot divide weight evenly'
+            factor = self.weight.shape[0] // sum(strides)
+            # decompose weight according to strides
+            strided_weights, _acm = [], 0
+            for i in range(len(strides)):
+                strided_weights.append(self.weight[_acm:_acm+factor*strides[i], :].detach())
+                _acm += factor*strides[i]
+            new_weight = torch.cat([
+                strided_weight[
+                    (strided_weight.shape[0]//mp_size)*mp_rank:
+                    (strided_weight.shape[0]//mp_size)*(mp_rank+1)
+                    ]
+                for strided_weight in strided_weights
+            ], dim=0).contiguous().view(output_size_per_partition, self.input_size)
+            new_weights.append(torch.clone(new_weight).detach())
+            if self.bias is not None:
+                # decompose bias according to strides
+                strided_biases, _acm = [], 0
+                for i in range(len(strides)):
+                    strided_biases.append(self.bias[_acm:_acm+factor*strides[i]].detach())
+                    _acm += factor*strides[i]
+                new_bias = torch.cat([
+                    strided_bias[
+                        (strided_bias.shape[0]//mp_size)*mp_rank:
+                        (strided_bias.shape[0]//mp_size)*(mp_rank+1)
+                        ]
+                    for strided_bias in strided_biases
+                ], dim=0).contiguous().view(output_size_per_partition)
+                new_biases.append(torch.clone(new_bias).detach())
+        return new_weights, new_biases
 
 class RowParallelLinear(torch.nn.Module):
     """Linear layer with row parallelism.
 
     The linear layer is defined as Y = XA + b. A is parallelized along
     its first dimension and X along its second dimension as:
                -   -
@@ -394,7 +454,25 @@
         mp_rank = get_model_parallel_rank()
         self.original_weight = self.weight
         self.weight = torch.nn.Parameter(torch.clone(
             self.weight[:, mp_rank*self.input_size_per_partition
                             :(mp_rank+1)*self.input_size_per_partition],
             ).detach())
         del self.original_weight
+
+    def partition(self, new_model_parallel_size=None):
+        assert self.input_size_per_partition == self.input_size
+        if new_model_parallel_size is None:
+            new_model_parallel_size = get_model_parallel_world_size()
+        input_size_per_partition = divide(self.input_size, new_model_parallel_size)
+        new_weights = []
+        new_biases = []
+        for rank in range(new_model_parallel_size):
+            mp_rank = rank
+            weight = torch.clone(
+                self.weight[:, mp_rank*input_size_per_partition
+                                :(mp_rank+1)*input_size_per_partition],
+                ).detach()
+            new_weights.append(weight)
+            if self.bias is not None:
+                new_biases.append(torch.clone(self.bias.data).detach())
+        return new_weights, new_biases
```

### Comparing `SwissArmyTransformer-0.4.0/sat/mpu/mappings.py` & `SwissArmyTransformer-0.4.1/sat/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/mpu/utils.py` & `SwissArmyTransformer-0.4.1/sat/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/__init__.py` & `SwissArmyTransformer-0.4.1/sat/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp` & `SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/multi_tensor_apply.cuh` & `SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/csrc/adam/multi_tensor_ema_adam.cu` & `SwissArmyTransformer-0.4.1/sat/ops/csrc/adam/multi_tensor_ema_adam.cu`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/csrc/includes/type_shim.h` & `SwissArmyTransformer-0.4.1/sat/ops/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/fused_ema_adam.py` & `SwissArmyTransformer-0.4.1/sat/ops/fused_ema_adam.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/layernorm.py` & `SwissArmyTransformer-0.4.1/sat/ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/local_attention_function.py` & `SwissArmyTransformer-0.4.1/sat/ops/local_attention_function.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/memory_efficient_attention.py` & `SwissArmyTransformer-0.4.1/sat/ops/memory_efficient_attention.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/ops_builder/__init__.py` & `SwissArmyTransformer-0.4.1/sat/ops/ops_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/ops_builder/builder.py` & `SwissArmyTransformer-0.4.1/sat/ops/ops_builder/builder.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/ops/ops_builder/fused_ema_adam.py` & `SwissArmyTransformer-0.4.1/sat/ops/ops_builder/fused_ema_adam.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/quantization/kernels.py` & `SwissArmyTransformer-0.4.1/sat/quantization/kernels.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/resources/download.py` & `SwissArmyTransformer-0.4.1/sat/resources/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,18 @@
                     pbar.update(len(chunk))
 
 def auto_create(name, *, path=None, url=None):
     if path is None:
         path = os.getenv('SAT_HOME', '~/.sat_models') # TODO Rename
     path = os.path.expanduser(path)
     model_path = os.path.join(path, name)
+    if url == 'local':
+        return model_path
     os.makedirs(os.path.dirname(model_path), exist_ok=True)
-    lock = FileLock(model_path + '.lock')
+    lock = FileLock(model_path + '.lock', mode=0o777)
     with lock:
         if url is None:
             url = MODEL_URLS[name]
         if os.path.isdir(model_path) and not url.startswith('r2://'):
             pass
         elif os.path.isdir(model_path) and url.startswith('r2://') and url.endswith('.zip'):
             pass
```

### Comparing `SwissArmyTransformer-0.4.0/sat/resources/urls.py` & `SwissArmyTransformer-0.4.1/sat/resources/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 MODEL_URLS = {
-    'bert-base-uncased': 'https://cloud.tsinghua.edu.cn/f/f45fff1a308846cfa63a/?dl=1',
-    'bert-large-uncased': 'https://cloud.tsinghua.edu.cn/f/6d4f38c96e8c4c16917e/?dl=1',
-    'roberta-base': 'https://cloud.tsinghua.edu.cn/f/307fd141932440bc92da/?dl=1',
-    'roberta-large': 'https://cloud.tsinghua.edu.cn/f/66c42c24ca304cecaf7e/?dl=1',
-    'vit-base-patch16-224-in21k': 'https://cloud.tsinghua.edu.cn/f/fdf40233d9034b6a8bdc/?dl=1',
-    'deit-tiny': 'https://cloud.tsinghua.edu.cn/f/b759657cb80e4bc69303/?dl=1',
-    'deit-small': 'https://cloud.tsinghua.edu.cn/f/51498210e2c943dbbef1/?dl=1',
-    'deit-base': 'https://cloud.tsinghua.edu.cn/f/9a26fd1aee7146e1a848/?dl=1',
-    'cait-s24-224': 'https://cloud.tsinghua.edu.cn/f/bdfb12396000468b8bb9/?dl=1',
-    'gpt2': 'https://cloud.tsinghua.edu.cn/f/4448cff2f1644bd88fa9/?dl=1',
-    'chatglm-6b': 'https://cloud.tsinghua.edu.cn/f/26587ca6dd6f45f1ae85/?dl=1',
+    'bert-base-uncased': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fbert-base-uncased.zip&dl=1',
+    'bert-large-uncased': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fbert-large-uncased.zip&dl=1',
+    'roberta-base': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Froberta-base.zip&dl=1',
+    'roberta-large': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Froberta-large.zip&dl=1',
+    'vit-base-patch16-224-in21k': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fvit-base-patch16-224-in21k.zip&dl=1',
+    'deit-tiny': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fdeit-tiny.zip&dl=1',
+    'deit-small': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fdeit-small.zip&dl=1',
+    'deit-base': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fdeit-base.zip&dl=1',
+    'cait-s24-224': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fcait-s24-224.zip&dl=1',
+    'gpt2': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fgpt2.zip&dl=1',
+    'chatglm-6b': 'r2://chatglm-6b.zip',
     'chatglm2-6b': 'r2://chatglm2-6b.zip',
-    'eva02_L_pt_m38m_p14': 'https://cloud.tsinghua.edu.cn/f/98feef10af4f4ff79764/?dl=1',
-    'llama-7b': 'https://cloud.tsinghua.edu.cn/f/8b5c193342c842988357/?dl=1',
-    'llama-13b': 'https://cloud.tsinghua.edu.cn/f/8a9bc9a95d8d40d9a971/?dl=1',
-    # CLIP
-    'clip': 'https://cloud.tsinghua.edu.cn/f/bd29f0537f9949e6a4fb/?dl=1', # vit-base-patch32
+    'eva02_L_pt_m38m_p14': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Feva02_L_pt_m38m_p14.zip&dl=1',
+    'llama-7b': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fllama-7b.zip&dl=1',
+    'llama-13b': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fllama-13b.zip&dl=1',
+    'llama-30b': 'r2://llama-30b',
+    'llama-65b': 'r2://llama-65b',
+    'clip': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fclip.zip&dl=1',
     'clip-vit-base-patch16': 'https://lfs.aminer.cn/misc/clip/clip-vit-base-patch16.zip',
     'clip-vit-large-patch14': 'https://lfs.aminer.cn/misc/clip/clip-vit-large-patch14.zip',
-    'yolos-tiny': 'https://cloud.tsinghua.edu.cn/f/8ee048b6a1f1403d9253/?dl=1',
-    'mae-vit-base': 'https://cloud.tsinghua.edu.cn/f/5ab3543f0e1d4507ad8c/?dl=1',
+    'yolos-tiny': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fyolos-tiny.zip&dl=1',
+    'mae-vit-base': 'https://cloud.tsinghua.edu.cn/d/dd80f9d39d454bc29ce4/files/?p=%2Fmae-vit-base.zip&dl=1',
+
     'cogview-base': 'https://cloud.tsinghua.edu.cn/f/df21f6d4109b4285bfd9/?dl=1',
     'glm-large-zh': 'https://lfs.aminer.cn/misc/cogview/glm/glm-large-zh.zip',
     'glm-large-en-blank': 'https://lfs.aminer.cn/misc/cogview/glm/glm-large-en-blank.zip',
     'glm-10b-en': 'https://lfs.aminer.cn/misc/cogview/glm/glm-10b-en.zip',
     'glm-10b-zh': 'https://lfs.aminer.cn/misc/cogview/glm/glm-10b-zh.zip',
     # 'glm-large-zh': 'https://cloud.tsinghua.edu.cn/f/df21f6d4109b4285bfd9/?dl=1',
     # 'glm-large-en-blank': 'https://cloud.tsinghua.edu.cn/f/df21f6d4109b4285bfd9/?dl=1',
```

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/__init__.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/sp_tokenizer.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/templates.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/templates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/unified_tokenizer.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/unified_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/api.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/api.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/vqvae_diffusion.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/vqvae_diffusion.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae/vqvae_zc.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae/vqvae_zc.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/cogview/vqvae_tokenizer.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/cogview/vqvae_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model` & `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab` & `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt` & `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt` & `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt` & `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json` & `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt` & `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json` & `SwissArmyTransformer-0.4.1/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/glm/sp_tokenizer.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/glm/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization_gpt2.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/glm/tokenization_wordpiece.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/glm/tokenization_wordpiece.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/hf_tokenizer.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/ice_tokenizer.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/ice_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/tokenization/icetk_glm_130B/tokenizer.py` & `SwissArmyTransformer-0.4.1/sat/tokenization/icetk_glm_130B/tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/training/deepspeed_training.py` & `SwissArmyTransformer-0.4.1/sat/training/deepspeed_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -525,14 +525,16 @@
     log_string += ' learning rate {:.3E} |'.format(lr)
     log_string += ' total loss {:.6E} |'.format(loss)
     for key in avg_metrics:
         log_string += ' {} {:.6E} |'.format(key, avg_metrics[key])
     if args.fp16:
         log_string += ' loss scale {:.1f} |'.format(
             optimizer.cur_scale if args.deepspeed else optimizer.loss_scale)
+    log_string += 'speed {:.2f} samples/(min*GPU)'.format(
+        (args.gradient_accumulation_steps * args.batch_size / args.model_parallel_size / (elapsed_time / 60000.0)))
     print_rank0(log_string)
     if summary_writer is not None:
         summary_writer.add_scalar(f'Train/lr', lr, step)
         summary_writer.add_scalar(f'Train/train_loss', loss, step)
         summary_writer.add_scalar(f'Train/elapsed_time', elapsed_time, step)
         for key in avg_metrics:
             summary_writer.add_scalar('Train/'+key, avg_metrics[key], step)
```

### Comparing `SwissArmyTransformer-0.4.0/sat/training/deepspeed_zero1.json` & `SwissArmyTransformer-0.4.1/sat/training/deepspeed_zero2.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7152777777777777%*

 * *Differences: {"'activation_checkpointing'": "{'cpu_checkpointing': False}",*

 * * "'bf16'": "OrderedDict([('enabled', False)])",*

 * * "'offload_optimizer'": "OrderedDict([('device', 'cpu'), ('pin_memory', True)])",*

 * * "'steps_per_print'": '1',*

 * * "'zero_optimization'": "{'stage': 2, 'overlap_comm': True, 'reduce_scatter': True, "*

 * *                        "'reduce_bucket_size': 40000000.0, 'allgather_bucket_size': 100000000.0, "*

 * *                        "'round_robin_gradients': False, delete: ['cpu_offload']}"}*

```diff
@@ -1,40 +1,49 @@
 {
     "activation_checkpointing": {
         "contiguous_memory_optimization": false,
+        "cpu_checkpointing": false,
         "partition_activations": false
     },
+    "bf16": {
+        "enabled": false
+    },
     "fp16": {
         "enabled": true,
         "hysteresis": 2,
         "loss_scale": 0,
         "loss_scale_window": 400,
         "min_loss_scale": 1
     },
     "gradient_accumulation_steps": 1,
     "gradient_clipping": 0.1,
+    "offload_optimizer": {
+        "device": "cpu",
+        "pin_memory": true
+    },
     "optimizer": {
         "params": {
             "betas": [
                 0.9,
                 0.95
             ],
             "eps": 1e-08,
             "lr": 0.0002,
             "weight_decay": 0.0001
         },
         "type": "Adam"
     },
+    "steps_per_print": 1,
     "train_micro_batch_size_per_gpu": 1,
     "wall_clock_breakdown": false,
     "zero_allow_untested_optimizer": true,
     "zero_optimization": {
-        "allgather_bucket_size": 1000000000,
+        "allgather_bucket_size": 100000000.0,
         "contiguous_gradients": false,
-        "cpu_offload": false,
         "load_from_fp32_weights": false,
-        "overlap_comm": false,
-        "reduce_bucket_size": 100000000,
-        "reduce_scatter": false,
-        "stage": 1
+        "overlap_comm": true,
+        "reduce_bucket_size": 40000000.0,
+        "reduce_scatter": true,
+        "round_robin_gradients": false,
+        "stage": 2
     }
 }
```

### Comparing `SwissArmyTransformer-0.4.0/sat/training/learning_rates.py` & `SwissArmyTransformer-0.4.1/sat/training/learning_rates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/training/model_io.py` & `SwissArmyTransformer-0.4.1/sat/training/model_io.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/training/utils.py` & `SwissArmyTransformer-0.4.1/sat/training/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/sat/transformer_defaults.py` & `SwissArmyTransformer-0.4.1/sat/transformer_defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,22 +48,25 @@
     # expand head dim to query dim, if necessary
     # only useful for multi-query attention
     batch_size, num_query_heads = query_layer.shape[:2] # [b, np, s, hn]
     num_kv_heads = key_layer.shape[1] # [b, np, s, hn]
     key_layer = key_layer.unsqueeze(2).expand(-1, -1, num_query_heads//num_kv_heads, -1, -1).contiguous().view(batch_size, num_query_heads, *key_layer.shape[2:])
     value_layer = value_layer.unsqueeze(2).expand(-1, -1, num_query_heads//num_kv_heads, -1, -1).contiguous().view(batch_size, num_query_heads, *value_layer.shape[2:])
 
-    if int(torch.__version__.split('.')[0]) >= 2:
-        assert scaling_attention_score == True
+    is_low_triangle = (attention_mask == torch.ones_like(attention_mask, dtype=torch.float).tril()).all()
+    is_full = (attention_mask is None) or (attention_mask > 0).all()
+
+    if int(torch.__version__.split('.')[0]) >= 2 and scaling_attention_score and (is_full or is_low_triangle):
+        # Pytorch 2.0 attention uses very much memory if attention_mask is float, and has NaN bug if attention_mask is None.
         dropout_p = 0. if attention_dropout is None or not attention_dropout.training else attention_dropout.p
-        attention_mask = (attention_mask >= 0.5).bool()
         return torch.nn.functional.scaled_dot_product_attention(
             query_layer, key_layer, value_layer, 
-            attention_mask,
-            dropout_p
+            attn_mask=None,
+            dropout_p=dropout_p,
+            is_causal=is_low_triangle.item()
         )
     else:
         return standard_attention(
             query_layer, key_layer, value_layer, attention_mask,
             attention_dropout=attention_dropout, log_attention_weights=log_attention_weights,
             scaling_attention_score=scaling_attention_score, **kwargs
         )
```

### Comparing `SwissArmyTransformer-0.4.0/setup.py` & `SwissArmyTransformer-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def _requirements():
     return Path("requirements.txt").read_text()
 
 setup(
     name="SwissArmyTransformer",
-    version='0.4.0',
+    version='0.4.1',
     description="A transformer-based framework with finetuning as the first class citizen.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=_requirements(),
     entry_points={},
     packages=find_packages(),
     url="https://github.com/THUDM/SwissArmyTransformer",
```

### Comparing `SwissArmyTransformer-0.4.0/tests/test_base_model.py` & `SwissArmyTransformer-0.4.1/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/tests/test_inference.py` & `SwissArmyTransformer-0.4.1/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/tests/test_mea.py` & `SwissArmyTransformer-0.4.1/tests/test_mea.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/tests/test_model_parallel.py` & `SwissArmyTransformer-0.4.1/tests/test_model_parallel.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/tests/test_nested_model.py` & `SwissArmyTransformer-0.4.1/tests/test_nested_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/tests/test_speed.py` & `SwissArmyTransformer-0.4.1/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/tests/test_train.py` & `SwissArmyTransformer-0.4.1/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/tests/test_train_dp.py` & `SwissArmyTransformer-0.4.1/tests/test_train_dp.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.0/tests/test_train_nested.py` & `SwissArmyTransformer-0.4.1/tests/test_train_nested.py`

 * *Files identical despite different names*

