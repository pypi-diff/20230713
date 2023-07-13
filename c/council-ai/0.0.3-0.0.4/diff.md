# Comparing `tmp/council_ai-0.0.3.tar.gz` & `tmp/council_ai-0.0.4.tar.gz`

## Comparing `council_ai-0.0.3.tar` & `council_ai-0.0.4.tar`

### file list

```diff
@@ -1,122 +1,126 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.3/Makefile
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.3/requirements.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/agent_tests/__init__.py
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/agent_tests/agent_tests.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/controller/__init__.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/controller/basic_controller.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/controller/llm_controller.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/__init__.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/agent.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/agent_chain.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/budget.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/cancellation_token.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/chain.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/controller_base.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/evaluator_base.py
--rw-r--r--   0        0        0    14710 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/execution_context.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/execution_unit.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/result.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/runners.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/scorer_base.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/core/skill_base.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/evaluator/__init__.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/evaluator/basic_evaluator.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/evaluator/llm_evaluator.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/llm/__init__.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/llm/azure_configuration.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/llm/azure_llm.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/llm/llm_base.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/llm/llm_exception.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/llm/llm_message.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/llm/openai_configuration.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/llm/openai_llm.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/mocks/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/prompt/__init__.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/prompt/prompt_builder.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/scorer/__init__.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/scorer/llm_similarity_scorer.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/skill/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/skill/llm_skill.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/skill/google/__init__.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/skill/google/google_news_skill.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/skill/google/google_search_skill.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/skill/google/google_context/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/skill/google/google_context/context_provider.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/skill/google/google_context/google_news.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/skill/google/google_context/google_search.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/skill/google/google_context/schemas.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/utils/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/utils/env.py
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 council_ai-0.0.3/council/utils/option.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/.gitignore
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/Makefile
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/README.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/docker-compose.yaml
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/dockerfile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/make.bat
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/requirements.txt
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/conf.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/index.rst
--rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/_static/00_chainml_logo.png
--rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/_static/02_chainml_logo_black.png
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/concepts/key_concepts.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/contributing/contributing.rst
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/examples/langchain_llm_integration.ipynb
--rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/examples/my_first_agent.ipynb
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/getting_started/usage.rst
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/introduction/introduction.rst
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context.rst
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/controller.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/core.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/evaluator.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/llm.rst
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/runners.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/scorer.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/skill.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/utils.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/agent_context.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/agent_message.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/chain_context.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/chain_history.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/chat_history.rst
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/chat_message_base.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/iteration_context.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/scored_agent_message.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/skill_context.rst
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/skill_error_message.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/skill_message.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/skill_success_message.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/context/user_message.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/controller/basic_controller.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/controller/llm_controller.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/core/agent.rst
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/core/agent_result.rst
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/core/budget.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/core/chain.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/core/controller_base.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/core/evaluator_base.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/core/scorer_base.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/core/similarity_scorer_exception.rst
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/core/skill_base.rst
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/evaluator/basic_evaluator.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/evaluator/llm_evaluator.rst
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/llm/azure_configuration.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/llm/azure_llm.rst
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/llm/llm_base.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/llm/llm_message.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/llm/openai_configuration.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/llm/openai_llm.rst
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/runners/parallel_for.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/scorer/llm_similarity_scorer.rst
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/skill/llm_skill.rst
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/skill/google/google_news_skill.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/skill/google/google_search_skill.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/utils/option.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.3/docs/source/reference/utils/option_exception.rst
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.3/stubs/GoogleNews.pyi
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 council_ai-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.3/LICENSE
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 council_ai-0.0.3/README.md
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 council_ai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 council_ai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.4/Makefile
+-rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.4/engine_flow.png
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.4/requirements.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agent_tests/__init__.py
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agent_tests/agent_tests.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agents/__init__.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agents/agent.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agents/agent_chain.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agents/agent_result.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/controllers/__init__.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/controllers/basic_controller.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/controllers/controller_base.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/controllers/llm_controller.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/budget.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/cancellation_token.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/chain.py
+-rw-r--r--   0        0        0    14710 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/execution_context.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/execution_unit.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/result.py
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/runners.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/scorer_base.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/skill_base.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/evaluators/__init__.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/evaluators/basic_evaluator.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/evaluators/evaluator_base.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/__init__.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/azure_configuration.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/azure_llm.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/llm_base.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/llm_exception.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/llm_message.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/openai_configuration.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/openai_llm.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/mocks/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/prompt/__init__.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/prompt/prompt_builder.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/scorer/__init__.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/scorer/llm_similarity_scorer.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/llm_skill.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/__init__.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_news_skill.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_search_skill.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_context/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_context/context_provider.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_context/google_news.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_context/google_search.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_context/schemas.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/utils/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/utils/env.py
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/utils/option.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/.gitignore
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/Makefile
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/README.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/docker-compose.yaml
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/dockerfile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/make.bat
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/requirements.txt
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/conf.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/index.rst
+-rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/_static/00_chainml_logo.png
+-rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/_static/02_chainml_logo_black.png
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/concepts/key_concepts.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/contributing/contributing.rst
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/examples/langchain_llm_integration.ipynb
+-rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/examples/my_first_agent.ipynb
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/getting_started/usage.rst
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/introduction/introduction.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/agents.rst
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/controllers.rst
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/evaluators.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm.rst
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/runners.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/scorer.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/skill.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/utils.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/agents/agent.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/agents/agent_result.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/agent_context.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/agent_message.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/chain_context.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/chain_history.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/chat_history.rst
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/chat_message_base.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/iteration_context.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/scored_agent_message.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/skill_context.rst
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/skill_error_message.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/skill_message.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/skill_success_message.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/user_message.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/controllers/basic_controller.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/controllers/controller_base.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/controllers/llm_controller.rst
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core/budget.rst
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core/chain.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core/scorer_base.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core/similarity_scorer_exception.rst
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core/skill_base.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/evaluators/basic_evaluator.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/evaluators/evaluator_base.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/evaluators/llm_evaluator.rst
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/azure_configuration.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/azure_llm.rst
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/llm_base.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/llm_message.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/openai_configuration.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/openai_llm.rst
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/runners/parallel_for.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/scorer/llm_similarity_scorer.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/skill/llm_skill.rst
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/skill/google/google_news_skill.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/skill/google/google_search_skill.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/utils/option.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/utils/option_exception.rst
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.4/stubs/GoogleNews.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.4/LICENSE
+-rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 council_ai-0.0.4/README.md
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 council_ai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 council_ai-0.0.4/PKG-INFO
```

