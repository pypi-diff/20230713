# Comparing `tmp/eyeball_pp-0.0.1.tar.gz` & `tmp/eyeball_pp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeball_pp-0.0.1.tar", last modified: Wed Jul 12 18:32:02 2023, max compression
+gzip compressed data, was "eyeball_pp-0.0.2.tar", last modified: Thu Jul 13 04:43:51 2023, max compression
```

## Comparing `eyeball_pp-0.0.1.tar` & `eyeball_pp-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-12 18:32:02.881831 eyeball_pp-0.0.1/
--rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.1/LICENSE
--rw-r--r--   0 revant     (501) staff       (20)     8414 2023-07-12 18:32:02.881950 eyeball_pp-0.0.1/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)     8031 2023-07-10 21:36:50.000000 eyeball_pp-0.0.1/README.md
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-12 18:32:02.880201 eyeball_pp-0.0.1/eyeball_pp/
--rw-r--r--   0 revant     (501) staff       (20)      757 2023-06-27 22:22:21.000000 eyeball_pp-0.0.1/eyeball_pp/__init__.py
--rw-r--r--   0 revant     (501) staff       (20)     1997 2023-07-10 21:36:14.000000 eyeball_pp-0.0.1/eyeball_pp/classes.py
--rw-r--r--   0 revant     (501) staff       (20)     1993 2023-06-27 21:29:21.000000 eyeball_pp-0.0.1/eyeball_pp/comparators.py
--rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.1/eyeball_pp/compare_checkpoints.py
--rw-r--r--   0 revant     (501) staff       (20)    35127 2023-07-12 18:19:03.000000 eyeball_pp-0.0.1/eyeball_pp/eval.py
--rw-r--r--   0 revant     (501) staff       (20)    23024 2023-07-12 18:25:38.000000 eyeball_pp-0.0.1/eyeball_pp/recorders.py
--rw-r--r--   0 revant     (501) staff       (20)      374 2023-06-30 00:16:29.000000 eyeball_pp-0.0.1/eyeball_pp/utils.py
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-12 18:32:02.881615 eyeball_pp-0.0.1/eyeball_pp.egg-info/
--rw-r--r--   0 revant     (501) staff       (20)     8414 2023-07-12 18:32:02.000000 eyeball_pp-0.0.1/eyeball_pp.egg-info/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)      340 2023-07-12 18:32:02.000000 eyeball_pp-0.0.1/eyeball_pp.egg-info/SOURCES.txt
--rw-r--r--   0 revant     (501) staff       (20)        1 2023-07-12 18:32:02.000000 eyeball_pp-0.0.1/eyeball_pp.egg-info/dependency_links.txt
--rw-r--r--   0 revant     (501) staff       (20)       11 2023-07-12 18:32:02.000000 eyeball_pp-0.0.1/eyeball_pp.egg-info/top_level.txt
--rw-r--r--   0 revant     (501) staff       (20)      527 2023-07-12 18:32:02.882654 eyeball_pp-0.0.1/setup.cfg
--rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.1/setup.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-13 04:43:51.671836 eyeball_pp-0.0.2/
+-rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.2/LICENSE
+-rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-13 04:43:51.671933 eyeball_pp-0.0.2/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)     8520 2023-07-12 19:49:37.000000 eyeball_pp-0.0.2/README.md
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-13 04:43:51.670347 eyeball_pp-0.0.2/eyeball_pp/
+-rw-r--r--   0 revant     (501) staff       (20)      757 2023-06-27 22:22:21.000000 eyeball_pp-0.0.2/eyeball_pp/__init__.py
+-rw-r--r--   0 revant     (501) staff       (20)     2096 2023-07-12 21:34:21.000000 eyeball_pp-0.0.2/eyeball_pp/classes.py
+-rw-r--r--   0 revant     (501) staff       (20)     2137 2023-07-12 21:50:50.000000 eyeball_pp-0.0.2/eyeball_pp/comparators.py
+-rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.2/eyeball_pp/compare_checkpoints.py
+-rw-r--r--   0 revant     (501) staff       (20)    39224 2023-07-13 04:42:50.000000 eyeball_pp-0.0.2/eyeball_pp/eval.py
+-rw-r--r--   0 revant     (501) staff       (20)    25534 2023-07-13 04:40:36.000000 eyeball_pp-0.0.2/eyeball_pp/recorders.py
+-rw-r--r--   0 revant     (501) staff       (20)      374 2023-06-30 00:16:29.000000 eyeball_pp-0.0.2/eyeball_pp/utils.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-13 04:43:51.671639 eyeball_pp-0.0.2/eyeball_pp.egg-info/
+-rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-13 04:43:51.000000 eyeball_pp-0.0.2/eyeball_pp.egg-info/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)      340 2023-07-13 04:43:51.000000 eyeball_pp-0.0.2/eyeball_pp.egg-info/SOURCES.txt
+-rw-r--r--   0 revant     (501) staff       (20)        1 2023-07-13 04:43:51.000000 eyeball_pp-0.0.2/eyeball_pp.egg-info/dependency_links.txt
+-rw-r--r--   0 revant     (501) staff       (20)       11 2023-07-13 04:43:51.000000 eyeball_pp-0.0.2/eyeball_pp.egg-info/top_level.txt
+-rw-r--r--   0 revant     (501) staff       (20)      527 2023-07-13 04:43:51.672428 eyeball_pp-0.0.2/setup.cfg
+-rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.2/setup.py
```

### Comparing `eyeball_pp-0.0.1/LICENSE` & `eyeball_pp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.1/PKG-INFO` & `eyeball_pp-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball_pp
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -23,29 +23,30 @@
 
 # Installation
 eyeball_pp is a python library which can be installed via pip 
 
 `pip install eyeball_pp`
 
 # Concepts 
-eyeball_pp has 3 simple concepts -- record, rerun and compare.
+eyeball_pp has 3 simple concepts -- record, rerun and compare. To see a detailed example check out the examples/ folder in the repo
 
 ## Record
 eyeball_pp consists of a recorder which records the inputs and outputs of your task runs as you are running it and saves them as checkpoints. You can record this locally while developing or from a production system. You can optionally record human feedback for the task output too.
 
