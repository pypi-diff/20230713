# Comparing `tmp/llmreflect-0.0.7.tar.gz` & `tmp/llmreflect-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreflect-0.0.7.tar", max compression
+gzip compressed data, was "llmreflect-0.0.8.tar", max compression
```

## Comparing `llmreflect-0.0.7.tar` & `llmreflect-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4061 2023-07-11 18:08:29.939687 llmreflect-0.0.7/README.md
--rw-r--r--   0        0        0     3771 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/BasicAgent.py
--rw-r--r--   0        0        0     2570 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/EvaluationAgent.py
--rw-r--r--   0        0        0     3092 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/ModerateAgent.py
--rw-r--r--   0        0        0     9630 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/PostgresqlAgent.py
--rw-r--r--   0        0        0     2278 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/QuestionAgent.py
--rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Agents/__init__.py
--rw-r--r--   0        0        0     2522 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Chains/BasicChain.py
--rw-r--r--   0        0        0    21670 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Chains/DatabaseChain.py
--rw-r--r--   0        0        0     1786 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Chains/ModerateChain.py
--rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Chains/__init__.py
--rw-r--r--   0        0        0     8381 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/BasicPrompt.py
--rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/__init__.py
--rw-r--r--   0        0        0     2807 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/promptbase/gradingpostgresql.json
--rw-r--r--   0        0        0     2366 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/promptbase/moderatepostgresql.json
--rw-r--r--   0        0        0     4951 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/promptbase/postgresql.json
--rw-r--r--   0        0        0     1119 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/promptbase/postgresqlfix.json
--rw-r--r--   0        0        0     2084 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Prompt/promptbase/questionpostgresql.json
--rw-r--r--   0        0        0     1941 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Retriever/BasicRetriever.py
--rw-r--r--   0        0        0     4219 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Retriever/DatabaseRetriever.py
--rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Retriever/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Tests/__init__.py
--rw-r--r--   0        0        0     7612 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Tests/test_chains.py
--rw-r--r--   0        0        0      442 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Utils/__init__.py
--rw-r--r--   0        0        0      690 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Utils/database.py
--rw-r--r--   0        0        0     5685 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/Utils/log.py
--rw-r--r--   0        0        0        0 2023-07-11 18:08:29.939687 llmreflect-0.0.7/llmreflect/__init__.py
--rw-r--r--   0        0        0      478 2023-07-11 18:08:29.939687 llmreflect-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 llmreflect-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     4061 2023-07-12 21:23:45.064165 llmreflect-0.0.8/README.md
+-rw-r--r--   0        0        0     3957 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Agents/BasicAgent.py
+-rw-r--r--   0        0        0     2570 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Agents/EvaluationAgent.py
+-rw-r--r--   0        0        0     3092 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Agents/ModerateAgent.py
+-rw-r--r--   0        0        0     9630 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Agents/PostgresqlAgent.py
+-rw-r--r--   0        0        0     2278 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Agents/QuestionAgent.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Agents/__init__.py
+-rw-r--r--   0        0        0     2679 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Chains/BasicChain.py
+-rw-r--r--   0        0        0    21670 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Chains/DatabaseChain.py
+-rw-r--r--   0        0        0     1786 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Chains/ModerateChain.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Chains/__init__.py
+-rw-r--r--   0        0        0     8381 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Prompt/BasicPrompt.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Prompt/__init__.py
+-rw-r--r--   0        0        0     2807 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Prompt/promptbase/gradingpostgresql.json
+-rw-r--r--   0        0        0     2366 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Prompt/promptbase/moderatepostgresql.json
+-rw-r--r--   0        0        0     4951 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Prompt/promptbase/postgresql.json
+-rw-r--r--   0        0        0     1119 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Prompt/promptbase/postgresqlfix.json
+-rw-r--r--   0        0        0     2084 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Prompt/promptbase/questionpostgresql.json
+-rw-r--r--   0        0        0     1941 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Retriever/BasicRetriever.py
+-rw-r--r--   0        0        0     4219 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Retriever/DatabaseRetriever.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Retriever/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Tests/__init__.py
+-rw-r--r--   0        0        0     8035 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Tests/test_chains.py
+-rw-r--r--   0        0        0      442 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Utils/__init__.py
+-rw-r--r--   0        0        0      690 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Utils/database.py
+-rw-r--r--   0        0        0     9708 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/Utils/log.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:23:45.064165 llmreflect-0.0.8/llmreflect/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-12 21:23:45.064165 llmreflect-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 llmreflect-0.0.8/PKG-INFO
```

### Comparing `llmreflect-0.0.7/README.md` & `llmreflect-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Agents/BasicAgent.py` & `llmreflect-0.0.8/llmreflect/Agents/BasicAgent.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from typing import Any
 from langchain.chains import LLMChain
 from llmreflect.Prompt.BasicPrompt import BasicPrompt
 from langchain.base_language import BaseLanguageModel
 from abc import ABC, abstractclassmethod
 from llmreflect.Retriever.BasicRetriever import BasicRetriever
 from dataclasses import dataclass
 from langchain.chat_models import ChatOpenAI
 from llmreflect.Utils.log import get_logger