### Comparing `council_ai-0.0.3/council/agent_tests/agent_tests.py` & `council_ai-0.0.4/council/agent_tests/agent_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 from enum import Enum
-from typing import List, Dict, Any, Sequence
+from typing import List, Dict, Any, Sequence, Optional
 import progressbar  # type: ignore
+from council.agents import Agent
 
 from council.core import (
-    Agent,
     ScorerBase,
     AgentContext,
     ChatHistory,
     Budget,
     ScorerException,
 )
 
@@ -179,16 +179,19 @@
         result = {"results": results}
         return result
 
 
 class AgentTestSuite:
     _test_cases: List[AgentTestCase]
 
-    def __init__(self, test_cases: List[AgentTestCase] = []):
-        self._test_cases = test_cases
+    def __init__(self, test_cases: Optional[List[AgentTestCase]] = None):
+        if test_cases is not None:
+            self._test_cases = test_cases
+        else:
+            self._test_cases = []
 
     def add_test_case(self, prompt: str, scorers: List[ScorerBase]) -> "AgentTestSuite":
         self._test_cases.append(AgentTestCase(prompt, scorers))
         return self
 
     def run(self, agent: Agent, show_progressbar: bool = True) -> AgentTestSuiteResult:
         pb = None
```

### Comparing `council_ai-0.0.3/council/controller/basic_controller.py` & `council_ai-0.0.4/council/controllers/basic_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List
 
-from council.core import ControllerBase, AgentContext, Chain, Budget
+from .controller_base import ControllerBase
+from council.core import AgentContext, Chain, Budget
 from council.core.execution_context import ScoredAgentMessage
 from council.core.execution_unit import ExecutionUnit
 
 
 class BasicController(ControllerBase):
     """a basic controller that requests all chains to be executed and returns all results"""
```

### Comparing `council_ai-0.0.3/council/controller/llm_controller.py` & `council_ai-0.0.4/council/controllers/llm_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import List, Tuple
 
