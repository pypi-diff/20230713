# Comparing `tmp/db-gpt-0.2.8.tar.gz` & `tmp/db-gpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db-gpt-0.2.8.tar", last modified: Tue Jul 11 07:35:39 2023, max compression
+gzip compressed data, was "db-gpt-0.3.0.tar", last modified: Thu Jul 13 11:38:22 2023, max compression
```

## Comparing `db-gpt-0.2.8.tar` & `db-gpt-0.3.0.tar`

### file list

```diff
@@ -1,248 +1,248 @@
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.614894 db-gpt-0.2.8/
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.469304 db-gpt-0.2.8/DB_GPT.egg-info/
--rw-r--r--   0 chenketing   (502) staff       (20)     8144 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/PKG-INFO
--rw-r--r--   0 chenketing   (502) staff       (20)     6845 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/SOURCES.txt
--rw-r--r--   0 chenketing   (502) staff       (20)        1 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/dependency_links.txt
--rw-r--r--   0 chenketing   (502) staff       (20)       56 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/entry_points.txt
--rw-r--r--   0 chenketing   (502) staff       (20)     1155 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/requires.txt
--rw-r--r--   0 chenketing   (502) staff       (20)       12 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/top_level.txt
--rw-r--r--   0 chenketing   (502) staff       (20)     1067 2023-06-20 09:57:25.000000 db-gpt-0.2.8/LICENSE
--rw-r--r--   0 chenketing   (502) staff       (20)     8144 2023-07-11 07:35:39.614493 db-gpt-0.2.8/PKG-INFO
--rw-r--r--   0 chenketing   (502) staff       (20)     7613 2023-07-10 06:54:41.000000 db-gpt-0.2.8/README.md
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.472997 db-gpt-0.2.8/pilot/
--rw-r--r--   0 chenketing   (502) staff       (20)      206 2023-07-10 08:01:44.000000 db-gpt-0.2.8/pilot/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.475656 db-gpt-0.2.8/pilot/agent/
--rw-r--r--   0 chenketing   (502) staff       (20)       46 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/agent/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      179 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/agent/agent.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2266 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/agent/agent_manager.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4025 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/agent/json_fix_llm.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.477034 db-gpt-0.2.8/pilot/chain/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/chain/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)       46 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/chain/audio.py
--rw-r--r--   0 chenketing   (502) staff       (20)       47 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/chain/visual.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.479255 db-gpt-0.2.8/pilot/commands/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.480535 db-gpt-0.2.8/pilot/commands/built_in/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/built_in/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1430 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/built_in/audio_text.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3509 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/built_in/image_gen.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4602 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/command.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5168 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/command_mange.py
--rw-r--r--   0 chenketing   (502) staff       (20)      128 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/exception_not_commands.py
--rw-r--r--   0 chenketing   (502) staff       (20)      244 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/times.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.484603 db-gpt-0.2.8/pilot/common/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/common/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      803 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/common/custom_data_structure.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1516 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/common/formatting.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3044 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/common/markdown_text.py
--rw-r--r--   0 chenketing   (502) staff       (20)     6545 2023-06-27 11:35:59.000000 db-gpt-0.2.8/pilot/common/plugins.py
--rw-r--r--   0 chenketing   (502) staff       (20)      239 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/common/schema.py
--rw-r--r--   0 chenketing   (502) staff       (20)    17355 2023-07-10 06:54:41.000000 db-gpt-0.2.8/pilot/common/sql_database.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.486621 db-gpt-0.2.8/pilot/configs/
--rw-r--r--   0 chenketing   (502) staff       (20)      452 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/configs/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     7429 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/configs/config.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2219 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/configs/model_config.py
--rw-r--r--   0 chenketing   (502) staff       (20)    13673 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/conversation.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.496369 db-gpt-0.2.8/pilot/embedding_engine/
--rw-r--r--   0 chenketing   (502) staff       (20)      877 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/EncodeTextLoader.py
--rw-r--r--   0 chenketing   (502) staff       (20)      289 2023-07-10 08:01:44.000000 db-gpt-0.2.8/pilot/embedding_engine/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2486 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/chn_document_splitter.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1023 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/csv_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2459 2023-07-11 07:28:43.000000 db-gpt-0.2.8/pilot/embedding_engine/embedding_engine.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.497094 db-gpt-0.2.8/pilot/embedding_engine/external/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/external/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3649 2023-07-11 02:16:19.000000 db-gpt-0.2.8/pilot/embedding_engine/knowledge_type.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2200 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/embedding_engine/markdown_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2052 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/embedding_engine/pdf_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2102 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/pdf_loader.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1965 2023-07-10 07:29:21.000000 db-gpt-0.2.8/pilot/embedding_engine/ppt_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1729 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/search_milvus.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3094 2023-07-11 07:34:47.000000 db-gpt-0.2.8/pilot/embedding_engine/source_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)      883 2023-07-10 07:28:43.000000 db-gpt-0.2.8/pilot/embedding_engine/string_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1922 2023-07-10 07:28:43.000000 db-gpt-0.2.8/pilot/embedding_engine/url_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1793 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/embedding_engine/word_embedding.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.497690 db-gpt-0.2.8/pilot/inference_parsers/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/inference_parsers/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2234 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/inference_parsers/base.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.499344 db-gpt-0.2.8/pilot/json_utils/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/json_utils/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3609 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/json_utils/json_fix_general.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2270 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/json_utils/utilities.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.500359 db-gpt-0.2.8/pilot/log/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/log/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      531 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/log/json_handler.py
--rw-r--r--   0 chenketing   (502) staff       (20)     9846 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/logs.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.501033 db-gpt-0.2.8/pilot/memory/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/memory/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.503823 db-gpt-0.2.8/pilot/memory/chat_history/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/memory/chat_history/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1079 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/memory/chat_history/base.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5319 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/memory/chat_history/duckdb_history.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1496 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/memory/chat_history/file_history.py
--rw-r--r--   0 chenketing   (502) staff       (20)      968 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/memory/chat_history/mem_history.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.507772 db-gpt-0.2.8/pilot/model/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     6541 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/adapter.py
--rw-r--r--   0 chenketing   (502) staff       (20)      206 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/base.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.510962 db-gpt-0.2.8/pilot/model/cache/
--rw-r--r--   0 chenketing   (502) staff       (20)      130 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/cache/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      617 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/cache/base.py
--rw-r--r--   0 chenketing   (502) staff       (20)      718 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/cache/disk_cache.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1060 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/cache/gpt_cache.py
--rw-r--r--   0 chenketing   (502) staff       (20)      599 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/cache/memory_cache.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3955 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/compression.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.516836 db-gpt-0.2.8/pilot/model/llm_out/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2251 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/llm_out/chatglm_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1546 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/falcon_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2001 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/gorilla_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)      568 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/gpt4all_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3276 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/guanaco_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2679 2023-07-10 06:54:41.000000 db-gpt-0.2.8/pilot/model/llm_out/proxy_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     7674 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/model/llm_out/vicuna_base_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2606 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/vicuna_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3113 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/llm_utils.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3949 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/loader.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.517493 db-gpt-0.2.8/pilot/model/proxy/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/proxy/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.517795 db-gpt-0.2.8/pilot/openapi/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/openapi/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.519038 db-gpt-0.2.8/pilot/openapi/api_v1/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-26 11:33:41.000000 db-gpt-0.2.8/pilot/openapi/api_v1/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     9550 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/openapi/api_v1/api_v1.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1559 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/openapi/api_v1/api_view_model.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.520091 db-gpt-0.2.8/pilot/out_parser/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/out_parser/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     8144 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/out_parser/base.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.523707 db-gpt-0.2.8/pilot/prompts/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/prompts/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1453 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/prompts/base.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1063 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/prompts/example_base.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5623 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/prompts/generator.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2596 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/prompts/prompt_new.py
--rw-r--r--   0 chenketing   (502) staff       (20)    11978 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/prompts/prompt_template.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.527233 db-gpt-0.2.8/pilot/scene/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2437 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/base.py
--rw-r--r--   0 chenketing   (502) staff       (20)    12576 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/base_chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3683 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/base_message.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.529295 db-gpt-0.2.8/pilot/scene/chat_dashboard/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.530151 db-gpt-0.2.8/pilot/scene/chat_dashboard/business_cockpit/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/business_cockpit/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4957 2023-07-10 06:54:41.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/chat.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.530858 db-gpt-0.2.8/pilot/scene/chat_dashboard/data_preparation/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/data_preparation/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1383 2023-07-10 06:54:41.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/data_preparation/report_schma.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1359 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2432 2023-07-10 06:54:41.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.531803 db-gpt-0.2.8/pilot/scene/chat_db/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_db/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.533876 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1969 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1218 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/example.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2285 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2257 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/prompt.py
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_db/example.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.535848 db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2047 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2634 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.538569 db-gpt-0.2.8/pilot/scene/chat_execution/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_execution/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2830 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_execution/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1182 2023-07-06 05:46:38.000000 db-gpt-0.2.8/pilot/scene/chat_execution/example.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1510 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_execution/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1732 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_execution/prompt.py
--rw-r--r--   0 chenketing   (502) staff       (20)        1 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_execution/prompt_v2.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1216 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_factory.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.539125 db-gpt-0.2.8/pilot/scene/chat_knowledge/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.540987 db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1882 2023-07-11 02:36:56.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1881 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.542880 db-gpt-0.2.8/pilot/scene/chat_knowledge/default/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/default/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2088 2023-07-11 02:46:32.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/default/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/default/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1979 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/default/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.544808 db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1036 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      709 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1507 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.546787 db-gpt-0.2.8/pilot/scene/chat_knowledge/url/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/url/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2217 2023-07-11 02:46:32.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/url/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/url/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1975 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/url/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.548805 db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2073 2023-07-11 02:46:32.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1972 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.551115 db-gpt-0.2.8/pilot/scene/chat_normal/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_normal/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1034 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_normal/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-30 02:43:35.000000 db-gpt-0.2.8/pilot/scene/chat_normal/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)      820 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_normal/prompt.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4091 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/message.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.557182 db-gpt-0.2.8/pilot/server/
--rw-r--r--   0 chenketing   (502) staff       (20)      312 2023-06-27 11:36:00.000000 db-gpt-0.2.8/pilot/server/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3874 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/server/chat_adapter.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3299 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/dbgpt_server.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2761 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/server/gradio_css.py
--rw-r--r--   0 chenketing   (502) staff       (20)     7338 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/server/gradio_patch.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.590366 db-gpt-0.2.8/pilot/server/knowledge/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5529 2023-07-10 07:05:37.000000 db-gpt-0.2.8/pilot/server/knowledge/api.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4680 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/chunk_db.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5141 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/document_db.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.592923 db-gpt-0.2.8/pilot/server/knowledge/request/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/request/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1747 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/request/request.py
--rw-r--r--   0 chenketing   (502) staff       (20)      721 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/request/response.py
--rw-r--r--   0 chenketing   (502) staff       (20)     7435 2023-07-11 02:33:25.000000 db-gpt-0.2.8/pilot/server/knowledge/service.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3902 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/space_db.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5841 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/llmserver.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2545 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/server/vectordb_qa.py
--rw-r--r--   0 chenketing   (502) staff       (20)    23645 2023-07-10 12:58:18.000000 db-gpt-0.2.8/pilot/server/webserver.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1622 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/webserver_base.py
--rw-r--r--   0 chenketing   (502) staff       (20)      697 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/singleton.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.598541 db-gpt-0.2.8/pilot/speech/
--rw-r--r--   0 chenketing   (502) staff       (20)       62 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1114 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/base.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1166 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/brian.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2956 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/speech/eleven_labs.py
--rw-r--r--   0 chenketing   (502) staff       (20)      453 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/gtts.py
--rw-r--r--   0 chenketing   (502) staff       (20)      518 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/macos_tts.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1425 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/say.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.601706 db-gpt-0.2.8/pilot/summary/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/summary/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      635 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/summary/db_summary.py
--rw-r--r--   0 chenketing   (502) staff       (20)     6906 2023-07-11 02:46:32.000000 db-gpt-0.2.8/pilot/summary/db_summary_client.py
--rw-r--r--   0 chenketing   (502) staff       (20)     8382 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/summary/mysql_db_summary.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4148 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/utils.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.609608 db-gpt-0.2.8/pilot/vector_store/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/vector_store/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1382 2023-07-11 02:25:57.000000 db-gpt-0.2.8/pilot/vector_store/chroma_store.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1042 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/vector_store/connector.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2594 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/vector_store/extract_tovec.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3587 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/vector_store/file_loader.py
--rw-r--r--   0 chenketing   (502) staff       (20)    12126 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/vector_store/milvus_store.py
--rw-r--r--   0 chenketing   (502) staff       (20)      506 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/vector_store/vector_store_base.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5312 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/vector_store/weaviate_store.py
--rw-r--r--   0 chenketing   (502) staff       (20)       38 2023-07-11 07:35:39.615054 db-gpt-0.2.8/setup.cfg
--rw-r--r--   0 chenketing   (502) staff       (20)     1201 2023-07-11 07:35:28.000000 db-gpt-0.2.8/setup.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.610825 db-gpt-0.2.8/tests/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/tests/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.611998 db-gpt-0.2.8/tests/unit/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-10 07:52:37.000000 db-gpt-0.2.8/tests/unit/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.613502 db-gpt-0.2.8/tests/unit/embedding_engine/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-10 07:53:06.000000 db-gpt-0.2.8/tests/unit/embedding_engine/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      678 2023-07-11 02:33:25.000000 db-gpt-0.2.8/tests/unit/embedding_engine/test_url_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4480 2023-06-20 09:57:25.000000 db-gpt-0.2.8/tests/unit/test_plugins.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.611814 db-gpt-0.3.0/
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.491120 db-gpt-0.3.0/DB_GPT.egg-info/
+-rw-r--r--   0 chenketing   (502) staff       (20)     8333 2023-07-13 11:38:22.000000 db-gpt-0.3.0/DB_GPT.egg-info/PKG-INFO
+-rw-r--r--   0 chenketing   (502) staff       (20)     6845 2023-07-13 11:38:22.000000 db-gpt-0.3.0/DB_GPT.egg-info/SOURCES.txt
+-rw-r--r--   0 chenketing   (502) staff       (20)        1 2023-07-13 11:38:22.000000 db-gpt-0.3.0/DB_GPT.egg-info/dependency_links.txt
+-rw-r--r--   0 chenketing   (502) staff       (20)       56 2023-07-13 11:38:22.000000 db-gpt-0.3.0/DB_GPT.egg-info/entry_points.txt
+-rw-r--r--   0 chenketing   (502) staff       (20)     1155 2023-07-13 11:38:22.000000 db-gpt-0.3.0/DB_GPT.egg-info/requires.txt
+-rw-r--r--   0 chenketing   (502) staff       (20)       12 2023-07-13 11:38:22.000000 db-gpt-0.3.0/DB_GPT.egg-info/top_level.txt
+-rw-r--r--   0 chenketing   (502) staff       (20)     1067 2023-06-20 09:57:25.000000 db-gpt-0.3.0/LICENSE
+-rw-r--r--   0 chenketing   (502) staff       (20)     8333 2023-07-13 11:38:22.611178 db-gpt-0.3.0/PKG-INFO
+-rw-r--r--   0 chenketing   (502) staff       (20)     7802 2023-07-13 11:24:50.000000 db-gpt-0.3.0/README.md
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.494756 db-gpt-0.3.0/pilot/
+-rw-r--r--   0 chenketing   (502) staff       (20)      206 2023-07-10 08:01:44.000000 db-gpt-0.3.0/pilot/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.497518 db-gpt-0.3.0/pilot/agent/
+-rw-r--r--   0 chenketing   (502) staff       (20)       46 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/agent/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      179 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/agent/agent.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2266 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/agent/agent_manager.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4025 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/agent/json_fix_llm.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.498934 db-gpt-0.3.0/pilot/chain/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/chain/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)       46 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/chain/audio.py
+-rw-r--r--   0 chenketing   (502) staff       (20)       47 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/chain/visual.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.501328 db-gpt-0.3.0/pilot/commands/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/commands/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.502605 db-gpt-0.3.0/pilot/commands/built_in/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/commands/built_in/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1430 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/commands/built_in/audio_text.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3509 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/commands/built_in/image_gen.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4602 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/commands/command.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5168 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/commands/command_mange.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      128 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/commands/exception_not_commands.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      244 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/commands/times.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.506558 db-gpt-0.3.0/pilot/common/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/common/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      803 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/common/custom_data_structure.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1516 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/common/formatting.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3044 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/common/markdown_text.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     6545 2023-06-27 11:35:59.000000 db-gpt-0.3.0/pilot/common/plugins.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      239 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/common/schema.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    17778 2023-07-13 11:10:27.000000 db-gpt-0.3.0/pilot/common/sql_database.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.508841 db-gpt-0.3.0/pilot/configs/
+-rw-r--r--   0 chenketing   (502) staff       (20)      452 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/configs/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     7484 2023-07-12 06:27:47.000000 db-gpt-0.3.0/pilot/configs/config.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2219 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/configs/model_config.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    13673 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/conversation.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.519903 db-gpt-0.3.0/pilot/embedding_engine/
+-rw-r--r--   0 chenketing   (502) staff       (20)      877 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/embedding_engine/EncodeTextLoader.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      289 2023-07-10 08:01:44.000000 db-gpt-0.3.0/pilot/embedding_engine/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2486 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/embedding_engine/chn_document_splitter.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1814 2023-07-13 11:10:27.000000 db-gpt-0.3.0/pilot/embedding_engine/csv_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3427 2023-07-13 06:54:15.000000 db-gpt-0.3.0/pilot/embedding_engine/embedding_engine.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.520554 db-gpt-0.3.0/pilot/embedding_engine/external/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/embedding_engine/external/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3963 2023-07-13 06:54:15.000000 db-gpt-0.3.0/pilot/embedding_engine/knowledge_type.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2260 2023-07-13 11:10:27.000000 db-gpt-0.3.0/pilot/embedding_engine/markdown_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1859 2023-07-13 11:10:27.000000 db-gpt-0.3.0/pilot/embedding_engine/pdf_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2102 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/embedding_engine/pdf_loader.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1893 2023-07-13 11:10:27.000000 db-gpt-0.3.0/pilot/embedding_engine/ppt_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1729 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/embedding_engine/search_milvus.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3374 2023-07-13 06:54:15.000000 db-gpt-0.3.0/pilot/embedding_engine/source_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1871 2023-07-13 11:10:27.000000 db-gpt-0.3.0/pilot/embedding_engine/string_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2031 2023-07-13 11:10:27.000000 db-gpt-0.3.0/pilot/embedding_engine/url_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1902 2023-07-13 11:10:27.000000 db-gpt-0.3.0/pilot/embedding_engine/word_embedding.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.521142 db-gpt-0.3.0/pilot/inference_parsers/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/inference_parsers/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2234 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/inference_parsers/base.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.522671 db-gpt-0.3.0/pilot/json_utils/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/json_utils/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3609 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/json_utils/json_fix_general.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2270 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/json_utils/utilities.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.523760 db-gpt-0.3.0/pilot/log/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/log/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      531 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/log/json_handler.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     9846 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/logs.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.524541 db-gpt-0.3.0/pilot/memory/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/memory/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.527293 db-gpt-0.3.0/pilot/memory/chat_history/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/memory/chat_history/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1079 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/memory/chat_history/base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5319 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/memory/chat_history/duckdb_history.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1496 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/memory/chat_history/file_history.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      968 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/memory/chat_history/mem_history.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.532041 db-gpt-0.3.0/pilot/model/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/model/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     8520 2023-07-12 06:27:47.000000 db-gpt-0.3.0/pilot/model/adapter.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      206 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/model/base.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.535654 db-gpt-0.3.0/pilot/model/cache/
+-rw-r--r--   0 chenketing   (502) staff       (20)      130 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/model/cache/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      617 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/model/cache/base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      718 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/model/cache/disk_cache.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1060 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/model/cache/gpt_cache.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      599 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/model/cache/memory_cache.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3955 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/model/compression.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.542788 db-gpt-0.3.0/pilot/model/llm_out/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/model/llm_out/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2251 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/model/llm_out/chatglm_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1546 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/model/llm_out/falcon_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2001 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/model/llm_out/gorilla_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      568 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/model/llm_out/gpt4all_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3276 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/model/llm_out/guanaco_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2679 2023-07-10 06:54:41.000000 db-gpt-0.3.0/pilot/model/llm_out/proxy_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     7674 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/model/llm_out/vicuna_base_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2606 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/model/llm_out/vicuna_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3113 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/model/llm_utils.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3949 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/model/loader.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.543577 db-gpt-0.3.0/pilot/model/proxy/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/model/proxy/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.544264 db-gpt-0.3.0/pilot/openapi/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/openapi/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.545884 db-gpt-0.3.0/pilot/openapi/api_v1/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-26 11:33:41.000000 db-gpt-0.3.0/pilot/openapi/api_v1/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     9550 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/openapi/api_v1/api_v1.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1559 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/openapi/api_v1/api_view_model.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.546825 db-gpt-0.3.0/pilot/out_parser/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/out_parser/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     8144 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/out_parser/base.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.550694 db-gpt-0.3.0/pilot/prompts/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/prompts/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1453 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/prompts/base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1063 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/prompts/example_base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5623 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/prompts/generator.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2596 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/prompts/prompt_new.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    11978 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/prompts/prompt_template.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.554920 db-gpt-0.3.0/pilot/scene/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2437 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    12576 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/base_chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3683 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/base_message.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.557403 db-gpt-0.3.0/pilot/scene/chat_dashboard/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/scene/chat_dashboard/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.558146 db-gpt-0.3.0/pilot/scene/chat_dashboard/business_cockpit/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/scene/chat_dashboard/business_cockpit/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4957 2023-07-10 06:54:41.000000 db-gpt-0.3.0/pilot/scene/chat_dashboard/chat.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.558758 db-gpt-0.3.0/pilot/scene/chat_dashboard/data_preparation/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/scene/chat_dashboard/data_preparation/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1383 2023-07-10 06:54:41.000000 db-gpt-0.3.0/pilot/scene/chat_dashboard/data_preparation/report_schma.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1359 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_dashboard/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2432 2023-07-10 06:54:41.000000 db-gpt-0.3.0/pilot/scene/chat_dashboard/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.560316 db-gpt-0.3.0/pilot/scene/chat_db/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_db/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.562962 db-gpt-0.3.0/pilot/scene/chat_db/auto_execute/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_db/auto_execute/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1969 2023-07-13 07:42:59.000000 db-gpt-0.3.0/pilot/scene/chat_db/auto_execute/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1218 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_db/auto_execute/example.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2285 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_db/auto_execute/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2257 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_db/auto_execute/prompt.py
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_db/example.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.565355 db-gpt-0.3.0/pilot/scene/chat_db/professional_qa/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_db/professional_qa/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2047 2023-07-13 11:00:11.000000 db-gpt-0.3.0/pilot/scene/chat_db/professional_qa/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_db/professional_qa/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2634 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_db/professional_qa/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.568793 db-gpt-0.3.0/pilot/scene/chat_execution/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_execution/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2830 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_execution/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1182 2023-07-06 05:46:38.000000 db-gpt-0.3.0/pilot/scene/chat_execution/example.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1510 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_execution/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1732 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_execution/prompt.py
+-rw-r--r--   0 chenketing   (502) staff       (20)        1 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/scene/chat_execution/prompt_v2.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1216 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_factory.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.569437 db-gpt-0.3.0/pilot/scene/chat_knowledge/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.571282 db-gpt-0.3.0/pilot/scene/chat_knowledge/custom/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/custom/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1882 2023-07-11 02:36:56.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/custom/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/custom/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1881 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/custom/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.573825 db-gpt-0.3.0/pilot/scene/chat_knowledge/default/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/default/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2088 2023-07-11 02:46:32.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/default/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/default/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1979 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/default/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.576014 db-gpt-0.3.0/pilot/scene/chat_knowledge/inner_db_summary/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/inner_db_summary/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1036 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/inner_db_summary/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      709 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/inner_db_summary/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1507 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/inner_db_summary/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.578176 db-gpt-0.3.0/pilot/scene/chat_knowledge/url/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/url/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2217 2023-07-11 02:46:32.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/url/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/url/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1975 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/url/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.580274 db-gpt-0.3.0/pilot/scene/chat_knowledge/v1/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/v1/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2073 2023-07-11 02:46:32.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/v1/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/v1/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1972 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_knowledge/v1/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.583169 db-gpt-0.3.0/pilot/scene/chat_normal/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/scene/chat_normal/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1034 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_normal/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-30 02:43:35.000000 db-gpt-0.3.0/pilot/scene/chat_normal/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      820 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/scene/chat_normal/prompt.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4091 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/scene/message.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.589619 db-gpt-0.3.0/pilot/server/
+-rw-r--r--   0 chenketing   (502) staff       (20)      312 2023-06-27 11:36:00.000000 db-gpt-0.3.0/pilot/server/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3874 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/server/chat_adapter.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3305 2023-07-13 05:45:41.000000 db-gpt-0.3.0/pilot/server/dbgpt_server.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2761 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/server/gradio_css.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     7338 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/server/gradio_patch.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.593352 db-gpt-0.3.0/pilot/server/knowledge/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/server/knowledge/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5529 2023-07-10 07:05:37.000000 db-gpt-0.3.0/pilot/server/knowledge/api.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4680 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/server/knowledge/chunk_db.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5141 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/server/knowledge/document_db.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.594990 db-gpt-0.3.0/pilot/server/knowledge/request/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/server/knowledge/request/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1747 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/server/knowledge/request/request.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      721 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/server/knowledge/request/response.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     8296 2023-07-12 09:50:42.000000 db-gpt-0.3.0/pilot/server/knowledge/service.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3902 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/server/knowledge/space_db.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5841 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/server/llmserver.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2545 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/server/vectordb_qa.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    23645 2023-07-10 12:58:18.000000 db-gpt-0.3.0/pilot/server/webserver.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1622 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/server/webserver_base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      697 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/singleton.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.599653 db-gpt-0.3.0/pilot/speech/
+-rw-r--r--   0 chenketing   (502) staff       (20)       62 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/speech/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1114 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/speech/base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1166 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/speech/brian.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2956 2023-07-05 08:29:49.000000 db-gpt-0.3.0/pilot/speech/eleven_labs.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      453 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/speech/gtts.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      518 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/speech/macos_tts.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1425 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/speech/say.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.602176 db-gpt-0.3.0/pilot/summary/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/summary/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      635 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/summary/db_summary.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     7125 2023-07-13 11:01:28.000000 db-gpt-0.3.0/pilot/summary/db_summary_client.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     8382 2023-07-13 11:01:33.000000 db-gpt-0.3.0/pilot/summary/mysql_db_summary.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4148 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/utils.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.607447 db-gpt-0.3.0/pilot/vector_store/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/vector_store/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1382 2023-07-11 02:25:57.000000 db-gpt-0.3.0/pilot/vector_store/chroma_store.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1380 2023-07-12 06:21:39.000000 db-gpt-0.3.0/pilot/vector_store/connector.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2594 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/vector_store/extract_tovec.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3587 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/vector_store/file_loader.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    12121 2023-07-12 03:06:43.000000 db-gpt-0.3.0/pilot/vector_store/milvus_store.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      506 2023-06-20 09:57:25.000000 db-gpt-0.3.0/pilot/vector_store/vector_store_base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5312 2023-07-06 07:40:51.000000 db-gpt-0.3.0/pilot/vector_store/weaviate_store.py
+-rw-r--r--   0 chenketing   (502) staff       (20)       38 2023-07-13 11:38:22.611904 db-gpt-0.3.0/setup.cfg
+-rw-r--r--   0 chenketing   (502) staff       (20)     1201 2023-07-13 11:37:51.000000 db-gpt-0.3.0/setup.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.608212 db-gpt-0.3.0/tests/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.3.0/tests/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.608808 db-gpt-0.3.0/tests/unit/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-10 07:52:37.000000 db-gpt-0.3.0/tests/unit/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-13 11:38:22.610219 db-gpt-0.3.0/tests/unit/embedding_engine/
+-rw-r--r--   0 chenketing   (502) staff       (20)     1120 2023-07-12 03:06:43.000000 db-gpt-0.3.0/tests/unit/embedding_engine/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      665 2023-07-12 03:06:43.000000 db-gpt-0.3.0/tests/unit/embedding_engine/test_url_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4480 2023-06-20 09:57:25.000000 db-gpt-0.3.0/tests/unit/test_plugins.py
```

### Comparing `db-gpt-0.2.8/DB_GPT.egg-info/PKG-INFO` & `db-gpt-0.3.0/DB_GPT.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-gpt
-Version: 0.2.8
+Version: 0.3.0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/csunny/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -24,45 +24,71 @@
 
 [**简体中文**](README.zh.md) |[**Discord**](https://discord.com/invite/EUEBmdpd) |[**Documents**](https://db-gpt.readthedocs.io/en/latest/)|[**Wechat**](https://github.com/csunny/DB-GPT/blob/main/README.zh.md#%E8%81%94%E7%B3%BB%E6%88%91%E4%BB%AC) 
 
 </div>
 
 ## What is DB-GPT?
 
-As large models are released and iterated upon, they are becoming increasingly intelligent. However, in the process of using large models, we face significant challenges in data security and privacy. We need to ensure that our sensitive data and environments remain completely controlled and avoid any data privacy leaks or security risks. Based on this, we have launched the DB-GPT project to build a complete private large model solution for all database-based scenarios. This solution supports local deployment, allowing it to be applied not only in independent private environments but also to be independently deployed and isolated according to business modules, ensuring that the ability of large models is absolutely private, secure, and controllable.
-
 DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 
-## News
-- [2023/07/06]🔥🔥🔥Brand-new DB-GPT product with a brand-new web UI. [documents](https://db-gpt.readthedocs.io/en/latest/getting_started/getting_started.html) 
-- [2023/06/25]🔥support chatglm2-6b model. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
-- [2023/06/14] support gpt4all model, which can run at M1/M2, or cpu machine. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
-- [2023/06/01]🔥 On the basis of the Vicuna-13B basic model, task chain calls are implemented through plugins. For example, the implementation of creating a database with a single sentence.[demo](./assets/auto_plugin.gif)
-- [2023/06/01]🔥 QLoRA guanaco(7b, 13b, 33b) support.
-- [2023/05/28] Learning from crawling data from the Internet [demo](./assets/dbgpt_demo.gif)
-- [2023/05/21] Generate SQL and execute it automatically. [demo](./assets/chat-data.gif)
-- [2023/05/15] Chat with documents. [demo](./assets/new_knownledge_en.gif)
-- [2023/05/06] SQL generation and diagnosis. [demo](./assets/demo_en.gif)
+[![Star History Chart](https://api.star-history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
 
 ## Demo
 
 Run on an RTX 4090 GPU.
 
-<p align="left">
-  <img src="./assets/dbgpt_demo.gif" width="800px" />
-</p>
-
+https://github.com/csunny/DB-GPT/assets/13723926/55f31781-1d49-4757-b96e-7ef6d3dbcf80
 
 <!-- <video id="video" controls="" preload="auto" poster="assets/exector_sql.png">
       <source id="mp4" src="https://github.com/csunny/DB-GPT/assets/17919400/654b5a49-5ea4-4c02-b5b2-72d089dcc1f0" type="video/mp4">
 </videos> -->
 
 
+#### Chat with data, and figure charts.
+
+<p align="left">
+  <img src="./assets/dashboard.png" width="800px" />
+</p>
+
+#### Text2SQL, generate SQL from chat
+<p align="left">
+  <img src="./assets/chatSQL.png" width="800px" />
+</p>
 
+#### Chat with database meta information.
+<p align="left">
+  <img src="./assets/chatdb.png" width="800px" />
+</p>
 
+#### Chat with data, and execute results.
+<p align="left">
+  <img src="./assets/chatdata.png" width="800px" />
+</p>
+
+#### Knownledge space to manage docs.
+<p align="left">
+  <img src="./assets/ks.png" width="800px" />
+</p>
+
+#### Chat with knowledge, such as txt、pdf、csv、words. etc
+<p align="left">
+  <img src="./assets/chat_knowledge.png" width="800px" />
+</p>
+
+## Releases 
+- [2023/07/12]🔥🔥🔥DB-GPT Python API 0.3.0. [documents](https://db-gpt.readthedocs.io/en/latest/getting_started/installation.html) 
+- [2023/07/06]🔥🔥🔥Brand-new DB-GPT product with a brand-new web UI. [documents](https://db-gpt.readthedocs.io/en/latest/getting_started/getting_started.html) 
+- [2023/06/25]🔥support chatglm2-6b model. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
+- [2023/06/14] support gpt4all model, which can run at M1/M2, or cpu machine. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
+- [2023/06/01]🔥 On the basis of the Vicuna-13B basic model, task chain calls are implemented through plugins. For example, the implementation of creating a database with a single sentence.[demo](./assets/auto_plugin.gif)
+- [2023/06/01]🔥 QLoRA guanaco(7b, 13b, 33b) support.
+- [2023/05/28] Learning from crawling data from the Internet [demo](./assets/dbgpt_demo.gif)
+- [2023/05/21] Generate SQL and execute it automatically. [demo](./assets/chat-data.gif)
+- [2023/05/15] Chat with documents. [demo](./assets/new_knownledge_en.gif)
+- [2023/05/06] SQL generation and diagnosis. [demo](./assets/demo_en.gif)
 
 ## Features
 
 Currently, we have released multiple key features, which are listed below to demonstrate our current capabilities:
 
 - SQL language capabilities
   - SQL generation
@@ -83,15 +109,14 @@
   - TODO: codegen2, codet5p
 
 
 ## Introduction 
 DB-GPT creates a vast model operating system using [FastChat](https://github.com/lm-sys/FastChat) and offers a large language model powered by [Vicuna](https://huggingface.co/Tribbiani/vicuna-7b). In addition, we provide private domain knowledge base question-answering capability. Furthermore, we also provide support for additional plugins, and our design natively supports the Auto-GPT plugin.Our vision is to make it easier and more convenient to build  applications around databases and llm.
 
 
-
 Is the architecture of the entire DB-GPT shown in the following figure:
 
 <p align="center">
   <img src="./assets/DB-GPT.png" width="800" />
 </p>
 
 The core capabilities mainly consist of the following parts:
@@ -134,16 +159,22 @@
 - [ChatGLM](https://github.com/THUDM/ChatGLM-6B) as the base model
 - [llama_index](https://github.com/jerryjliu/llama_index) for enhancing database-related knowledge using [in-context learning](https://arxiv.org/abs/2301.00234) based on existing knowledge bases.
 
 ## Contribution
 
 - Please run `black .` before submitting the code.
 
+## RoadMap
+
+<p align="left">
+  <img src="./assets/roadmap.jpg" width="800px" />
+</p>
+
 ## Licence
 
 The MIT License (MIT)
 
 ## Contact Information
 We are working on building a community, if you have any ideas about building the community, feel free to contact us. [Discord](https://discord.gg/4BNdxm5d)
 
-[![Star History Chart](https://api.star-history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
+
```

#### html2text {}

```diff
@@ -1,70 +1,76 @@
-Metadata-Version: 2.1 Name: db-gpt Version: 0.2.8 Summary: DB-GPT is an
+Metadata-Version: 2.1 Name: db-gpt Version: 0.3.0 Summary: DB-GPT is an
 experimental open-source project that uses localized GPT large models to
 interact with your data and environment. With this solution, you can be assured
 that there is no risk of data leakage, and your data is 100% private and
 secure. Home-page: https://github.com/csunny/DB-GPT Author: csunny Author-
 email: cfqcsunny@gmail.com License: https://opensource.org/license/mit/
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # DB-GPT: Revolutionizing Database Interactions with Private LLM
 Technology
                                 [stars] [forks]
   [**ç®ä½ä¸­æ**](README.zh.md) |[**Discord**](https://discord.com/invite/
      EUEBmdpd) |[**Documents**](https://db-gpt.readthedocs.io/en/latest/)|
            [**Wechat**](https://github.com/csunny/DB-GPT/blob/main/
               README.zh.md#%E8%81%94%E7%B3%BB%E6%88%91%E4%BB%AC)
-## What is DB-GPT? As large models are released and iterated upon, they are
-becoming increasingly intelligent. However, in the process of using large
-models, we face significant challenges in data security and privacy. We need to
-ensure that our sensitive data and environments remain completely controlled
-and avoid any data privacy leaks or security risks. Based on this, we have
-launched the DB-GPT project to build a complete private large model solution
-for all database-based scenarios. This solution supports local deployment,
-allowing it to be applied not only in independent private environments but also
-to be independently deployed and isolated according to business modules,
-ensuring that the ability of large models is absolutely private, secure, and
-controllable. DB-GPT is an experimental open-source project that uses localized
-GPT large models to interact with your data and environment. With this
-solution, you can be assured that there is no risk of data leakage, and your
-data is 100% private and secure. ## News - [2023/07/06]ð¥ð¥ð¥Brand-new
-DB-GPT product with a brand-new web UI. [documents](https://db-
-gpt.readthedocs.io/en/latest/getting_started/getting_started.html) - [2023/06/
-25]ð¥support chatglm2-6b model. [documents](https://db-gpt.readthedocs.io/en/
-latest/modules/llms.html) - [2023/06/14] support gpt4all model, which can run
-at M1/M2, or cpu machine. [documents](https://db-gpt.readthedocs.io/en/latest/
-modules/llms.html) - [2023/06/01]ð¥ On the basis of the Vicuna-13B basic
-model, task chain calls are implemented through plugins. For example, the
-implementation of creating a database with a single sentence.[demo](./assets/
-auto_plugin.gif) - [2023/06/01]ð¥ QLoRA guanaco(7b, 13b, 33b) support. -
-[2023/05/28] Learning from crawling data from the Internet [demo](./assets/
-dbgpt_demo.gif) - [2023/05/21] Generate SQL and execute it automatically.
-[demo](./assets/chat-data.gif) - [2023/05/15] Chat with documents. [demo](./
-assets/new_knownledge_en.gif) - [2023/05/06] SQL generation and diagnosis.
-[demo](./assets/demo_en.gif) ## Demo Run on an RTX 4090 GPU.
-[./assets/dbgpt_demo.gif]
- ## Features Currently, we have released multiple key features, which are
-listed below to demonstrate our current capabilities: - SQL language
-capabilities - SQL generation - SQL diagnosis - Private domain Q&A and data
-processing - Knowledge Management(We currently support many document formats:
-txt, pdf, md, html, doc, ppt, and url.) - Database knowledge Q&A - knowledge
-Embedding - Plugins - Support custom plugin execution tasks and natively
-support the Auto-GPT plugin, such as: - Automatic execution of SQL and
-retrieval of query results - Automatic crawling and learning of knowledge -
-Unified vector storage/indexing of knowledge base - Support for unstructured
-data such as PDF, TXT, Markdown, CSV, DOC, PPT, and WebURL - Multi LLMs Support
-- Supports multiple large language models, currently supporting Vicuna (7b,
-13b), ChatGLM-6b (int4, int8), guanaco(7b,13b,33b), Gorilla(7b,13b) - TODO:
-codegen2, codet5p ## Introduction DB-GPT creates a vast model operating system
-using [FastChat](https://github.com/lm-sys/FastChat) and offers a large
-language model powered by [Vicuna](https://huggingface.co/Tribbiani/vicuna-7b).
-In addition, we provide private domain knowledge base question-answering
-capability. Furthermore, we also provide support for additional plugins, and
-our design natively supports the Auto-GPT plugin.Our vision is to make it
-easier and more convenient to build applications around databases and llm. Is
-the architecture of the entire DB-GPT shown in the following figure:
+## What is DB-GPT? DB-GPT is an experimental open-source project that uses
+localized GPT large models to interact with your data and environment. With
+this solution, you can be assured that there is no risk of data leakage, and
+your data is 100% private and secure. [![Star History Chart](https://api.star-
+history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
+## Demo Run on an RTX 4090 GPU. https://github.com/csunny/DB-GPT/assets/
+13723926/55f31781-1d49-4757-b96e-7ef6d3dbcf80  #### Chat with data, and figure
+charts.
+[./assets/dashboard.png]
+#### Text2SQL, generate SQL from chat
+[./assets/chatSQL.png]
+#### Chat with database meta information.
+[./assets/chatdb.png]
+#### Chat with data, and execute results.
+[./assets/chatdata.png]
+#### Knownledge space to manage docs.
+[./assets/ks.png]
+#### Chat with knowledge, such as txtãpdfãcsvãwords. etc
+[./assets/chat_knowledge.png]
+## Releases - [2023/07/12]ð¥ð¥ð¥DB-GPT Python API 0.3.0. [documents]
+(https://db-gpt.readthedocs.io/en/latest/getting_started/installation.html) -
+[2023/07/06]ð¥ð¥ð¥Brand-new DB-GPT product with a brand-new web UI.
+[documents](https://db-gpt.readthedocs.io/en/latest/getting_started/
+getting_started.html) - [2023/06/25]ð¥support chatglm2-6b model. [documents]
+(https://db-gpt.readthedocs.io/en/latest/modules/llms.html) - [2023/06/14]
+support gpt4all model, which can run at M1/M2, or cpu machine. [documents]
+(https://db-gpt.readthedocs.io/en/latest/modules/llms.html) - [2023/06/01]ð¥
+On the basis of the Vicuna-13B basic model, task chain calls are implemented
+through plugins. For example, the implementation of creating a database with a
+single sentence.[demo](./assets/auto_plugin.gif) - [2023/06/01]ð¥ QLoRA
+guanaco(7b, 13b, 33b) support. - [2023/05/28] Learning from crawling data from
+the Internet [demo](./assets/dbgpt_demo.gif) - [2023/05/21] Generate SQL and
+execute it automatically. [demo](./assets/chat-data.gif) - [2023/05/15] Chat
+with documents. [demo](./assets/new_knownledge_en.gif) - [2023/05/06] SQL
+generation and diagnosis. [demo](./assets/demo_en.gif) ## Features Currently,
+we have released multiple key features, which are listed below to demonstrate
+our current capabilities: - SQL language capabilities - SQL generation - SQL
+diagnosis - Private domain Q&A and data processing - Knowledge Management(We
+currently support many document formats: txt, pdf, md, html, doc, ppt, and
+url.) - Database knowledge Q&A - knowledge Embedding - Plugins - Support custom
+plugin execution tasks and natively support the Auto-GPT plugin, such as: -
+Automatic execution of SQL and retrieval of query results - Automatic crawling
+and learning of knowledge - Unified vector storage/indexing of knowledge base -
+Support for unstructured data such as PDF, TXT, Markdown, CSV, DOC, PPT, and
+WebURL - Multi LLMs Support - Supports multiple large language models,
+currently supporting Vicuna (7b, 13b), ChatGLM-6b (int4, int8), guanaco
+(7b,13b,33b), Gorilla(7b,13b) - TODO: codegen2, codet5p ## Introduction DB-GPT
+creates a vast model operating system using [FastChat](https://github.com/lm-
+sys/FastChat) and offers a large language model powered by [Vicuna](https://
+huggingface.co/Tribbiani/vicuna-7b). In addition, we provide private domain
+knowledge base question-answering capability. Furthermore, we also provide
+support for additional plugins, and our design natively supports the Auto-GPT
+plugin.Our vision is to make it easier and more convenient to build
+applications around databases and llm. Is the architecture of the entire DB-GPT
+shown in the following figure:
                              [./assets/DB-GPT.png]
 The core capabilities mainly consist of the following parts: 1. Knowledge base
 capability: Supports private domain knowledge base question-answering
 capability. 2. Large-scale model management capability: Provides a large model
 operating environment based on FastChat. 3. Unified data vector storage and
 indexing: Provides a uniform way to store and index various data types. 4.
 Connection module: Used to connect different modules and data sources to
@@ -91,12 +97,12 @@
 Significant-Gravitas/Auto-GPT) universal plugin template - [Hugging Face]
 (https://huggingface.co/) for big model management - [Chroma](https://
 github.com/chroma-core/chroma) for vector storage - [Milvus](https://milvus.io/
 ) for distributed vector storage - [ChatGLM](https://github.com/THUDM/ChatGLM-
 6B) as the base model - [llama_index](https://github.com/jerryjliu/llama_index)
 for enhancing database-related knowledge using [in-context learning](https://
 arxiv.org/abs/2301.00234) based on existing knowledge bases. ## Contribution -
-Please run `black .` before submitting the code. ## Licence The MIT License
-(MIT) ## Contact Information We are working on building a community, if you
-have any ideas about building the community, feel free to contact us. [Discord]
-(https://discord.gg/4BNdxm5d) [![Star History Chart](https://api.star-
-history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
+Please run `black .` before submitting the code. ## RoadMap
+[./assets/roadmap.jpg]
+## Licence The MIT License (MIT) ## Contact Information We are working on
+building a community, if you have any ideas about building the community, feel
+free to contact us. [Discord](https://discord.gg/4BNdxm5d)
```

### Comparing `db-gpt-0.2.8/DB_GPT.egg-info/SOURCES.txt` & `db-gpt-0.3.0/DB_GPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/DB_GPT.egg-info/requires.txt` & `db-gpt-0.3.0/DB_GPT.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/LICENSE` & `db-gpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/PKG-INFO` & `db-gpt-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-gpt
-Version: 0.2.8
+Version: 0.3.0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/csunny/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -24,45 +24,71 @@
 
 [**简体中文**](README.zh.md) |[**Discord**](https://discord.com/invite/EUEBmdpd) |[**Documents**](https://db-gpt.readthedocs.io/en/latest/)|[**Wechat**](https://github.com/csunny/DB-GPT/blob/main/README.zh.md#%E8%81%94%E7%B3%BB%E6%88%91%E4%BB%AC) 
 
 </div>
 
 ## What is DB-GPT?
 
-As large models are released and iterated upon, they are becoming increasingly intelligent. However, in the process of using large models, we face significant challenges in data security and privacy. We need to ensure that our sensitive data and environments remain completely controlled and avoid any data privacy leaks or security risks. Based on this, we have launched the DB-GPT project to build a complete private large model solution for all database-based scenarios. This solution supports local deployment, allowing it to be applied not only in independent private environments but also to be independently deployed and isolated according to business modules, ensuring that the ability of large models is absolutely private, secure, and controllable.
-
 DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 
-## News
-- [2023/07/06]🔥🔥🔥Brand-new DB-GPT product with a brand-new web UI. [documents](https://db-gpt.readthedocs.io/en/latest/getting_started/getting_started.html) 
-- [2023/06/25]🔥support chatglm2-6b model. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
-- [2023/06/14] support gpt4all model, which can run at M1/M2, or cpu machine. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
-- [2023/06/01]🔥 On the basis of the Vicuna-13B basic model, task chain calls are implemented through plugins. For example, the implementation of creating a database with a single sentence.[demo](./assets/auto_plugin.gif)
-- [2023/06/01]🔥 QLoRA guanaco(7b, 13b, 33b) support.
-- [2023/05/28] Learning from crawling data from the Internet [demo](./assets/dbgpt_demo.gif)
-- [2023/05/21] Generate SQL and execute it automatically. [demo](./assets/chat-data.gif)
-- [2023/05/15] Chat with documents. [demo](./assets/new_knownledge_en.gif)
-- [2023/05/06] SQL generation and diagnosis. [demo](./assets/demo_en.gif)
+[![Star History Chart](https://api.star-history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
 
 ## Demo
 
 Run on an RTX 4090 GPU.
 
-<p align="left">
-  <img src="./assets/dbgpt_demo.gif" width="800px" />
-</p>
-
+https://github.com/csunny/DB-GPT/assets/13723926/55f31781-1d49-4757-b96e-7ef6d3dbcf80
 
 <!-- <video id="video" controls="" preload="auto" poster="assets/exector_sql.png">
       <source id="mp4" src="https://github.com/csunny/DB-GPT/assets/17919400/654b5a49-5ea4-4c02-b5b2-72d089dcc1f0" type="video/mp4">
 </videos> -->
 
 
+#### Chat with data, and figure charts.
+
+<p align="left">
+  <img src="./assets/dashboard.png" width="800px" />
+</p>
+
+#### Text2SQL, generate SQL from chat
+<p align="left">
+  <img src="./assets/chatSQL.png" width="800px" />
+</p>
 
+#### Chat with database meta information.
+<p align="left">
+  <img src="./assets/chatdb.png" width="800px" />
+</p>
 
+#### Chat with data, and execute results.
+<p align="left">
+  <img src="./assets/chatdata.png" width="800px" />
+</p>
+
+#### Knownledge space to manage docs.
+<p align="left">
+  <img src="./assets/ks.png" width="800px" />
+</p>
+
+#### Chat with knowledge, such as txt、pdf、csv、words. etc
+<p align="left">
+  <img src="./assets/chat_knowledge.png" width="800px" />
+</p>
+
+## Releases 
+- [2023/07/12]🔥🔥🔥DB-GPT Python API 0.3.0. [documents](https://db-gpt.readthedocs.io/en/latest/getting_started/installation.html) 
+- [2023/07/06]🔥🔥🔥Brand-new DB-GPT product with a brand-new web UI. [documents](https://db-gpt.readthedocs.io/en/latest/getting_started/getting_started.html) 
+- [2023/06/25]🔥support chatglm2-6b model. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
+- [2023/06/14] support gpt4all model, which can run at M1/M2, or cpu machine. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
+- [2023/06/01]🔥 On the basis of the Vicuna-13B basic model, task chain calls are implemented through plugins. For example, the implementation of creating a database with a single sentence.[demo](./assets/auto_plugin.gif)
+- [2023/06/01]🔥 QLoRA guanaco(7b, 13b, 33b) support.
+- [2023/05/28] Learning from crawling data from the Internet [demo](./assets/dbgpt_demo.gif)
+- [2023/05/21] Generate SQL and execute it automatically. [demo](./assets/chat-data.gif)
+- [2023/05/15] Chat with documents. [demo](./assets/new_knownledge_en.gif)
+- [2023/05/06] SQL generation and diagnosis. [demo](./assets/demo_en.gif)
 
 ## Features
 
 Currently, we have released multiple key features, which are listed below to demonstrate our current capabilities:
 
 - SQL language capabilities
   - SQL generation
@@ -83,15 +109,14 @@
   - TODO: codegen2, codet5p
 
 
 ## Introduction 
 DB-GPT creates a vast model operating system using [FastChat](https://github.com/lm-sys/FastChat) and offers a large language model powered by [Vicuna](https://huggingface.co/Tribbiani/vicuna-7b). In addition, we provide private domain knowledge base question-answering capability. Furthermore, we also provide support for additional plugins, and our design natively supports the Auto-GPT plugin.Our vision is to make it easier and more convenient to build  applications around databases and llm.
 
 
-
 Is the architecture of the entire DB-GPT shown in the following figure:
 
 <p align="center">
   <img src="./assets/DB-GPT.png" width="800" />
 </p>
 
 The core capabilities mainly consist of the following parts:
@@ -134,16 +159,22 @@
 - [ChatGLM](https://github.com/THUDM/ChatGLM-6B) as the base model
 - [llama_index](https://github.com/jerryjliu/llama_index) for enhancing database-related knowledge using [in-context learning](https://arxiv.org/abs/2301.00234) based on existing knowledge bases.
 
 ## Contribution
 
 - Please run `black .` before submitting the code.
 
+## RoadMap
+
+<p align="left">
+  <img src="./assets/roadmap.jpg" width="800px" />
+</p>
+
 ## Licence
 
 The MIT License (MIT)
 
 ## Contact Information
 We are working on building a community, if you have any ideas about building the community, feel free to contact us. [Discord](https://discord.gg/4BNdxm5d)
 
-[![Star History Chart](https://api.star-history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
+
```

#### html2text {}

```diff
@@ -1,70 +1,76 @@
-Metadata-Version: 2.1 Name: db-gpt Version: 0.2.8 Summary: DB-GPT is an
+Metadata-Version: 2.1 Name: db-gpt Version: 0.3.0 Summary: DB-GPT is an
 experimental open-source project that uses localized GPT large models to
 interact with your data and environment. With this solution, you can be assured
 that there is no risk of data leakage, and your data is 100% private and
 secure. Home-page: https://github.com/csunny/DB-GPT Author: csunny Author-
 email: cfqcsunny@gmail.com License: https://opensource.org/license/mit/
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # DB-GPT: Revolutionizing Database Interactions with Private LLM
 Technology
                                 [stars] [forks]
   [**ç®ä½ä¸­æ**](README.zh.md) |[**Discord**](https://discord.com/invite/
      EUEBmdpd) |[**Documents**](https://db-gpt.readthedocs.io/en/latest/)|
            [**Wechat**](https://github.com/csunny/DB-GPT/blob/main/
               README.zh.md#%E8%81%94%E7%B3%BB%E6%88%91%E4%BB%AC)
-## What is DB-GPT? As large models are released and iterated upon, they are
-becoming increasingly intelligent. However, in the process of using large
-models, we face significant challenges in data security and privacy. We need to
-ensure that our sensitive data and environments remain completely controlled
-and avoid any data privacy leaks or security risks. Based on this, we have
-launched the DB-GPT project to build a complete private large model solution
-for all database-based scenarios. This solution supports local deployment,
-allowing it to be applied not only in independent private environments but also
-to be independently deployed and isolated according to business modules,
-ensuring that the ability of large models is absolutely private, secure, and
-controllable. DB-GPT is an experimental open-source project that uses localized
-GPT large models to interact with your data and environment. With this
-solution, you can be assured that there is no risk of data leakage, and your
-data is 100% private and secure. ## News - [2023/07/06]ð¥ð¥ð¥Brand-new
-DB-GPT product with a brand-new web UI. [documents](https://db-
-gpt.readthedocs.io/en/latest/getting_started/getting_started.html) - [2023/06/
-25]ð¥support chatglm2-6b model. [documents](https://db-gpt.readthedocs.io/en/
-latest/modules/llms.html) - [2023/06/14] support gpt4all model, which can run
-at M1/M2, or cpu machine. [documents](https://db-gpt.readthedocs.io/en/latest/
-modules/llms.html) - [2023/06/01]ð¥ On the basis of the Vicuna-13B basic
-model, task chain calls are implemented through plugins. For example, the
-implementation of creating a database with a single sentence.[demo](./assets/
-auto_plugin.gif) - [2023/06/01]ð¥ QLoRA guanaco(7b, 13b, 33b) support. -
-[2023/05/28] Learning from crawling data from the Internet [demo](./assets/
-dbgpt_demo.gif) - [2023/05/21] Generate SQL and execute it automatically.
-[demo](./assets/chat-data.gif) - [2023/05/15] Chat with documents. [demo](./
-assets/new_knownledge_en.gif) - [2023/05/06] SQL generation and diagnosis.
-[demo](./assets/demo_en.gif) ## Demo Run on an RTX 4090 GPU.
-[./assets/dbgpt_demo.gif]
- ## Features Currently, we have released multiple key features, which are
-listed below to demonstrate our current capabilities: - SQL language
-capabilities - SQL generation - SQL diagnosis - Private domain Q&A and data
-processing - Knowledge Management(We currently support many document formats:
-txt, pdf, md, html, doc, ppt, and url.) - Database knowledge Q&A - knowledge
-Embedding - Plugins - Support custom plugin execution tasks and natively
-support the Auto-GPT plugin, such as: - Automatic execution of SQL and
-retrieval of query results - Automatic crawling and learning of knowledge -
-Unified vector storage/indexing of knowledge base - Support for unstructured
-data such as PDF, TXT, Markdown, CSV, DOC, PPT, and WebURL - Multi LLMs Support
-- Supports multiple large language models, currently supporting Vicuna (7b,
-13b), ChatGLM-6b (int4, int8), guanaco(7b,13b,33b), Gorilla(7b,13b) - TODO:
-codegen2, codet5p ## Introduction DB-GPT creates a vast model operating system
-using [FastChat](https://github.com/lm-sys/FastChat) and offers a large
-language model powered by [Vicuna](https://huggingface.co/Tribbiani/vicuna-7b).
-In addition, we provide private domain knowledge base question-answering
-capability. Furthermore, we also provide support for additional plugins, and
-our design natively supports the Auto-GPT plugin.Our vision is to make it
-easier and more convenient to build applications around databases and llm. Is
-the architecture of the entire DB-GPT shown in the following figure:
+## What is DB-GPT? DB-GPT is an experimental open-source project that uses
+localized GPT large models to interact with your data and environment. With
+this solution, you can be assured that there is no risk of data leakage, and
+your data is 100% private and secure. [![Star History Chart](https://api.star-
+history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
+## Demo Run on an RTX 4090 GPU. https://github.com/csunny/DB-GPT/assets/
+13723926/55f31781-1d49-4757-b96e-7ef6d3dbcf80  #### Chat with data, and figure
+charts.
+[./assets/dashboard.png]
+#### Text2SQL, generate SQL from chat
+[./assets/chatSQL.png]
+#### Chat with database meta information.
+[./assets/chatdb.png]
+#### Chat with data, and execute results.
+[./assets/chatdata.png]
+#### Knownledge space to manage docs.
+[./assets/ks.png]
+#### Chat with knowledge, such as txtãpdfãcsvãwords. etc
+[./assets/chat_knowledge.png]
+## Releases - [2023/07/12]ð¥ð¥ð¥DB-GPT Python API 0.3.0. [documents]
+(https://db-gpt.readthedocs.io/en/latest/getting_started/installation.html) -
+[2023/07/06]ð¥ð¥ð¥Brand-new DB-GPT product with a brand-new web UI.
+[documents](https://db-gpt.readthedocs.io/en/latest/getting_started/
+getting_started.html) - [2023/06/25]ð¥support chatglm2-6b model. [documents]
+(https://db-gpt.readthedocs.io/en/latest/modules/llms.html) - [2023/06/14]
+support gpt4all model, which can run at M1/M2, or cpu machine. [documents]
+(https://db-gpt.readthedocs.io/en/latest/modules/llms.html) - [2023/06/01]ð¥
+On the basis of the Vicuna-13B basic model, task chain calls are implemented
+through plugins. For example, the implementation of creating a database with a
+single sentence.[demo](./assets/auto_plugin.gif) - [2023/06/01]ð¥ QLoRA
+guanaco(7b, 13b, 33b) support. - [2023/05/28] Learning from crawling data from
+the Internet [demo](./assets/dbgpt_demo.gif) - [2023/05/21] Generate SQL and
+execute it automatically. [demo](./assets/chat-data.gif) - [2023/05/15] Chat
+with documents. [demo](./assets/new_knownledge_en.gif) - [2023/05/06] SQL
+generation and diagnosis. [demo](./assets/demo_en.gif) ## Features Currently,
+we have released multiple key features, which are listed below to demonstrate
+our current capabilities: - SQL language capabilities - SQL generation - SQL
+diagnosis - Private domain Q&A and data processing - Knowledge Management(We
+currently support many document formats: txt, pdf, md, html, doc, ppt, and
+url.) - Database knowledge Q&A - knowledge Embedding - Plugins - Support custom
+plugin execution tasks and natively support the Auto-GPT plugin, such as: -
+Automatic execution of SQL and retrieval of query results - Automatic crawling
+and learning of knowledge - Unified vector storage/indexing of knowledge base -
+Support for unstructured data such as PDF, TXT, Markdown, CSV, DOC, PPT, and
+WebURL - Multi LLMs Support - Supports multiple large language models,
+currently supporting Vicuna (7b, 13b), ChatGLM-6b (int4, int8), guanaco
+(7b,13b,33b), Gorilla(7b,13b) - TODO: codegen2, codet5p ## Introduction DB-GPT
+creates a vast model operating system using [FastChat](https://github.com/lm-
+sys/FastChat) and offers a large language model powered by [Vicuna](https://
+huggingface.co/Tribbiani/vicuna-7b). In addition, we provide private domain
+knowledge base question-answering capability. Furthermore, we also provide
+support for additional plugins, and our design natively supports the Auto-GPT
+plugin.Our vision is to make it easier and more convenient to build
+applications around databases and llm. Is the architecture of the entire DB-GPT
+shown in the following figure:
                              [./assets/DB-GPT.png]
 The core capabilities mainly consist of the following parts: 1. Knowledge base
 capability: Supports private domain knowledge base question-answering
 capability. 2. Large-scale model management capability: Provides a large model
 operating environment based on FastChat. 3. Unified data vector storage and
 indexing: Provides a uniform way to store and index various data types. 4.
 Connection module: Used to connect different modules and data sources to
@@ -91,12 +97,12 @@
 Significant-Gravitas/Auto-GPT) universal plugin template - [Hugging Face]
 (https://huggingface.co/) for big model management - [Chroma](https://
 github.com/chroma-core/chroma) for vector storage - [Milvus](https://milvus.io/
 ) for distributed vector storage - [ChatGLM](https://github.com/THUDM/ChatGLM-
 6B) as the base model - [llama_index](https://github.com/jerryjliu/llama_index)
 for enhancing database-related knowledge using [in-context learning](https://
 arxiv.org/abs/2301.00234) based on existing knowledge bases. ## Contribution -
-Please run `black .` before submitting the code. ## Licence The MIT License
-(MIT) ## Contact Information We are working on building a community, if you
-have any ideas about building the community, feel free to contact us. [Discord]
-(https://discord.gg/4BNdxm5d) [![Star History Chart](https://api.star-
-history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
+Please run `black .` before submitting the code. ## RoadMap
+[./assets/roadmap.jpg]
+## Licence The MIT License (MIT) ## Contact Information We are working on
+building a community, if you have any ideas about building the community, feel
+free to contact us. [Discord](https://discord.gg/4BNdxm5d)
```

### Comparing `db-gpt-0.2.8/README.md` & `db-gpt-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,45 +12,71 @@
 
 [**简体中文**](README.zh.md) |[**Discord**](https://discord.com/invite/EUEBmdpd) |[**Documents**](https://db-gpt.readthedocs.io/en/latest/)|[**Wechat**](https://github.com/csunny/DB-GPT/blob/main/README.zh.md#%E8%81%94%E7%B3%BB%E6%88%91%E4%BB%AC) 
 
 </div>
 
 ## What is DB-GPT?
 
-As large models are released and iterated upon, they are becoming increasingly intelligent. However, in the process of using large models, we face significant challenges in data security and privacy. We need to ensure that our sensitive data and environments remain completely controlled and avoid any data privacy leaks or security risks. Based on this, we have launched the DB-GPT project to build a complete private large model solution for all database-based scenarios. This solution supports local deployment, allowing it to be applied not only in independent private environments but also to be independently deployed and isolated according to business modules, ensuring that the ability of large models is absolutely private, secure, and controllable.
-
 DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 
-## News
-- [2023/07/06]🔥🔥🔥Brand-new DB-GPT product with a brand-new web UI. [documents](https://db-gpt.readthedocs.io/en/latest/getting_started/getting_started.html) 
-- [2023/06/25]🔥support chatglm2-6b model. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
-- [2023/06/14] support gpt4all model, which can run at M1/M2, or cpu machine. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
-- [2023/06/01]🔥 On the basis of the Vicuna-13B basic model, task chain calls are implemented through plugins. For example, the implementation of creating a database with a single sentence.[demo](./assets/auto_plugin.gif)
-- [2023/06/01]🔥 QLoRA guanaco(7b, 13b, 33b) support.
-- [2023/05/28] Learning from crawling data from the Internet [demo](./assets/dbgpt_demo.gif)
-- [2023/05/21] Generate SQL and execute it automatically. [demo](./assets/chat-data.gif)
-- [2023/05/15] Chat with documents. [demo](./assets/new_knownledge_en.gif)
-- [2023/05/06] SQL generation and diagnosis. [demo](./assets/demo_en.gif)
+[![Star History Chart](https://api.star-history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
 
 ## Demo
 
 Run on an RTX 4090 GPU.
 
-<p align="left">
-  <img src="./assets/dbgpt_demo.gif" width="800px" />
-</p>
-
+https://github.com/csunny/DB-GPT/assets/13723926/55f31781-1d49-4757-b96e-7ef6d3dbcf80
 
 <!-- <video id="video" controls="" preload="auto" poster="assets/exector_sql.png">
       <source id="mp4" src="https://github.com/csunny/DB-GPT/assets/17919400/654b5a49-5ea4-4c02-b5b2-72d089dcc1f0" type="video/mp4">
 </videos> -->
 
 
+#### Chat with data, and figure charts.
+
+<p align="left">
+  <img src="./assets/dashboard.png" width="800px" />
+</p>
+
+#### Text2SQL, generate SQL from chat
+<p align="left">
+  <img src="./assets/chatSQL.png" width="800px" />
+</p>
 
+#### Chat with database meta information.
+<p align="left">
+  <img src="./assets/chatdb.png" width="800px" />
+</p>
 
+#### Chat with data, and execute results.
+<p align="left">
+  <img src="./assets/chatdata.png" width="800px" />
+</p>
+
+#### Knownledge space to manage docs.
+<p align="left">
+  <img src="./assets/ks.png" width="800px" />
+</p>
+
+#### Chat with knowledge, such as txt、pdf、csv、words. etc
+<p align="left">
+  <img src="./assets/chat_knowledge.png" width="800px" />
+</p>
+
+## Releases 
+- [2023/07/12]🔥🔥🔥DB-GPT Python API 0.3.0. [documents](https://db-gpt.readthedocs.io/en/latest/getting_started/installation.html) 
+- [2023/07/06]🔥🔥🔥Brand-new DB-GPT product with a brand-new web UI. [documents](https://db-gpt.readthedocs.io/en/latest/getting_started/getting_started.html) 
+- [2023/06/25]🔥support chatglm2-6b model. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
+- [2023/06/14] support gpt4all model, which can run at M1/M2, or cpu machine. [documents](https://db-gpt.readthedocs.io/en/latest/modules/llms.html) 
+- [2023/06/01]🔥 On the basis of the Vicuna-13B basic model, task chain calls are implemented through plugins. For example, the implementation of creating a database with a single sentence.[demo](./assets/auto_plugin.gif)
+- [2023/06/01]🔥 QLoRA guanaco(7b, 13b, 33b) support.
+- [2023/05/28] Learning from crawling data from the Internet [demo](./assets/dbgpt_demo.gif)
+- [2023/05/21] Generate SQL and execute it automatically. [demo](./assets/chat-data.gif)
+- [2023/05/15] Chat with documents. [demo](./assets/new_knownledge_en.gif)
+- [2023/05/06] SQL generation and diagnosis. [demo](./assets/demo_en.gif)
 
 ## Features
 
 Currently, we have released multiple key features, which are listed below to demonstrate our current capabilities:
 
 - SQL language capabilities
   - SQL generation
@@ -71,15 +97,14 @@
   - TODO: codegen2, codet5p
 
 
 ## Introduction 
 DB-GPT creates a vast model operating system using [FastChat](https://github.com/lm-sys/FastChat) and offers a large language model powered by [Vicuna](https://huggingface.co/Tribbiani/vicuna-7b). In addition, we provide private domain knowledge base question-answering capability. Furthermore, we also provide support for additional plugins, and our design natively supports the Auto-GPT plugin.Our vision is to make it easier and more convenient to build  applications around databases and llm.
 
 
-
 Is the architecture of the entire DB-GPT shown in the following figure:
 
 <p align="center">
   <img src="./assets/DB-GPT.png" width="800" />
 </p>
 
 The core capabilities mainly consist of the following parts:
@@ -122,16 +147,22 @@
 - [ChatGLM](https://github.com/THUDM/ChatGLM-6B) as the base model
 - [llama_index](https://github.com/jerryjliu/llama_index) for enhancing database-related knowledge using [in-context learning](https://arxiv.org/abs/2301.00234) based on existing knowledge bases.
 
 ## Contribution
 
 - Please run `black .` before submitting the code.
 
+## RoadMap
+
+<p align="left">
+  <img src="./assets/roadmap.jpg" width="800px" />
+</p>
+
 ## Licence
 
 The MIT License (MIT)
 
 ## Contact Information
 We are working on building a community, if you have any ideas about building the community, feel free to contact us. [Discord](https://discord.gg/4BNdxm5d)
 
-[![Star History Chart](https://api.star-history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
+
```

#### html2text {}

```diff
@@ -1,62 +1,68 @@
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
                                 [stars] [forks]
   [**ç®ä½ä¸­æ**](README.zh.md) |[**Discord**](https://discord.com/invite/
      EUEBmdpd) |[**Documents**](https://db-gpt.readthedocs.io/en/latest/)|
            [**Wechat**](https://github.com/csunny/DB-GPT/blob/main/
               README.zh.md#%E8%81%94%E7%B3%BB%E6%88%91%E4%BB%AC)
-## What is DB-GPT? As large models are released and iterated upon, they are
-becoming increasingly intelligent. However, in the process of using large
-models, we face significant challenges in data security and privacy. We need to
-ensure that our sensitive data and environments remain completely controlled
-and avoid any data privacy leaks or security risks. Based on this, we have
-launched the DB-GPT project to build a complete private large model solution
-for all database-based scenarios. This solution supports local deployment,
-allowing it to be applied not only in independent private environments but also
-to be independently deployed and isolated according to business modules,
-ensuring that the ability of large models is absolutely private, secure, and
-controllable. DB-GPT is an experimental open-source project that uses localized
-GPT large models to interact with your data and environment. With this
-solution, you can be assured that there is no risk of data leakage, and your
-data is 100% private and secure. ## News - [2023/07/06]ð¥ð¥ð¥Brand-new
-DB-GPT product with a brand-new web UI. [documents](https://db-
-gpt.readthedocs.io/en/latest/getting_started/getting_started.html) - [2023/06/
-25]ð¥support chatglm2-6b model. [documents](https://db-gpt.readthedocs.io/en/
-latest/modules/llms.html) - [2023/06/14] support gpt4all model, which can run
-at M1/M2, or cpu machine. [documents](https://db-gpt.readthedocs.io/en/latest/
-modules/llms.html) - [2023/06/01]ð¥ On the basis of the Vicuna-13B basic
-model, task chain calls are implemented through plugins. For example, the
-implementation of creating a database with a single sentence.[demo](./assets/
-auto_plugin.gif) - [2023/06/01]ð¥ QLoRA guanaco(7b, 13b, 33b) support. -
-[2023/05/28] Learning from crawling data from the Internet [demo](./assets/
-dbgpt_demo.gif) - [2023/05/21] Generate SQL and execute it automatically.
-[demo](./assets/chat-data.gif) - [2023/05/15] Chat with documents. [demo](./
-assets/new_knownledge_en.gif) - [2023/05/06] SQL generation and diagnosis.
-[demo](./assets/demo_en.gif) ## Demo Run on an RTX 4090 GPU.
-[./assets/dbgpt_demo.gif]
- ## Features Currently, we have released multiple key features, which are
-listed below to demonstrate our current capabilities: - SQL language
-capabilities - SQL generation - SQL diagnosis - Private domain Q&A and data
-processing - Knowledge Management(We currently support many document formats:
-txt, pdf, md, html, doc, ppt, and url.) - Database knowledge Q&A - knowledge
-Embedding - Plugins - Support custom plugin execution tasks and natively
-support the Auto-GPT plugin, such as: - Automatic execution of SQL and
-retrieval of query results - Automatic crawling and learning of knowledge -
-Unified vector storage/indexing of knowledge base - Support for unstructured
-data such as PDF, TXT, Markdown, CSV, DOC, PPT, and WebURL - Multi LLMs Support
-- Supports multiple large language models, currently supporting Vicuna (7b,
-13b), ChatGLM-6b (int4, int8), guanaco(7b,13b,33b), Gorilla(7b,13b) - TODO:
-codegen2, codet5p ## Introduction DB-GPT creates a vast model operating system
-using [FastChat](https://github.com/lm-sys/FastChat) and offers a large
-language model powered by [Vicuna](https://huggingface.co/Tribbiani/vicuna-7b).
-In addition, we provide private domain knowledge base question-answering
-capability. Furthermore, we also provide support for additional plugins, and
-our design natively supports the Auto-GPT plugin.Our vision is to make it
-easier and more convenient to build applications around databases and llm. Is
-the architecture of the entire DB-GPT shown in the following figure:
+## What is DB-GPT? DB-GPT is an experimental open-source project that uses
+localized GPT large models to interact with your data and environment. With
+this solution, you can be assured that there is no risk of data leakage, and
+your data is 100% private and secure. [![Star History Chart](https://api.star-
+history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
+## Demo Run on an RTX 4090 GPU. https://github.com/csunny/DB-GPT/assets/
+13723926/55f31781-1d49-4757-b96e-7ef6d3dbcf80  #### Chat with data, and figure
+charts.
+[./assets/dashboard.png]
+#### Text2SQL, generate SQL from chat
+[./assets/chatSQL.png]
+#### Chat with database meta information.
+[./assets/chatdb.png]
+#### Chat with data, and execute results.
+[./assets/chatdata.png]
+#### Knownledge space to manage docs.
+[./assets/ks.png]
+#### Chat with knowledge, such as txtãpdfãcsvãwords. etc
+[./assets/chat_knowledge.png]
+## Releases - [2023/07/12]ð¥ð¥ð¥DB-GPT Python API 0.3.0. [documents]
+(https://db-gpt.readthedocs.io/en/latest/getting_started/installation.html) -
+[2023/07/06]ð¥ð¥ð¥Brand-new DB-GPT product with a brand-new web UI.
+[documents](https://db-gpt.readthedocs.io/en/latest/getting_started/
+getting_started.html) - [2023/06/25]ð¥support chatglm2-6b model. [documents]
+(https://db-gpt.readthedocs.io/en/latest/modules/llms.html) - [2023/06/14]
+support gpt4all model, which can run at M1/M2, or cpu machine. [documents]
+(https://db-gpt.readthedocs.io/en/latest/modules/llms.html) - [2023/06/01]ð¥
+On the basis of the Vicuna-13B basic model, task chain calls are implemented
+through plugins. For example, the implementation of creating a database with a
+single sentence.[demo](./assets/auto_plugin.gif) - [2023/06/01]ð¥ QLoRA
+guanaco(7b, 13b, 33b) support. - [2023/05/28] Learning from crawling data from
+the Internet [demo](./assets/dbgpt_demo.gif) - [2023/05/21] Generate SQL and
+execute it automatically. [demo](./assets/chat-data.gif) - [2023/05/15] Chat
+with documents. [demo](./assets/new_knownledge_en.gif) - [2023/05/06] SQL
+generation and diagnosis. [demo](./assets/demo_en.gif) ## Features Currently,
+we have released multiple key features, which are listed below to demonstrate
+our current capabilities: - SQL language capabilities - SQL generation - SQL
+diagnosis - Private domain Q&A and data processing - Knowledge Management(We
+currently support many document formats: txt, pdf, md, html, doc, ppt, and
+url.) - Database knowledge Q&A - knowledge Embedding - Plugins - Support custom
+plugin execution tasks and natively support the Auto-GPT plugin, such as: -
+Automatic execution of SQL and retrieval of query results - Automatic crawling
+and learning of knowledge - Unified vector storage/indexing of knowledge base -
+Support for unstructured data such as PDF, TXT, Markdown, CSV, DOC, PPT, and
+WebURL - Multi LLMs Support - Supports multiple large language models,
+currently supporting Vicuna (7b, 13b), ChatGLM-6b (int4, int8), guanaco
+(7b,13b,33b), Gorilla(7b,13b) - TODO: codegen2, codet5p ## Introduction DB-GPT
+creates a vast model operating system using [FastChat](https://github.com/lm-
+sys/FastChat) and offers a large language model powered by [Vicuna](https://
+huggingface.co/Tribbiani/vicuna-7b). In addition, we provide private domain
+knowledge base question-answering capability. Furthermore, we also provide
+support for additional plugins, and our design natively supports the Auto-GPT
+plugin.Our vision is to make it easier and more convenient to build
+applications around databases and llm. Is the architecture of the entire DB-GPT
+shown in the following figure:
                              [./assets/DB-GPT.png]
 The core capabilities mainly consist of the following parts: 1. Knowledge base
 capability: Supports private domain knowledge base question-answering
 capability. 2. Large-scale model management capability: Provides a large model
 operating environment based on FastChat. 3. Unified data vector storage and
 indexing: Provides a uniform way to store and index various data types. 4.
 Connection module: Used to connect different modules and data sources to
@@ -83,12 +89,12 @@
 Significant-Gravitas/Auto-GPT) universal plugin template - [Hugging Face]
 (https://huggingface.co/) for big model management - [Chroma](https://
 github.com/chroma-core/chroma) for vector storage - [Milvus](https://milvus.io/
 ) for distributed vector storage - [ChatGLM](https://github.com/THUDM/ChatGLM-
 6B) as the base model - [llama_index](https://github.com/jerryjliu/llama_index)
 for enhancing database-related knowledge using [in-context learning](https://
 arxiv.org/abs/2301.00234) based on existing knowledge bases. ## Contribution -
-Please run `black .` before submitting the code. ## Licence The MIT License
-(MIT) ## Contact Information We are working on building a community, if you
-have any ideas about building the community, feel free to contact us. [Discord]
-(https://discord.gg/4BNdxm5d) [![Star History Chart](https://api.star-
-history.com/svg?repos=csunny/DB-GPT)](https://star-history.com/#csunny/DB-GPT)
+Please run `black .` before submitting the code. ## RoadMap
+[./assets/roadmap.jpg]
+## Licence The MIT License (MIT) ## Contact Information We are working on
+building a community, if you have any ideas about building the community, feel
+free to contact us. [Discord](https://discord.gg/4BNdxm5d)
```

### Comparing `db-gpt-0.2.8/pilot/agent/agent_manager.py` & `db-gpt-0.3.0/pilot/agent/agent_manager.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/agent/json_fix_llm.py` & `db-gpt-0.3.0/pilot/agent/json_fix_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/commands/built_in/audio_text.py` & `db-gpt-0.3.0/pilot/commands/built_in/audio_text.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/commands/built_in/image_gen.py` & `db-gpt-0.3.0/pilot/commands/built_in/image_gen.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/commands/command.py` & `db-gpt-0.3.0/pilot/commands/command.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/commands/command_mange.py` & `db-gpt-0.3.0/pilot/commands/command_mange.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/common/custom_data_structure.py` & `db-gpt-0.3.0/pilot/common/custom_data_structure.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/common/formatting.py` & `db-gpt-0.3.0/pilot/common/formatting.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/common/markdown_text.py` & `db-gpt-0.3.0/pilot/common/markdown_text.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/common/plugins.py` & `db-gpt-0.3.0/pilot/common/plugins.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/common/sql_database.py` & `db-gpt-0.3.0/pilot/common/sql_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,15 +340,22 @@
     def get_database_list(self):
         session = self._db_sessions()
         cursor = session.execute(text(" show databases;"))
         results = cursor.fetchall()
         return [
             d[0]
             for d in results
-            if d[0] not in ["information_schema", "performance_schema", "sys", "mysql"]
+            if d[0]
+            not in [
+                "information_schema",
+                "performance_schema",
+                "sys",
+                "mysql",
+                "knowledge_management",
+            ]
         ]
 
     def convert_sql_write_to_select(self, write_sql):
         """
         SQL classification processing
         author:xiangh8
         Args:
@@ -417,15 +424,21 @@
         return [(index[2], index[4]) for index in indexes]
 
     def get_show_create_table(self, table_name):
         """Get table show create table about specified table."""
         session = self._db_sessions()
         cursor = session.execute(text(f"SHOW CREATE TABLE  {table_name}"))
         ans = cursor.fetchall()
-        return ans[0][1]
+        res = ans[0][1]
+        res = re.sub(r"\s*ENGINE\s*=\s*InnoDB\s*", " ", res, flags=re.IGNORECASE)
+        res = re.sub(
+            r"\s*DEFAULT\s*CHARSET\s*=\s*\w+\s*", " ", res, flags=re.IGNORECASE
+        )
+        res = re.sub(r"\s*COLLATE\s*=\s*\w+\s*", " ", res, flags=re.IGNORECASE)
+        return res
 
     def get_fields(self, table_name):
         """Get column fields about specified table."""
         session = self._db_sessions()
         cursor = session.execute(
             text(
                 f"SELECT COLUMN_NAME, COLUMN_TYPE, COLUMN_DEFAULT, IS_NULLABLE, COLUMN_COMMENT  from information_schema.COLUMNS where table_name='{table_name}'".format(
```

### Comparing `db-gpt-0.2.8/pilot/configs/config.py` & `db-gpt-0.3.0/pilot/configs/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         self.LANGUAGE = os.getenv("LANGUAGE", "en")
         self.WEB_SERVER_PORT = int(os.getenv("WEB_SERVER_PORT", 7860))
 
         self.debug_mode = False
         self.skip_reprompt = False
         self.temperature = float(os.getenv("TEMPERATURE", 0.7))
 
+        self.NUM_GPUS = int(os.getenv("NUM_GPUS", 1))
+
         self.execute_local_commands = (
             os.getenv("EXECUTE_LOCAL_COMMANDS", "False") == "True"
         )
         # User agent header to use when making HTTP requests
         # Some websites might just completely deny request with an error code if
         # no user agent was found.
         self.user_agent = os.getenv(
```

### Comparing `db-gpt-0.2.8/pilot/configs/model_config.py` & `db-gpt-0.3.0/pilot/configs/model_config.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/conversation.py` & `db-gpt-0.3.0/pilot/conversation.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/embedding_engine/EncodeTextLoader.py` & `db-gpt-0.3.0/pilot/embedding_engine/EncodeTextLoader.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/embedding_engine/chn_document_splitter.py` & `db-gpt-0.3.0/pilot/embedding_engine/chn_document_splitter.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/embedding_engine/knowledge_type.py` & `db-gpt-0.3.0/pilot/embedding_engine/knowledge_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,37 +36,45 @@
     HIVE = "HIVE"
     PRESTO = "PRESTO"
     KAFKA = "KAFKA"
     SPARK = "SPARK"
     YOUTUBE = "YOUTUBE"
 
 
-def get_knowledge_embedding(knowledge_type, knowledge_source, vector_store_config):
+def get_knowledge_embedding(
+    knowledge_type, knowledge_source, vector_store_config, source_reader, text_splitter
+):
     match knowledge_type:
         case KnowledgeType.DOCUMENT.value:
             extension = "." + knowledge_source.rsplit(".", 1)[-1]
             if extension in DocumentEmbeddingType:
                 knowledge_class, knowledge_args = DocumentEmbeddingType[extension]
                 embedding = knowledge_class(
                     knowledge_source,
                     vector_store_config=vector_store_config,
+                    source_reader=source_reader,
+                    text_splitter=text_splitter,
                     **knowledge_args,
                 )
                 return embedding
             raise ValueError(f"Unsupported knowledge document type '{extension}'")
         case KnowledgeType.URL.value:
             embedding = URLEmbedding(
                 file_path=knowledge_source,
                 vector_store_config=vector_store_config,
+                source_reader=source_reader,
+                text_splitter=text_splitter,
             )
             return embedding
         case KnowledgeType.TEXT.value:
             embedding = StringEmbedding(
                 file_path=knowledge_source,
                 vector_store_config=vector_store_config,
+                source_reader=source_reader,
+                text_splitter=text_splitter,
             )
             return embedding
         case KnowledgeType.OSS.value:
             raise Exception("OSS have not integrate")
         case KnowledgeType.S3.value:
             raise Exception("S3 have not integrate")
         case KnowledgeType.NOTION.value:
```

### Comparing `db-gpt-0.2.8/pilot/embedding_engine/pdf_embedding.py` & `db-gpt-0.3.0/pilot/embedding_engine/string_embedding.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from typing import List
+from typing import List, Optional
 
-from langchain.document_loaders import PyPDFLoader
 from langchain.schema import Document
-from langchain.text_splitter import SpacyTextSplitter, RecursiveCharacterTextSplitter
+from langchain.text_splitter import (
+    TextSplitter,
+    SpacyTextSplitter,
+    RecursiveCharacterTextSplitter,
+)
 
-from pilot.configs.config import Config
 from pilot.embedding_engine import SourceEmbedding, register
 
-CFG = Config()
 
+class StringEmbedding(SourceEmbedding):
+    """string embedding for read string document."""
 
-class PDFEmbedding(SourceEmbedding):
-    """pdf embedding for read pdf document."""
-
-    def __init__(self, file_path, vector_store_config):
-        """Initialize with pdf path."""
-        super().__init__(file_path, vector_store_config)
+    def __init__(
+        self,
+        file_path,
+        vector_store_config,
+        source_reader: Optional = None,
+        text_splitter: Optional[TextSplitter] = None,
+    ):
+        """Initialize raw text word path."""
+        super().__init__(
+            file_path=file_path,
+            vector_store_config=vector_store_config,
+            source_reader=None,
+            text_splitter=None,
+        )
         self.file_path = file_path
         self.vector_store_config = vector_store_config
+        self.source_reader = source_reader or None
+        self.text_splitter = text_splitter or None
 
     @register
     def read(self):
-        """Load from pdf path."""
-        loader = PyPDFLoader(self.file_path)
-        # textsplitter = CHNDocumentSplitter(
-        #     pdf=True, sentence_size=CFG.KNOWLEDGE_CHUNK_SIZE
-        # )
-        # textsplitter = SpacyTextSplitter(
-        #     pipeline="zh_core_web_sm",
-        #     chunk_size=CFG.KNOWLEDGE_CHUNK_SIZE,
-        #     chunk_overlap=100,
-        # )
-        if CFG.LANGUAGE == "en":
-            text_splitter = RecursiveCharacterTextSplitter(
-                chunk_size=CFG.KNOWLEDGE_CHUNK_SIZE,
-                chunk_overlap=20,
-                length_function=len,
-            )
-        else:
+        """Load from String path."""
+        metadata = {"source": "raw text"}
+        docs = [Document(page_content=self.file_path, metadata=metadata)]
+        if self.text_splitter is None:
             try:
-                text_splitter = SpacyTextSplitter(
+                self.text_splitter = SpacyTextSplitter(
                     pipeline="zh_core_web_sm",
-                    chunk_size=CFG.KNOWLEDGE_CHUNK_SIZE,
+                    chunk_size=500,
                     chunk_overlap=100,
                 )
             except Exception:
-                text_splitter = RecursiveCharacterTextSplitter(
-                    chunk_size=CFG.KNOWLEDGE_CHUNK_SIZE, chunk_overlap=50
+                self.text_splitter = RecursiveCharacterTextSplitter(
+                    chunk_size=100, chunk_overlap=50
                 )
-        return loader.load_and_split(text_splitter)
+            return self.text_splitter.split_documents(docs)
+        return docs
 
     @register
     def data_process(self, documents: List[Document]):
         i = 0
         for d in documents:
             documents[i].page_content = d.page_content.replace("\n", "")
             i += 1
```

### Comparing `db-gpt-0.2.8/pilot/embedding_engine/pdf_loader.py` & `db-gpt-0.3.0/pilot/embedding_engine/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/embedding_engine/search_milvus.py` & `db-gpt-0.3.0/pilot/embedding_engine/search_milvus.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/embedding_engine/source_embedding.py` & `db-gpt-0.3.0/pilot/embedding_engine/source_embedding.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from abc import ABC, abstractmethod
 from typing import Dict, List, Optional
 
 from chromadb.errors import NotEnoughElementsException
+from langchain.text_splitter import TextSplitter
+
 from pilot.vector_store.connector import VectorStoreConnector
 
 registered_methods = []
 
 
 def register(method):
     registered_methods.append(method.__name__)
@@ -19,35 +21,39 @@
     include data read, data process, data split, data to vector, data index vector store
     Implementations should implement the  method
     """
 
     def __init__(
         self,
         file_path,
-        vector_store_config,
+        vector_store_config: {},
+        source_reader: Optional = None,
+        text_splitter: Optional[TextSplitter] = None,
         embedding_args: Optional[Dict] = None,
     ):
         """Initialize with Loader url, model_name, vector_store_config"""
         self.file_path = file_path
         self.vector_store_config = vector_store_config
+        self.source_reader = source_reader or None
+        self.text_splitter = text_splitter or None
         self.embedding_args = embedding_args
         self.embeddings = vector_store_config["embeddings"]
 
     @abstractmethod
     @register
     def read(self) -> List[ABC]:
         """read datasource into document objects."""
 
     @register
     def data_process(self, text):
         """pre process data."""
 
     @register
-    def text_split(self, text):
-        """text split chunk"""
+    def text_splitter(self, text_splitter: TextSplitter):
+        """add text split chunk"""
         pass
 
     @register
     def text_to_vector(self, docs):
         """transform vector"""
         pass
```

### Comparing `db-gpt-0.2.8/pilot/embedding_engine/word_embedding.py` & `db-gpt-0.3.0/pilot/embedding_engine/pdf_embedding.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from typing import List
+from typing import List, Optional
 
-from langchain.document_loaders import UnstructuredWordDocumentLoader
+from langchain.document_loaders import PyPDFLoader
 from langchain.schema import Document
-from langchain.text_splitter import SpacyTextSplitter, RecursiveCharacterTextSplitter
+from langchain.text_splitter import (
+    SpacyTextSplitter,
+    RecursiveCharacterTextSplitter,
+    TextSplitter,
+)
 
-from pilot.configs.config import Config
 from pilot.embedding_engine import SourceEmbedding, register
 
-CFG = Config()
 
+class PDFEmbedding(SourceEmbedding):
+    """pdf embedding for read pdf document."""
 
-class WordEmbedding(SourceEmbedding):
-    """word embedding for read word document."""
-
-    def __init__(self, file_path, vector_store_config):
-        """Initialize with word path."""
-        super().__init__(file_path, vector_store_config)
+    def __init__(
+        self,
+        file_path,
+        vector_store_config,
+        source_reader: Optional = None,
+        text_splitter: Optional[TextSplitter] = None,
+    ):
+        """Initialize pdf word path."""
+        super().__init__(
+            file_path, vector_store_config, source_reader=None, text_splitter=None
+        )
         self.file_path = file_path
         self.vector_store_config = vector_store_config
+        self.source_reader = source_reader or None
+        self.text_splitter = text_splitter or None
 
     @register
     def read(self):
-        """Load from word path."""
-        loader = UnstructuredWordDocumentLoader(self.file_path)
-        if CFG.LANGUAGE == "en":
-            text_splitter = RecursiveCharacterTextSplitter(
-                chunk_size=CFG.KNOWLEDGE_CHUNK_SIZE,
-                chunk_overlap=20,
-                length_function=len,
-            )
-        else:
+        """Load from pdf path."""
+        if self.source_reader is None:
+            self.source_reader = PyPDFLoader(self.file_path)
+        if self.text_splitter is None:
             try:
-                text_splitter = SpacyTextSplitter(
+                self.text_splitter = SpacyTextSplitter(
                     pipeline="zh_core_web_sm",
-                    chunk_size=CFG.KNOWLEDGE_CHUNK_SIZE,
+                    chunk_size=100,
                     chunk_overlap=100,
                 )
             except Exception:
-                text_splitter = RecursiveCharacterTextSplitter(
-                    chunk_size=CFG.KNOWLEDGE_CHUNK_SIZE, chunk_overlap=50
+                self.text_splitter = RecursiveCharacterTextSplitter(
+                    chunk_size=100, chunk_overlap=50
                 )
-        return loader.load_and_split(text_splitter)
+
+        return self.source_reader.load_and_split(self.text_splitter)
 
     @register
     def data_process(self, documents: List[Document]):
         i = 0
         for d in documents:
             documents[i].page_content = d.page_content.replace("\n", "")
             i += 1
```

### Comparing `db-gpt-0.2.8/pilot/inference_parsers/base.py` & `db-gpt-0.3.0/pilot/inference_parsers/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/json_utils/json_fix_general.py` & `db-gpt-0.3.0/pilot/json_utils/json_fix_general.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/json_utils/utilities.py` & `db-gpt-0.3.0/pilot/json_utils/utilities.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/log/json_handler.py` & `db-gpt-0.3.0/pilot/log/json_handler.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/logs.py` & `db-gpt-0.3.0/pilot/logs.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/memory/chat_history/base.py` & `db-gpt-0.3.0/pilot/memory/chat_history/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/memory/chat_history/duckdb_history.py` & `db-gpt-0.3.0/pilot/memory/chat_history/duckdb_history.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/memory/chat_history/file_history.py` & `db-gpt-0.3.0/pilot/memory/chat_history/file_history.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/memory/chat_history/mem_history.py` & `db-gpt-0.3.0/pilot/memory/chat_history/mem_history.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/cache/base.py` & `db-gpt-0.3.0/pilot/model/cache/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/cache/disk_cache.py` & `db-gpt-0.3.0/pilot/model/cache/disk_cache.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/cache/gpt_cache.py` & `db-gpt-0.3.0/pilot/model/cache/gpt_cache.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/cache/memory_cache.py` & `db-gpt-0.3.0/pilot/model/cache/memory_cache.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/compression.py` & `db-gpt-0.3.0/pilot/model/compression.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/llm_out/chatglm_llm.py` & `db-gpt-0.3.0/pilot/model/llm_out/chatglm_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/llm_out/falcon_llm.py` & `db-gpt-0.3.0/pilot/model/llm_out/falcon_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/llm_out/gorilla_llm.py` & `db-gpt-0.3.0/pilot/model/llm_out/gorilla_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/llm_out/gpt4all_llm.py` & `db-gpt-0.3.0/pilot/model/llm_out/gpt4all_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/llm_out/guanaco_llm.py` & `db-gpt-0.3.0/pilot/model/llm_out/guanaco_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/llm_out/proxy_llm.py` & `db-gpt-0.3.0/pilot/model/llm_out/proxy_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/llm_out/vicuna_base_llm.py` & `db-gpt-0.3.0/pilot/model/llm_out/vicuna_base_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/llm_out/vicuna_llm.py` & `db-gpt-0.3.0/pilot/model/llm_out/vicuna_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/llm_utils.py` & `db-gpt-0.3.0/pilot/model/llm_utils.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/model/loader.py` & `db-gpt-0.3.0/pilot/model/loader.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/openapi/api_v1/api_v1.py` & `db-gpt-0.3.0/pilot/openapi/api_v1/api_v1.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/openapi/api_v1/api_view_model.py` & `db-gpt-0.3.0/pilot/openapi/api_v1/api_view_model.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/out_parser/base.py` & `db-gpt-0.3.0/pilot/out_parser/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/prompts/base.py` & `db-gpt-0.3.0/pilot/prompts/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/prompts/example_base.py` & `db-gpt-0.3.0/pilot/prompts/example_base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/prompts/generator.py` & `db-gpt-0.3.0/pilot/prompts/generator.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/prompts/prompt_new.py` & `db-gpt-0.3.0/pilot/prompts/prompt_new.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/prompts/prompt_template.py` & `db-gpt-0.3.0/pilot/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/base.py` & `db-gpt-0.3.0/pilot/scene/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/base_chat.py` & `db-gpt-0.3.0/pilot/scene/base_chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/base_message.py` & `db-gpt-0.3.0/pilot/scene/base_message.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_dashboard/chat.py` & `db-gpt-0.3.0/pilot/scene/chat_dashboard/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_dashboard/data_preparation/report_schma.py` & `db-gpt-0.3.0/pilot/scene/chat_dashboard/data_preparation/report_schma.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_dashboard/out_parser.py` & `db-gpt-0.3.0/pilot/scene/chat_dashboard/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_dashboard/prompt.py` & `db-gpt-0.3.0/pilot/scene/chat_dashboard/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/chat.py` & `db-gpt-0.3.0/pilot/scene/chat_db/auto_execute/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/example.py` & `db-gpt-0.3.0/pilot/scene/chat_db/auto_execute/example.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/out_parser.py` & `db-gpt-0.3.0/pilot/scene/chat_db/auto_execute/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/prompt.py` & `db-gpt-0.3.0/pilot/scene/chat_db/auto_execute/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/chat.py` & `db-gpt-0.3.0/pilot/scene/chat_db/professional_qa/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/out_parser.py` & `db-gpt-0.3.0/pilot/scene/chat_db/professional_qa/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/prompt.py` & `db-gpt-0.3.0/pilot/scene/chat_db/professional_qa/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_execution/chat.py` & `db-gpt-0.3.0/pilot/scene/chat_execution/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_execution/example.py` & `db-gpt-0.3.0/pilot/scene/chat_execution/example.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_execution/out_parser.py` & `db-gpt-0.3.0/pilot/scene/chat_execution/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_execution/prompt.py` & `db-gpt-0.3.0/pilot/scene/chat_execution/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_factory.py` & `db-gpt-0.3.0/pilot/scene/chat_factory.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/chat.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/custom/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/out_parser.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/custom/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/prompt.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/custom/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/default/chat.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/default/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/default/out_parser.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/default/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/default/prompt.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/default/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/chat.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/inner_db_summary/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/out_parser.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/inner_db_summary/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/prompt.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/inner_db_summary/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/url/chat.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/url/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/url/out_parser.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/url/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/url/prompt.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/url/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/chat.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/v1/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/out_parser.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/v1/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/prompt.py` & `db-gpt-0.3.0/pilot/scene/chat_knowledge/v1/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_normal/chat.py` & `db-gpt-0.3.0/pilot/scene/chat_normal/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_normal/out_parser.py` & `db-gpt-0.3.0/pilot/scene/chat_normal/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/chat_normal/prompt.py` & `db-gpt-0.3.0/pilot/scene/chat_normal/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/scene/message.py` & `db-gpt-0.3.0/pilot/scene/message.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/chat_adapter.py` & `db-gpt-0.3.0/pilot/server/chat_adapter.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/dbgpt_server.py` & `db-gpt-0.3.0/pilot/server/dbgpt_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import atexit
 import traceback
 import os
 import shutil
 import argparse
 import sys
 
 ROOT_PATH = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
@@ -32,15 +33,15 @@
 static_file_path = os.path.join(os.getcwd(), "server/static")
 
 
 CFG = Config()
 logger = build_logger("webserver", LOGDIR + "webserver.log")
 
 
-def signal_handler(sig, frame):
+def signal_handler():
     print("in order to avoid chroma db atexit problem")
     os._exit(0)
 
 
 def swagger_monkey_patch(*args, **kwargs):
     return get_swagger_ui_html(
         *args,
@@ -92,15 +93,14 @@
     parser.add_argument(
         "-light",
         "--light",
         default=False,
         action="store_true",
         help="enable light mode",
     )
-    signal.signal(signal.SIGINT, signal_handler)
 
     # init server config
     args = parser.parse_args()
     server_init(args)
 
     if not args.light:
         print("Model Unified Deployment Mode!")
@@ -110,7 +110,8 @@
         CFG.NEW_SERVER_MODE = True
     else:
         CFG.SERVER_LIGHT_MODE = True
 
     import uvicorn
 
     uvicorn.run(app, host="0.0.0.0", port=args.port)
+    signal.signal(signal.SIGINT, signal_handler())
```

### Comparing `db-gpt-0.2.8/pilot/server/gradio_css.py` & `db-gpt-0.3.0/pilot/server/gradio_css.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/gradio_patch.py` & `db-gpt-0.3.0/pilot/server/gradio_patch.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/knowledge/api.py` & `db-gpt-0.3.0/pilot/server/knowledge/api.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/knowledge/chunk_db.py` & `db-gpt-0.3.0/pilot/server/knowledge/chunk_db.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/knowledge/document_db.py` & `db-gpt-0.3.0/pilot/server/knowledge/document_db.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/knowledge/request/request.py` & `db-gpt-0.3.0/pilot/server/knowledge/request/request.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/knowledge/request/response.py` & `db-gpt-0.3.0/pilot/server/knowledge/request/response.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/knowledge/service.py` & `db-gpt-0.3.0/pilot/server/knowledge/service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import threading
 from datetime import datetime
 
+from langchain.text_splitter import RecursiveCharacterTextSplitter, SpacyTextSplitter
+
 from pilot.configs.config import Config
 from pilot.configs.model_config import LLM_MODEL_CONFIG, KNOWLEDGE_UPLOAD_ROOT_PATH
 from pilot.embedding_engine.embedding_engine import EmbeddingEngine
 from pilot.logs import logger
 from pilot.server.knowledge.chunk_db import (
     DocumentChunkEntity,
     DocumentChunkDao,
@@ -118,23 +120,42 @@
             if (
                 doc.status == SyncStatus.RUNNING.name
                 or doc.status == SyncStatus.FINISHED.name
             ):
                 raise Exception(
                     f" doc:{doc.doc_name} status is {doc.status}, can not sync"
                 )
+
+            if CFG.LANGUAGE == "en":
+                text_splitter = RecursiveCharacterTextSplitter(
+                    chunk_size=CFG.KNOWLEDGE_CHUNK_SIZE,
+                    chunk_overlap=20,
+                    length_function=len,
+                )
+            else:
+                try:
+                    text_splitter = SpacyTextSplitter(
+                        pipeline="zh_core_web_sm",
+                        chunk_size=CFG.KNOWLEDGE_CHUNK_SIZE,
+                        chunk_overlap=100,
+                    )
+                except Exception:
+                    text_splitter = RecursiveCharacterTextSplitter(
+                        chunk_size=CFG.KNOWLEDGE_CHUNK_SIZE, chunk_overlap=50
+                    )
             client = EmbeddingEngine(
                 knowledge_source=doc.content,
                 knowledge_type=doc.doc_type.upper(),
                 model_name=LLM_MODEL_CONFIG[CFG.EMBEDDING_MODEL],
                 vector_store_config={
                     "vector_store_name": space_name,
                     "vector_store_type": CFG.VECTOR_STORE_TYPE,
                     "chroma_persist_path": KNOWLEDGE_UPLOAD_ROOT_PATH,
                 },
+                text_splitter=text_splitter,
             )
             chunk_docs = client.read()
             # update document status
             doc.status = SyncStatus.RUNNING.name
             doc.chunk_size = len(chunk_docs)
             doc.gmt_modified = datetime.now()
             knowledge_document_dao.update_knowledge_document(doc)
```

### Comparing `db-gpt-0.2.8/pilot/server/knowledge/space_db.py` & `db-gpt-0.3.0/pilot/server/knowledge/space_db.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/llmserver.py` & `db-gpt-0.3.0/pilot/server/llmserver.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/vectordb_qa.py` & `db-gpt-0.3.0/pilot/server/vectordb_qa.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/webserver.py` & `db-gpt-0.3.0/pilot/server/webserver.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/server/webserver_base.py` & `db-gpt-0.3.0/pilot/server/webserver_base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/singleton.py` & `db-gpt-0.3.0/pilot/singleton.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/speech/base.py` & `db-gpt-0.3.0/pilot/speech/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/speech/brian.py` & `db-gpt-0.3.0/pilot/speech/brian.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/speech/eleven_labs.py` & `db-gpt-0.3.0/pilot/speech/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/speech/macos_tts.py` & `db-gpt-0.3.0/pilot/speech/macos_tts.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/speech/say.py` & `db-gpt-0.3.0/pilot/speech/say.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/summary/db_summary.py` & `db-gpt-0.3.0/pilot/summary/db_summary.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/summary/db_summary_client.py` & `db-gpt-0.3.0/pilot/summary/db_summary_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         ans = [d.page_content for d in table_docs]
         return ans
 
     def get_similar_tables(self, dbname, query, topk):
         """get user query related tables info"""
         vector_store_config = {
             "vector_store_name": dbname + "_summary",
+            "chroma_persist_path": KNOWLEDGE_UPLOAD_ROOT_PATH,
             "vector_store_type": CFG.VECTOR_STORE_TYPE,
             "chroma_persist_path": KNOWLEDGE_UPLOAD_ROOT_PATH,
         }
         knowledge_embedding_client = EmbeddingEngine(
             model_name=LLM_MODEL_CONFIG[CFG.EMBEDDING_MODEL],
             vector_store_config=vector_store_config,
         )
@@ -113,19 +114,19 @@
             related_tables = _get_llm_response(
                 query, dbname, table_docs[0].page_content
             )
         related_table_summaries = []
         for table in related_tables:
             vector_store_config = {
                 "vector_store_name": dbname + "_" + table + "_ts",
+                "chroma_persist_path": KNOWLEDGE_UPLOAD_ROOT_PATH,
                 "vector_store_type": CFG.VECTOR_STORE_TYPE,
                 "chroma_persist_path": KNOWLEDGE_UPLOAD_ROOT_PATH,
             }
             knowledge_embedding_client = EmbeddingEngine(
-                file_path="",
                 model_name=LLM_MODEL_CONFIG[CFG.EMBEDDING_MODEL],
                 vector_store_config=vector_store_config,
             )
             table_summery = knowledge_embedding_client.similar_search(query, 1)
             related_table_summaries.append(table_summery[0].page_content)
         return related_table_summaries
 
@@ -134,14 +135,16 @@
         dbs = db.get_database_list()
         for dbname in dbs:
             self.db_summary_embedding(dbname)
 
     def init_db_profile(self, db_summary_client, dbname, embeddings):
         profile_store_config = {
             "vector_store_name": dbname + "_profile",
+            "chroma_persist_path": KNOWLEDGE_UPLOAD_ROOT_PATH,
+            "vector_store_type": CFG.VECTOR_STORE_TYPE,
             "embeddings": embeddings,
         }
         embedding = StringEmbedding(
             file_path=db_summary_client.get_db_summery(),
             vector_store_config=profile_store_config,
         )
         if not embedding.vector_name_exist():
```

### Comparing `db-gpt-0.2.8/pilot/summary/mysql_db_summary.py` & `db-gpt-0.3.0/pilot/summary/mysql_db_summary.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/utils.py` & `db-gpt-0.3.0/pilot/utils.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/vector_store/chroma_store.py` & `db-gpt-0.3.0/pilot/vector_store/chroma_store.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/vector_store/extract_tovec.py` & `db-gpt-0.3.0/pilot/vector_store/extract_tovec.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/vector_store/file_loader.py` & `db-gpt-0.3.0/pilot/vector_store/file_loader.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/pilot/vector_store/milvus_store.py` & `db-gpt-0.3.0/pilot/vector_store/milvus_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 from typing import Any, Iterable, List, Optional, Tuple
 
 from langchain.docstore.document import Document
 from pymilvus import Collection, DataType, connections, utility
 
-from pilot.configs.config import Config
 from pilot.vector_store.vector_store_base import VectorStoreBase
 
 
-CFG = Config()
-
-
 class MilvusStore(VectorStoreBase):
     """Milvus database"""
 
     def __init__(self, ctx: {}) -> None:
         """init a milvus storage connection.
 
         Args:
             ctx ({}): MilvusStore global config.
         """
         # self.configure(cfg)
 
         connect_kwargs = {}
-        self.uri = CFG.MILVUS_URL
-        self.port = CFG.MILVUS_PORT
-        self.username = CFG.MILVUS_USERNAME
-        self.password = CFG.MILVUS_PASSWORD
+        self.uri = ctx.get("milvus_url", None)
+        self.port = ctx.get("milvus_port", None)
+        self.username = ctx.get("milvus_username", None)
+        self.password = ctx.get("milvus_password", None)
         self.collection_name = ctx.get("vector_store_name", None)
         self.secure = ctx.get("secure", None)
         self.embedding = ctx.get("embeddings", None)
         self.fields = []
         self.alias = "default"
 
         # use HNSW by default.
```

### Comparing `db-gpt-0.2.8/pilot/vector_store/weaviate_store.py` & `db-gpt-0.3.0/pilot/vector_store/weaviate_store.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.8/setup.py` & `db-gpt-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             if require.strip() and not require.startswith("#")
         ]
 
 
 setuptools.setup(
     name="db-gpt",
     packages=find_packages(),
-    version="0.2.8",
+    version="0.3.0",
     author="csunny",
     author_email="cfqcsunny@gmail.com",
     description="DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment."
     " With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=parse_requirements("requirements.txt"),
```

### Comparing `db-gpt-0.2.8/tests/unit/embedding_engine/test_url_embedding.py` & `db-gpt-0.3.0/tests/unit/embedding_engine/test_url_embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from pilot import EmbeddingEngine, KnowledgeType
 
 url = "https://db-gpt.readthedocs.io/en/latest/getting_started/getting_started.html"
 embedding_model = "text2vec"
 vector_store_type = "Chroma"
 chroma_persist_path = "your_persist_path"
 vector_store_config = {
-            "vector_store_name": url.replace(":", ""),
-            "vector_store_type": vector_store_type,
-            "chroma_persist_path": chroma_persist_path
-        }
-embedding_engine = EmbeddingEngine(knowledge_source=url, knowledge_type=KnowledgeType.URL.value, model_name=embedding_model, vector_store_config=vector_store_config)
+    "vector_store_name": url.replace(":", ""),
+    "vector_store_type": vector_store_type,
+    "chroma_persist_path": chroma_persist_path,
+}
+embedding_engine = EmbeddingEngine(
+    knowledge_source=url,
+    knowledge_type=KnowledgeType.URL.value,
+    model_name=embedding_model,
+    vector_store_config=vector_store_config,
+)
 
 # embedding url content to vector store
 embedding_engine.knowledge_embedding()
-
```

### Comparing `db-gpt-0.2.8/tests/unit/test_plugins.py` & `db-gpt-0.3.0/tests/unit/test_plugins.py`

 * *Files identical despite different names*