-You can record your task using the `record_task` decorator. This will record every run of this function call as a `Checkpoint` for future comparison.
+You can record your task using the `record_task` decorator. This will record every run of this function call as a `Checkpoint` for future comparison. The args_to_record specify which inputs to record and the function return value is saved as the output.
 ```python
 import eyeball_pp
 
 @eyeball_pp.record_task(args_to_record=['input_a', 'input_b'])
 def your_task_function(input_a, input_b):
   # Your task can run arbitrary code
   ...
   return task_output
 ```
+If you want to record additional inputs within your function call you can just call `eyeball_pp.record_input('variable_name', value)` inside your function.
 
 If your sytem is more complicated, you can also use the `record_input` and `record_output` functions with the start_recording_session context manager
 ```python
 import eyeball_pp
 
 # your task code 
 ...
@@ -60,14 +61,16 @@
 
 ```python
 eyeball_pp.record_input(task_name="your_task", checkpoint_id="some_custom_unique_id", variable_name="input_a", value=input_a_value)
 ..
 eyeball_pp.record_output(task_name="your_task", checkpoint_id="some_custom_unique_id", variable_name='output', output=output)
 ```
 
+Data by default gets recorded as yaml files in your repo so you can always inspect it, change it or delete it.
+
 ## Rerun
 You can then re-run these pre-recorded examples as you make changes. This will only re-run each unique set of input variables. eg. if you recorded a run of `your_task_function(1, 2)` 5 times and `your_task_function(3, 4)` 2 times, the re-run would only run 2 examples -- (1, 2) and (3, 4). Each of these re-runs is saved as a new checkpoint for comparison later. 
 ```python
 from eyeball_pp import rerun_recorded_examples 
 
 for input_vars in rerun_recorded_examples():
   your_task_function(input_vars['input_a'], input_vars['input_b'])
@@ -77,15 +80,15 @@
 ```python
 from eyeball_pp import get_eval_param, rerun_recorded_examples 
 
 for vars in rerun_recorded_examples({'model': 'gpt-4', 'temperature': 0.7}, {'model': 'mpt-30b-chat'}):
   your_task_function(vars['input_a'], vars['input_b'])
 
 # You can access these eval params from anywhere in your code
-@eyeball_pp.record_task
+@eyeball_pp.record_task(args_to_record=['input_a', 'input_b'])
 def your_task_function(input_a, input_b):
   ...
   model = get_eval_param('model') or 'gpt-3.5-turbo'
   temperature = get_eval_param('temperature') or 0.5
 ```
 
 ## Compare
@@ -108,15 +111,15 @@
 
 Summary:
 2/2 examples got better in their most recent runs
 The param combination (model=gpt-4, temperature=0.7) works better for 2/2 examples than the default params
 The param combination (model=claude-v1, temperature=None) works equally as good as the (model=gpt-4, temperature=0.7) combination for 2/2 examples
 ```
 
-The comparison will also output a .md file in your repo with the comparison results in a tabular format.
+The comparison will also output a benchmark.md file in your repo with the comparison results in a tabular format.
 
 # Configuration 
 
 ## Serialization
 For the `record_task` decorator you need to ensure that the inputs to the function and outputs are json serialable. If the variables are custom classes you can define the `to_json` and `from_json` functions on that object. If you want to skip serializing some inputs you can specify that in the decorator as `args_to_skip` 
 eg. 
 ```python
```

### Comparing `eyeball_pp-0.0.1/README.md` & `eyeball_pp-0.0.2/eyeball_pp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: eyeball-pp
+Version: 0.0.2
+Summary: A python package for evaluating tasks which use llms
+Home-page: https://github.com/revantk/eyeball-plus-plus
+Author: Revant
+Author-email: revant.kapoor@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Eyeball++ 
 _Ridiculously simple evaluation for LLM agents_
 
 eyeball_pp is a framework to evaluate and benchmark tasks which use llms.
 
 This framework helps you answer questions like: "Which llm is the best for my specific task?" or "This prompt change looks good on the example I just tested, does it work with all the other things I've tested?"
 
@@ -11,29 +23,30 @@
 
 # Installation
 eyeball_pp is a python library which can be installed via pip 
 
 `pip install eyeball_pp`
 
 # Concepts 
-eyeball_pp has 3 simple concepts -- record, rerun and compare.
+eyeball_pp has 3 simple concepts -- record, rerun and compare. To see a detailed example check out the examples/ folder in the repo
 
 ## Record
 eyeball_pp consists of a recorder which records the inputs and outputs of your task runs as you are running it and saves them as checkpoints. You can record this locally while developing or from a production system. You can optionally record human feedback for the task output too.
 
-You can record your task using the `record_task` decorator. This will record every run of this function call as a `Checkpoint` for future comparison.
+You can record your task using the `record_task` decorator. This will record every run of this function call as a `Checkpoint` for future comparison. The args_to_record specify which inputs to record and the function return value is saved as the output.
 ```python
 import eyeball_pp
 
 @eyeball_pp.record_task(args_to_record=['input_a', 'input_b'])
 def your_task_function(input_a, input_b):
   # Your task can run arbitrary code
   ...
   return task_output
 ```
+If you want to record additional inputs within your function call you can just call `eyeball_pp.record_input('variable_name', value)` inside your function.
 
 If your sytem is more complicated, you can also use the `record_input` and `record_output` functions with the start_recording_session context manager
 ```python
 import eyeball_pp
 
 # your task code 
 ...
@@ -48,14 +61,16 @@
 
 ```python
 eyeball_pp.record_input(task_name="your_task", checkpoint_id="some_custom_unique_id", variable_name="input_a", value=input_a_value)
 ..
 eyeball_pp.record_output(task_name="your_task", checkpoint_id="some_custom_unique_id", variable_name='output', output=output)
 ```
 
+Data by default gets recorded as yaml files in your repo so you can always inspect it, change it or delete it.
+
 ## Rerun
 You can then re-run these pre-recorded examples as you make changes. This will only re-run each unique set of input variables. eg. if you recorded a run of `your_task_function(1, 2)` 5 times and `your_task_function(3, 4)` 2 times, the re-run would only run 2 examples -- (1, 2) and (3, 4). Each of these re-runs is saved as a new checkpoint for comparison later. 
 ```python
 from eyeball_pp import rerun_recorded_examples 
 
 for input_vars in rerun_recorded_examples():
   your_task_function(input_vars['input_a'], input_vars['input_b'])