-from council.core import AgentContext, Budget, ControllerBase
+from .controller_base import ControllerBase
+from council.core import AgentContext, Budget
 from council.core.chain import Chain
 from council.core.execution_context import ScoredAgentMessage
 from council.core.execution_unit import ExecutionUnit
 from council.llm import LLMMessage, LLMBase
 from council.utils import Option
 
 logger = logging.getLogger(__name__)
```

### Comparing `council_ai-0.0.3/council/core/agent.py` & `council_ai-0.0.4/council/agents/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,23 @@
 import logging
-from typing import List, Optional
-from collections.abc import Sequence
+from typing import List
 
 from council.core.budget import Budget
 from council.core.chain import Chain
-from council.core.controller_base import ControllerBase
-from council.core.evaluator_base import EvaluatorBase
-from council.core.execution_context import AgentContext, ScoredAgentMessage, AgentMessage
+from council.controllers import ControllerBase, BasicController
+from council.evaluators.evaluator_base import EvaluatorBase
+from council.core.execution_context import AgentContext, ChatHistory
 from council.core.runners import new_runner_executor
-from council.utils import Option
+from .agent_result import AgentResult
+from ..core import SkillBase
+from ..evaluators import BasicEvaluator
 
 logger = logging.getLogger(__name__)
 
 
-class AgentResult:
-    """
-    Represent the execution result of an :class:`Agent`
-    """
-
-    _messages: List[ScoredAgentMessage]
-
-    def __init__(self, messages: Optional[List[ScoredAgentMessage]] = None):
-        """
-        Initialize a new instance.
-
-        Parameters:
-            messages(Optional[List[ScoredAgentMessage]]): an optional list of messages
-        """
-        self._messages = messages if messages is not None else []
-
-    @property
-    def messages(self) -> Sequence[ScoredAgentMessage]:
-        """
-        An unordered list of messages, with their scores.
-
-        Returns:
-            Sequence[ScoredAgentMessage]:
-        """
-        return self._messages
-
-    @property
-    def best_message(self) -> AgentMessage:
-        """
-        The message with the highest score. If multiple messages have the highest score, the first one is returned.
-
-        Returns:
-            AgentMessage:
-
-        Raises:
-            ValueError: there is no messages
-        """
-        return max(self._messages, key=lambda item: item.score).message
-
-    @property
-    def try_best_message(self) -> Option[AgentMessage]:
-        """
-        The message with the highest score, if any. See :meth:`best_message` for more details
-
-        Returns:
-            Option[AgentMessage]: the message with the highest score, wrapped into :meth:`.Option.some`, if some,
-                :meth:`.Option.none` otherwise
-        """
-        if len(self._messages) == 0:
-            return Option.none()
-        return Option.some(self.best_message)
-
-
 class Agent:
     """
     Represents an agent that executes a set of chains to interact with the environment.
 
     Attributes:
         controller (ControllerBase): The controller responsible for generating execution plans.
         chains (List[Chain]): The list of chains that the agent executes.
@@ -89,15 +37,15 @@
             chains (List[Chain]): The list of chains that the agent executes.
             evaluator (EvaluatorBase): The evaluator responsible for evaluating the agent's performance.
         """
         self.controller = controller
         self.chains = chains
         self.evaluator = evaluator
 
