# Comparing `tmp/llama_index-0.7.6.tar.gz` & `tmp/llama_index-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.7.6.tar", last modified: Wed Jul 12 17:39:44 2023, max compression
+gzip compressed data, was "llama_index-0.7.7.tar", last modified: Thu Jul 13 15:59:54 2023, max compression
```

## Comparing `llama_index-0.7.6.tar` & `llama_index-0.7.7.tar`

### file list

```diff
@@ -1,672 +1,672 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.424668 llama_index-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-12 17:39:23.000000 llama_index-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 17:39:23.000000 llama_index-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-12 17:39:44.420668 llama_index-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-12 17:39:23.000000 llama_index-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.320667 llama_index-0.7.6/llama_index/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.324668 llama_index-0.7.6/llama_index/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/context_retriever_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    18652 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/openai_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.324668 llama_index-0.7.6/llama_index/agent/react/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/react/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/react/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/react/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/react/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/react/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/react/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/retriever_openai_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/agent/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.324668 llama_index-0.7.6/llama_index/bridge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/bridge/langchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.324668 llama_index-0.7.6/llama_index/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/callbacks/aim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/callbacks/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/callbacks/token_counting.py
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/callbacks/wandb_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.328667 llama_index-0.7.6/llama_index/chat_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/chat_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/chat_engine/condense_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/chat_engine/react.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/chat_engine/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/chat_engine/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/chat_engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.328667 llama_index-0.7.6/llama_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.328667 llama_index-0.7.6/llama_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/data_structs/document_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/data_structs/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.328667 llama_index-0.7.6/llama_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/embeddings/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.332667 llama_index-0.7.6/llama_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/evaluation/guideline_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.332667 llama_index-0.7.6/llama_index/graph_stores/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/graph_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16582 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/graph_stores/nebulagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/graph_stores/registery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/graph_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/graph_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.332667 llama_index-0.7.6/llama_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14414 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.332667 llama_index-0.7.6/llama_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.332667 llama_index-0.7.6/llama_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.332667 llama_index-0.7.6/llama_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.332667 llama_index-0.7.6/llama_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.336668 llama_index-0.7.6/llama_index/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/document_summary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/document_summary/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.336668 llama_index-0.7.6/llama_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.336668 llama_index-0.7.6/llama_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.336668 llama_index-0.7.6/llama_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/knowledge_graph/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.336668 llama_index-0.7.6/llama_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.340668 llama_index-0.7.6/llama_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/postprocessor/cohere_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/postprocessor/llm_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/postprocessor/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/postprocessor/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.340668 llama_index-0.7.6/llama_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.340668 llama_index-0.7.6/llama_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/query/query_transform/feedback_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.344668 llama_index-0.7.6/llama_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/struct_store/json_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.344668 llama_index-0.7.6/llama_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/tree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.344668 llama_index-0.7.6/llama_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/vector_store/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.344668 llama_index-0.7.6/llama_index/indices/vector_store/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/vector_store/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.344668 llama_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/indices/vector_store/retrievers/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.344668 llama_index-0.7.6/llama_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.348668 llama_index-0.7.6/llama_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/langchain_helpers/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.348668 llama_index-0.7.6/llama_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/structured.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.348668 llama_index-0.7.6/llama_index/llm_predictor/vellum/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/vellum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/vellum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/vellum/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/vellum/prompt_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/vellum/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llm_predictor/vellum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.352668 llama_index-0.7.6/llama_index/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/anthropic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/azure_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/langchain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/llms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.352668 llama_index-0.7.6/llama_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.352668 llama_index-0.7.6/llama_index/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/memory/chat_memory_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/memory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.352668 llama_index-0.7.6/llama_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/node_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.352668 llama_index-0.7.6/llama_index/node_parser/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/node_parser/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/node_parser/extractors/metadata_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.356668 llama_index-0.7.6/llama_index/objects/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/objects/base_node_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/objects/table_node_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/objects/tool_node_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.356668 llama_index-0.7.6/llama_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/output_parsers/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/output_parsers/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/output_parsers/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/output_parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.356668 llama_index-0.7.6/llama_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.356668 llama_index-0.7.6/llama_index/program/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/base_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/guidance_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/llm_program.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/llm_prompt_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/openai_program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.356668 llama_index-0.7.6/llama_index/program/predefined/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/predefined/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/predefined/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.360668 llama_index-0.7.6/llama_index/program/predefined/evaporate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/predefined/evaporate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/predefined/evaporate/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/predefined/evaporate/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/program/predefined/evaporate/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.360668 llama_index-0.7.6/llama_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/choice_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/guidance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/prompt_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/prompts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.364668 llama_index-0.7.6/llama_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/citation_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.364668 llama_index-0.7.6/llama_index/query_engine/flare/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/flare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/flare/answer_inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/flare/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/flare/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/flare/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/pandas_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/retry_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/retry_source_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/sql_join_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/sql_vector_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/sub_question_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.364668 llama_index-0.7.6/llama_index/question_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/question_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/question_gen/guidance_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/question_gen/llm_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/question_gen/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/question_gen/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/question_gen/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.368668 llama_index-0.7.6/llama_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.368668 llama_index-0.7.6/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.372668 llama_index-0.7.6/llama_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/docs_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/epub_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/image_caption_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/image_vision_llm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/ipynb_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/markdown_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/mbox_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/slides_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/tabular_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/file/video_audio_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.372668 llama_index-0.7.6/llama_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.372668 llama_index-0.7.6/llama_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.372668 llama_index-0.7.6/llama_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/psychic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.376668 llama_index-0.7.6/llama_index/readers/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.376668 llama_index-0.7.6/llama_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.376668 llama_index-0.7.6/llama_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.376668 llama_index-0.7.6/llama_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.376668 llama_index-0.7.6/llama_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response/pprint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.380668 llama_index-0.7.6/llama_index/response_synthesizers/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/accumulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/compact_and_accumulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/compact_and_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/no_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/simple_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/tree_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/response_synthesizers/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.380668 llama_index-0.7.6/llama_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/retrievers/recursive_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.380668 llama_index-0.7.6/llama_index/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/selectors/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/selectors/pydantic_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/selectors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.380668 llama_index-0.7.6/llama_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.384668 llama_index-0.7.6/llama_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/docstore/dynamodb_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/docstore/redis_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.384668 llama_index-0.7.6/llama_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/index_store/dynamodb_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/index_store/redis_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.384668 llama_index-0.7.6/llama_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/kvstore/dynamodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/kvstore/redis_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/kvstore/s3_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.384668 llama_index-0.7.6/llama_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.388668 llama_index-0.7.6/llama_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/function_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/ondemand_loader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/query_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.388668 llama_index-0.7.6/llama_index/tools/tool_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/tool_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/tool_spec/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.388668 llama_index-0.7.6/llama_index/tools/tool_spec/load_and_search/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/tool_spec/load_and_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/tool_spec/load_and_search/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.388668 llama_index-0.7.6/llama_index/tools/tool_spec/notion/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/tool_spec/notion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/tool_spec/notion/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.388668 llama_index-0.7.6/llama_index/tools/tool_spec/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/tool_spec/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/tool_spec/slack/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.388668 llama_index-0.7.6/llama_index/tts/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tts/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/tts/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.396668 llama_index-0.7.6/llama_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/deeplake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.396668 llama_index-0.7.6/llama_index/vector_stores/docarray/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/docarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/docarray/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/docarray/hnsw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/docarray/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/lancedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)    17241 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/supabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/tair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/typesense.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-12 17:39:23.000000 llama_index-0.7.6/llama_index/vector_stores/weaviate_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.320667 llama_index-0.7.6/llama_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-12 17:39:44.000000 llama_index-0.7.6/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21410 2023-07-12 17:39:44.000000 llama_index-0.7.6/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:39:44.000000 llama_index-0.7.6/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 17:39:44.000000 llama_index-0.7.6/llama_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 17:39:44.000000 llama_index-0.7.6/llama_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-12 17:39:23.000000 llama_index-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:39:44.424668 llama_index-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-12 17:39:23.000000 llama_index-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.396668 llama_index-0.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.396668 llama_index-0.7.6/tests/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/callbacks/test_llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/callbacks/test_token_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.396668 llama_index-0.7.6/tests/chat_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/chat_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/chat_engine/test_condense_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/chat_engine/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.396668 llama_index-0.7.6/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.400668 llama_index-0.7.6/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.400668 llama_index-0.7.6/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.400668 llama_index-0.7.6/tests/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/document_summary/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/document_summary/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.400668 llama_index-0.7.6/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.400668 llama_index-0.7.6/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.400668 llama_index-0.7.6/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.400668 llama_index-0.7.6/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.404668 llama_index-0.7.6/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/postprocessor/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/postprocessor/test_llm_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/postprocessor/test_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.404668 llama_index-0.7.6/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.404668 llama_index-0.7.6/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/query/test_embedding_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.404668 llama_index-0.7.6/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/struct_store/test_json_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.404668 llama_index-0.7.6/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.408668 llama_index-0.7.6/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.408668 llama_index-0.7.6/tests/indices/vector_store/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/auto_retriever/test_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.408668 llama_index-0.7.6/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.408668 llama_index-0.7.6/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.408668 llama_index-0.7.6/tests/llm_predictor/vellum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llm_predictor/vellum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llm_predictor/vellum/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llm_predictor/vellum/test_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llm_predictor/vellum/test_prompt_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llm_predictor/vellum/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.412668 llama_index-0.7.6/tests/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llms/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llms/test_anthropic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llms/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llms/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llms/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llms/test_openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/llms/test_palm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.412668 llama_index-0.7.6/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.412668 llama_index-0.7.6/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.412668 llama_index-0.7.6/tests/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/objects/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/objects/test_node_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.412668 llama_index-0.7.6/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/output_parsers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/output_parsers/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/output_parsers/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/output_parsers/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.416668 llama_index-0.7.6/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.416668 llama_index-0.7.6/tests/program/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/program/test_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/program/test_llm_program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.416668 llama_index-0.7.6/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/prompts/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/prompts/test_guidance_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.416668 llama_index-0.7.6/tests/question_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/question_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/question_gen/test_guidance_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/question_gen/test_llm_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.416668 llama_index-0.7.6/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.416668 llama_index-0.7.6/tests/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.416668 llama_index-0.7.6/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.420668 llama_index-0.7.6/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/storage/docstore/test_dynamodb_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/storage/docstore/test_redis_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/storage/test_storage_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.420668 llama_index-0.7.6/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.420668 llama_index-0.7.6/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/tools/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/tools/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/tools/test_ondemand_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/tools/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.420668 llama_index-0.7.6/tests/tools/tool_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/tools/tool_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/tools/tool_spec/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:44.420668 llama_index-0.7.6/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/vector_stores/test_docarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/vector_stores/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/vector_stores/test_qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/vector_stores/test_tair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-12 17:39:23.000000 llama_index-0.7.6/tests/vector_stores/test_weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.155260 llama_index-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-13 15:59:37.000000 llama_index-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-13 15:59:37.000000 llama_index-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-13 15:59:54.155260 llama_index-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-13 15:59:37.000000 llama_index-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.099259 llama_index-0.7.7/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.099259 llama_index-0.7.7/llama_index/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/context_retriever_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/openai_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.099259 llama_index-0.7.7/llama_index/agent/react/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/react/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/react/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/react/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/react/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/react/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/react/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/retriever_openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/agent/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.099259 llama_index-0.7.7/llama_index/bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/bridge/langchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.099259 llama_index-0.7.7/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/callbacks/aim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/callbacks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/callbacks/token_counting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/callbacks/wandb_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.099259 llama_index-0.7.7/llama_index/chat_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/chat_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/chat_engine/condense_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/chat_engine/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/chat_engine/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/chat_engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.099259 llama_index-0.7.7/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.103260 llama_index-0.7.7/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/data_structs/document_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/data_structs/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.103260 llama_index-0.7.7/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.103260 llama_index-0.7.7/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/evaluation/guideline_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.103260 llama_index-0.7.7/llama_index/graph_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19697 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/graph_stores/nebulagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/graph_stores/registery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/graph_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/graph_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.103260 llama_index-0.7.7/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.103260 llama_index-0.7.7/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.103260 llama_index-0.7.7/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.103260 llama_index-0.7.7/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.103260 llama_index-0.7.7/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.107260 llama_index-0.7.7/llama_index/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/document_summary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/document_summary/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.107260 llama_index-0.7.7/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.107260 llama_index-0.7.7/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.107260 llama_index-0.7.7/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/knowledge_graph/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.107260 llama_index-0.7.7/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.107260 llama_index-0.7.7/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/postprocessor/cohere_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/postprocessor/llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/postprocessor/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/postprocessor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.107260 llama_index-0.7.7/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.107260 llama_index-0.7.7/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/query/query_transform/feedback_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.111260 llama_index-0.7.7/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/struct_store/json_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.111260 llama_index-0.7.7/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/tree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.111260 llama_index-0.7.7/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/vector_store/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.111260 llama_index-0.7.7/llama_index/indices/vector_store/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/vector_store/retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.111260 llama_index-0.7.7/llama_index/indices/vector_store/retrievers/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/indices/vector_store/retrievers/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.111260 llama_index-0.7.7/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.111260 llama_index-0.7.7/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/langchain_helpers/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.111260 llama_index-0.7.7/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.111260 llama_index-0.7.7/llama_index/llm_predictor/vellum/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/vellum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/vellum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/vellum/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/vellum/prompt_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/vellum/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llm_predictor/vellum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.115260 llama_index-0.7.7/llama_index/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/anthropic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/azure_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/langchain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/llms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.115260 llama_index-0.7.7/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.115260 llama_index-0.7.7/llama_index/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/memory/chat_memory_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/memory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.115260 llama_index-0.7.7/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/node_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.115260 llama_index-0.7.7/llama_index/node_parser/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/node_parser/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/node_parser/extractors/metadata_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.115260 llama_index-0.7.7/llama_index/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/objects/base_node_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/objects/table_node_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/objects/tool_node_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.115260 llama_index-0.7.7/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/output_parsers/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/output_parsers/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/output_parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.115260 llama_index-0.7.7/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.119260 llama_index-0.7.7/llama_index/program/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/base_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/guidance_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/llm_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/llm_prompt_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/openai_program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.119260 llama_index-0.7.7/llama_index/program/predefined/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/predefined/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/predefined/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.119260 llama_index-0.7.7/llama_index/program/predefined/evaporate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/predefined/evaporate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/predefined/evaporate/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/predefined/evaporate/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/program/predefined/evaporate/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.119260 llama_index-0.7.7/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/choice_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/guidance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/prompt_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/prompts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.119260 llama_index-0.7.7/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/citation_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.123260 llama_index-0.7.7/llama_index/query_engine/flare/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/flare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/flare/answer_inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/flare/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/flare/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/flare/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/knowledge_graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/pandas_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/retry_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/retry_source_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/sql_join_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/sql_vector_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/sub_question_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.123260 llama_index-0.7.7/llama_index/question_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/question_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/question_gen/guidance_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/question_gen/llm_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/question_gen/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/question_gen/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/question_gen/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.123260 llama_index-0.7.7/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.123260 llama_index-0.7.7/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.127260 llama_index-0.7.7/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/docs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/epub_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/image_caption_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/image_vision_llm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/ipynb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/markdown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/mbox_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/slides_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/tabular_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/file/video_audio_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.127260 llama_index-0.7.7/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.127260 llama_index-0.7.7/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.127260 llama_index-0.7.7/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/psychic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.127260 llama_index-0.7.7/llama_index/readers/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.127260 llama_index-0.7.7/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.127260 llama_index-0.7.7/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.127260 llama_index-0.7.7/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.127260 llama_index-0.7.7/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response/pprint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.131260 llama_index-0.7.7/llama_index/response_synthesizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/compact_and_accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/compact_and_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/no_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/simple_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/tree_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/response_synthesizers/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.131260 llama_index-0.7.7/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/retrievers/recursive_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.131260 llama_index-0.7.7/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/selectors/pydantic_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.131260 llama_index-0.7.7/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.131260 llama_index-0.7.7/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/docstore/dynamodb_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/docstore/redis_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.131260 llama_index-0.7.7/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/index_store/dynamodb_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/index_store/redis_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.131260 llama_index-0.7.7/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/kvstore/dynamodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/kvstore/redis_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/kvstore/s3_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.135260 llama_index-0.7.7/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.135260 llama_index-0.7.7/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/function_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/ondemand_loader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/query_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.135260 llama_index-0.7.7/llama_index/tools/tool_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/tool_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/tool_spec/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.135260 llama_index-0.7.7/llama_index/tools/tool_spec/load_and_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/tool_spec/load_and_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/tool_spec/load_and_search/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.135260 llama_index-0.7.7/llama_index/tools/tool_spec/notion/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/tool_spec/notion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/tool_spec/notion/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.135260 llama_index-0.7.7/llama_index/tools/tool_spec/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/tool_spec/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/tool_spec/slack/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.135260 llama_index-0.7.7/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.139260 llama_index-0.7.7/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/deeplake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.139260 llama_index-0.7.7/llama_index/vector_stores/docarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/docarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/docarray/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/docarray/hnsw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/docarray/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/supabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/tair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/typesense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-13 15:59:37.000000 llama_index-0.7.7/llama_index/vector_stores/weaviate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.099259 llama_index-0.7.7/llama_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-13 15:59:54.000000 llama_index-0.7.7/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-07-13 15:59:54.000000 llama_index-0.7.7/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:59:54.000000 llama_index-0.7.7/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-13 15:59:54.000000 llama_index-0.7.7/llama_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 15:59:54.000000 llama_index-0.7.7/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-13 15:59:37.000000 llama_index-0.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:59:54.155260 llama_index-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-13 15:59:37.000000 llama_index-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.139260 llama_index-0.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.139260 llama_index-0.7.7/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/callbacks/test_token_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.139260 llama_index-0.7.7/tests/chat_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/chat_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/chat_engine/test_condense_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/chat_engine/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.139260 llama_index-0.7.7/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.139260 llama_index-0.7.7/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.139260 llama_index-0.7.7/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.139260 llama_index-0.7.7/tests/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/document_summary/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/document_summary/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.139260 llama_index-0.7.7/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.143260 llama_index-0.7.7/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.143260 llama_index-0.7.7/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.143260 llama_index-0.7.7/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.143260 llama_index-0.7.7/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/postprocessor/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/postprocessor/test_llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/postprocessor/test_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.143260 llama_index-0.7.7/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.143260 llama_index-0.7.7/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/query/test_embedding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.143260 llama_index-0.7.7/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/struct_store/test_json_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.143260 llama_index-0.7.7/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.147260 llama_index-0.7.7/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.147260 llama_index-0.7.7/tests/indices/vector_store/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/auto_retriever/test_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.147260 llama_index-0.7.7/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.147260 llama_index-0.7.7/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.147260 llama_index-0.7.7/tests/llm_predictor/vellum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llm_predictor/vellum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llm_predictor/vellum/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llm_predictor/vellum/test_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llm_predictor/vellum/test_prompt_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llm_predictor/vellum/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.147260 llama_index-0.7.7/tests/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llms/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llms/test_anthropic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llms/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llms/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llms/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llms/test_openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/llms/test_palm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.147260 llama_index-0.7.7/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.147260 llama_index-0.7.7/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.147260 llama_index-0.7.7/tests/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/objects/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/objects/test_node_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/output_parsers/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/output_parsers/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/output_parsers/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/program/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/program/test_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/program/test_llm_program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/prompts/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/prompts/test_guidance_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/question_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/question_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/question_gen/test_guidance_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/question_gen/test_llm_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/storage/docstore/test_dynamodb_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/storage/docstore/test_redis_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/storage/test_storage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/tools/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/tools/test_ondemand_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/tools/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.151260 llama_index-0.7.7/tests/tools/tool_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/tools/tool_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/tools/tool_spec/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:54.155260 llama_index-0.7.7/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/vector_stores/test_docarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/vector_stores/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/vector_stores/test_tair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-13 15:59:37.000000 llama_index-0.7.7/tests/vector_stores/test_weaviate.py
```

### Comparing `llama_index-0.7.6/LICENSE` & `llama_index-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/PKG-INFO` & `llama_index-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_index
-Version: 0.7.6
+Version: 0.7.7
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 Author: Jerry Liu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `llama_index-0.7.6/README.md` & `llama_index-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/__init__.py` & `llama_index-0.7.7/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/agent/context_retriever_agent.py` & `llama_index-0.7.7/llama_index/agent/context_retriever_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Context retriever agent."""
 
-from typing import List, Type, Optional
+from typing import List, Optional, Type
 
 from llama_index.agent.openai_agent import (
     DEFAULT_MAX_FUNCTION_CALLS,
     DEFAULT_MODEL_NAME,
-    SUPPORTED_MODEL_NAMES,
     BaseOpenAIAgent,
 )
 from llama_index.bridge.langchain import print_text
-from llama_index.chat_engine.types import AgentChatResponse
 from llama_index.callbacks.base import CallbackManager
+from llama_index.chat_engine.types import AgentChatResponse
 from llama_index.indices.base_retriever import BaseRetriever
-from llama_index.llms.base import ChatMessage
+from llama_index.llms.base import LLM, ChatMessage
 from llama_index.llms.openai import OpenAI
+from llama_index.llms.openai_utils import is_function_calling_model
 from llama_index.memory import BaseMemory, ChatMemoryBuffer
 from llama_index.prompts.prompts import QuestionAnswerPrompt
 from llama_index.schema import NodeWithScore
 from llama_index.tools import BaseTool
 
 # inspired by DEFAULT_QA_PROMPT_TMPL from llama_index/prompts/default_prompts.py
 DEFAULT_QA_PROMPT_TMPL = (
@@ -82,15 +82,15 @@
     @classmethod
     def from_tools_and_retriever(
         cls,
         tools: List[BaseTool],
         retriever: BaseRetriever,
         qa_prompt: Optional[QuestionAnswerPrompt] = None,
         context_separator: str = "\n",
-        llm: Optional[OpenAI] = None,
+        llm: Optional[LLM] = None,
         chat_history: Optional[List[ChatMessage]] = None,
         memory: Optional[BaseMemory] = None,
         memory_cls: Type[BaseMemory] = ChatMemoryBuffer,
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
@@ -112,18 +112,17 @@
         qa_prompt = qa_prompt or DEFAULT_QA_PROMPT
         chat_history = chat_history or []
         memory = memory or memory_cls.from_defaults(chat_history=chat_history)
         llm = llm or OpenAI(model=DEFAULT_MODEL_NAME)
         if not isinstance(llm, OpenAI):
             raise ValueError("llm must be a OpenAI instance")
 
-        if llm.model not in SUPPORTED_MODEL_NAMES:
+        if is_function_calling_model(llm.model):
             raise ValueError(
-                f"Model name {llm.model} not supported. "
-                f"Supported model names: {SUPPORTED_MODEL_NAMES}"
+                f"Model name {llm.model} does not support function calling API."
             )
         if system_prompt is not None:
             if prefix_messages is not None:
                 raise ValueError(
                     "Cannot specify both system_prompt and prefix_messages"
                 )
             prefix_messages = [ChatMessage(content=system_prompt, role="system")]
```

