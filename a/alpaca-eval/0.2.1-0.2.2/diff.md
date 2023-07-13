# Comparing `tmp/alpaca_eval-0.2.1.tar.gz` & `tmp/alpaca_eval-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.2.1.tar", last modified: Tue Jul 11 01:19:06 2023, max compression
+gzip compressed data, was "alpaca_eval-0.2.2.tar", last modified: Thu Jul 13 13:08:58 2023, max compression
```

## Comparing `alpaca_eval-0.2.1.tar` & `alpaca_eval-0.2.2.tar`

### file list

```diff
@@ -1,207 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    66370 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    65548 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.911748 alpaca_eval-0.2.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/example/outputs.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.907747 alpaca_eval-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 01:18:53.000000 alpaca_eval-0.2.1/src/alpaca_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/annotators/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34017 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/test/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/test/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.907747 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.911748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/airoboros-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/airoboros-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/baize-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/baize-v2-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/cohere/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/cohere/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/cohere-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/minotaur-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-v2-w-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat8192-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/opencoderplus-15b/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/ultralm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    66370 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/tests/test_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/tests/test_decoders_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/tests/test_pairwise_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    66370 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    65548 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.437964 alpaca_eval-0.2.2/example/
+-rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/example/outputs.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.425964 alpaca_eval-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.441964 alpaca_eval-0.2.2/src/alpaca_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 13:08:38.000000 alpaca_eval-0.2.2/src/alpaca_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.445964 alpaca_eval-0.2.2/src/alpaca_eval/annotators/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23087 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/annotators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.445964 alpaca_eval-0.2.2/src/alpaca_eval/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.445964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.445964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.445964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.449964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.449964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.449964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/test/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.429964 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.437964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/baize-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/baize-v2-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/claude-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/claude-2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/cohere-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-v2-w-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat8192-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/opencoderplus-15b/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/ultralm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.441964 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    66370 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/tests/test_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/tests/test_decoders_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.2.1/LICENSE` & `alpaca_eval-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/PKG-INFO` & `alpaca_eval-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.2.1
+Version: 0.2.2
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.1 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.2 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
```

### Comparing `alpaca_eval-0.2.1/README.md` & `alpaca_eval-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/example/outputs.json` & `alpaca_eval-0.2.2/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/setup.py` & `alpaca_eval-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     name="alpaca_eval",
     version=version,
     description="AlpacaEval : An Automatic Evaluator of Instruction-following Models",
     package_dir={"": "src"},
     packages=setuptools.find_packages("src"),
     author="The Alpaca Team",
     install_requires=[
+        "python-dotenv",
         "datasets",
         "openai",
         "pandas",
         "tiktoken>=0.3.2",
         "fire",
     ],
     extras_require={
```

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/analyze.py` & `alpaca_eval-0.2.2/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.2.2/src/alpaca_eval/completion_parsers.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/constants.py` & `alpaca_eval-0.2.2/src/alpaca_eval/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 CURRENT_DIR = Path(__file__).parent
 EVALUATORS_CONFIG_DIR = CURRENT_DIR / "evaluators_configs"
 MODELS_CONFIG_DIR = CURRENT_DIR / "models_configs"
 
 MINIMAL_MODELS = (
     "gpt4",
     "claude",
+    "claude-2",
     "chatgpt",
     "wizardlm-13b",
     "vicuna-13b",
     "guanaco-65b",
     "oasst-rlhf-llama-33b",
     "text_davinci_003",
     "alpaca-farm-ppo-human",
```

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.2.2/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.2.2/src/alpaca_eval/decoders/anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,14 @@
 
     return completion
 
 
 def _get_price_per_token(model):
     """Returns the price per token for a given model"""
     # https://cdn2.assets-servd.host/anthropic-website/production/images/model_pricing_may2023.pdf
-    if "claude-v1" in model:
+    if "claude-v1" in model or "claude-2" in model:
         return (
             11.02 / 1e6
         )  # that's not completely true because decoding is 32.68 but close enough given that most is context
     else:
         logging.warning(f"Unknown model {model} for computing price per token.")
         return np.nan
```

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.2.2/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.2.2/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.2.2/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.2.2/src/alpaca_eval/decoders/openai.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base
 gpt4,95.27950310559004,0.716281440286153,minimal,12,805,761,32
+claude-2,91.35572139303483,0.9897323784630048,minimal,1,804,734,69
 vicuna-33b-v1.3,88.99253731343283,1.095692216068168,verified,5,804,713,86
 claude,88.38509316770187,1.1144875403283188,minimal,9,805,707,89
 openchat-v2-w-13b,87.1268656716418,1.1769197439396015,community,3,804,699,102
 wizardlm-13b-v1.1,86.31840796019901,1.2063217831272972,community,4,804,692,108
 chatgpt,86.08695652173914,1.2110077772660273,minimal,6,805,690,109
 openchat-v2-13b,84.96894409937889,1.2572979835605944,community,2,805,683,120
 vicuna-13b-v1.3,82.11180124223603,1.348769957803504,verified,2,805,660,143
```

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv` & `alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/main.py` & `alpaca_eval-0.2.2/src/alpaca_eval/main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/metrics.py` & `alpaca_eval-0.2.2/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/plotting.py` & `alpaca_eval-0.2.2/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval/utils.py` & `alpaca_eval-0.2.2/src/alpaca_eval/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.2.2/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-eval
-Version: 0.2.1
+Version: 0.2.2
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.1 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.2 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
```

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.2.2/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/alpaca_eval.egg-info/PKG-INFO
 src/alpaca_eval.egg-info/SOURCES.txt
 src/alpaca_eval.egg-info/dependency_links.txt
 src/alpaca_eval.egg-info/entry_points.txt
 src/alpaca_eval.egg-info/requires.txt
 src/alpaca_eval.egg-info/top_level.txt
 src/alpaca_eval/annotators/__init__.py
+src/alpaca_eval/annotators/base.py
 src/alpaca_eval/annotators/pairwise_evaluator.py
 src/alpaca_eval/decoders/__init__.py
 src/alpaca_eval/decoders/anthropic.py
 src/alpaca_eval/decoders/cohere.py
 src/alpaca_eval/decoders/huggingface_api.py
 src/alpaca_eval/decoders/huggingface_local.py
 src/alpaca_eval/decoders/openai.py
@@ -50,14 +51,15 @@
 src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
 src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
 src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
 src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
 src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
 src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
 src/alpaca_eval/evaluators_configs/claude/configs.yaml
+src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
 src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
 src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
 src/alpaca_eval/evaluators_configs/cohere/configs.yaml
 src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
 src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
 src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
 src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
@@ -83,14 +85,15 @@
 src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
 src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
 src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
 src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
 src/alpaca_eval/models_configs/chatgpt/configs.yaml
 src/alpaca_eval/models_configs/claude/configs.yaml
 src/alpaca_eval/models_configs/claude/prompt.txt
+src/alpaca_eval/models_configs/claude-2/configs.yaml
 src/alpaca_eval/models_configs/cohere/configs.yaml
 src/alpaca_eval/models_configs/cohere/prompt.txt
 src/alpaca_eval/models_configs/cohere-chat/configs.yaml
 src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
 src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
 src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
 src/alpaca_eval/models_configs/gpt4/configs.yaml
```

### Comparing `alpaca_eval-0.2.1/src/alpaca_eval.egg-info/requires.txt` & `alpaca_eval-0.2.2/src/alpaca_eval.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+python-dotenv
 datasets
 openai
 pandas
 tiktoken>=0.3.2
 fire
 
 [all]
```

### Comparing `alpaca_eval-0.2.1/tests/test_analyze.py` & `alpaca_eval-0.2.2/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/tests/test_decoders_unit.py` & `alpaca_eval-0.2.2/tests/test_decoders_unit.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/tests/test_main.py` & `alpaca_eval-0.2.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.1/tests/test_pairwise_evaluator.py` & `alpaca_eval-0.2.2/tests/test_pairwise_evaluator.py`

 * *Files identical despite different names*