-    def execute(self, context: AgentContext, budget: Budget) -> AgentResult:
+    def execute(self, context: AgentContext, budget: Budget = Budget.default()) -> AgentResult:
         """
         Executes the agent's chains based on the provided context and budget.
 
         Args:
             context (AgentContext): The context for executing the chains.
             budget (Budget): The budget for agent execution.
 
@@ -133,7 +81,33 @@
                 if len(result) > 0:
                     return AgentResult(messages=result)
 
             return AgentResult()
         finally:
             logger.info('message="agent execution ended"')
             executor.shutdown(wait=False, cancel_futures=True)
+
+    @staticmethod
+    def from_skill(skill: SkillBase) -> "Agent":
+        """
+        Helper function to create a new agent with a  :class:`.BasicController`, a
+            :class:`.BasicEvaluator` and a single :class:`.SkillBase` wrapped into a `class:.Chain`
+
+        Parameters:
+             skill(SkillBase): a skill
+        Returns:
+            Agent: a new instance
+        """
+        chain = Chain(name="BasicChain", description="basic chain", runners=[skill])
+        return Agent(controller=BasicController(), chains=[chain], evaluator=BasicEvaluator())
+
+    def execute_from_user_message(self, message: str) -> AgentResult:
+        """
+        Helper function that executes an agent with a simple user message.
+
+        Parameters:
+            message(str): the user message
+        Returns:
+             AgentResult:
+        """
+        context = AgentContext(ChatHistory.from_user_message(message))
+        return self.execute(context)
```

### Comparing `council_ai-0.0.3/council/core/agent_chain.py` & `council_ai-0.0.4/council/agents/agent_chain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional, Any
 
-from council.core import Chain, Agent, AgentContext, ChainContext, Budget
+from .agent import Agent
+from council.core import Chain, AgentContext, ChainContext, Budget
 from council.core.execution_context import SkillSuccessMessage
 from council.core.runners import RunnerExecutor
 
 
 class AgentChain(Chain):
     def __init__(self, name: str, description: str, agent: Agent):
         super().__init__(name, description, [])
```

### Comparing `council_ai-0.0.3/council/core/budget.py` & `council_ai-0.0.4/council/core/budget.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,14 +41,24 @@
             True is the budget is expired. Otherwise False
         """
         return self.deadline < time.monotonic()
 
     def __repr__(self):
         return f"Budget({self.duration})"
 
+    @staticmethod
+    def default() -> "Budget":
+        """
+        Helper function that create a new Budget with a default value.
+
+        Returns:
+            Budget
+        """
+        return Budget(duration=30)
+
 
 class InfiniteBudget(Budget):
     def __init__(self):
         super().__init__(10000)
 
     def remaining(self) -> Budget:
         return Budget(10000)
```

### Comparing `council_ai-0.0.3/council/core/chain.py` & `council_ai-0.0.4/council/core/chain.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/core/controller_base.py` & `council_ai-0.0.4/council/controllers/controller_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/core/evaluator_base.py` & `council_ai-0.0.4/council/evaluators/evaluator_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/core/execution_context.py` & `council_ai-0.0.4/council/core/execution_context.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/core/result.py` & `council_ai-0.0.4/council/core/result.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/core/runners.py` & `council_ai-0.0.4/council/core/runners.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/core/scorer_base.py` & `council_ai-0.0.4/council/core/scorer_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/core/skill_base.py` & `council_ai-0.0.4/council/core/skill_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/evaluator/basic_evaluator.py` & `council_ai-0.0.4/council/evaluators/basic_evaluator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 from council.core import AgentContext, Budget
-from council.core.evaluator_base import EvaluatorBase
+from council.evaluators.evaluator_base import EvaluatorBase
 from council.core.execution_context import (
     ScoredAgentMessage,
     SkillSuccessMessage,
     AgentMessage,
 )
```

### Comparing `council_ai-0.0.3/council/evaluator/llm_evaluator.py` & `council_ai-0.0.4/council/evaluators/llm_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 LLMEvaluator implementation.
 
 This evaluator uses the given `LLM` to evaluate the chain's responses.
 """
 import logging
 from typing import List
 
-from council.core import EvaluatorBase, AgentContext, Budget
+from council.core import AgentContext, Budget
 from council.core.execution_context import ScoredAgentMessage, AgentMessage, SkillMessage, UserMessage, Option
+from council.evaluators import EvaluatorBase
 from council.llm import LLMBase, LLMMessage
 
 
 class LLMEvaluator(EvaluatorBase):
     """Evaluator using an `LLM` to evaluate chain responses."""
 
     def __init__(self, llm: LLMBase):
```

### Comparing `council_ai-0.0.3/council/llm/azure_configuration.py` & `council_ai-0.0.4/council/llm/azure_configuration.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/llm/azure_llm.py` & `council_ai-0.0.4/council/llm/azure_llm.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/llm/llm_base.py` & `council_ai-0.0.4/council/llm/llm_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/llm/llm_message.py` & `council_ai-0.0.4/council/llm/llm_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,18 +71,20 @@
             content (str): the message content
         """
         return LLMMessage(role=LLMMessageRole.Assistant, content=content)
 
     def dict(self) -> dict[str, str]:
         return {"role": self._role, "content": self._content}
 
+    @property
     def content(self) -> str:
         """Retrieve the content of the `LLMMessage`"""
         return self._content
 