### Comparing `llama_index-0.7.6/llama_index/agent/openai_agent.py` & `llama_index-0.7.7/llama_index/agent/openai_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,29 @@
 import asyncio
 import json
 import time
 from abc import abstractmethod
 from threading import Thread
-from typing import (
-    Callable,
-    List,
-    Tuple,
-    Type,
-    Optional,
-)
-
-from llama_index.chat_engine.types import (
-    AgentChatResponse,
-    StreamingAgentChatResponse,
-)
+from typing import Callable, List, Optional, Tuple, Type
+
+from llama_index.agent.types import BaseAgent
 from llama_index.callbacks.base import CallbackManager
+from llama_index.chat_engine.types import AgentChatResponse, StreamingAgentChatResponse
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
-from llama_index.llms.base import (
-    ChatMessage,
-    MessageRole,
-)
+from llama_index.llms.base import LLM, ChatMessage, MessageRole
 from llama_index.llms.openai import OpenAI
+from llama_index.llms.openai_utils import is_function_calling_model
 from llama_index.memory import BaseMemory, ChatMemoryBuffer
 from llama_index.response.schema import RESPONSE_TYPE, Response
 from llama_index.schema import BaseNode, NodeWithScore
-from llama_index.agent.types import BaseAgent
 from llama_index.tools import BaseTool, ToolOutput
 
 DEFAULT_MAX_FUNCTION_CALLS = 5
 DEFAULT_MODEL_NAME = "gpt-3.5-turbo-0613"
-SUPPORTED_MODEL_NAMES = [
-    "gpt-3.5-turbo-0613",
-    "gpt-4-0613",
-]
 
 
 def get_function_by_name(tools: List[BaseTool], name: str) -> BaseTool:
     """Get function by name."""
     name_to_tool = {tool.metadata.name: tool for tool in tools}
     if name not in name_to_tool:
         raise ValueError(f"Tool with name {name} not found")