@@ -65,15 +80,15 @@
 ```python
 from eyeball_pp import get_eval_param, rerun_recorded_examples 
 
 for vars in rerun_recorded_examples({'model': 'gpt-4', 'temperature': 0.7}, {'model': 'mpt-30b-chat'}):
   your_task_function(vars['input_a'], vars['input_b'])
 
 # You can access these eval params from anywhere in your code
-@eyeball_pp.record_task
+@eyeball_pp.record_task(args_to_record=['input_a', 'input_b'])
 def your_task_function(input_a, input_b):
   ...
   model = get_eval_param('model') or 'gpt-3.5-turbo'
   temperature = get_eval_param('temperature') or 0.5
 ```
 
 ## Compare
@@ -96,15 +111,15 @@
 
 Summary:
 2/2 examples got better in their most recent runs
 The param combination (model=gpt-4, temperature=0.7) works better for 2/2 examples than the default params
 The param combination (model=claude-v1, temperature=None) works equally as good as the (model=gpt-4, temperature=0.7) combination for 2/2 examples
 ```
 
-The comparison will also output a .md file in your repo with the comparison results in a tabular format.
+The comparison will also output a benchmark.md file in your repo with the comparison results in a tabular format.
 
 # Configuration 
 
 ## Serialization
 For the `record_task` decorator you need to ensure that the inputs to the function and outputs are json serialable. If the variables are custom classes you can define the `to_json` and `from_json` functions on that object. If you want to skip serializing some inputs you can specify that in the decorator as `args_to_skip` 
 eg. 
 ```python
```

### Comparing `eyeball_pp-0.0.1/eyeball_pp/__init__.py` & `eyeball_pp-0.0.2/eyeball_pp/__init__.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.1/eyeball_pp/classes.py` & `eyeball_pp-0.0.2/eyeball_pp/classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from enum import IntEnum
-from typing import Callable
+from typing import Any, Callable
 from dataclasses import dataclass
+from typing import Protocol
 
 
 class FeedbackResult(IntEnum):
     POSITIVE = 1
     NEGATIVE = -1
     NEUTRAL = 0
 
@@ -46,15 +47,23 @@
 
     @staticmethod
     def from_dict(data):
         return OutputScore(score=data["score"], message=data["message"])
 
 
 # Compare the output of two checkpoints for a given objective
-# The comparator should return the output of -- How would you rate checkpoint b compared to checkpoint a? Is it positive, negative or neutral?
-# First input is the objective , second is a dictionary of input variables, third is the value for a, fourth is the value for b
-OutputComparator = Callable[[str, dict[str, str], str, str], OutputFeedback]
+# The comparator should return the output of -- How would you rate the newer_checkpoint output compared to older_checkpoint output? Is it positive, negative or neutral?
+class OutputComparator(Protocol):
+    def __call__(
+        self,
+        objective: str,
+        input_variables: dict[str, str],
+        older_checkpoint_output: str,
+        newer_checkpoint_output: str,
+    ) -> OutputFeedback:
+        ...
+
 
 # The output scorer is used to score the output of a model given the objective and inputs
 # The scorer should return a float with a higher value indicating a better output
 # First input is the objective , second is a dictionary of input variables, third is the value for the output
 OutputScorer = Callable[[str, dict[str, str], str], OutputScore]
```

### Comparing `eyeball_pp-0.0.1/eyeball_pp/comparators.py` & `eyeball_pp-0.0.2/eyeball_pp/comparators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from .classes import FeedbackResult, OutputFeedback, OutputScore
 import openai
 
 