+    @property
     def role(self) -> LLMMessageRole:
         """Retrieve the role of the `LLMMessage`"""
         return self._role
 
     def is_of_role(self, role: LLMMessageRole) -> bool:
         """Check the role of the `LLMMessage`"""
         return self._role == role
```

### Comparing `council_ai-0.0.3/council/llm/openai_configuration.py` & `council_ai-0.0.4/council/llm/openai_configuration.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/llm/openai_llm.py` & `council_ai-0.0.4/council/llm/openai_llm.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/mocks/__init__.py` & `council_ai-0.0.4/council/mocks/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,64 @@
 import time
 import random
-from typing import List, Any, Callable, Optional
+from typing import List, Any, Callable, Optional, Protocol
 
-from council.core import Agent, AgentContext, Budget, ScorerBase, AgentResult, SkillBase
-from council.core.execution_context import ScoredAgentMessage, AgentMessage, SkillContext, SkillMessage
+from council.agents import Agent, AgentResult
+from council.core import AgentContext, Budget, ScorerBase, SkillBase
+from council.core.execution_context import (
+    ScoredAgentMessage,
+    AgentMessage,
+    SkillContext,
+    SkillMessage,
+    SkillSuccessMessage,
+)
 from council.llm import LLMBase, LLMMessage
 
 
+class LLMMessagesToStr(Protocol):
+    def __call__(self, messages: List[LLMMessage]) -> str:
+        ...
+
+
+def llm_message_content_to_str(messages: List[LLMMessage]) -> str:
+    return "\n".join([msg.content for msg in messages])
+
+
 class MockSkill(SkillBase):
     def __init__(self, name: str = "mock", action: Optional[Callable[[SkillContext, Budget], SkillMessage]] = None):
         super().__init__(name)
         self._action = action if action is not None else self.empty_message
 
     def execute(self, context: SkillContext, budget: Budget) -> SkillMessage:
         return self._action(context, budget)
 
     def empty_message(self, context: SkillContext, budget: Budget):
         return self.build_success_message("")
 
+    def set_action_custom_message(self, message: str) -> None:
+        self._action = lambda context, budget: self.build_success_message(message)
+
 
 class MockLLM(LLMBase):
-    def __init__(self, response: List[str]):
-        self.response = "\n".join(response)
+    def __init__(self, action: Optional[LLMMessagesToStr] = None):
+        self._action = action
 
     def _post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> str:
-        return self.response
+        if self._action is not None:
+            return self._action(messages)
+        return f"{self.__class__.__name__}"
+
+    @staticmethod
+    def from_responses(responses: List[str]) -> "MockLLM":
+        value = "\n".join([r for r in responses])
+        return MockLLM(action=(lambda x: value))
+
+    @staticmethod
+    def from_response(response: str) -> "MockLLM":
+        return MockLLM(action=(lambda x: response))
 
 
 class MockErrorSimilarityScorer(ScorerBase):
     def __init__(self, exception: Exception = Exception()):
         self.exception = exception
 
     def _score(self, message: AgentMessage) -> float:
@@ -47,19 +77,19 @@
     ):
         self.message = message
         self.data = data
         self.score = score
         self.sleep = sleep
         self.sleep_interval = sleep_interval
 
-    def execute(self, context: AgentContext, budget: Budget) -> AgentResult:
+    def execute(self, context: AgentContext, budget: Budget = Budget.default()) -> AgentResult:
         time.sleep(random.uniform(self.sleep, self.sleep + self.sleep_interval))
         return AgentResult([ScoredAgentMessage(AgentMessage(self.message, self.data), score=self.score)])
 
 
 class MockErrorAgent(Agent):
     # noinspection PyMissingConstructor
     def __init__(self, exception: Exception = Exception()):
         self.exception = exception
 
-    def execute(self, context: AgentContext, budget: Budget) -> AgentResult:
+    def execute(self, context: AgentContext, budget: Budget = Budget.default()) -> AgentResult:
         raise self.exception
```

### Comparing `council_ai-0.0.3/council/prompt/prompt_builder.py` & `council_ai-0.0.4/council/prompt/prompt_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,63 @@
+import logging
 from typing import Any, List, Optional
 
 from jinja2 import Template
 
 from council.core import ChainContext, ChatMessageKind