@@ -369,15 +354,15 @@
         )
         self._tools = tools
 
     @classmethod
     def from_tools(
         cls,
         tools: Optional[List[BaseTool]] = None,
-        llm: Optional[OpenAI] = None,
+        llm: Optional[LLM] = None,
         chat_history: Optional[List[ChatMessage]] = None,
         memory: Optional[BaseMemory] = None,
         memory_cls: Type[BaseMemory] = ChatMemoryBuffer,
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
@@ -386,18 +371,17 @@
         tools = tools or []
         chat_history = chat_history or []
         memory = memory or memory_cls.from_defaults(chat_history)
         llm = llm or OpenAI(model=DEFAULT_MODEL_NAME)
         if not isinstance(llm, OpenAI):
             raise ValueError("llm must be a OpenAI instance")
 
-        if llm.model not in SUPPORTED_MODEL_NAMES:
+        if not is_function_calling_model(llm.model):
             raise ValueError(
-                f"Model name {llm.model} not supported. "
-                f"Supported model names: {SUPPORTED_MODEL_NAMES}"
+                f"Model name {llm.model} does not support function calling API. "
             )
 
         if system_prompt is not None:
             if prefix_messages is not None:
                 raise ValueError(
                     "Cannot specify both system_prompt and prefix_messages"
                 )
@@ -474,18 +458,17 @@
         chat_history = chat_history or []
         memory = memory or memory_cls.from_defaults(chat_history)
 
         llm = llm or OpenAI(model=DEFAULT_MODEL_NAME)
         if not isinstance(llm, OpenAI):
             raise ValueError("llm must be a OpenAI instance")
 
-        if llm.model not in SUPPORTED_MODEL_NAMES:
+        if not is_function_calling_model(llm.model):
             raise ValueError(
-                f"Model name {llm.model} not supported. "
-                f"Supported model names: {SUPPORTED_MODEL_NAMES}"
+                f"Model name {llm.model} does not support function calling API. "
             )
 
         if system_prompt is not None:
             if prefix_messages is not None:
                 raise ValueError(
                     "Cannot specify both system_prompt and prefix_messages"
                 )
```

### Comparing `llama_index-0.7.6/llama_index/agent/react/base.py` & `llama_index-0.7.7/llama_index/agent/react/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/agent/react/formatter.py` & `llama_index-0.7.7/llama_index/agent/react/formatter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/agent/react/output_parser.py` & `llama_index-0.7.7/llama_index/agent/react/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/agent/react/prompts.py` & `llama_index-0.7.7/llama_index/agent/react/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/agent/react/types.py` & `llama_index-0.7.7/llama_index/agent/react/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/agent/retriever_openai_agent.py` & `llama_index-0.7.7/llama_index/agent/retriever_openai_agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Retriever OpenAI agent."""
 
-from typing import List, Type, Optional
+from typing import List, Optional, Type
 
 from llama_index.agent.openai_agent import (
     DEFAULT_MAX_FUNCTION_CALLS,
     DEFAULT_MODEL_NAME,
-    SUPPORTED_MODEL_NAMES,
     BaseOpenAIAgent,
 )
 from llama_index.callbacks.base import CallbackManager
 from llama_index.llms.base import ChatMessage
 from llama_index.llms.openai import OpenAI
+from llama_index.llms.openai_utils import is_function_calling_model
 from llama_index.memory import BaseMemory, ChatMemoryBuffer
 from llama_index.objects.base import ObjectRetriever
 from llama_index.tools.types import BaseTool
 
 
 class FnRetrieverOpenAIAgent(BaseOpenAIAgent):
     """Function Retriever OpenAI Agent.
@@ -59,19 +59,19 @@
     ) -> "FnRetrieverOpenAIAgent":
         chat_history = chat_history or []
         memory = memory or memory_cls.from_defaults(chat_history=chat_history)
         llm = llm or OpenAI(model=DEFAULT_MODEL_NAME)
         if not isinstance(llm, OpenAI):
             raise ValueError("llm must be a OpenAI instance")
 
-        if llm.model not in SUPPORTED_MODEL_NAMES:
+        if not is_function_calling_model(llm.model):
             raise ValueError(
-                f"Model name {llm.model} not supported. "
-                f"Supported model names: {SUPPORTED_MODEL_NAMES}"
+                f"Model name {llm.model} does not support function calling API. "
             )
+
         if system_prompt is not None:
             if prefix_messages is not None:
                 raise ValueError(
                     "Cannot specify both system_prompt and prefix_messages"
                 )
             prefix_messages = [ChatMessage(content=system_prompt, role="system")]
```

### Comparing `llama_index-0.7.6/llama_index/agent/types.py` & `llama_index-0.7.7/llama_index/agent/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/async_utils.py` & `llama_index-0.7.7/llama_index/async_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/bridge/langchain.py` & `llama_index-0.7.7/llama_index/bridge/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/callbacks/aim.py` & `llama_index-0.7.7/llama_index/callbacks/aim.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/callbacks/base.py` & `llama_index-0.7.7/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/callbacks/llama_debug.py` & `llama_index-0.7.7/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/callbacks/schema.py` & `llama_index-0.7.7/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/callbacks/token_counting.py` & `llama_index-0.7.7/llama_index/callbacks/token_counting.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/callbacks/wandb_callback.py` & `llama_index-0.7.7/llama_index/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/chat_engine/condense_question.py` & `llama_index-0.7.7/llama_index/chat_engine/condense_question.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/chat_engine/simple.py` & `llama_index-0.7.7/llama_index/chat_engine/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/chat_engine/types.py` & `llama_index-0.7.7/llama_index/chat_engine/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import queue
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Generator, List, Optional
 
-from llama_index.tools import ToolOutput
-from llama_index.llms.base import ChatMessage, ChatResponseGen, ChatResponseAsyncGen
+from llama_index.llms.base import ChatMessage, ChatResponseAsyncGen, ChatResponseGen
 from llama_index.memory import BaseMemory
+from llama_index.tools import ToolOutput
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class AgentChatResponse:
     """Agent chat response."""
@@ -150,19 +150,35 @@
     """Chat Engine Modes."""
 
     SIMPLE = "simple"
     """Corresponds to `SimpleChatEngine`.
     
     Chat with LLM, without making use of a knowledge base.
     """
+
     CONDENSE_QUESTION = "condense_question"
     """Corresponds to `CondenseQuestionChatEngine`.
     
     First generate a standalone question from conversation context and last message,
     then query the query engine for a response.
     """
+
     REACT = "react"
-    """Corresponds to `ReActChatEngine`.
+    """Corresponds to `ReActAgent`.
     
     Use a ReAct agent loop with query engine tools. 
-    Implemented via LangChain agent.
+    """
+
+    OPENAI = "openai"
+    """Corresponds to `OpenAIAgent`.
+    
+    Use an OpenAI function calling agent loop.
+
+    NOTE: only works with OpenAI models that support function calling API.
+    """
+
+    BEST = "best"
+    """Select the best chat engine based on the current LLM.
+
+    Corresponds to `OpenAIAgent` if using an OpenAI model that supports 
+    function calling API, otherwise, corresponds to `ReActAgent`.
     """
```

### Comparing `llama_index-0.7.6/llama_index/chat_engine/utils.py` & `llama_index-0.7.7/llama_index/chat_engine/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/composability/joint_qa_summary.py` & `llama_index-0.7.7/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/data_structs/data_structs.py` & `llama_index-0.7.7/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/data_structs/document_summary.py` & `llama_index-0.7.7/llama_index/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/data_structs/registry.py` & `llama_index-0.7.7/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/data_structs/struct_type.py` & `llama_index-0.7.7/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/data_structs/table.py` & `llama_index-0.7.7/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/embeddings/base.py` & `llama_index-0.7.7/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/embeddings/google.py` & `llama_index-0.7.7/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/embeddings/langchain.py` & `llama_index-0.7.7/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/embeddings/openai.py` & `llama_index-0.7.7/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/embeddings/utils.py` & `llama_index-0.7.7/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/evaluation/base.py` & `llama_index-0.7.7/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/evaluation/dataset_generation.py` & `llama_index-0.7.7/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/evaluation/guideline_eval.py` & `llama_index-0.7.7/llama_index/evaluation/guideline_eval.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/graph_stores/nebulagraph.py` & `llama_index-0.7.7/llama_index/graph_stores/nebulagraph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,35 @@
 """NebulaGraph graph store index."""
 import logging
 import os
+from string import Template
 from typing import Any, Dict, List, Optional
 
+from tenacity import retry, stop_after_attempt, wait_random_exponential
+
 from llama_index.graph_stores.types import GraphStore
 
 QUOTE = '"'
 RETRY_TIMES = 3
+WAIT_MIN_SECONDS = 0.1
+WAIT_MAX_SECONDS = 20
 
 logger = logging.getLogger(__name__)
 
 
+rel_query = Template(
+    """
+MATCH ()-[e:`$edge_type`]->()
+  WITH e limit 1
+MATCH (m)-[:`$edge_type`]->(n) WHERE id(m) == src(e) AND id(n) == dst(e)
+RETURN "(:" + tags(m)[0] + ")-[:$edge_type]->(:" + tags(n)[0] + ")" AS rels
+"""
+)
+
+
 def hash_string_to_rank(string: str) -> int:
     # get signed 64-bit hash value
     signed_hash = hash(string)
 
     # reduce the hash value to a 64-bit range
     mask = (1 << 64) - 1
     signed_hash &= mask
@@ -62,16 +77,16 @@
 class NebulaGraphStore(GraphStore):
     """NebulaGraph graph store."""
 
     def __init__(
         self,
         session_pool: Optional[Any] = None,
         space_name: Optional[str] = None,
-        edge_types: Optional[List[str]] = ["rel"],
-        rel_prop_names: Optional[List[str]] = ["predicate"],
+        edge_types: Optional[List[str]] = ["relationship"],
+        rel_prop_names: Optional[List[str]] = ["relationship"],
         tags: Optional[List[str]] = ["entity"],
         session_pool_kwargs: Optional[Dict[str, Any]] = {},
         **kwargs: Any,
     ) -> None:
         """Initialize NebulaGraph graph store.
 
         Args:
@@ -88,21 +103,14 @@
             raise ImportError(
                 "Please install NebulaGraph Python client first: "
                 "`pip install nebula3-python`"
             )
         assert space_name is not None, "space_name should be provided."
         self._space_name = space_name
         self._session_pool_kwargs = session_pool_kwargs
-        if (
-            self._session_pool_kwargs is not None
-            and "retry" in self._session_pool_kwargs
-        ):
-            self._retry = self._session_pool_kwargs.pop("retry")
-        else:
-            self._retry = RETRY_TIMES
 
         if session_pool is None:
             self.init_session_pool()
 
         self._tags = tags or ["entity"]
         self._edge_types = edge_types or ["rel"]
         self._rel_prop_names = rel_prop_names or ["predicate"]
@@ -149,51 +157,68 @@
         self._session_pool = session_pool
         return self._session_pool
 
     def __del__(self) -> None:
         """Close NebulaGraph session pool."""
         self._session_pool.close()
 
+    @retry(
+        wait=wait_random_exponential(min=WAIT_MIN_SECONDS, max=WAIT_MAX_SECONDS),
+        stop=stop_after_attempt(RETRY_TIMES),
+    )
     def execute(self, query: str, param_map: Optional[Dict[str, Any]] = {}) -> Any:
         """Execute query.
 
         Args:
             query: Query.
             param_map: Parameter map.
 
         Returns:
             Query result.
         """
         from nebula3.Exception import IOErrorException
         from nebula3.fbthrift.transport.TTransport import TTransportException
 