+from llmreflect.Utils.log import openai_trace_var
 
 
 @dataclass
 class LLM_BACKBONE_MODEL:
     gpt_4 = "gpt-4"
     gpt_4_0314 = "gpt-4-0314"
     gpt_4_0613 = "gpt-4-0613"
@@ -60,14 +62,17 @@
         """_summary_
         showing inputs for the prompt template being used
         Returns:
             _type_: _description_
         """
         return self.prompt.input_variables
 
+    def predict(self, **kwargs: Any) -> str:
+        return super().predict([openai_trace_var.get()], **kwargs)
+
 
 class OpenAIAgent(Agent):
     '''
     Abstract class for agent, in this design each agent should have
     a retriever, retriever is for retrieving the final result based
     on the gross output by LLM.
     For example, a database retriever does the following job:
```

### Comparing `llmreflect-0.0.7/llmreflect/Agents/EvaluationAgent.py` & `llmreflect-0.0.8/llmreflect/Agents/EvaluationAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Agents/ModerateAgent.py` & `llmreflect-0.0.8/llmreflect/Agents/ModerateAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Agents/PostgresqlAgent.py` & `llmreflect-0.0.8/llmreflect/Agents/PostgresqlAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Agents/QuestionAgent.py` & `llmreflect-0.0.8/llmreflect/Agents/QuestionAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Chains/BasicChain.py` & `llmreflect-0.0.8/llmreflect/Chains/BasicChain.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from abc import ABC, abstractclassmethod
 from llmreflect.Retriever.BasicRetriever import BasicRetriever
 from llmreflect.Agents.BasicAgent import Agent
 from llmreflect.Prompt.BasicPrompt import BasicPrompt
 from typing import Any, List
 from langchain.llms.openai import OpenAI
-from langchain.callbacks import get_openai_callback
 from llmreflect.Utils.log import get_logger, openai_cb_2_str
+from llmreflect.Utils.log import get_openai_tracer
 
 
 class BasicChain(ABC):
     '''
     Abstract class for Chain class.
     A chain class should be the atomic unit for completing a job.
     A chain contains at least two components:
     1. an agent 2. a retriever
     A chain object must have the function to perform a job.
     '''
     def __init__(self, agent: Agent, retriever: BasicRetriever):
-        self.agent = agent
-        self.retriever = retriever
+        object.__setattr__(self, 'agent', agent)
+        object.__setattr__(self, 'retriever', retriever)
         self.agent.equip_retriever(self.retriever)
-        self.logger = get_logger(self.__class__.__name__)
+        object.__setattr__(self, 'logger', get_logger(self.__class__.__name__))
 
     @abstractclassmethod
     def from_config(cls,
                     open_ai_key: str,
                     prompt_name: str = 'questionpostgresql',
                     temperature: float = 0.0):
         llm = OpenAI(temperature=temperature, openai_api_key=open_ai_key)
@@ -36,37 +36,37 @@
 
     @abstractclassmethod
     def perform(self, **kwargs: Any):
         result = self.agent.predict(kwargs)
         return result
 
     def perform_cost_monitor(self, **kwargs: Any):
-        with get_openai_callback() as cb:
+        with get_openai_tracer(id=self.__class__.__name__) as cb:
             result = self.perform(**kwargs)
         self.logger.cost(openai_cb_2_str(cb))
         return result, cb
 
 
 class BasicCombinedChain(ABC):
     '''
     Abstract class for combined Chain class.
     A combined chain is a chain with multiple chains
     A chain class should be the atomic unit for completing a job.
     A chain object must have the function to perform a job.
     '''
     def __init__(self, chains: List[BasicChain]):
-        self.chains = chains
-        self.logger = get_logger(self.__class__.__name__)
+        object.__setattr__(self, "chains", chains)
+        object.__setattr__(self, "logger", get_logger(self.__class__.__name__))
 
     @abstractclassmethod
     def from_config(cls, **kwargs: Any):
         return
 
     @abstractclassmethod
     def perform(self, **kwargs: Any):
         return
 
     def perform_cost_monitor(self, **kwargs: Any):
-        with get_openai_callback() as cb:
+        with get_openai_tracer(id=self.__class__.__name__) as cb:
             result = self.perform(**kwargs)
         self.logger.cost(openai_cb_2_str(cb))
         return result, cb
```

### Comparing `llmreflect-0.0.7/llmreflect/Chains/DatabaseChain.py` & `llmreflect-0.0.8/llmreflect/Chains/DatabaseChain.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Chains/ModerateChain.py` & `llmreflect-0.0.8/llmreflect/Chains/ModerateChain.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Prompt/BasicPrompt.py` & `llmreflect-0.0.8/llmreflect/Prompt/BasicPrompt.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Prompt/promptbase/gradingpostgresql.json` & `llmreflect-0.0.8/llmreflect/Prompt/promptbase/gradingpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Prompt/promptbase/moderatepostgresql.json` & `llmreflect-0.0.8/llmreflect/Prompt/promptbase/moderatepostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Prompt/promptbase/postgresql.json` & `llmreflect-0.0.8/llmreflect/Prompt/promptbase/postgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Prompt/promptbase/postgresqlfix.json` & `llmreflect-0.0.8/llmreflect/Prompt/promptbase/postgresqlfix.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Prompt/promptbase/questionpostgresql.json` & `llmreflect-0.0.8/llmreflect/Prompt/promptbase/questionpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Retriever/BasicRetriever.py` & `llmreflect-0.0.8/llmreflect/Retriever/BasicRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Retriever/DatabaseRetriever.py` & `llmreflect-0.0.8/llmreflect/Retriever/DatabaseRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/llmreflect/Tests/test_chains.py` & `llmreflect-0.0.8/llmreflect/Tests/test_chains.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Have not figured out a way to test current chains without database.
 Future work...
 """
 import os
 import pytest
-from llmreflect.Utils.log import get_logger
+from llmreflect.Utils.log import get_logger, traces_2_str
 
 LOGGER = get_logger("test")
 
 
 def in_workflow():
     return os.getenv("GITHUB_ACTIONS")\
         or os.getenv("TRAVIS") \
@@ -36,23 +36,24 @@
             'tb_appointment_patients',
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ],
         open_ai_key=config('OPENAI_API_KEY')
     )
 
-    result, _ = ch.perform_cost_monitor(
+    result, traces = ch.perform_cost_monitor(
         user_input="give me a list of patients",
         explain_moderate=True)
-
+    LOGGER.debug(traces_2_str(traces))
     assert result['moderate_decision']
 
-    result, _ = ch.perform_cost_monitor(
+    result, traces = ch.perform_cost_monitor(
         user_input="Cats are the true rulers",
         explain_moderate=True)
+    LOGGER.debug(traces_2_str(traces))
     assert not result['moderate_decision']
     assert len(result['moderate_explanation']) > 0
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
@@ -65,22 +66,24 @@
             'tb_patient',
             'tb_patients_allergies',
             'tb_appointment_patients',
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ]
     )
-    result, _ = ch.perform_cost_monitor(
+    result, traces = ch.perform_cost_monitor(
         user_input="give me a list of patients",
         with_explanation=True)
     assert result['decision']
+    LOGGER.debug(traces_2_str(traces))
 
-    result, _ = ch.perform_cost_monitor(
+    result, traces = ch.perform_cost_monitor(
         user_input="Cats are the true rulers",
         with_explanation=True)
+    LOGGER.debug(traces_2_str(traces))
     assert not result['decision']
     assert len(result['explanation']) > 0
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
@@ -104,15 +107,15 @@
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ],
         a_max_output_tokens=512,
         g_max_output_tokens=256,
         open_ai_key=config('OPENAI_API_KEY')
     )
-    logs, _ = ch.perform_cost_monitor(n_question=N_QUESTIONS)
+    logs, traces = ch.perform_cost_monitor(n_question=N_QUESTIONS)
     if SAVE_LOG:
         df = pd.DataFrame.from_records(logs)
         df.to_csv("self_grading.csv")
     else:
         for log in logs:
             LOGGER.info("Question: " + log["question"])
             LOGGER.info("Query: " + log["cmd"])
@@ -120,14 +123,15 @@
             LOGGER.info("Score: %.2f" % log["grading"])
             LOGGER.info("Explain: " + log["explanation"])
             assert len(log["question"]) > 0
             assert len(log["cmd"]) > 0
             assert len(log["summary"]) > 0
             assert len(log["explanation"]) > 0
             assert log["grading"] >= 0
+    LOGGER.debug(traces_2_str(traces))
 
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
 def test_self_fix_chain():
     from llmreflect.Chains.DatabaseChain import DatabaseQuestionChain,\
@@ -174,37 +178,42 @@
         prompt_name="postgresqlfix",
         max_output_tokens=max_output_tokens,
         temperature=0.1,
         sample_rows=0,
         max_rows_return=500
     )
 
-    questions, _ = q_ch.perform_cost_monitor(n_questions=5)
+    questions, traces = q_ch.perform_cost_monitor(n_questions=5)
+    LOGGER.debug(traces_2_str(traces))
+
     for q in questions:
-        cmd_summary, _ = a_ch.perform_cost_monitor(user_input=q)
+        cmd_summary, traces = a_ch.perform_cost_monitor(user_input=q)
+        LOGGER.debug(traces_2_str(traces))
         cmd = cmd_summary['cmd']
         summary = cmd_summary['summary']
         if "Error" not in summary:
             crooked_cmd = cmd.replace("tb_", "")
             crooked_summary = a_ch.retriever.retrieve_summary(
                 llm_output=crooked_cmd)
             LOGGER.info("Question: " + q)
             LOGGER.info("Crooked command: " + crooked_cmd)
             LOGGER.info("Crooked summary: " + crooked_summary)
-            result_dict, _ = self_fix_ch.perform_cost_monitor(
+            result_dict, traces = self_fix_ch.perform_cost_monitor(
                 user_input=q,
                 history=crooked_cmd,
                 his_error=crooked_summary
             )
             fixed_cmd = result_dict['cmd']
             fixed_summary = result_dict['summary']
             LOGGER.info("Fixed command: " + fixed_cmd)
             LOGGER.info("Fixed summary: " + fixed_summary)
             assert "error" not in fixed_summary.lower()
 
+            LOGGER.debug(traces_2_str(traces))
+
 
 @pytest.mark.skipif(bool(in_workflow()),
                     reason="Only test database operations \
                     in local env")
 def test_answerNfix_chain():
 
     from llmreflect.Chains.DatabaseChain import DatabaseAnswerNFixChain
@@ -221,11 +230,12 @@
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ],
         open_ai_key=config('OPENAI_API_KEY'),
         answer_chain_prompt_name="postgresql",
         fix_chain_prompt_name="postgresqlfix"
     )
-    result_dict, _ = ch.perform_cost_monitor(
+    result_dict, traces = ch.perform_cost_monitor(
         user_input="give me a list overweight patients")
     assert len(result_dict['summary']) > 0
     assert type(result_dict['error']) is list
+    LOGGER.debug(traces_2_str(traces))
```

### Comparing `llmreflect-0.0.7/llmreflect/Utils/database.py` & `llmreflect-0.0.8/llmreflect/Utils/database.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.7/PKG-INFO` & `llmreflect-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmreflect
-Version: 0.0.7
+Version: 0.0.8
 Summary: a package for llm self-reflection
 Author: alchemistwu
 Author-email: alchemistwu0521@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