-from council.llm import LLMMessage
+
+logger = logging.getLogger(__name__)
 
 
 class PromptBuilder:
+    """
+    A class for building prompts using a Jinja2 template and optional instructions.
+
+    Args:
+        t (str): The Jinja2 template string for the prompt.
+        instructions (Optional[List[str]]): Optional instructions to be appended to the prompt.
+
+    Attributes:
+        _template (Template): The Jinja2 template object.
+        _instructions (str): The instructions to be appended to the prompt.
+
+    Methods:
+        apply(context: ChainContext) -> str:
+            Builds and returns the prompt by rendering the template and appending instructions.
+
+    """
+
     def __init__(self, t: str, instructions: Optional[List[str]] = None):
+        """
+        Initializes a PromptBuilder instance.
+
+        Args:
+            t (str): The Jinja2 template string for the prompt.
+            instructions (Optional[List[str]]): Optional instructions to be appended to the prompt.
+        """
+
         self._template = Template(t)
         if instructions is not None and len(instructions) > 0:
             self._instructions = "\n# Instructions: "
             self._instructions += "\n".join(instructions)
         else:
             self._instructions = ""
 
     def apply(self, context: ChainContext) -> str:
+        """
+        Builds and returns the prompt by rendering the template and appending instructions.
+
+        Args:
+            context (ChainContext): The context object containing the necessary data for rendering the template.
+
+        Returns:
+            str: The generated prompt string.
+
+        """
+
         template_context = {
             "chat_history": self.__build_chat_history(context),
             "chain_history": self.__build_chain_history(context),
         }
 
         prompt = self._template.render(template_context)
         prompt += self._instructions
@@ -57,16 +95,7 @@
             }
 
         last_message = context.current.last_message()
         return {
             "messages": [msg.message for msg in context.current.messages],
             "last_message": last_message.map_or(lambda m: m.message, ""),
         }
-
-
-class PromptToMessages:
-    def __init__(self, prompt_builder: PromptBuilder):
-        self.p = prompt_builder
-
-    def get_messages_from_prompt(self, context: ChainContext) -> List[LLMMessage]:
-        msg = self.p.apply(context)
-        return [LLMMessage.system_message(msg)]
```

### Comparing `council_ai-0.0.3/council/scorer/llm_similarity_scorer.py` & `council_ai-0.0.4/council/scorer/llm_similarity_scorer.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/skill/llm_skill.py` & `council_ai-0.0.4/council/agents/agent_result.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,58 @@
-from typing import List, Protocol
+from collections.abc import Sequence
+from typing import List, Optional
 
-from council.core import SkillBase, Budget
-from council.core.execution_context import SkillMessage, SkillSuccessMessage, SkillContext
-from council.llm import LLMBase, LLMMessage
+from council.core.execution_context import ScoredAgentMessage, AgentMessage
+from council.utils import Option
 
 
-class ReturnMessages(Protocol):
-    def __call__(self, context: SkillContext) -> List[LLMMessage]:
-        ...
+class AgentResult:
+    """
+    Represent the execution result of an :class:`Agent`
+    """
 
+    _messages: List[ScoredAgentMessage]
 
-def get_chat_history(context: SkillContext) -> List[LLMMessage]:
-    # Convert chat's history and give it to the inner llm
-    return LLMMessage.from_chat_messages(context.chatHistory.messages)
-
-
-def get_last_messages(context: SkillContext) -> List[LLMMessage]:
-    if context.iteration.is_some():
-        it_ctxt = context.iteration.unwrap()
-        msg = LLMMessage.user_message(it_ctxt.value)
-        return [msg]
-    last_message = context.current.last_message()
-    if last_message.is_none():
-        return get_chat_history(context)
-    msg = LLMMessage.user_message(last_message.unwrap().message)
-    return [msg]
-
-
-class LLMSkill(SkillBase):
-    """Skill to interact with an `LLM`."""
-
-    def __init__(
-        self,
-        llm: LLMBase,
-        name: str = "LLMSkill",
-        system_prompt: str = "",
-        context_messages: ReturnMessages = get_last_messages,
-    ):
+    def __init__(self, messages: Optional[List[ScoredAgentMessage]] = None):
         """
-        Initialize a new instance of LLMSkill.
+        Initialize a new instance.
 
         Parameters:
-            llm (LLMBase): The instance of the LLM (Language Model) to interact with.
-            system_prompt (str): Optional system prompt to provide to the language model.
-            context_messages (Callable[[ChainContext], List[LLMMessage]]): Optional callable to retrieve
-                context messages.
+            messages(Optional[List[ScoredAgentMessage]]): an optional list of messages
+        """
+        self._messages = messages if messages is not None else []
+
+    @property
+    def messages(self) -> Sequence[ScoredAgentMessage]:
+        """
+        An unordered list of messages, with their scores.
 
         Returns:
-            None
+            Sequence[ScoredAgentMessage]:
         """