-        retry = self._retry
-        while retry > 0:
-            try:
-                result = self._session_pool.execute_parameter(query, param_map)
-                if not result.is_succeeded():
-                    raise ValueError(result.error_msg())
-                return result
-            except (TTransportException, IOErrorException) as e:
-                # connection issue, try to recreate session pool
-                if retry > 0:
-                    retry -= 2
-                    # try to recreate session pool
-                    self.init_session_pool()
-                else:
-                    raise e
-            except ValueError as e:
-                # query failed on db side
-                if retry > 0:
-                    retry -= 1
-                    continue
-                else:
-                    raise e
-            except Exception as e:
-                raise e
+        try:
+            result = self._session_pool.execute_parameter(query, param_map)
+            if result is None:
+                raise ValueError(f"Query failed. Query: {query}, Param: {param_map}")
+            if not result.is_succeeded():
+                raise ValueError(
+                    f"Query failed. Query: {query}, Param: {param_map}"
+                    f"Error message: {result.error_msg()}"
+                )
+            return result
+        except (TTransportException, IOErrorException, RuntimeError) as e:
+            logger.error(
+                f"Connection issue, try to recreate session pool. Query: {query}, "
+                f"Param: {param_map}"
+                f"Erorr: {e}"
+            )
+            self.init_session_pool()
+            logger.info(
+                f"Session pool recreated. Query: {query}, Param: {param_map}"
+                f"This was due to error: {e}, and now retrying."
+            )
+            raise e
+
+        except ValueError as e:
+            # query failed on db side
+            logger.error(
+                f"Query failed. Query: {query}, Param: {param_map}"
+                f"Error message: {e}"
+            )
+            raise e
+        except Exception as e:
+            # other exceptions
+            logger.error(
+                f"Query failed. Query: {query}, Param: {param_map}"
+                f"Error message: {e}"
+            )
+            raise e
 
     @classmethod
     def from_dict(cls, config_dict: Dict[str, Any]) -> "GraphStore":
         """Initialize graph store from configuration dictionary.
 
         Args:
             config_dict: Configuration dictionary.
@@ -360,15 +385,15 @@
         """Get rel map."""
         # We put rels in a long list for depth>= 1, this is different from
         # SimpleGraphStore.get_rel_map() though.
         # But this makes more sense for multi-hop relation path.
 
         # lower case subjs
         if subjs is not None:
-            subjs = [escape_str(subj.lower()) for subj in subjs]
+            subjs = [escape_str(subj) for subj in subjs]
             if len(subjs) == 0:
                 return {}
 
         return self.get_flat_rel_map(subjs, depth)
 
     def upsert_triplet(self, subj: str, rel: str, obj: str) -> None:
         """Add triplet."""
@@ -377,27 +402,27 @@
         #   makes (n:1) edge_type.prop_name --> triplet.rel
         # thus we have to assume rel to be the first edge_type.prop_name
         # here in upsert_triplet().
         # This applies to the type of entity(tags) with subject and object, too,
         # thus we have to assume subj to be the first entity.tag_name
 
         # lower case subj, rel, obj
-        subj = escape_str(subj.lower())
-        rel = escape_str(rel.lower())
-        obj = escape_str(obj.lower())
+        subj = escape_str(subj)
+        rel = escape_str(rel)
+        obj = escape_str(obj)
 
         edge_type = self._edge_types[0]
         rel_prop_name = self._rel_prop_names[0]
         entity_type = self._tags[0]
         rel_hash = hash_string_to_rank(rel)
         dml_query = (
-            f"INSERT VERTEX `{entity_type}`() "
-            f"  VALUES {QUOTE}{subj}{QUOTE}:();"
-            f"INSERT VERTEX `{entity_type}`() "
-            f"  VALUES {QUOTE}{obj}{QUOTE}:();"
+            f"INSERT VERTEX `{entity_type}`(name) "
+            f"  VALUES {QUOTE}{subj}{QUOTE}:({QUOTE}{subj}{QUOTE});"
+            f"INSERT VERTEX `{entity_type}`(name) "
+            f"  VALUES {QUOTE}{obj}{QUOTE}:({QUOTE}{obj}{QUOTE});"
             f"INSERT EDGE `{edge_type}`(`{rel_prop_name}`) "
             f"  VALUES "
             f"{QUOTE}{subj}{QUOTE}->{QUOTE}{obj}{QUOTE}"
             f"@{rel_hash}:({QUOTE}{rel}{QUOTE});"
         )
         logger.debug(f"upsert_triplet() DML query: {dml_query}")
         result = self.execute(dml_query)
@@ -411,17 +436,17 @@
            we have to assume rel to be the first edge_type.prop_name.
         2. After edge being deleted, we need to check if the subj or
            obj are isolated vertices,
            if so, delete them, too.
         """
 
         # lower case subj, rel, obj
-        subj = escape_str(subj.lower())
-        rel = escape_str(rel.lower())
-        obj = escape_str(obj.lower())
+        subj = escape_str(subj)
+        rel = escape_str(rel)
+        obj = escape_str(obj)
 
         # DELETE EDGE serve "player100" -> "team204"@7696463696635583936;
         edge_type = self._edge_types[0]
         # rel_prop_name = self._rel_prop_names[0]
         rel_hash = hash_string_to_rank(rel)
         dml_query = (
             f"DELETE EDGE `{edge_type}`"
@@ -449,7 +474,60 @@
         vertex_ids = ",".join([f"{QUOTE}{v.cast()}{QUOTE}" for v in isolated])
         dml_query = f"DELETE VERTEX {vertex_ids};"
 
         result = self.execute(dml_query)
         assert (
             result and result.is_succeeded()
         ), f"Failed to delete isolated vertices: {isolated}, query: {dml_query}"
+
+    def refresh_schema(self) -> None:
+        """
+        Refreshes the NebulaGraph Store Schema.
+        """
+        tags_schema, edge_types_schema, relationships = [], [], []
+        for tag in self.execute("SHOW TAGS").column_values("Name"):
+            tag_name = tag.cast()
+            tag_schema = {"tag": tag_name, "properties": []}
+            r = self.execute(f"DESCRIBE TAG `{tag_name}`")
+            props, types = r.column_values("Field"), r.column_values("Type")
+            for i in range(r.row_size()):
+                tag_schema["properties"].append((props[i].cast(), types[i].cast()))
+            tags_schema.append(tag_schema)
+        for edge_type in self.execute("SHOW EDGES").column_values("Name"):
+            edge_type_name = edge_type.cast()
+            edge_schema = {"edge": edge_type_name, "properties": []}
+            r = self.execute(f"DESCRIBE EDGE `{edge_type_name}`")
+            props, types = r.column_values("Field"), r.column_values("Type")
+            for i in range(r.row_size()):
+                edge_schema["properties"].append((props[i].cast(), types[i].cast()))
+            edge_types_schema.append(edge_schema)
+
+            # build relationships types
+            r = self.execute(
+                rel_query.substitute(edge_type=edge_type_name)
+            ).column_values("rels")
+            if len(r) > 0:
+                relationships.append(r[0].cast())
+
+        self.schema = (
+            f"Node properties: {tags_schema}\n"
+            f"Edge properties: {edge_types_schema}\n"
+            f"Relationships: {relationships}\n"
+        )
+
+    def get_schema(self, refresh: bool = False) -> str:
+        """Get the schema of the NebulaGraph store."""
+        if self.schema and not refresh:
+            return self.schema
+        self.refresh_schema()
+        logger.debug(f"get_schema() schema:\n{self.schema}")
+        return self.schema
+
+    def query(self, query: str, param_map: Optional[Dict[str, Any]] = {}) -> Any:
+        result = self.execute(query, param_map)
+        columns = result.keys()
+        d: Dict[str, list] = {}
+        for col_num in range(result.col_size()):
+            col_name = columns[col_num]
+            col_list = result.column_values(col_name)
+            d[col_name] = [x.cast() for x in col_list]
+        return d
```

### Comparing `llama_index-0.7.6/llama_index/graph_stores/registery.py` & `llama_index-0.7.7/llama_index/graph_stores/registery.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/graph_stores/simple.py` & `llama_index-0.7.7/llama_index/graph_stores/simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,14 +124,22 @@
         dirpath = os.path.dirname(persist_path)
         if not fs.exists(dirpath):
             fs.makedirs(dirpath)
 
         with fs.open(persist_path, "w") as f:
             json.dump(self._data.to_dict(), f)
 
+    def get_schema(self, refresh: bool = False) -> str:
+        """Get the schema of the Simple Graph store."""
+        raise NotImplementedError("SimpleGraphStore does not support get_schema")
+
+    def query(self, query: str, param_map: Optional[Dict[str, Any]] = {}) -> Any:
+        """Query the Simple Graph store."""
+        raise NotImplementedError("SimpleGraphStore does not support query")
+
     @classmethod
     def from_persist_path(
         cls, persist_path: str, fs: Optional[fsspec.AbstractFileSystem] = None
     ) -> "SimpleGraphStore":
         """Create a SimpleGraphStore from a persist directory."""
         fs = fs or fsspec.filesystem("file")
         if not fs.exists(persist_path):
```

### Comparing `llama_index-0.7.6/llama_index/graph_stores/types.py` & `llama_index-0.7.7/llama_index/graph_stores/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,19 @@
         get: Callable[[str], List[List[str]]]: Get triplets for a given subject.
         get_rel_map: Callable[[Optional[List[str]], int], Dict[str, List[List[str]]]]:
             Get subjects' rel map in max depth.
         upsert_triplet: Callable[[str, str, str], None]: Upsert a triplet.
         delete: Callable[[str, str, str], None]: Delete a triplet.
         persist: Callable[[str, Optional[fsspec.AbstractFileSystem]], None]:
             Persist the graph store to a file.
+        get_schema: Callable[[bool], str]: Get the schema of the graph store.
     """
 
+    schema: str = ""
+
     @property
     def client(self) -> Any:
         """Get client."""
         ...
 
     def get(self, subj: str) -> List[List[str]]:
         """Get triplets."""
@@ -48,7 +51,15 @@
         ...
 
     def persist(
         self, persist_path: str, fs: Optional[fsspec.AbstractFileSystem] = None
     ) -> None:
         """Persist the graph store to a file."""
         return None
+
+    def get_schema(self, refresh: bool = False) -> str:
+        """Get the schema of the graph store."""
+        ...
+
+    def query(self, query: str, param_map: Optional[Dict[str, Any]] = {}) -> Any:
+        """Query the graph store with statement and parameters."""
+        ...
```

### Comparing `llama_index-0.7.6/llama_index/img_utils.py` & `llama_index-0.7.7/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/__init__.py` & `llama_index-0.7.7/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/base.py` & `llama_index-0.7.7/llama_index/indices/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Base index classes."""
 import logging
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Generic, List, Optional, Sequence, Type, TypeVar
+from typing import Any, Dict, Generic, List, Optional, Sequence, Type, TypeVar, cast
 
 from llama_index.chat_engine.types import BaseChatEngine, ChatMode
 from llama_index.data_structs.data_structs import IndexStruct
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.service_context import ServiceContext
+from llama_index.llms.openai import OpenAI
+from llama_index.llms.openai_utils import is_function_calling_model
 from llama_index.schema import BaseNode, Document
 from llama_index.storage.docstore.types import BaseDocumentStore, RefDocInfo
 from llama_index.storage.storage_context import StorageContext
 
 IS = TypeVar("IS", bound=IndexStruct)
 IndexType = TypeVar("IndexType", bound="BaseIndex")
 
@@ -336,37 +338,64 @@
 
         kwargs["retriever"] = retriever
         if "service_context" not in kwargs:
             kwargs["service_context"] = self._service_context
         return RetrieverQueryEngine.from_args(**kwargs)
 
     def as_chat_engine(
-        self, chat_mode: ChatMode = ChatMode.CONDENSE_QUESTION, **kwargs: Any
+        self, chat_mode: ChatMode = ChatMode.BEST, **kwargs: Any
     ) -> BaseChatEngine:
+        query_engine = self.as_query_engine(**kwargs)
+        if "service_context" not in kwargs:
+            kwargs["service_context"] = self._service_context
+
+        # resolve chat mode
+        if chat_mode == ChatMode.BEST:
+            # get LLM
+            service_context = cast(ServiceContext, kwargs["service_context"])
+            llm = service_context.llm
+
+            if isinstance(llm, OpenAI) and is_function_calling_model(llm.model):
+                chat_mode = ChatMode.OPENAI
+            else:
+                chat_mode = ChatMode.REACT
+
         if chat_mode == ChatMode.CONDENSE_QUESTION:
             # NOTE: lazy import
             from llama_index.chat_engine import CondenseQuestionChatEngine
 
-            query_engine = self.as_query_engine(**kwargs)
-            if "service_context" not in kwargs:
-                kwargs["service_context"] = self._service_context
             return CondenseQuestionChatEngine.from_defaults(
                 query_engine=query_engine,
                 **kwargs,
             )
-        elif chat_mode == ChatMode.REACT:
+        elif chat_mode in [ChatMode.REACT, ChatMode.OPENAI]:
             # NOTE: lazy import
-            from llama_index.chat_engine import ReActChatEngine
+            from llama_index.agent import OpenAIAgent, ReActAgent
+            from llama_index.tools.query_engine import QueryEngineTool
 
-            query_engine = self.as_query_engine(**kwargs)
-            if "service_context" not in kwargs:
-                kwargs["service_context"] = self._service_context
-            return ReActChatEngine.from_query_engine(
-                query_engine=query_engine,
-                **kwargs,
-            )
+            # convert query engine to tool
+            query_engine_tool = QueryEngineTool.from_defaults(query_engine=query_engine)
+
+            # get LLM
+            service_context = cast(ServiceContext, kwargs.pop("service_context"))
+            llm = service_context.llm
+
+            if chat_mode == ChatMode.REACT:
+                return ReActAgent.from_tools(
+                    tools=[query_engine_tool],
+                    llm=llm,
+                    **kwargs,
+                )
+            elif chat_mode == ChatMode.OPENAI:
+                return OpenAIAgent.from_tools(
+                    tools=[query_engine_tool],
+                    llm=llm,
+                    **kwargs,
+                )
+            else:
+                raise ValueError(f"Unknown chat mode: {chat_mode}")
         else:
             raise ValueError(f"Unknown chat mode: {chat_mode}")
 
 
 # legacy
 BaseGPTIndex = BaseIndex
```

### Comparing `llama_index-0.7.6/llama_index/indices/base_retriever.py` & `llama_index-0.7.7/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/common/struct_store/base.py` & `llama_index-0.7.7/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.7.7/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.7.7/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/common_tree/base.py` & `llama_index-0.7.7/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/composability/graph.py` & `llama_index-0.7.7/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/document_summary/base.py` & `llama_index-0.7.7/llama_index/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/document_summary/retrievers.py` & `llama_index-0.7.7/llama_index/indices/document_summary/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/empty/base.py` & `llama_index-0.7.7/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/empty/retrievers.py` & `llama_index-0.7.7/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.7.7/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/keyword_table/base.py` & `llama_index-0.7.7/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.7.7/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.7.7/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.7.7/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/keyword_table/utils.py` & `llama_index-0.7.7/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.7.7/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/knowledge_graph/retriever.py` & `llama_index-0.7.7/llama_index/indices/knowledge_graph/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/list/base.py` & `llama_index-0.7.7/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/list/retrievers.py` & `llama_index-0.7.7/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/loading.py` & `llama_index-0.7.7/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/postprocessor/__init__.py` & `llama_index-0.7.7/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/postprocessor/cohere_rerank.py` & `llama_index-0.7.7/llama_index/indices/postprocessor/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/postprocessor/llm_rerank.py` & `llama_index-0.7.7/llama_index/indices/postprocessor/llm_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/postprocessor/node.py` & `llama_index-0.7.7/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/postprocessor/node_recency.py` & `llama_index-0.7.7/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/postprocessor/optimizer.py` & `llama_index-0.7.7/llama_index/indices/postprocessor/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/postprocessor/pii.py` & `llama_index-0.7.7/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/prompt_helper.py` & `llama_index-0.7.7/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/query/base.py` & `llama_index-0.7.7/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/query/embedding_utils.py` & `llama_index-0.7.7/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/query/query_transform/base.py` & `llama_index-0.7.7/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/query/query_transform/feedback_transform.py` & `llama_index-0.7.7/llama_index/indices/query/query_transform/feedback_transform.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.7.7/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/query/schema.py` & `llama_index-0.7.7/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/registry.py` & `llama_index-0.7.7/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/service_context.py` & `llama_index-0.7.7/llama_index/indices/service_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,11 +221,17 @@
             embed_model=embed_model,
             prompt_helper=prompt_helper,
             node_parser=node_parser,
             llama_logger=llama_logger,  # deprecated
             callback_manager=callback_manager,
         )
 