-def comparator_from_scores(
-    score_a: OutputScore, score_b: OutputScore
+def output_feedback_from_scores(
+    older_score: OutputScore, newer_score: OutputScore
 ) -> OutputFeedback:
-    if score_a == score_b:
+    if older_score == newer_score:
         return OutputFeedback(
             FeedbackResult.NEUTRAL,
-            f"Score {score_a} is equal to {score_b}",
+            f"Score {older_score} is equal to {newer_score}",
         )
-    elif score_a > score_b:
+    elif older_score > newer_score:
         return OutputFeedback(
             FeedbackResult.NEGATIVE,
-            f"Score {score_b} is worse than {score_b}",
+            f"Score {newer_score} is worse than {newer_score}",
         )
     else:
         return OutputFeedback(
             FeedbackResult.POSITIVE,
-            f"Score {score_b} is better than {score_a}",
+            f"Score {newer_score} is better than {older_score}",
         )
 
 
 def model_graded_comparator(
-    objective: str, inputs: dict[str, str], output_a: str, output_b: str
+    objective: str,
+    input_variables: dict[str, str],
+    older_checkpoint_output: str,
+    newer_checkpoint_output: str,
 ) -> OutputFeedback:
-    input_str = "\n".join([f"{key}: {val}" for key, val in inputs.items()])
+    input_str = "\n".join([f"{key}: {val}" for key, val in input_variables.items()])
 
     system_msg = f"""
 You are a human evaluator trying to grade the response of a function based on the following objective and inputs.
 
 Objective:
 {objective}
 
@@ -37,18 +40,18 @@
 {input_str}
 """
 
     is_b_better = f"""
 Keeping the objectives and the inputs in mind, which of the following responses is better?
 
 Response A:
-{output_a}
+{older_checkpoint_output}
 
 Response B:
-{output_b}
+{newer_checkpoint_output}
 
 Give your reasoning followed by one of the following options:
 Yes -- if Response A is better than B
 No -- if Response B is better than A
 Same -- if both are equally good
 """
     response = openai.ChatCompletion.create(  # type: ignore
```

### Comparing `eyeball_pp-0.0.1/eyeball_pp/eval.py` & `eyeball_pp-0.0.2/eyeball_pp/eval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from collections import defaultdict
 from contextlib import contextmanager
 from enum import Enum
 import inspect
 import json
+import os
 from .recorders import (
     Checkpoint,
     ComparisonResult,
     DiskRecorder,
     FileRecorder,
     MemoryRecorder,
     EvalRecorder,
     get_input_hash,
 )
-from .comparators import model_graded_comparator, comparator_from_scores
+from .comparators import model_graded_comparator, output_feedback_from_scores
 from .classes import (
     FeedbackResult,
     OutputComparator,
     OutputScore,
     OutputScorer,
     OutputFeedback,
 )
@@ -35,15 +36,16 @@
 )
 from functools import wraps
 from dataclasses import dataclass
 import dataclasses
 import datetime
 from .utils import get_user_input
 from .classes import FeedbackResult
-
+from rich.console import Console
+from rich.table import Table
 
 GREEN = "\x1b[32m"
 ORANGE = "\x1b[33m"
 RED = "\x1b[31m"
 BOLD = "\x1b[1m"
 UNDERLINE = "\x1b[4m"
 ITALIC = "\x1b[3m"
@@ -102,15 +104,16 @@
         self.set_config(**config_kwargs)
 
     def _get_config(self, **override_config_kwargs) -> EvaluatorConfig:
         return EvaluatorConfig._merge(self.config, **override_config_kwargs)
 
     def set_config(self, **config_kwargs) -> None:
         self.config = EvaluatorConfig._merge(self.config, **config_kwargs)
-        self.recorder: EvalRecorder = FileRecorder(self.config.dir_path)
+        self.data_dir = os.path.join(self.config.dir_path, "eyeball_data")
+        self.recorder: EvalRecorder = FileRecorder(self.data_dir)
 
     @contextmanager
     def start_recording_session(
         self,
         task_name: str,
         checkpoint_id: Optional[str] = None,
         checkpoint_id_to_rerun: Optional[str] = None,
@@ -596,14 +599,97 @@
                     f"Must provide a task_name as you have multiple tasks recorded -- Found: {task_names}"
                 )
         input_hash = get_input_hash(
             {k: self._serialize(v) for k, v in input_vars.items()}
         )
         self.recorder.delete_checkpoints_for_input_hash(task_name, input_hash)
 
+    def compute_latest_comparison_results(self, task_name: str) -> None:
+        input_names: set[str] = set()
+        rows: list[dict[str, str]] = []
+        comparison_column_names = [
+            "latest_checkpoint",
+            "previous_checkpoint",
+            "the_checkpoint_before",
+        ]
+
+        for input_hash in self.recorder.get_input_hashes(task_name):
+            checkpoints = self.recorder.get_latest_checkpoints(
+                task_name, input_hash, num_checkpoints=1
+            )
+            if len(checkpoints) == 0:
+                continue
+
+            checkpoint = self.recorder.get_checkpoint(task_name, checkpoints[0])
+            if checkpoint is None:
+                continue
+
+            row_data = {}
+            input_names.update(checkpoint.input_variables.keys())
+            for input_name, input_value in checkpoint.input_variables.items():
+                row_data[input_name] = input_value
+
+            comparison_results = self.recorder.get_comparison_results_for_input_hash(
+                task_name=task_name,
+                input_hash=input_hash,
+                num_results=len(comparison_column_names),
+            )
+            sorted_comparison_results = sorted(
+                comparison_results,
+                key=lambda x: x.newer_checkpoint_id,
+                reverse=True,
+            )
+            for idx, comparison_result in enumerate(sorted_comparison_results):
+                msg = comparison_result.output_feedback.result.name
+                new_checkpoint = self.recorder.get_checkpoint(
+                    task_name=task_name,
+                    checkpoint_id=comparison_result.newer_checkpoint_id,
+                )
+                if new_checkpoint is not None:
+                    if new_checkpoint.output_score is not None:
+                        msg += f" (score: {new_checkpoint.output_score})"
+                    eval_params_str = ", ".join(
+                        f"{k}={v}" for k, v in new_checkpoint.eval_params.items()
+                    )
+                    if eval_params_str:
+                        msg += f" ({eval_params_str})"
+                row_data[comparison_column_names[idx]] = msg
+
+            rows.append(row_data)
+
+        md_data = []
+        table = Table(title="Comparison Results")
+
+        if len(rows) > 0:
+            column_names = sorted(list(input_names)) + comparison_column_names
+            for column_name in column_names:
+                table.add_column(column_name, justify="left")
+
+            md_data.append("| " + " | ".join(column_names) + " |")
+
+            for row in rows:
+                row_tuple = tuple(
+                    row.get(column_name, "") for column_name in column_names
+                )
+                table.add_row(*row_tuple)
+                md_data.append("| " + " | ".join(row_tuple) + " |")
+
+            task_data_dir = os.path.join(self.data_dir, task_name)
+            if not os.path.exists(task_data_dir):
+                os.makedirs(task_data_dir)
+
+            with open(
+                os.path.join(task_data_dir, "benchmark.md"),
+                "w+",
+            ) as f:
+                f.write("\n".join(md_data))
+
+            console = Console()
+            console.print(table)
+
     def compare_recorded_checkpoints(
         self,
         task_name: Optional[str] = None,
         num_input_hashes: int = 5,
         num_checkpoints_per_input_hash: int = 3,
         task_objective: Optional[str] = None,
         output_comparator: Optional[OutputComparator] = None,
@@ -659,15 +745,15 @@
                         checkpoint is not None
                         and checkpoint.output is not None
                         and checkpoint.output != "null"
                         and checkpoint.output != "None"
                     ):
                         filtered_checkpoint_ids.append(checkpoind_id)
                         checkpoints[checkpoind_id] = checkpoint
-                checkpoint_ids = filtered_checkpoint_ids
+                checkpoint_ids = sorted(filtered_checkpoint_ids, reverse=True)
 
                 if len(checkpoint_ids) == 0:
                     continue
 
                 scores: dict[str, OutputScore] = {}
                 if output_scorer is not None:
                     print(f"\nInput #{idx} - Scoring {len(checkpoint_ids)} checkpoints")
@@ -696,146 +782,149 @@
                         )
                         scores[checkpoint_id] = score
                         print(f"Scored {checkpoint_id}: {score}")
 
                 if len(checkpoint_ids) < 2:
                     continue
 