+        return self._messages
 
-        super().__init__(name=name)
-        self._llm = llm
-        self._context_messages = context_messages
-        self._system_prompt = LLMMessage.system_message(system_prompt)
+    @property
+    def best_message(self) -> AgentMessage:
+        """
+        The message with the highest score. If multiple messages have the highest score, the first one is returned.
 
-    def execute(self, context: SkillContext, _budget: Budget) -> SkillMessage:
-        """Execute `LLMSkill`."""
+        Returns:
+            AgentMessage:
 
-        history_messages = self._context_messages(context)
+        Raises:
+            ValueError: there is no messages
+        """
+        return max(self._messages, key=lambda item: item.score).message
 
-        # Prepend the system prompt
-        messages = [self._system_prompt, *history_messages]
-        llm_response = self._llm.post_chat_request(messages=messages)
+    @property
+    def try_best_message(self) -> Option[AgentMessage]:
+        """
+        The message with the highest score, if any. See :meth:`best_message` for more details
 
-        return SkillSuccessMessage(skill_name=self.name, message=llm_response, data=None)
+        Returns:
+            Option[AgentMessage]: the message with the highest score, wrapped into :meth:`.Option.some`, if some,
+                :meth:`.Option.none` otherwise
+        """
+        if len(self._messages) == 0:
+            return Option.none()
+        return Option.some(self.best_message)
```

### Comparing `council_ai-0.0.3/council/skill/google/google_news_skill.py` & `council_ai-0.0.4/council/skill/google/google_news_skill.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/skill/google/google_search_skill.py` & `council_ai-0.0.4/council/skill/google/google_search_skill.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/skill/google/google_context/context_provider.py` & `council_ai-0.0.4/council/skill/google/google_context/context_provider.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/skill/google/google_context/google_news.py` & `council_ai-0.0.4/council/skill/google/google_context/google_news.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/skill/google/google_context/google_search.py` & `council_ai-0.0.4/council/skill/google/google_context/google_search.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/skill/google/google_context/schemas.py` & `council_ai-0.0.4/council/skill/google/google_context/schemas.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/utils/env.py` & `council_ai-0.0.4/council/utils/env.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/council/utils/option.py` & `council_ai-0.0.4/council/utils/option.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/docs/Makefile` & `council_ai-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/docs/make.bat` & `council_ai-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/docs/source/conf.py` & `council_ai-0.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/docs/source/index.rst` & `council_ai-0.0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/docs/source/_static/00_chainml_logo.png` & `council_ai-0.0.4/docs/source/_static/00_chainml_logo.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/docs/source/_static/02_chainml_logo_black.png` & `council_ai-0.0.4/docs/source/_static/02_chainml_logo_black.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/docs/source/examples/langchain_llm_integration.ipynb` & `council_ai-0.0.4/docs/source/examples/langchain_llm_integration.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/docs/source/examples/my_first_agent.ipynb` & `council_ai-0.0.4/docs/source/examples/my_first_agent.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991666666666666%*

 * *Differences: {"'cells'": "{12: {'source': {insert: [(0, 'from council.controllers import LLMController\\n')], "*

 * *            "delete: [0]}}, 14: {'source': {insert: [(0, 'from council.evaluators import "*

 * *            "LLMEvaluator\\n')], delete: [0]}}, 16: {'source': {insert: [(0, 'from council.agents "*

 * *            "import Agent\\n'), (1, 'from council.core import Budget\\n')], delete: [0]}}}"}*