+    @property
+    def llm(self) -> LLM:
+        if not isinstance(self.llm_predictor, LLMPredictor):
+            raise ValueError("llm_predictor must be an instance of LLMPredictor")
+        return self.llm_predictor.llm
+
 
 def set_global_service_context(service_context: Optional[ServiceContext]) -> None:
     """Helper function to set the global service context."""
     llama_index.global_service_context = service_context
```

### Comparing `llama_index-0.7.6/llama_index/indices/struct_store/__init__.py` & `llama_index-0.7.7/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/struct_store/base.py` & `llama_index-0.7.7/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.7.7/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/struct_store/json_query.py` & `llama_index-0.7.7/llama_index/indices/struct_store/json_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/struct_store/pandas.py` & `llama_index-0.7.7/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/struct_store/sql.py` & `llama_index-0.7.7/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.7.7/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/tree/__init__.py` & `llama_index-0.7.7/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.7.7/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/tree/base.py` & `llama_index-0.7.7/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/tree/inserter.py` & `llama_index-0.7.7/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.7.7/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.7.7/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.7.7/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/tree/utils.py` & `llama_index-0.7.7/llama_index/indices/tree/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/utils.py` & `llama_index-0.7.7/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/vector_store/base.py` & `llama_index-0.7.7/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py` & `llama_index-0.7.7/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py` & `llama_index-0.7.7/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py` & `llama_index-0.7.7/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/indices/vector_store/retrievers/retriever.py` & `llama_index-0.7.7/llama_index/indices/vector_store/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.7.7/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.7.7/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.7.7/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.7.7/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.7.7/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.7.7/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/langchain_helpers/streaming.py` & `llama_index-0.7.7/llama_index/langchain_helpers/streaming.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.7.7/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llm_predictor/base.py` & `llama_index-0.7.7/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llm_predictor/mock.py` & `llama_index-0.7.7/llama_index/llm_predictor/mock.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llm_predictor/structured.py` & `llama_index-0.7.7/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llm_predictor/utils.py` & `llama_index-0.7.7/llama_index/llm_predictor/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llm_predictor/vellum/predictor.py` & `llama_index-0.7.7/llama_index/llm_predictor/vellum/predictor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llm_predictor/vellum/prompt_registry.py` & `llama_index-0.7.7/llama_index/llm_predictor/vellum/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llm_predictor/vellum/types.py` & `llama_index-0.7.7/llama_index/llm_predictor/vellum/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/__init__.py` & `llama_index-0.7.7/llama_index/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/anthropic.py` & `llama_index-0.7.7/llama_index/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/anthropic_utils.py` & `llama_index-0.7.7/llama_index/llms/anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/azure_openai.py` & `llama_index-0.7.7/llama_index/llms/azure_openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/base.py` & `llama_index-0.7.7/llama_index/llms/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     def __str__(self) -> str:
         return str(self.message)
 
 
 ChatResponseGen = Generator[ChatResponse, None, None]
 ChatResponseAsyncGen = AsyncGenerator[ChatResponse, None]
 
+
 # ===== Generic Model Output - Completion =====
 class CompletionResponse(BaseModel):
     """Completion response."""
 
     text: str
     additional_kwargs: dict = Field(default_factory=dict)
     raw: Optional[dict] = None
```

### Comparing `llama_index-0.7.6/llama_index/llms/custom.py` & `llama_index-0.7.7/llama_index/llms/custom.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/generic_utils.py` & `llama_index-0.7.7/llama_index/llms/generic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/huggingface.py` & `llama_index-0.7.7/llama_index/llms/huggingface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/langchain.py` & `llama_index-0.7.7/llama_index/llms/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/langchain_utils.py` & `llama_index-0.7.7/llama_index/llms/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/mock.py` & `llama_index-0.7.7/llama_index/llms/mock.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/openai.py` & `llama_index-0.7.7/llama_index/llms/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/llms/openai_utils.py` & `llama_index-0.7.7/llama_index/llms/openai_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -177,14 +177,20 @@
     return context_size
 
 
 def is_chat_model(model: str) -> bool:
     return model in CHAT_MODELS
 
 
+def is_function_calling_model(model: str) -> bool:
+    is_chat_model_ = is_chat_model(model)
+    is_old = "0314" in model or "0301" in model
+    return is_chat_model_ and not is_old
+
+
 def get_completion_endpoint(is_chat_model: bool) -> CompletionClientType:
     if is_chat_model:
         return openai.ChatCompletion
     else:
         return openai.Completion
```

### Comparing `llama_index-0.7.6/llama_index/llms/palm.py` & `llama_index-0.7.7/llama_index/llms/palm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/logger/base.py` & `llama_index-0.7.7/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/memory/chat_memory_buffer.py` & `llama_index-0.7.7/llama_index/memory/chat_memory_buffer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/memory/types.py` & `llama_index-0.7.7/llama_index/memory/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/node_parser/extractors/metadata_extractors.py` & `llama_index-0.7.7/llama_index/node_parser/extractors/metadata_extractors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/node_parser/interface.py` & `llama_index-0.7.7/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/node_parser/node_utils.py` & `llama_index-0.7.7/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/node_parser/simple.py` & `llama_index-0.7.7/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/objects/__init__.py` & `llama_index-0.7.7/llama_index/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/objects/base.py` & `llama_index-0.7.7/llama_index/objects/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/objects/base_node_mapping.py` & `llama_index-0.7.7/llama_index/objects/base_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/objects/table_node_mapping.py` & `llama_index-0.7.7/llama_index/objects/table_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/objects/tool_node_mapping.py` & `llama_index-0.7.7/llama_index/objects/tool_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/output_parsers/guardrails.py` & `llama_index-0.7.7/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/output_parsers/langchain.py` & `llama_index-0.7.7/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/output_parsers/pydantic.py` & `llama_index-0.7.7/llama_index/output_parsers/pydantic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/output_parsers/selection.py` & `llama_index-0.7.7/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/output_parsers/utils.py` & `llama_index-0.7.7/llama_index/output_parsers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/playground/base.py` & `llama_index-0.7.7/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/program/__init__.py` & `llama_index-0.7.7/llama_index/program/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/program/guidance_program.py` & `llama_index-0.7.7/llama_index/program/guidance_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/program/llm_program.py` & `llama_index-0.7.7/llama_index/program/llm_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/program/llm_prompt_program.py` & `llama_index-0.7.7/llama_index/program/llm_prompt_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/program/openai_program.py` & `llama_index-0.7.7/llama_index/program/openai_program.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from typing import Any, Dict, Optional, Type, Union
 
-from llama_index.llms.openai import OpenAI
-from llama_index.llms.base import ChatMessage, MessageRole
-from llama_index.llms.openai_utils import to_openai_function
-from llama_index.types import Model
+from pydantic import BaseModel
 
+from llama_index.llms.base import ChatMessage, MessageRole
+from llama_index.llms.openai import OpenAI
+from llama_index.llms.openai_utils import is_function_calling_model, to_openai_function
 from llama_index.program.llm_prompt_program import BaseLLMFunctionProgram
 from llama_index.prompts.base import Prompt
-from pydantic import BaseModel
-
-SUPPORTED_MODEL_NAMES = [
-    "gpt-3.5-turbo-0613",
-    "gpt-4-0613",
-]
+from llama_index.types import Model
 
 
 def _default_function_call(output_cls: Type[BaseModel]) -> Dict[str, Any]:
     """Default OpenAI function to call."""
     schema = output_cls.schema()
     return {
         "name": schema["title"],
@@ -55,19 +50,19 @@
         function_call: Optional[Union[str, Dict[str, Any]]] = None,
         **kwargs: Any,
     ) -> "OpenAIPydanticProgram":
         llm = llm or OpenAI(model="gpt-3.5-turbo-0613")
         if not isinstance(llm, OpenAI):
             raise ValueError("llm must be a OpenAI instance")
 
-        if llm.model not in SUPPORTED_MODEL_NAMES:
+        if not is_function_calling_model(llm.model):
             raise ValueError(
-                f"Model name {llm.model} not supported. "
-                f"Supported model names: {SUPPORTED_MODEL_NAMES}"
+                f"Model name {llm.model} does not support function calling API. "
             )
