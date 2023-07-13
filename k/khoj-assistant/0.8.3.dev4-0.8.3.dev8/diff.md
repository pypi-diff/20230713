# Comparing `tmp/khoj_assistant-0.8.3.dev4.tar.gz` & `tmp/khoj_assistant-0.8.3.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jul 11 04:27:58 2023, max compression
+gzip compressed data, last modified: Thu Jul 13 05:22:49 2023, max compression
```

## Comparing `khoj_assistant-0.8.3.dev4.tar` & `khoj_assistant-0.8.3.dev8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/__init__.py
--rw-r--r--   0        0        0    11626 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/configure.py
--rw-r--r--   0        0        0     5389 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     4897 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    18018 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    16252 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6930 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     7322 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0     3401 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_notion_input.html
--rw-r--r--   0        0        0    18924 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3660 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     2433 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     1578 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     7946 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4455 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     4824 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     3991 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     8304 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13517 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0     9295 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/notion/notion_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5397 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    20526 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/routers/api.py
--rw-r--r--   0        0        0      167 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     2895 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0     5524 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7566 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11237 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2042 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2571 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2710 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6889 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4338 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/LICENSE
--rw-r--r--   0        0        0    24858 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/README.md
--rw-r--r--   0        0        0     2792 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/pyproject.toml
--rw-r--r--   0        0        0    27222 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11626 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/configure.py
+-rw-r--r--   0        0        0     5515 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     4897 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    18018 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    16252 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     7322 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0     3401 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_notion_input.html
+-rw-r--r--   0        0        0    18924 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3660 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     2433 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     1578 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     7946 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4455 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     4824 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     3991 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     8304 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13517 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0     9295 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/notion/notion_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5397 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    20526 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/routers/api.py
+-rw-r--r--   0        0        0      167 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     2895 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0     5524 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7566 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11237 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2042 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2571 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2710 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6889 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4338 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/LICENSE
+-rw-r--r--   0        0        0    24858 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/README.md
+-rw-r--r--   0        0        0     2792 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/pyproject.toml
+-rw-r--r--   0        0        0    27222 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/PKG-INFO
```

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/configure.py` & `khoj_assistant-0.8.3.dev8/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/main.py` & `khoj_assistant-0.8.3.dev8/src/khoj/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Standard Packages
 import os
 import signal
 import sys
+
+if sys.stdout is None:
+    sys.stdout = open(os.devnull, "w")
+if sys.stderr is None:
+    sys.stderr = open(os.devnull, "w")
+
 import logging
 import threading
 import warnings
 from platform import system
 import webbrowser
 
 # Ignore non-actionable warnings
```

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/404.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/chat.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/config.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_notion_input.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_notion_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/index.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/notion/notion_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/notion/notion_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/routers/api.py` & `khoj_assistant-0.8.3.dev8/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/routers/helpers.py` & `khoj_assistant-0.8.3.dev8/src/khoj/routers/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/routers/web_client.py` & `khoj_assistant-0.8.3.dev8/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/search_type/image_search.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/search_type/text_search.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/utils/cli.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/utils/config.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/utils/constants.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/utils/helpers.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/utils/jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/utils/models.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/utils/state.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/src/khoj/utils/yaml.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/.gitignore` & `khoj_assistant-0.8.3.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/LICENSE` & `khoj_assistant-0.8.3.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/README.md` & `khoj_assistant-0.8.3.dev8/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/pyproject.toml` & `khoj_assistant-0.8.3.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev4/PKG-INFO` & `khoj_assistant-0.8.3.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.8.3.dev4
+Version: 0.8.3.dev8
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