+                # Newer checkpoints are at the start of the list so for every comparison
+                # we compare the newer_checkpoint_id with the older_checkpoint_id
                 to_compare = [
                     (checkpoint_ids[i], checkpoint_ids[i + 1])
                     for i in range(len(checkpoint_ids) - 1)
                 ]
 
                 print(f"\nInput #{idx} - Running {len(to_compare)} comparison(s)")
 
-                for checkpoint_id_a, checkpoint_id_b in to_compare:
-                    checkpoint_a = self.recorder.get_checkpoint(
+                for newer_checkpoint_id, older_checkpoint_id in to_compare:
+                    newer_checkpoint = self.recorder.get_checkpoint(
                         task_name=task_name,
-                        checkpoint_id=checkpoint_id_a,
+                        checkpoint_id=newer_checkpoint_id,
                     )
-                    checkpoint_b = self.recorder.get_checkpoint(
+                    older_checkpoint = self.recorder.get_checkpoint(
                         task_name=task_name,
-                        checkpoint_id=checkpoint_id_b,
+                        checkpoint_id=older_checkpoint_id,
                     )
 
-                    if checkpoint_a is None or checkpoint_b is None:
+                    if newer_checkpoint is None or older_checkpoint is None:
                         print(
-                            f"Could not find checkpoint {checkpoint_id_a} or {checkpoint_id_b}"
+                            f"Could not find checkpoint {newer_checkpoint_id} or {older_checkpoint_id}"
                         )
                         continue
 
-                    output_a = checkpoint_a.output
-                    output_b = checkpoint_b.output
+                    newer_checkpoint_output = newer_checkpoint.output
+                    older_checkpoint_output = older_checkpoint.output
 
-                    assert output_a is not None
-                    assert output_b is not None
+                    assert newer_checkpoint_output is not None
+                    assert older_checkpoint_output is not None
 
                     should_record_comparison = True
                     if use_cached_comparisons and (
                         comparator_result := self.recorder.get_comparison_result(
                             task_name=task_name,
-                            checkpoint_id_a=checkpoint_id_a,
-                            checkpoint_id_b=checkpoint_id_b,
+                            older_checkpoint_id=older_checkpoint_id,
+                            newer_checkpoint_id=newer_checkpoint_id,
                         )
                     ):
                         print(f"Using cached comparison result for {input_hash}")
                         should_record_comparison = False
                         output_comparison_feedback = comparator_result.output_feedback
                     elif output_comparator is not None:
                         output_comparison_feedback = output_comparator(
-                            task_objective or "",
-                            checkpoint_a.get_input_variables(),
-                            output_a,
-                            output_b,
+                            objective=task_objective or "",
+                            input_variables=newer_checkpoint.get_input_variables(),
+                            older_checkpoint_output=older_checkpoint_output,
+                            newer_checkpoint_output=newer_checkpoint_output,
                         )
                     elif output_scorer is not None:
-                        output_comparison_feedback = comparator_from_scores(
-                            scores[checkpoint_id_a], scores[checkpoint_id_b]
+                        output_comparison_feedback = output_feedback_from_scores(
+                            older_score=scores[older_checkpoint_id],
+                            newer_score=scores[newer_checkpoint_id],
                         )
                     else:
                         raise ValueError(
                             "Should not happen. We need an output comparator or output scorer"
                         )
 
-                    a_unique_params = []
-                    b_unqiue_params = []
+                    new_unique_params = []
+                    old_unqiue_params = []
                     for key in (
-                        checkpoint_a.eval_params.keys()
-                        | checkpoint_b.eval_params.keys()
+                        newer_checkpoint.eval_params.keys()
+                        | older_checkpoint.eval_params.keys()
                     ):
-                        param_val_a = checkpoint_a.eval_params.get(key)
-                        param_val_b = checkpoint_b.eval_params.get(key)
+                        param_val_a = newer_checkpoint.eval_params.get(key)
+                        param_val_b = older_checkpoint.eval_params.get(key)
                         if param_val_a != param_val_b:
                             if param_val_a is not None:
-                                a_unique_params.append(f"{key}={param_val_a}")
+                                new_unique_params.append(f"{key}={param_val_a}")
                             elif param_val_b is not None:
-                                b_unqiue_params.append(f"{key}={param_val_b}")
+                                old_unqiue_params.append(f"{key}={param_val_b}")
 
-                    a_unique_params_str = (
-                        ("(" + ", ".join(a_unique_params) + ")")
-                        if len(a_unique_params) > 0
+                    new_unique_params_str = (
+                        ("(" + ", ".join(new_unique_params) + ")")
+                        if len(new_unique_params) > 0
                         else ""
                     )
-                    b_unique_params_str = (
-                        ("(" + ", ".join(b_unqiue_params) + ")")
-                        if len(b_unqiue_params) > 0
+                    old_unique_params_str = (
+                        ("(" + ", ".join(old_unqiue_params) + ")")
+                        if len(old_unqiue_params) > 0
                         else ""
                     )
 
-                    a_params_str = ",".join(
-                        f"{k}={v}" for k, v in checkpoint_a.eval_params.items()
+                    new_params_str = ",".join(
+                        f"{k}={v}" for k, v in newer_checkpoint.eval_params.items()
                     )
-                    b_params_str = ",".join(
-                        f"{k}={v}" for k, v in checkpoint_b.eval_params.items()
+                    old_params_str = ",".join(
+                        f"{k}={v}" for k, v in older_checkpoint.eval_params.items()
                     )
 
-                    rerun_id_a = (
-                        checkpoint_a.rerun_metadata.get("id")
-                        if checkpoint_a.rerun_metadata is not None
+                    rerun_id_new = (
+                        newer_checkpoint.rerun_metadata.get("id")
+                        if newer_checkpoint.rerun_metadata is not None
                         else None
                     )
-                    rerun_id_b = (
-                        checkpoint_b.rerun_metadata.get("id")
-                        if checkpoint_b.rerun_metadata is not None
+                    rerun_id_old = (
+                        older_checkpoint.rerun_metadata.get("id")
+                        if older_checkpoint.rerun_metadata is not None
                         else None
                     )
 
                     num_comparisons += 1
 
                     if output_comparison_feedback.result == FeedbackResult.NEUTRAL:
                         print(
-                            f"{ORANGE}[neutral] task output is the same between checkpoints {checkpoint_id_a} {a_unique_params_str} & {checkpoint_id_b} {b_unique_params_str} {END_CLR}"
+                            f"{ORANGE}[neutral] task output is the same between checkpoints {older_checkpoint_id} {old_unique_params_str} & {newer_checkpoint_id} {new_unique_params_str} {END_CLR}"
                         )
-                        params_to_succesful_examples[a_params_str] += 1
-                        params_to_succesful_examples[b_params_str] += 1
-                        if rerun_id_a is not None:
-                            rerun_to_succesful_examples[rerun_id_a] += 1
-                        if rerun_id_b is not None:
-                            rerun_to_succesful_examples[rerun_id_b] += 1
+                        params_to_succesful_examples[new_params_str] += 1
+                        params_to_succesful_examples[old_params_str] += 1
+                        if rerun_id_new is not None:
+                            rerun_to_succesful_examples[rerun_id_new] += 1
+                        if rerun_id_old is not None:
+                            rerun_to_succesful_examples[rerun_id_old] += 1
                     elif output_comparison_feedback.result == FeedbackResult.NEGATIVE:
                         print(
-                            f"{RED}[regression] task output was better in checkpoint {checkpoint_id_a} {a_unique_params_str} than {checkpoint_id_b} {b_unique_params_str} {END_CLR}"
+                            f"{RED}[regression] task output was better in the older checkpoint {older_checkpoint_id} {old_unique_params_str} than {newer_checkpoint_id} {new_unique_params_str} {END_CLR}"
                         )
-                        params_to_succesful_examples[a_params_str] += 1
-                        if rerun_id_a is not None:
-                            rerun_to_succesful_examples[rerun_id_a] += 1
+                        params_to_succesful_examples[old_params_str] += 1
+                        if rerun_id_old is not None:
+                            rerun_to_succesful_examples[rerun_id_old] += 1
                     else:
                         print(
-                            f"{GREEN}[improvement] task output improved from checkpoint {checkpoint_id_a} {a_unique_params_str} to {checkpoint_id_b} {b_unique_params_str}{END_CLR}"
+                            f"{GREEN}[improvement] task output improved from checkpoint {older_checkpoint_id} {old_unique_params_str} to {newer_checkpoint_id} {new_unique_params_str}{END_CLR}"
                         )
-                        params_to_succesful_examples[b_params_str] += 1
-                        if rerun_id_b is not None:
-                            rerun_to_succesful_examples[rerun_id_b] += 1
+                        params_to_succesful_examples[new_params_str] += 1
+                        if rerun_id_new is not None:
+                            rerun_to_succesful_examples[rerun_id_new] += 1
                     if should_record_comparison:
                         self.recorder.record_comparison_result(
                             task_name=task_name,
                             input_hash=input_hash,
                             result=ComparisonResult(
-                                checkpoint_id_a=checkpoint_id_a,
-                                checkpoint_id_b=checkpoint_id_b,
+                                older_checkpoint_id=older_checkpoint_id,
+                                newer_checkpoint_id=newer_checkpoint_id,
                                 output_feedback=output_comparison_feedback,
                             ),
                         )
 
             print("\nSummary:")
             print("---------")
             if len(rerun_to_succesful_examples) > 0:
@@ -853,14 +942,16 @@
             for params, num_successes in sorted(
                 params_to_succesful_examples.items(), key=lambda x: x[1], reverse=True
             ):
                 if params == "":
                     params = "default"
                 print(f"{params}: {num_successes}/{num_comparisons} successes")
 
+            self.compute_latest_comparison_results(task_name)
+
         finally:
             self.mode = EvaluatorMode.RECORD
 
 
 _default_evaluator = Evaluator()
```

### Comparing `eyeball_pp-0.0.1/eyeball_pp/recorders.py` & `eyeball_pp-0.0.2/eyeball_pp/recorders.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import dataclasses
 
 from .classes import OutputFeedback, OutputScore
 
 
 @dataclass
 class ComparisonResult:
-    checkpoint_id_a: str
-    checkpoint_id_b: str
+    older_checkpoint_id: str
+    newer_checkpoint_id: str
     output_feedback: OutputFeedback
 
 
 def get_input_hash(input_variables: dict[str, str]) -> str:
     sorted_input_vars = sorted(
         [
             (str(var_name), str(var_val))
@@ -130,23 +130,21 @@
         result: ComparisonResult,
     ) -> None:
         ...
 
     def get_comparison_result(
         self,
         task_name: str,
-        checkpoint_id_a: str,
-        checkpoint_id_b: str,
+        older_checkpoint_id: str,
+        newer_checkpoint_id: str,
     ) -> Optional[ComparisonResult]:
         ...
 
     def get_comparison_results_for_input_hash(
-        self,
-        task_name: str,
-        input_hash: str,
+        self, task_name: str, input_hash: str, num_results: int = 3
     ) -> list[ComparisonResult]:
         ...
 
     def delete_checkpoints_for_input_hash(
         self,
         task_name: str,
         input_hash: str,
@@ -300,15 +298,15 @@
     def record_comparison_result(
         self,
         task_name: str,
         input_hash: str,
         result: ComparisonResult,
     ) -> None:
         task = self.tasks[task_name]
-        key = f"{result.checkpoint_id_a},{result.checkpoint_id_b}"
+        key = f"{result.older_checkpoint_id},{result.newer_checkpoint_id}"
         task.comparison_results[key] = result
 
         if input_hash not in task.input_hash_to_comparison_results:
             task.input_hash_to_comparison_results[input_hash] = set()
         task.input_hash_to_comparison_results[input_hash].add(key)
 
     def record_output_score(
@@ -321,52 +319,53 @@
             task_name=task_name, checkpoint_id=checkpoint_id
         )
         checkpoint.output_score = score
 
     def get_comparison_result(
         self,
         task_name: str,
-        checkpoint_id_a: str,
-        checkpoint_id_b: str,
+        older_checkpoint_id: str,
+        newer_checkpoint_id: str,
     ) -> Optional[ComparisonResult]:
         task = self.tasks[task_name]
-        key = f"{checkpoint_id_a},{checkpoint_id_b}"
+        key = f"{older_checkpoint_id},{newer_checkpoint_id}"
         if key not in task.comparison_results:
             return None
         return task.comparison_results[key]
 
     def get_comparison_results_for_input_hash(
         self,
         task_name: str,
         input_hash: str,
+        num_results: int = 3,
     ) -> list[ComparisonResult]:
         task = self.tasks[task_name]
         if input_hash not in task.input_hash_to_comparison_results:
             return []
         comparison_results = task.input_hash_to_comparison_results[input_hash]
-        return [task.comparison_results[key] for key in comparison_results]
+        return [task.comparison_results[key] for key in comparison_results][
+            :num_results
+        ]
 
     def delete_checkpoints_for_input_hash(
         self,
         task_name: str,
         input_hash: str,
     ) -> None:
         task = self.tasks[task_name]
-        print(input_hash)
-        print(task.input_hashes.keys())
         if input_hash not in task.input_hashes:
             return
         for checkpoint_id in task.input_hashes[input_hash]:
             del task.checkpoints[checkpoint_id]
         del task.input_hashes[input_hash]
 
 
 class FileRecorder(EvalRecorder):
     def __init__(self, dir_path: str) -> None:
-        self.dir_path = os.path.join(dir_path, "eyeball_data")
+        self.dir_path = dir_path
         if not os.path.exists(self.dir_path):
             os.makedirs(self.dir_path)
         self.yaml_dicts: dict[str, dict[str, str]] = {}
 
     def _record_checkpoint(
         self,
         task_name: str,
@@ -562,40 +561,94 @@
     def get_task_names(self) -> list[str]:
         task_names = []
         for dir_name in os.listdir(self.dir_path):
             if os.path.isdir(os.path.join(self.dir_path, dir_name)):
                 task_names.append(dir_name)
         return task_names
 
-    def _write_latest_comparison_results(self, task_name: str) -> None:
-        ...
-
     def record_comparison_result(
         self,
         task_name: str,
         input_hash: str,
         result: ComparisonResult,
     ) -> None:
-        # TODO: record as a md file
-        ...
+        comparison_dir = os.path.join(self.dir_path, task_name, "comparison_results")
+        if not os.path.exists(comparison_dir):
+            os.makedirs(comparison_dir)
+
+        file_name = f"{input_hash}_{result.older_checkpoint_id}_{result.newer_checkpoint_id}.yaml"
+        file_path = os.path.join(comparison_dir, file_name)
+        yaml.dump(
+            result.output_feedback.as_dict(),
+            open(file_path, "w+"),
+        )
 
     def get_comparison_result(
         self,
         task_name: str,
-        checkpoint_id_a: str,
-        checkpoint_id_b: str,
+        older_checkpoint_id: str,
+        newer_checkpoint_id: str,
     ) -> Optional[ComparisonResult]:
-        ...
+        comparison_dir = os.path.join(self.dir_path, task_name, "comparison_results")
+        if not os.path.exists(comparison_dir):
+            return None
+
+        for file_name in os.listdir(comparison_dir):
+            splits = os.path.splitext(file_name)[0].split("_")
+            if len(splits) != 3:
+                continue
+
+            if splits[1] != older_checkpoint_id:
+                continue
+
+            if splits[2] != newer_checkpoint_id:
+                continue
+
+            if file_name.endswith(".yaml"):
+                file_path = os.path.join(comparison_dir, file_name)
+                yaml_dict = yaml.load(open(file_path, "r"), Loader=yaml.FullLoader)
+                return ComparisonResult(
+                    older_checkpoint_id=older_checkpoint_id,
+                    newer_checkpoint_id=newer_checkpoint_id,
+                    output_feedback=OutputFeedback.from_dict(yaml_dict),
+                )
+        return None
 
     def get_comparison_results_for_input_hash(
         self,
         task_name: str,
         input_hash: str,
+        num_results: int = 3,
     ) -> list[ComparisonResult]:
-        ...
+        comparison_dir = os.path.join(self.dir_path, task_name, "comparison_results")
+        if not os.path.exists(comparison_dir):
+            return []
+
+        results: list[ComparisonResult] = []
+        for file_name in os.listdir(comparison_dir):
+            splits = os.path.splitext(file_name)[0].split("_")
+            if len(splits) != 3:
+                continue
+
+            if splits[0] != input_hash:
+                continue
+
+            if file_name.endswith(".yaml"):
+                file_path = os.path.join(comparison_dir, file_name)
+                yaml_dict = yaml.load(open(file_path, "r"), Loader=yaml.FullLoader)
+                results.append(
+                    ComparisonResult(
+                        older_checkpoint_id=splits[1],
+                        newer_checkpoint_id=splits[2],
+                        output_feedback=OutputFeedback.from_dict(yaml_dict),
+                    )
+                )
+        return sorted(results, key=lambda x: x.newer_checkpoint_id, reverse=True)[
+            :num_results
+        ]
 
     def delete_checkpoints_for_input_hash(
         self,
         task_name: str,
         input_hash: str,
     ) -> None:
         ...
@@ -694,30 +747,31 @@
             task_name=task_name, checkpoint_id=checkpoint_id, score=score
         )
         pickle.dump(self.memory_recorder, open(self.file_name, "wb"))
 
     def get_comparison_result(
         self,
         task_name: str,
-        checkpoint_id_a: str,
-        checkpoint_id_b: str,
+        older_checkpoint_id: str,
+        newer_checkpoint_id: str,
     ) -> Optional[ComparisonResult]:
         return self.memory_recorder.get_comparison_result(
             task_name=task_name,
-            checkpoint_id_a=checkpoint_id_a,
-            checkpoint_id_b=checkpoint_id_b,
+            older_checkpoint_id=older_checkpoint_id,
+            newer_checkpoint_id=newer_checkpoint_id,
         )
 
     def get_comparison_results_for_input_hash(
         self,
         task_name: str,
         input_hash: str,
+        num_results: int = 3,
     ) -> list[ComparisonResult]:
         return self.memory_recorder.get_comparison_results_for_input_hash(
-            task_name=task_name, input_hash=input_hash
+            task_name=task_name, input_hash=input_hash, num_results=num_results
         )
 
     def record_output(
         self,
         task_name: str,
         checkpoint_id: str,
         output: str,
@@ -734,7 +788,10 @@
         task_name: str,
         input_hash: str,
     ) -> None:
         self.memory_recorder.delete_checkpoints_for_input_hash(
             task_name=task_name, input_hash=input_hash
         )
         pickle.dump(self.memory_recorder, open(self.file_name, "wb"))
+
+    def compute_latest_comparison_results(self, task_name: str) -> None:
+        ...
```

### Comparing `eyeball_pp-0.0.1/eyeball_pp.egg-info/PKG-INFO` & `eyeball_pp-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: eyeball-pp
-Version: 0.0.1
-Summary: A python package for evaluating tasks which use llms
-Home-page: https://github.com/revantk/eyeball-plus-plus
-Author: Revant
-Author-email: revant.kapoor@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Eyeball++ 
 _Ridiculously simple evaluation for LLM agents_
 
 eyeball_pp is a framework to evaluate and benchmark tasks which use llms.
 
 This framework helps you answer questions like: "Which llm is the best for my specific task?" or "This prompt change looks good on the example I just tested, does it work with all the other things I've tested?"
 
@@ -23,29 +11,30 @@
 
 # Installation
 eyeball_pp is a python library which can be installed via pip 
 
 `pip install eyeball_pp`
 
 # Concepts 
-eyeball_pp has 3 simple concepts -- record, rerun and compare.
+eyeball_pp has 3 simple concepts -- record, rerun and compare. To see a detailed example check out the examples/ folder in the repo
 
 ## Record
 eyeball_pp consists of a recorder which records the inputs and outputs of your task runs as you are running it and saves them as checkpoints. You can record this locally while developing or from a production system. You can optionally record human feedback for the task output too.
 
-You can record your task using the `record_task` decorator. This will record every run of this function call as a `Checkpoint` for future comparison.
+You can record your task using the `record_task` decorator. This will record every run of this function call as a `Checkpoint` for future comparison. The args_to_record specify which inputs to record and the function return value is saved as the output.
 ```python
 import eyeball_pp
 
 @eyeball_pp.record_task(args_to_record=['input_a', 'input_b'])
 def your_task_function(input_a, input_b):
   # Your task can run arbitrary code
   ...
   return task_output
 ```
+If you want to record additional inputs within your function call you can just call `eyeball_pp.record_input('variable_name', value)` inside your function.
 
 If your sytem is more complicated, you can also use the `record_input` and `record_output` functions with the start_recording_session context manager
 ```python
 import eyeball_pp
 
 # your task code 
 ...
@@ -60,14 +49,16 @@
 
 ```python
 eyeball_pp.record_input(task_name="your_task", checkpoint_id="some_custom_unique_id", variable_name="input_a", value=input_a_value)
 ..
 eyeball_pp.record_output(task_name="your_task", checkpoint_id="some_custom_unique_id", variable_name='output', output=output)
 ```
 
+Data by default gets recorded as yaml files in your repo so you can always inspect it, change it or delete it.
+
 ## Rerun
 You can then re-run these pre-recorded examples as you make changes. This will only re-run each unique set of input variables. eg. if you recorded a run of `your_task_function(1, 2)` 5 times and `your_task_function(3, 4)` 2 times, the re-run would only run 2 examples -- (1, 2) and (3, 4). Each of these re-runs is saved as a new checkpoint for comparison later. 
 ```python
 from eyeball_pp import rerun_recorded_examples 
 
 for input_vars in rerun_recorded_examples():
   your_task_function(input_vars['input_a'], input_vars['input_b'])
@@ -77,15 +68,15 @@
 ```python
 from eyeball_pp import get_eval_param, rerun_recorded_examples 
 
 for vars in rerun_recorded_examples({'model': 'gpt-4', 'temperature': 0.7}, {'model': 'mpt-30b-chat'}):
   your_task_function(vars['input_a'], vars['input_b'])
 
 # You can access these eval params from anywhere in your code
-@eyeball_pp.record_task
+@eyeball_pp.record_task(args_to_record=['input_a', 'input_b'])
 def your_task_function(input_a, input_b):
   ...
   model = get_eval_param('model') or 'gpt-3.5-turbo'
   temperature = get_eval_param('temperature') or 0.5
 ```
 
 ## Compare
@@ -108,15 +99,15 @@
 
 Summary:
 2/2 examples got better in their most recent runs
 The param combination (model=gpt-4, temperature=0.7) works better for 2/2 examples than the default params
 The param combination (model=claude-v1, temperature=None) works equally as good as the (model=gpt-4, temperature=0.7) combination for 2/2 examples
 ```
 
-The comparison will also output a .md file in your repo with the comparison results in a tabular format.
+The comparison will also output a benchmark.md file in your repo with the comparison results in a tabular format.
 
 # Configuration 
 
 ## Serialization
 For the `record_task` decorator you need to ensure that the inputs to the function and outputs are json serialable. If the variables are custom classes you can define the `to_json` and `from_json` functions on that object. If you want to skip serializing some inputs you can specify that in the decorator as `args_to_skip` 
 eg. 
 ```python
```