+
         prompt = Prompt(prompt_template_str)
         function_call = function_call or _default_function_call(output_cls)
         return cls(
             output_cls=output_cls,
             llm=llm,
             prompt=prompt,
             function_call=function_call,
```

### Comparing `llama_index-0.7.6/llama_index/program/predefined/df.py` & `llama_index-0.7.7/llama_index/program/predefined/df.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/program/predefined/evaporate/base.py` & `llama_index-0.7.7/llama_index/program/predefined/evaporate/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/program/predefined/evaporate/extractor.py` & `llama_index-0.7.7/llama_index/program/predefined/evaporate/extractor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/program/predefined/evaporate/prompts.py` & `llama_index-0.7.7/llama_index/program/predefined/evaporate/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/prompts/base.py` & `llama_index-0.7.7/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/prompts/chat_prompts.py` & `llama_index-0.7.7/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/prompts/choice_select.py` & `llama_index-0.7.7/llama_index/prompts/choice_select.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.7.7/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/prompts/default_prompts.py` & `llama_index-0.7.7/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/prompts/guidance_utils.py` & `llama_index-0.7.7/llama_index/prompts/guidance_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/prompts/prompt_selector.py` & `llama_index-0.7.7/llama_index/prompts/prompt_selector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/prompts/prompt_type.py` & `llama_index-0.7.7/llama_index/prompts/prompt_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
     # schema extract
     SCHEMA_EXTRACT = "schema_extract"
 
     # text to sql
     TEXT_TO_SQL = "text_to_sql"
 
+    # text to graph query
+    TEXT_TO_GRAPH_QUERY = "text_to_graph_query"
+
     # table context
     TABLE_CONTEXT = "table_context"
 
     # KG extraction prompt
     KNOWLEDGE_TRIPLET_EXTRACT = "knowledge_triplet_extract"
 
     # Simple Input prompt
```

### Comparing `llama_index-0.7.6/llama_index/prompts/prompts.py` & `llama_index-0.7.7/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/prompts/system.py` & `llama_index-0.7.7/llama_index/prompts/system.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/prompts/utils.py` & `llama_index-0.7.7/llama_index/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/__init__.py` & `llama_index-0.7.7/llama_index/query_engine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from llama_index.query_engine.citation_query_engine import CitationQueryEngine
 from llama_index.query_engine.flare.base import FLAREInstructQueryEngine
 from llama_index.query_engine.graph_query_engine import ComposableGraphQueryEngine
+from llama_index.query_engine.knowledge_graph_query_engine import (
+    KnowledgeGraphQueryEngine,
+)
 from llama_index.query_engine.multistep_query_engine import MultiStepQueryEngine
 from llama_index.query_engine.pandas_query_engine import PandasQueryEngine
 from llama_index.query_engine.retriever_query_engine import RetrieverQueryEngine
 from llama_index.query_engine.retry_query_engine import (
     RetryGuidelineQueryEngine,
     RetryQueryEngine,
 )
 from llama_index.query_engine.retry_source_query_engine import RetrySourceQueryEngine
 from llama_index.query_engine.router_query_engine import (
-    ToolRetrieverRouterQueryEngine,
     RetrieverRouterQueryEngine,
     RouterQueryEngine,
+    ToolRetrieverRouterQueryEngine,
 )
 from llama_index.query_engine.sql_join_query_engine import SQLJoinQueryEngine
 from llama_index.query_engine.sql_vector_query_engine import SQLAutoVectorQueryEngine
 from llama_index.query_engine.sub_question_query_engine import (
     SubQuestionQueryEngine,
     SubQuestionAnswerPair,
 )
@@ -36,8 +39,9 @@
     "SQLJoinQueryEngine",
     "SQLAutoVectorQueryEngine",
     "RetryQueryEngine",
     "RetrySourceQueryEngine",
     "RetryGuidelineQueryEngine",
     "FLAREInstructQueryEngine",
     "PandasQueryEngine",
+    "KnowledgeGraphQueryEngine",
 ]
```

### Comparing `llama_index-0.7.6/llama_index/query_engine/citation_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/citation_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/flare/answer_inserter.py` & `llama_index-0.7.7/llama_index/query_engine/flare/answer_inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/flare/base.py` & `llama_index-0.7.7/llama_index/query_engine/flare/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/flare/output_parser.py` & `llama_index-0.7.7/llama_index/query_engine/flare/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/pandas_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/pandas_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/retry_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/retry_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/retry_source_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/retry_source_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/router_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/sql_join_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/sql_join_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/sql_vector_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/sql_vector_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/sub_question_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/sub_question_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.7.7/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/question_gen/guidance_generator.py` & `llama_index-0.7.7/llama_index/question_gen/guidance_generator.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/question_gen/llm_generators.py` & `llama_index-0.7.7/llama_index/question_gen/llm_generators.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/question_gen/output_parser.py` & `llama_index-0.7.7/llama_index/question_gen/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/question_gen/prompts.py` & `llama_index-0.7.7/llama_index/question_gen/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/question_gen/types.py` & `llama_index-0.7.7/llama_index/question_gen/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/__init__.py` & `llama_index-0.7.7/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/base.py` & `llama_index-0.7.7/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.7.7/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/chroma.py` & `llama_index-0.7.7/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/database.py` & `llama_index-0.7.7/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/deeplake.py` & `llama_index-0.7.7/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/discord_reader.py` & `llama_index-0.7.7/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/download.py` & `llama_index-0.7.7/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/elasticsearch.py` & `llama_index-0.7.7/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/faiss.py` & `llama_index-0.7.7/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/base.py` & `llama_index-0.7.7/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/docs_reader.py` & `llama_index-0.7.7/llama_index/readers/file/docs_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/epub_reader.py` & `llama_index-0.7.7/llama_index/readers/file/epub_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/image_caption_reader.py` & `llama_index-0.7.7/llama_index/readers/file/image_caption_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/image_reader.py` & `llama_index-0.7.7/llama_index/readers/file/image_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/image_vision_llm_reader.py` & `llama_index-0.7.7/llama_index/readers/file/image_vision_llm_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/ipynb_reader.py` & `llama_index-0.7.7/llama_index/readers/file/ipynb_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/markdown_reader.py` & `llama_index-0.7.7/llama_index/readers/file/markdown_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/mbox_reader.py` & `llama_index-0.7.7/llama_index/readers/file/mbox_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/slides_reader.py` & `llama_index-0.7.7/llama_index/readers/file/slides_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/tabular_reader.py` & `llama_index-0.7.7/llama_index/readers/file/tabular_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/file/video_audio_reader.py` & `llama_index-0.7.7/llama_index/readers/file/video_audio_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.7.7/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.7.7/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/github_readers/utils.py` & `llama_index-0.7.7/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.7.7/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.7.7/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/json.py` & `llama_index-0.7.7/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/make_com/wrapper.py` & `llama_index-0.7.7/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/mbox.py` & `llama_index-0.7.7/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/metal.py` & `llama_index-0.7.7/llama_index/readers/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/milvus.py` & `llama_index-0.7.7/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/mongo.py` & `llama_index-0.7.7/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/myscale.py` & `llama_index-0.7.7/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/notion.py` & `llama_index-0.7.7/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/obsidian.py` & `llama_index-0.7.7/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/pinecone.py` & `llama_index-0.7.7/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/psychic.py` & `llama_index-0.7.7/llama_index/readers/psychic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/qdrant.py` & `llama_index-0.7.7/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/redis/utils.py` & `llama_index-0.7.7/llama_index/readers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/slack.py` & `llama_index-0.7.7/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/steamship/file_reader.py` & `llama_index-0.7.7/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/string_iterable.py` & `llama_index-0.7.7/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/twitter.py` & `llama_index-0.7.7/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/weaviate/reader.py` & `llama_index-0.7.7/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/web.py` & `llama_index-0.7.7/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/wikipedia.py` & `llama_index-0.7.7/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/readers/youtube_transcript.py` & `llama_index-0.7.7/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response/notebook_utils.py` & `llama_index-0.7.7/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response/pprint_utils.py` & `llama_index-0.7.7/llama_index/response/pprint_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response/schema.py` & `llama_index-0.7.7/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/__init__.py` & `llama_index-0.7.7/llama_index/response_synthesizers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/accumulate.py` & `llama_index-0.7.7/llama_index/response_synthesizers/accumulate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/base.py` & `llama_index-0.7.7/llama_index/response_synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/compact_and_accumulate.py` & `llama_index-0.7.7/llama_index/response_synthesizers/compact_and_accumulate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/compact_and_refine.py` & `llama_index-0.7.7/llama_index/response_synthesizers/compact_and_refine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/factory.py` & `llama_index-0.7.7/llama_index/response_synthesizers/factory.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/generation.py` & `llama_index-0.7.7/llama_index/response_synthesizers/generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/no_text.py` & `llama_index-0.7.7/llama_index/response_synthesizers/no_text.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/refine.py` & `llama_index-0.7.7/llama_index/response_synthesizers/refine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/simple_summarize.py` & `llama_index-0.7.7/llama_index/response_synthesizers/simple_summarize.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/tree_summarize.py` & `llama_index-0.7.7/llama_index/response_synthesizers/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/response_synthesizers/type.py` & `llama_index-0.7.7/llama_index/response_synthesizers/type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/retrievers/__init__.py` & `llama_index-0.7.7/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/retrievers/recursive_retriever.py` & `llama_index-0.7.7/llama_index/retrievers/recursive_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/retrievers/transform_retriever.py` & `llama_index-0.7.7/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/schema.py` & `llama_index-0.7.7/llama_index/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import abstractmethod
 from enum import Enum, auto
 from hashlib import sha256
 from pydantic import BaseModel, Field, root_validator
 from typing import Any, Dict, List, Optional, Union
 
 from llama_index.bridge.langchain import Document as LCDocument
-
+from llama_index.utils import SAMPLE_TEXT
 
 DEFAULT_TEXT_NODE_TMPL = "{metadata_str}\n\n{content}"
 DEFAULT_METADATA_TMPL = "{key}: {value}"
 
 
 class NodeRelationship(str, Enum):
     """Node relationships used in `BaseNode` class.
@@ -377,13 +377,21 @@
         return LCDocument(page_content=self.text, metadata=metadata)
 
     @classmethod
     def from_langchain_format(cls, doc: LCDocument) -> "Document":
         """Convert struct from LangChain document format."""
         return cls(text=doc.page_content, metadata=doc.metadata)
 
+    @classmethod
+    def example(cls) -> "Document":
+        document = Document(
+            text=SAMPLE_TEXT,
+            metadata={"filename": "README.md", "category": "codebase"},
+        )
+        return document
+
 
 class ImageDocument(Document):
     """Data document containing an image."""
 
     # base64 encoded image str
     image: Optional[str] = None
```

### Comparing `llama_index-0.7.6/llama_index/selectors/llm_selectors.py` & `llama_index-0.7.7/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/selectors/prompts.py` & `llama_index-0.7.7/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/selectors/pydantic_selectors.py` & `llama_index-0.7.7/llama_index/selectors/pydantic_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/selectors/types.py` & `llama_index-0.7.7/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/docstore/__init__.py` & `llama_index-0.7.7/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/docstore/dynamodb_docstore.py` & `llama_index-0.7.7/llama_index/storage/docstore/dynamodb_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.7.7/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.7.7/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/docstore/redis_docstore.py` & `llama_index-0.7.7/llama_index/storage/docstore/redis_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/docstore/registry.py` & `llama_index-0.7.7/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.7.7/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/docstore/types.py` & `llama_index-0.7.7/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/docstore/utils.py` & `llama_index-0.7.7/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/index_store/dynamodb_index_store.py` & `llama_index-0.7.7/llama_index/storage/index_store/dynamodb_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.7.7/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.7.7/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/index_store/redis_index_store.py` & `llama_index-0.7.7/llama_index/storage/index_store/redis_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/index_store/simple_index_store.py` & `llama_index-0.7.7/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/index_store/types.py` & `llama_index-0.7.7/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/index_store/utils.py` & `llama_index-0.7.7/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/kvstore/dynamodb_kvstore.py` & `llama_index-0.7.7/llama_index/storage/kvstore/dynamodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.7.7/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/kvstore/redis_kvstore.py` & `llama_index-0.7.7/llama_index/storage/kvstore/redis_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/kvstore/s3_kvstore.py` & `llama_index-0.7.7/llama_index/storage/kvstore/s3_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.7.7/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/kvstore/types.py` & `llama_index-0.7.7/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/storage/storage_context.py` & `llama_index-0.7.7/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.7.7/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/token_counter/utils.py` & `llama_index-0.7.7/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tools/function_tool.py` & `llama_index-0.7.7/llama_index/tools/function_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tools/ondemand_loader_tool.py` & `llama_index-0.7.7/llama_index/tools/ondemand_loader_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tools/query_engine.py` & `llama_index-0.7.7/llama_index/tools/query_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Optional, cast
 
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.langchain_helpers.agents.tools import IndexToolConfig, LlamaIndexTool
 from llama_index.tools.types import BaseTool, ToolMetadata, ToolOutput
 
-DEFAULT_NAME = "Query Engine Tool"
+DEFAULT_NAME = "query_engine_tool"
 DEFAULT_DESCRIPTION = """Useful for running a natural language query
 against a knowledge base and get back a natural language response.
 """
 
 
 class QueryEngineTool(BaseTool):
     """Query engine tool.