```diff
@@ -155,15 +155,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "from council.controller import LLMController\n",
+                "from council.controllers import LLMController\n",
                 "\n",
                 "controller = LLMController(llm=azure_llm, response_threshold=5)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -177,15 +177,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "from council.evaluator import LLMEvaluator\n",
+                "from council.evaluators import LLMEvaluator\n",
                 "\n",
                 "evaluator = LLMEvaluator(llm=azure_llm)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -199,15 +199,16 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "from council.core import Agent, Budget\n",
+                "from council.agents import Agent\n",
+                "from council.core import Budget\n",
                 "\n",
                 "agent = Agent(controller=controller, chains=[finance_chain, game_chain, fake_chain], evaluator=evaluator)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
```

### Comparing `council_ai-0.0.3/docs/source/reference/runners.rst` & `council_ai-0.0.4/docs/source/reference/runners.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/docs/source/reference/runners/parallel_for.rst` & `council_ai-0.0.4/docs/source/reference/runners/parallel_for.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/stubs/GoogleNews.pyi` & `council_ai-0.0.4/stubs/GoogleNews.pyi`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/LICENSE` & `council_ai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.3/README.md` & `council_ai-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,33 +98,33 @@
 em_chain = Chain(name="Emoji Agent", description="Responds to every prompt with an emoji that best fits the prompt",
                  runners=[em_skill])
 ```
 
 Create a Controller to route prompts to chains. Here we use the straight-forward LLMController in which an LLM instance is tasked to make a routing decision.
 
 ```python
-from council.controller import LLMController
+from council.controllers import LLMController
 
 controller = LLMController(llm=openai_llm, response_threshold=5)
 ```
 
 Create an Evaluator. Here, we use an LLMEvaluator in which an LLM is tasked to evaluate each response received.
 
-
 ```python
-from council.evaluator import LLMEvaluator
+from council.evaluators import LLMEvaluator
 
 evaluator = LLMEvaluator(llm=openai_llm)
 ```
 
 Finalize setup of the Hello World first Agent by combining all components created.
 
 
 ```python
-from council.core import Agent, Budget
+from council.agents import Agent
+from council.core import Budget
 
 agent = Agent(controller=controller, chains=[hw_chain, em_chain], evaluator=evaluator)
 ```
 
 Now, we are ready to invoke the agent. The ChatHistory object is used to track message history between User and Agents.
 
 ```python
```

### Comparing `council_ai-0.0.3/pyproject.toml` & `council_ai-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "council-ai"
-version = "0.0.3"
+version = "0.0.4"
 description = "Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications"
 readme = "README.md"
 requires-python = ">=3.9"
+authors = []
+license = "Apache-2.0"
 
 dynamic = ["dependencies"]
 
+[project.urls]
+Source = "https://github.com/chain-ml/council"
+
 [tool.hatch.build]
 exclude = [
     ".github",
     "*-requirements.txt",
     "tests",
     "venv",
 ]
```

### Comparing `council_ai-0.0.3/PKG-INFO` & `council_ai-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: council-ai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications
+Project-URL: Source, https://github.com/chain-ml/council
+License-Expression: Apache-2.0
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: google-api-python-client-stubs
 Requires-Dist: google-api-python-client==2.93.0
 Requires-Dist: googlenews==1.6.8
 Requires-Dist: httpx==0.24.1
 Requires-Dist: jinja2~=3.1.2
@@ -115,33 +117,33 @@
 em_chain = Chain(name="Emoji Agent", description="Responds to every prompt with an emoji that best fits the prompt",
                  runners=[em_skill])
 ```
 
 Create a Controller to route prompts to chains. Here we use the straight-forward LLMController in which an LLM instance is tasked to make a routing decision.
 
 ```python
-from council.controller import LLMController
+from council.controllers import LLMController
 
 controller = LLMController(llm=openai_llm, response_threshold=5)
 ```
 
 Create an Evaluator. Here, we use an LLMEvaluator in which an LLM is tasked to evaluate each response received.
 
-
 ```python
-from council.evaluator import LLMEvaluator
+from council.evaluators import LLMEvaluator
 
 evaluator = LLMEvaluator(llm=openai_llm)
 ```
 
 Finalize setup of the Hello World first Agent by combining all components created.
 
 
 ```python
-from council.core import Agent, Budget
+from council.agents import Agent
+from council.core import Budget
 
 agent = Agent(controller=controller, chains=[hw_chain, em_chain], evaluator=evaluator)
 ```
 
 Now, we are ready to invoke the agent. The ChatHistory object is used to track message history between User and Agents.
 
 ```python
```