```

### Comparing `llama_index-0.7.6/llama_index/tools/query_plan.py` & `llama_index-0.7.7/llama_index/tools/query_plan.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tools/tool_spec/base.py` & `llama_index-0.7.7/llama_index/tools/tool_spec/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tools/tool_spec/load_and_search/base.py` & `llama_index-0.7.7/llama_index/tools/tool_spec/load_and_search/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tools/tool_spec/notion/base.py` & `llama_index-0.7.7/llama_index/tools/tool_spec/notion/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tools/tool_spec/slack/base.py` & `llama_index-0.7.7/llama_index/tools/tool_spec/slack/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tools/types.py` & `llama_index-0.7.7/llama_index/tools/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tools/utils.py` & `llama_index-0.7.7/llama_index/tools/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tts/bark.py` & `llama_index-0.7.7/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tts/base.py` & `llama_index-0.7.7/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/tts/elevenlabs.py` & `llama_index-0.7.7/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/types.py` & `llama_index-0.7.7/llama_index/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/utils.py` & `llama_index-0.7.7/llama_index/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -230,7 +230,35 @@
         from transformers import AutoTokenizer
     except ImportError:
         raise ValueError(
             "`transformers` package not found, please run `pip install transformers`"
         )
     tokenizer = AutoTokenizer.from_pretrained(model_name)
     return tokenizer.tokenize
+
+
+# Sample text from llama_index's readme
+SAMPLE_TEXT = """
+Context
+LLMs are a phenomenonal piece of technology for knowledge generation and reasoning. 
+They are pre-trained on large amounts of publicly available data.
+How do we best augment LLMs with our own private data?
+We need a comprehensive toolkit to help perform this data augmentation for LLMs.
+
+Proposed Solution
+That's where LlamaIndex comes in. LlamaIndex is a "data framework" to help 
+you build LLM  apps. It provides the following tools:
+
+Offers data connectors to ingest your existing data sources and data formats 
+(APIs, PDFs, docs, SQL, etc.)
+Provides ways to structure your data (indices, graphs) so that this data can be 
+easily used with LLMs.
+Provides an advanced retrieval/query interface over your data: 
+Feed in any LLM input prompt, get back retrieved context and knowledge-augmented output.
+Allows easy integrations with your outer application framework 
+(e.g. with LangChain, Flask, Docker, ChatGPT, anything else).
+LlamaIndex provides tools for both beginner users and advanced users. 
+Our high-level API allows beginner users to use LlamaIndex to ingest and 
+query their data in 5 lines of code. Our lower-level APIs allow advanced users to 
+customize and extend any module (data connectors, indices, retrievers, query engines, 
+reranking modules), to fit their needs.
+"""
```

### Comparing `llama_index-0.7.6/llama_index/vector_stores/__init__.py` & `llama_index-0.7.7/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.7.7/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/chroma.py` & `llama_index-0.7.7/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/deeplake.py` & `llama_index-0.7.7/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/docarray/base.py` & `llama_index-0.7.7/llama_index/vector_stores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/docarray/hnsw.py` & `llama_index-0.7.7/llama_index/vector_stores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/docarray/in_memory.py` & `llama_index-0.7.7/llama_index/vector_stores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/dynamodb.py` & `llama_index-0.7.7/llama_index/vector_stores/dynamodb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/faiss.py` & `llama_index-0.7.7/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/lancedb.py` & `llama_index-0.7.7/llama_index/vector_stores/lancedb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/metal.py` & `llama_index-0.7.7/llama_index/vector_stores/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/milvus.py` & `llama_index-0.7.7/llama_index/vector_stores/milvus.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,32 @@
 from llama_index.vector_stores.types import (
     NodeWithEmbedding,
     VectorStore,
     VectorStoreQuery,
     VectorStoreQueryMode,
     VectorStoreQueryResult,
 )
-from llama_index.vector_stores.utils import node_to_metadata_dict, metadata_dict_to_node
+from llama_index.vector_stores.utils import (
+    node_to_metadata_dict,
+    metadata_dict_to_node,
+    DEFAULT_DOC_ID_KEY,
+    DEFAULT_EMBEDDING_KEY,
+    DEFAULT_TEXT_KEY,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class MilvusVectorStore(VectorStore):
     """The Milvus Vector Store.
 
     In this vector store we store the text, its embedding and
     a few pieces of its metadata in a Milvus collection. This implemnetation
-    allows the use of an already existing collection if it is one that was created
-    this vector store. It also supports creating a new one if the collection doesnt
+    allows the use of an already existing collection.
+    It also supports creating a new one if the collection doesnt
     exist or if `overwrite` is set to True.
 
     Args:
         collection_name (str, optional): The name of the collection where data will be
             stored. Defaults to "llamalection".
         index_params (dict, optional): The index parameters for Milvus, if none are
             provided an HNSW index will be used. Defaults to None.
@@ -61,14 +67,18 @@
 
     def __init__(
         self,
         collection_name: str = "llamalection",
         index_params: Optional[dict] = None,
         search_params: Optional[dict] = None,
         dim: Optional[int] = None,
+        embedding_field: str = DEFAULT_EMBEDDING_KEY,
+        text_field: str = DEFAULT_TEXT_KEY,
+        doc_id_field: str = DEFAULT_DOC_ID_KEY,
+        consistency_level: Optional[str] = "Strong",
         host: str = "localhost",
         port: int = 19530,
         user: str = "",
         password: str = "",
         use_secure: bool = False,
         overwrite: bool = False,
         **kwargs: Any,
@@ -84,14 +94,18 @@
 
         from pymilvus import Collection, MilvusException, utility
 
         self.collection_name = collection_name
         self.search_params = search_params
         self.index_params = index_params
         self.dim = dim
+        self.embedding_field = embedding_field
+        self.text_field = text_field
+        self.doc_id_field = doc_id_field
+        self.consistency_level = consistency_level
         self.host = host
         self.port = port
         self.user = user
         self.password = password
         self.use_secure = use_secure
         self.overwrite = overwrite
 
@@ -109,17 +123,15 @@
         }
 
         # Generate a connection alias
         self._create_connection_alias()
 
         # Figure out if there is already a created collection
         if utility.has_collection(self.collection_name, using=self.alias):
-            self.collection = Collection(
-                self.collection_name, using=self.alias, consistency_level="Strong"
-            )
+            self.collection = Collection(self.collection_name, using=self.alias)
         else:
             self.collection = None
 
         # If a collection already exists and we are overwriting, delete it
         if self.collection is not None and self.overwrite is True:
             try:
                 utility.drop_collection(self.collection_name, using=self.alias)
@@ -196,27 +208,27 @@
                     dtype=DataType.VARCHAR,
                     description="Unique ID",
                     is_primary=True,
                     auto_id=False,
                     max_length=65535,
                 ),
                 FieldSchema(
-                    name="doc_id",
+                    name=self.doc_id_field,
                     dtype=DataType.VARCHAR,
                     description="Source document ID",
                     max_length=65535,
                 ),
                 FieldSchema(
-                    name="text",
+                    name=self.text_field,
                     dtype=DataType.VARCHAR,
                     description="The embedding vector",
                     max_length=65535,
                 ),
                 FieldSchema(
-                    name="embedding",
+                    name=self.embedding_field,
                     dtype=DataType.FLOAT_VECTOR,
                     description="The embedding vector",
                     dim=self.dim,
                 ),
                 FieldSchema(
                     name="node",
                     dtype=DataType.VARCHAR,
@@ -226,15 +238,15 @@
             ]
 
             col_schema = CollectionSchema(fields=fields)
             self.collection = Collection(
                 self.collection_name,
                 col_schema,
                 using=self.alias,
-                consistency_level="Strong",
+                consistency_level=self.consistency_level,
             )
             logger.debug(
                 f"Successfully created a new collection: {self.collection_name}"
             )
 
         except MilvusException as e:
             logger.debug(f"Failure to create a new collection: {self.collection_name}")
@@ -251,26 +263,30 @@
                     "index_type": "HNSW",
                     "params": {"M": 8, "efConstruction": 64},
                 }
             assert self.index_params is not None
 
             try:
                 self.collection.create_index(
-                    "embedding", index_params=self.index_params, using=self.alias
+                    self.embedding_field,
+                    index_params=self.index_params,
+                    using=self.alias,
                 )
             # If default did not work, most likely on Zilliz Cloud
             except MilvusException:
                 # Attempt creating autoindex
                 self.index_params = {
                     "metric_type": "IP",
                     "index_type": "AUTOINDEX",
                     "params": {},
                 }
                 self.collection.create_index(
-                    "embedding", index_params=self.index_params, using=self.alias
+                    self.embedding_field,
+                    index_params=self.index_params,
+                    using=self.alias,
                 )
 
             # If search params dont exist already, grab the default
             if self.search_params is None:
                 self.search_params = self.default_search_params[
                     self.index_params["index_type"]
                 ]
@@ -370,15 +386,17 @@
             doc_ids = [ref_doc_id]
         else:
             doc_ids = ref_doc_id  # type: ignore
 
         try:
             # Begin by querying for the primary keys to delete
             doc_ids = ['"' + entry + '"' for entry in doc_ids]
-            entries = self.collection.query(f"doc_id in [{','.join(doc_ids)}]")
+            entries = self.collection.query(
+                f"{self.doc_id_field} in [{','.join(doc_ids)}]"
+            )
             ids = [entry["id"] for entry in entries]
             ids = ['"' + entry + '"' for entry in ids]
             self.collection.delete(f"id in [{','.join(ids)}]")
             logger.debug(f"Successfully deleted embedding with doc_id: {doc_ids}")
         except MilvusException as e:
             logger.debug(f"Unsuccessfully deleted embedding with doc_id: {doc_ids}")
             raise e
@@ -386,14 +404,16 @@
     def query(self, query: VectorStoreQuery, **kwargs: Any) -> VectorStoreQueryResult:
         """Query index for top k most similar nodes.
 
         Args:
             query_embedding (List[float]): query embedding
             similarity_top_k (int): top k most similar nodes
             doc_ids (Optional[List[str]]): list of doc_ids to filter by
+            output_fields (Optional[List[str]]): list of fields to return
+            embedding_field (Optional[str]): name of embedding field
         """
         from pymilvus import MilvusException
 
         if self.collection is None:
             raise ValueError("Milvus instance not initialized.")
 
         if query.mode != VectorStoreQueryMode.DEFAULT:
@@ -401,60 +421,66 @@
 
         if query.filters is not None:
             raise ValueError("Metadata filters not implemented for Milvus yet.")
 
         expr: Optional[str] = None
         if query.doc_ids is not None and len(query.doc_ids) != 0:
             expr_list = ['"' + entry + '"' for entry in query.doc_ids]
-            expr = f"doc_id in [{','.join(expr_list)}]"
+            expr = f"{self.doc_id_field} in [{','.join(expr_list)}]"
+
+        if query.output_fields is None:
+            output_fields = [self.doc_id_field, self.text_field]
+
+        if query.embedding_field is None:
+            embedding_field = self.embedding_field
 
         try:
             res = self.collection.search(
                 [query.query_embedding],
-                "embedding",
+                embedding_field,
                 self.search_params,
                 limit=query.similarity_top_k,
-                output_fields=["doc_id", "text", "node"],
+                output_fields=output_fields + ["node"],
                 expr=expr,
             )
             logger.debug(
                 f"Successfully searched embedding in collection: {self.collection_name}"
                 f" Num Results: {len(res[0])}"
             )
         except MilvusException:
             # TODO: Legacy support for old dbs
             res = self.collection.search(
                 [query.query_embedding],
                 "embedding",
                 self.search_params,
                 limit=query.similarity_top_k,
-                output_fields=["doc_id", "text"],
+                output_fields=output_fields,
                 expr=expr,
             )
             logger.debug(
                 f"Successfully searched embedding in collection: {self.collection_name}"
                 f" Num Results: {len(res[0])}"
             )
 
         nodes = []
         similarities = []
         ids = []
 
         for hit in res[0]:
             try:
                 node = metadata_dict_to_node({"_node_content": hit.entity.get("node")})
-                node.text = hit.entity.get("text")
+                node.text = hit.entity.get(self.text_field)
             except Exception:
                 # TODO: Legacy support for old nodes
                 node = TextNode(
-                    text=hit.entity.get("text"),
+                    text=hit.entity.get(self.text_field),
                     id_=hit.id,
                     relationships={
                         NodeRelationship.SOURCE: RelatedNodeInfo(
-                            node_id=hit.entity.get("doc_id")
+                            node_id=hit.entity.get(self.doc_id_field)
                         ),
                     },
                 )
             nodes.append(node)
             similarities.append(hit.score)
             ids.append(hit.id)
```

### Comparing `llama_index-0.7.6/llama_index/vector_stores/mongodb.py` & `llama_index-0.7.7/llama_index/vector_stores/mongodb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/myscale.py` & `llama_index-0.7.7/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/opensearch.py` & `llama_index-0.7.7/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/pinecone.py` & `llama_index-0.7.7/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/postgres.py` & `llama_index-0.7.7/llama_index/vector_stores/postgres.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/qdrant.py` & `llama_index-0.7.7/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/redis.py` & `llama_index-0.7.7/llama_index/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/registry.py` & `llama_index-0.7.7/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/simple.py` & `llama_index-0.7.7/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/supabase.py` & `llama_index-0.7.7/llama_index/vector_stores/supabase.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/tair.py` & `llama_index-0.7.7/llama_index/vector_stores/tair.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/types.py` & `llama_index-0.7.7/llama_index/vector_stores/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,14 +120,16 @@
     """Vector store query."""
 
     query_embedding: Optional[List[float]] = None
     similarity_top_k: int = 1
     doc_ids: Optional[List[str]] = None
     node_ids: Optional[List[str]] = None
     query_str: Optional[str] = None
+    output_fields: Optional[List[str]] = None
+    embedding_field: Optional[str] = None
 
     mode: VectorStoreQueryMode = VectorStoreQueryMode.DEFAULT
 
     # NOTE: only for hybrid search (0 for bm25, 1 for vector search)
     alpha: Optional[float] = None
 
     # metadata filters
```

### Comparing `llama_index-0.7.6/llama_index/vector_stores/typesense.py` & `llama_index-0.7.7/llama_index/vector_stores/typesense.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/utils.py` & `llama_index-0.7.7/llama_index/vector_stores/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 from typing import Any, Dict, Tuple
 
 from llama_index.schema import BaseNode, NodeRelationship, RelatedNodeInfo, TextNode
 
 DEFAULT_TEXT_KEY = "text"
+DEFAULT_EMBEDDING_KEY = "embedding"
+DEFAULT_DOC_ID_KEY = "doc_id"
 
 
 def _validate_is_flat_dict(metadata_dict: dict) -> None:
     """
     Validate that metadata dict is flat,
     and key is str, and value is one of (str, int, float, None).
     """
```

### Comparing `llama_index-0.7.6/llama_index/vector_stores/weaviate.py` & `llama_index-0.7.7/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index/vector_stores/weaviate_utils.py` & `llama_index-0.7.7/llama_index/vector_stores/weaviate_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/llama_index.egg-info/PKG-INFO` & `llama_index-0.7.7/llama_index.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index
-Version: 0.7.6
+Version: 0.7.7
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 Author: Jerry Liu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `llama_index-0.7.6/llama_index.egg-info/SOURCES.txt` & `llama_index-0.7.7/llama_index.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 llama_index/callbacks/base.py
 llama_index/callbacks/llama_debug.py
 llama_index/callbacks/schema.py
 llama_index/callbacks/token_counting.py
 llama_index/callbacks/wandb_callback.py
 llama_index/chat_engine/__init__.py
 llama_index/chat_engine/condense_question.py
-llama_index/chat_engine/react.py
 llama_index/chat_engine/simple.py
 llama_index/chat_engine/types.py
 llama_index/chat_engine/utils.py
 llama_index/composability/__init__.py
 llama_index/composability/base.py
 llama_index/composability/joint_qa_summary.py
 llama_index/data_structs/__init__.py
@@ -224,14 +223,15 @@
 llama_index/prompts/prompt_type.py
 llama_index/prompts/prompts.py
 llama_index/prompts/system.py
 llama_index/prompts/utils.py
 llama_index/query_engine/__init__.py
 llama_index/query_engine/citation_query_engine.py
 llama_index/query_engine/graph_query_engine.py
+llama_index/query_engine/knowledge_graph_query_engine.py
 llama_index/query_engine/multistep_query_engine.py
 llama_index/query_engine/pandas_query_engine.py
 llama_index/query_engine/retriever_query_engine.py
 llama_index/query_engine/retry_query_engine.py
 llama_index/query_engine/retry_source_query_engine.py
 llama_index/query_engine/router_query_engine.py
 llama_index/query_engine/sql_join_query_engine.py
```

### Comparing `llama_index-0.7.6/setup.py` & `llama_index-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/callbacks/test_llama_debug.py` & `llama_index-0.7.7/tests/callbacks/test_llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/callbacks/test_token_counter.py` & `llama_index-0.7.7/tests/callbacks/test_token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/chat_engine/test_condense_question.py` & `llama_index-0.7.7/tests/chat_engine/test_condense_question.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/chat_engine/test_simple.py` & `llama_index-0.7.7/tests/chat_engine/test_simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/conftest.py` & `llama_index-0.7.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/embeddings/test_base.py` & `llama_index-0.7.7/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/composability/test_utils.py` & `llama_index-0.7.7/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/conftest.py` & `llama_index-0.7.7/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/document_summary/test_index.py` & `llama_index-0.7.7/tests/indices/document_summary/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/empty/test_base.py` & `llama_index-0.7.7/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/keyword_table/test_base.py` & `llama_index-0.7.7/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/keyword_table/test_retrievers.py` & `llama_index-0.7.7/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/keyword_table/test_utils.py` & `llama_index-0.7.7/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/knowledge_graph/test_base.py` & `llama_index-0.7.7/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/knowledge_graph/test_retrievers.py` & `llama_index-0.7.7/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/list/test_index.py` & `llama_index-0.7.7/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/list/test_retrievers.py` & `llama_index-0.7.7/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/postprocessor/test_base.py` & `llama_index-0.7.7/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/postprocessor/test_llm_rerank.py` & `llama_index-0.7.7/tests/indices/postprocessor/test_llm_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/postprocessor/test_optimizer.py` & `llama_index-0.7.7/tests/indices/postprocessor/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/query/conftest.py` & `llama_index-0.7.7/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/query/query_transform/test_base.py` & `llama_index-0.7.7/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/query/test_compose.py` & `llama_index-0.7.7/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/query/test_compose_vector.py` & `llama_index-0.7.7/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/query/test_embedding_utils.py` & `llama_index-0.7.7/tests/indices/query/test_embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/query/test_query_bundle.py` & `llama_index-0.7.7/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/struct_store/conftest.py` & `llama_index-0.7.7/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/struct_store/test_base.py` & `llama_index-0.7.7/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/struct_store/test_json_query.py` & `llama_index-0.7.7/tests/indices/struct_store/test_json_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/struct_store/test_sql_query.py` & `llama_index-0.7.7/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/test_loading.py` & `llama_index-0.7.7/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/test_loading_graph.py` & `llama_index-0.7.7/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/test_node_utils.py` & `llama_index-0.7.7/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/test_prompt_helper.py` & `llama_index-0.7.7/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/tree/conftest.py` & `llama_index-0.7.7/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/tree/test_embedding_retriever.py` & `llama_index-0.7.7/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/tree/test_index.py` & `llama_index-0.7.7/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/tree/test_retrievers.py` & `llama_index-0.7.7/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/vector_store/auto_retriever/test_output_parser.py` & `llama_index-0.7.7/tests/indices/vector_store/auto_retriever/test_output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/vector_store/conftest.py` & `llama_index-0.7.7/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/vector_store/mock_faiss.py` & `llama_index-0.7.7/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/vector_store/mock_services.py` & `llama_index-0.7.7/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/vector_store/test_faiss.py` & `llama_index-0.7.7/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/vector_store/test_myscale.py` & `llama_index-0.7.7/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/vector_store/test_pinecone.py` & `llama_index-0.7.7/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/vector_store/test_retrievers.py` & `llama_index-0.7.7/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/vector_store/test_simple.py` & `llama_index-0.7.7/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/indices/vector_store/utils.py` & `llama_index-0.7.7/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/langchain_helpers/test_text_splitter.py` & `llama_index-0.7.7/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/llm_predictor/test_base.py` & `llama_index-0.7.7/tests/llm_predictor/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 
 from llama_index.llm_predictor.structured import LLMPredictor, StructuredLLMPredictor
 from llama_index.types import BaseOutputParser
 from llama_index.prompts.prompts import Prompt, SimpleInputPrompt
 
 try:
-
     gptcache_installed = True
 except ImportError:
     gptcache_installed = False
 
 
 class MockOutputParser(BaseOutputParser):
     """Mock output parser."""
```

### Comparing `llama_index-0.7.6/tests/llm_predictor/vellum/conftest.py` & `llama_index-0.7.7/tests/llm_predictor/vellum/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/llm_predictor/vellum/test_predictor.py` & `llama_index-0.7.7/tests/llm_predictor/vellum/test_predictor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/llm_predictor/vellum/test_prompt_registry.py` & `llama_index-0.7.7/tests/llm_predictor/vellum/test_prompt_registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/llms/test_anthropic.py` & `llama_index-0.7.7/tests/llms/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/llms/test_anthropic_utils.py` & `llama_index-0.7.7/tests/llms/test_anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/llms/test_custom.py` & `llama_index-0.7.7/tests/llms/test_custom.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/llms/test_langchain.py` & `llama_index-0.7.7/tests/llms/test_langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/llms/test_openai.py` & `llama_index-0.7.7/tests/llms/test_openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/llms/test_openai_utils.py` & `llama_index-0.7.7/tests/llms/test_openai_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/llms/test_palm.py` & `llama_index-0.7.7/tests/llms/test_palm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/logger/test_base.py` & `llama_index-0.7.7/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/mock_utils/mock_predict.py` & `llama_index-0.7.7/tests/mock_utils/mock_predict.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/mock_utils/mock_prompts.py` & `llama_index-0.7.7/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/mock_utils/mock_text_splitter.py` & `llama_index-0.7.7/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/mock_utils/mock_utils.py` & `llama_index-0.7.7/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/objects/test_base.py` & `llama_index-0.7.7/tests/objects/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/objects/test_node_mapping.py` & `llama_index-0.7.7/tests/objects/test_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/output_parsers/test_base.py` & `llama_index-0.7.7/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/output_parsers/test_pydantic.py` & `llama_index-0.7.7/tests/output_parsers/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/output_parsers/test_selection.py` & `llama_index-0.7.7/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/playground/test_base.py` & `llama_index-0.7.7/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/program/test_guidance.py` & `llama_index-0.7.7/tests/program/test_guidance.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/program/test_llm_program.py` & `llama_index-0.7.7/tests/program/test_llm_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/prompts/test_base.py` & `llama_index-0.7.7/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/prompts/test_guidance_utils.py` & `llama_index-0.7.7/tests/prompts/test_guidance_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/question_gen/test_guidance_generator.py` & `llama_index-0.7.7/tests/question_gen/test_guidance_generator.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/question_gen/test_llm_generators.py` & `llama_index-0.7.7/tests/question_gen/test_llm_generators.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/readers/test_file.py` & `llama_index-0.7.7/tests/readers/test_file.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/readers/test_json.py` & `llama_index-0.7.7/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/readers/test_mongo.py` & `llama_index-0.7.7/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/selectors/test_llm_selectors.py` & `llama_index-0.7.7/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/storage/conftest.py` & `llama_index-0.7.7/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/storage/docstore/test_dynamodb_docstore.py` & `llama_index-0.7.7/tests/storage/docstore/test_dynamodb_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/storage/docstore/test_mongo_docstore.py` & `llama_index-0.7.7/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/storage/docstore/test_redis_docstore.py` & `llama_index-0.7.7/tests/storage/docstore/test_redis_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/storage/docstore/test_simple_docstore.py` & `llama_index-0.7.7/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/storage/test_storage_context.py` & `llama_index-0.7.7/tests/storage/test_storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/test_utils.py` & `llama_index-0.7.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/token_predictor/test_base.py` & `llama_index-0.7.7/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/tools/test_base.py` & `llama_index-0.7.7/tests/tools/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/tools/test_ondemand_loader.py` & `llama_index-0.7.7/tests/tools/test_ondemand_loader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/tools/test_utils.py` & `llama_index-0.7.7/tests/tools/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/tools/tool_spec/test_base.py` & `llama_index-0.7.7/tests/tools/tool_spec/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/vector_stores/test_docarray.py` & `llama_index-0.7.7/tests/vector_stores/test_docarray.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/vector_stores/test_postgres.py` & `llama_index-0.7.7/tests/vector_stores/test_postgres.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/vector_stores/test_qdrant.py` & `llama_index-0.7.7/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/vector_stores/test_tair.py` & `llama_index-0.7.7/tests/vector_stores/test_tair.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.6/tests/vector_stores/test_weaviate.py` & `llama_index-0.7.7/tests/vector_stores/test_weaviate.py`

 * *Files identical despite different names*

