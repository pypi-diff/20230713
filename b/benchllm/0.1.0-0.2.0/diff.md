# Comparing `tmp/benchllm-0.1.0.tar.gz` & `tmp/benchllm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchllm-0.1.0.tar", max compression
+gzip compressed data, was "benchllm-0.2.0.tar", max compression
```

## Comparing `benchllm-0.1.0.tar` & `benchllm-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,30 @@
--rw-r--r--   0        0        0     1059 2023-07-06 17:49:06.559536 benchllm-0.1.0/LICENSE
--rw-r--r--   0        0        0     6873 2023-07-06 17:49:06.559536 benchllm-0.1.0/README.md
--rw-r--r--   0        0        0     1329 2023-07-06 17:49:06.559536 benchllm-0.1.0/benchllm/__init__.py
--rw-r--r--   0        0        0      285 2023-07-06 17:49:06.559536 benchllm-0.1.0/benchllm/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 17:49:06.559536 benchllm-0.1.0/benchllm/cli/commands/__init__.py
--rw-r--r--   0        0        0      969 2023-07-06 17:49:06.559536 benchllm-0.1.0/benchllm/cli/commands/add_test.py
--rw-r--r--   0        0        0      901 2023-07-06 17:49:06.559536 benchllm-0.1.0/benchllm/cli/commands/evaluate.py
--rw-r--r--   0        0        0     1283 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/cli/commands/list_tests.py
--rw-r--r--   0        0        0     1448 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/cli/commands/run_suite.py
--rw-r--r--   0        0        0     2774 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/cli/evaluator.py
--rw-r--r--   0        0        0     5333 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/cli/listener.py
--rw-r--r--   0        0        0     3588 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/cli/main.py
--rw-r--r--   0        0        0     1052 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/cli/utils.py
--rw-r--r--   0        0        0     1497 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/data_types.py
--rw-r--r--   0        0        0     5981 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/evaluator.py
--rw-r--r--   0        0        0      244 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/input_types.py
--rw-r--r--   0        0        0     1086 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/listener.py
--rw-r--r--   0        0        0     1494 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/similarity.py
--rw-r--r--   0        0        0      748 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/singleton.py
--rw-r--r--   0        0        0     8813 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/tester.py
--rw-r--r--   0        0        0     2057 2023-07-06 17:49:06.563536 benchllm-0.1.0/benchllm/utils.py
--rw-r--r--   0        0        0     2065 2023-07-06 17:49:06.563536 benchllm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8082 1970-01-01 00:00:00.000000 benchllm-0.1.0/setup.py
--rw-r--r--   0        0        0     7887 1970-01-01 00:00:00.000000 benchllm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-13 15:45:09.119152 benchllm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8869 2023-07-13 15:45:09.119152 benchllm-0.2.0/README.md
+-rw-r--r--   0        0        0     1313 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/__init__.py
+-rw-r--r--   0        0        0     3654 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cache.py
+-rw-r--r--   0        0        0      285 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/commands/__init__.py
+-rw-r--r--   0        0        0      969 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/commands/add_test.py
+-rw-r--r--   0        0        0     1053 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/commands/evaluate.py
+-rw-r--r--   0        0        0     1283 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/commands/list_tests.py
+-rw-r--r--   0        0        0     1634 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/commands/run_suite.py
+-rw-r--r--   0        0        0      136 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/evaluator/__init__.py
+-rw-r--r--   0        0        0     1344 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/evaluator/interactive.py
+-rw-r--r--   0        0        0     1813 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/evaluator/web.py
+-rw-r--r--   0        0        0     5818 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/listener.py
+-rw-r--r--   0        0        0     3790 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/main.py
+-rw-r--r--   0        0        0     1502 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/cli/utils.py
+-rw-r--r--   0        0        0     1497 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/data_types.py
+-rw-r--r--   0        0        0      198 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/evaluator/__init__.py
+-rw-r--r--   0        0        0     4502 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/evaluator/evaluator.py
+-rw-r--r--   0        0        0      671 2023-07-13 15:45:09.119152 benchllm-0.2.0/benchllm/evaluator/semantic.py
+-rw-r--r--   0        0        0     1013 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/evaluator/string_match.py
+-rw-r--r--   0        0        0      276 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/input_types.py
+-rw-r--r--   0        0        0     1086 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/listener.py
+-rw-r--r--   0        0        0     1601 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/similarity.py
+-rw-r--r--   0        0        0      743 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/singleton.py
+-rw-r--r--   0        0        0     8813 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/tester.py
+-rw-r--r--   0        0        0     2824 2023-07-13 15:45:09.123152 benchllm-0.2.0/benchllm/utils.py
+-rw-r--r--   0        0        0     2065 2023-07-13 15:45:09.123152 benchllm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10173 1970-01-01 00:00:00.000000 benchllm-0.2.0/setup.py
+-rw-r--r--   0        0        0     9883 1970-01-01 00:00:00.000000 benchllm-0.2.0/PKG-INFO
```

### Comparing `benchllm-0.1.0/LICENSE` & `benchllm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `benchllm-0.1.0/README.md` & `benchllm-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,55 @@
-# BenchLLM
+# 🏋️‍♂️ BenchLLM 🏋️‍♀️
 
-BenchLLM is a Python-based open-source library that streamlines the testing process for Large Language Models (LLMs) and AI-powered applications. It offers an intuitive and robust way to validate and score the output of your code with minimal boilerplate or configuration.
+🦾 Continuous Integration for LLM powered applications 🦙🦅🤖
 
-BenchLLM is actively used at [V7](https://www.v7labs.com) for improving our LLM applications and now Open Sourced under MIT License to share with the wider community
+[![GitHub Repo stars](https://img.shields.io/github/stars/v7labs/BenchLLM?style=social)](https://github.com/v7labs/BenchLLM/stargazers)
+[![Twitter Follow](https://img.shields.io/twitter/follow/V7Labs?style=social)](https://twitter.com/V7Labs)
+[![Discord Follow](https://dcbadge.vercel.app/api/server/x7ExfHb3bG?style=flat)](https://discord.gg/x7ExfHb3bG)
 
-Use BenchLLM to:
+[**BenchLLM**](https://benchllm.com/) is a Python-based open-source library that streamlines the testing of Large Language Models (LLMs) and AI-powered applications. It measures the accuracy of your model, agents, or chains by validating responses on any number of tests via LLMs.
+
+BenchLLM is actively used at [V7](https://www.v7labs.com) for improving our LLM applications and is now Open Sourced under MIT License to share with the wider community
 
-- Easily set up a comprehensive testing suite for your LLMs.
-- Continous integration for your langchain/agents/models.
-- Elimiate flaky chains and create confidence in your code.
+## 💡 Get help on [Discord](https://discord.gg/x7ExfHb3bG) or [Tweet at us](https://twitter.com/V7Labs)
 
-> **NOTE:** BenchLLM is in the early stage of development and will be subject to rapid changes.
+<hr/>
 
-For bug reporting, feature requests, or contributions, please open an issue or submit a pull request (PR) on our GitHub page.
+Use BenchLLM to:
 
-## BenchLLM Testing Methodology
+- Test the responses of your LLM across any number of prompts.
+- Continuous integration for chains like [Langchain](https://github.com/hwchase17/langchain), agents like [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT), or LLM models like [Llama](https://github.com/facebookresearch/llama) or GPT-4.
+- Eliminate flaky chains and create confidence in your code.
+- Spot inaccurate responses and hallucinations in your application at every version.
+
+<hr/>
+
+> ⚠️ **NOTE:** BenchLLM is in the early stage of development and will be subject to rapid changes.
+>
+> For bug reporting, feature requests, or contributions, please open an issue or submit a pull request (PR) on our GitHub page.
+
+## 🧪 BenchLLM Testing Methodology
 
 BenchLLM implements a distinct two-step methodology for validating your machine learning models:
 
-1. **Testing**: This stage involves running your code against various tests and capturing the predictions produced by your model without immediate judgment or comparison.
+1. **Testing**: This stage involves running your code against any number of expected responses and capturing the predictions produced by your model without immediate judgment or comparison.
 
-2. **Evaluation**: During this phase, the recorded predictions are compared against the expected output. Detailed comparison reports, including pass/fail status and other metrics, are generated.
+2. **Evaluation**: The recorded predictions are compared against the expected output using LLMs to verify factual similarity (or optionally manually). Detailed comparison reports, including pass/fail status and other metrics, are generated.
 
 This methodical separation offers a comprehensive view of your model's performance and allows for better control and refinement of each step.
 
-## Install
+## 🚀 Install
 
 To install BenchLLM we use pip
 
 ```
-pip install git+https://github.com/v7labs/benchllm
+pip install benchllm
 ```
 
-## Usage
+## 💻 Usage
 
 Start by importing the library and use the @benchllm.test decorator to mark the function you'd like to test:
 
 ```python
 import benchllm
 
 # Your custom model implementation
@@ -98,30 +111,40 @@
 
 The non interactive evaluators also supports `--workers N` to run in the evaluations in parallel
 
 ```bash
 $ bench run --evaluator string-match --workers 5
 ```
 
-### Eval
+To accelerate the evaluation process, BenchLLM uses a cache. If a (prediction, expected) pair has been evaluated in the past and a cache was used, the evaluation output will be saved for future evaluations. There are several types of caches:
+
+- `memory`, only caches output values during the current run. This is particularly useful when running with `--retry-count N`
+- `file`, stores the cache at the end of the run as a JSON file in output/cache.json. This is the default behavior.
+- `none`, does not use any cache.
+
+```bash
+$ bench run examples --cache memory
+```
+
+### 🧮 Eval
 
-While bench run runs each test function and then evaluates their output, it can often be beneficial to separate these into two steps. For example, if you want a person to manually do the evaluation or if you want to try multiple evaluation methods on the same function.
+While _bench run_ runs each test function and then evaluates their output, it can often be beneficial to separate these into two steps. For example, if you want a person to manually do the evaluation or if you want to try multiple evaluation methods on the same function.
 
 ```bash
 $ bench run --no-eval
 ```
 
 This will generate json files in `output/latest/predictions`
 Then later you can evaluate them with
 
 ```bash
 $ bench eval output/latest/predictions
 ```
 
-## API
+## 🔌 API
 
 For more detailed control, BenchLLM provides an API.
 You are not required to add YML/JSON tests to be able to evaluate your model.
 You can instead:
 
 - Instantiate `Test` objects
 - Use a `Tester` object to generate predictions
@@ -145,24 +168,38 @@
 evaluator = StringMatchEvaluator()
 evaluator.load(predictions)
 results = evaluator.run()
 
 print(results)
 ```
 
-## Commands
+If you want to incorporate caching and run multiple parallel evaluation jobs, you can modify your evaluator as follows:
+
+```python
+from benchllm.cache import FileCache
+
+...
+
+evaluator = FileCache(StringMatchEvaluator(workers=2), Path("path/to/cache.json"))
+evaluator.load(predictions)
+results = evaluator.run()
+```
+
+In this example, `FileCache` is used to enable caching, and the `workers` parameter of `StringMatchEvaluator` is set to `2` to allow for parallel evaluations. The cache results are saved in a file specified by `Path("path/to/cache.json")`.
+
+## ☕️ Commands
 
 - `bench add`: Add a new test to a suite.
 - `bench tests`: List all tests in a suite.
 - `bench run`: Run all or target test suites.
 - `bench eval`: Runs the evaluation of an existing test run.
 
-## Contribute
+## 🙌 Contribute
 
-BenchLLM is developed for Python 3.10, although it may work with other Python versions as well. We recommend using a Python 3.10 environment. You can use conda or any other environment manager to set up the environment:
+BenchLLM is developed for Python 3.10, although it may work with other Python versions as well. We recommend using a Python 3.10 environment and pip >= 23. You can use conda or any other environment manager to set up the environment:
 
 ```bash
 $ conda create --name benchllm python=3.10
 $ conda activate benchllm
 $ pip install -e ".[dev]"
 ```
 
@@ -176,10 +213,10 @@
 
 1. Fork the repository.
 2. Create a new branch for your changes.
 3. Make your changes.
 4. Test your changes.
 5. Submit a pull request.
 
-We adhere to PEP8 style guide. Please follow this guide when contributing.
+We adhere to the PEP8 style guide. Please follow this guide when contributing.
 
-For further information and advanced usage, please refer to the comprehensive BenchLLM documentation. If you need any support, feel free to open an issue on our GitHub page.
+If you need any support, feel free to open an issue on our GitHub page.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `benchllm-0.1.0/benchllm/__init__.py` & `benchllm-0.2.0/benchllm/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 from pathlib import Path
-from typing import Any, Callable, Generic, Optional, Type, TypeVar
+from typing import Callable, Type, TypeVar
 
 from .data_types import Evaluation, Prediction, Test  # noqa
 from .evaluator import Evaluator, SemanticEvaluator, StringMatchEvaluator  # noqa
-from .input_types import ChatInput, SimilarityInput
+from .input_types import ChatInput, SimilarityInput  # noqa
 from .similarity import semantically_similar  # noqa
 from .singleton import TestSingleton  # noqa
 from .tester import Tester  # noqa
 
 T = TypeVar("T")
 
 __all__ = [
```

### Comparing `benchllm-0.1.0/benchllm/cli/commands/add_test.py` & `benchllm-0.2.0/benchllm/cli/commands/add_test.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.1.0/benchllm/cli/commands/evaluate.py` & `benchllm-0.2.0/benchllm/cli/commands/evaluate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from pathlib import Path
 
+from benchllm.cache import FileCache
 from benchllm.cli.listener import ReportListener, RichCliListener
-from benchllm.cli.utils import get_evaluator
-from benchllm.evaluator import load_prediction_files
-from benchllm.utils import find_json_yml_files
+from benchllm.cli.utils import add_cache, get_evaluator
+from benchllm.utils import find_json_yml_files, load_prediction_files
 
 
 def evaluate_predictions(
-    file_or_dir: list[Path], model: str, output_dir: Path, workers: int, evaluator_name: str
+    file_or_dir: list[Path], model: str, output_dir: Path, workers: int, evaluator_name: str, cache: str
 ) -> bool:
     files = find_json_yml_files(file_or_dir)
 
     cli_listener = RichCliListener(root_dir=Path.cwd(), interactive=evaluator_name == "interactive", eval_only=True)
     report_listener = ReportListener(output_dir=output_dir)
 
     load_prediction_files(file_or_dir)
 
     evaluator = get_evaluator(evaluator_name, model, workers)
+    evaluator = add_cache(cache, evaluator, output_dir.parent / "cache.json")
+
+    cli_listener.set_evaulator(evaluator)
+
     evaluator.add_listener(cli_listener)
     evaluator.add_listener(report_listener)
     for file in files:
         evaluator.load_prediction_file(file)
 
     evaluator.run()
     return not evaluator.failed
```

### Comparing `benchllm-0.1.0/benchllm/cli/commands/list_tests.py` & `benchllm-0.2.0/benchllm/cli/commands/list_tests.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.1.0/benchllm/cli/commands/run_suite.py` & `benchllm-0.2.0/benchllm/cli/commands/run_suite.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from pathlib import Path
 
 import typer
 
+from benchllm.cache import FileCache
 from benchllm.cli.listener import ReportListener, RichCliListener
-from benchllm.cli.utils import get_evaluator
+from benchllm.cli.utils import add_cache, get_evaluator
 from benchllm.tester import Tester
 from benchllm.utils import find_files
 
 
 def run_suite(
     *,
     file_search_paths: list[Path],
     model: str,
     output_dir: Path,
     no_eval: bool,
     workers: int,
     evaluator_name: str,
     retry_count: int,
+    cache: str,
 ) -> bool:
     files = find_files(file_search_paths)
     if not files:
         typer.secho(
             f"No python files with @benchllm.test found in {', '.join(map(str, file_search_paths))}",
             fg=typer.colors.RED,
             bold=True,
@@ -41,13 +43,17 @@
     # Finally, start collecting the predictions.
     tester.run()
 
     if no_eval:
         return True
 
     evaluator = get_evaluator(evaluator_name, model, workers)
+    evaluator = add_cache(cache, evaluator, output_dir.parent / "cache.json")
+
+    cli_listener.set_evaulator(evaluator)
+
     evaluator.add_listener(cli_listener)
     evaluator.add_listener(report_listener)
     evaluator.load(tester.predictions)
 
     evaluator.run()
     return not evaluator.failed
```

### Comparing `benchllm-0.1.0/benchllm/cli/listener.py` & `benchllm-0.2.0/benchllm/cli/listener.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import datetime
 import json
 from pathlib import Path
+from typing import Optional
 
 import typer
 from rich import print
 from rich.console import Console
 from rich.markup import render
 from rich.table import Table
 
+from benchllm.cache import MemoryCache
 from benchllm.data_types import Evaluation, FunctionID, Prediction, Test, TestFunction
+from benchllm.evaluator import Evaluator
 from benchllm.listener import EvaluatorListener, TesterListener
 
 
 class ReportListener(TesterListener, EvaluatorListener):
     def __init__(self, *, output_dir: Path) -> None:
         super().__init__()
         self.output_dir = output_dir
@@ -33,20 +36,31 @@
         path.parent.mkdir(parents=True, exist_ok=True)
 
         with open(path, "w") as f:
             json.dump(prediction_json, f, indent=2)
 
 
 class RichCliListener(TesterListener, EvaluatorListener):
-    def __init__(self, root_dir: Path, *, interactive: bool, test_only: bool = False, eval_only: bool = False) -> None:
+    def __init__(
+        self,
+        root_dir: Path,
+        *,
+        interactive: bool,
+        test_only: bool = False,
+        eval_only: bool = False,
+    ) -> None:
         super().__init__()
         self.root_dir = root_dir
         self.interactive = interactive
         self._eval_only = eval_only
         self._test_only = test_only
+        self._evaluator: Optional[Evaluator] = None
+
+    def set_evaulator(self, evaluator: Evaluator) -> None:
+        self._evaluator = evaluator
 
     def test_run_started(self) -> None:
         print_centered(" Run Tests ")
 
     def test_run_ended(self, predications: list[Prediction]) -> None:
         if not self._test_only:
             return
@@ -112,14 +126,17 @@
                 table.add_row(f"Input", str(prediction.test.input))
                 table.add_row(f"Output", f"[red]{prediction.output}[/red]")
                 for i, answer in enumerate(prediction.test.expected):
                     table.add_row(f"Expected #{i+1}", str(answer))
                 console.print(table)
 
         tmp = f" [red]{len(failed)} failed[/red], [green]{len(evaluations) - len(failed)} passed[/green], in [blue]{format_time(total_eval_time + total_test_time)}[/blue] "
+        if isinstance(self._evaluator, MemoryCache):
+            tmp += f"(cached hits {self._evaluator.num_cache_hits}, cached misses {self._evaluator.num_cache_misses}) "
+
         print_centered(tmp)
 
 
 def print_centered(text: str, sep: str = "=") -> None:
     console = Console()
     terminal_width = console.width
```

### Comparing `benchllm-0.1.0/benchllm/cli/main.py` & `benchllm-0.2.0/benchllm/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,26 +24,28 @@
         ),
     ] = None,
     model: Annotated[str, typer.Option(help="Model to use to run the evaluation.")] = "gpt-3",
     eval: Annotated[bool, typer.Option(help="Run final evaluation.")] = True,
     workers: Annotated[int, typer.Option(help="Number of workers to use to run the evaluation.")] = 1,
     retry_count: Annotated[int, typer.Option(help="Rerun tests to spot flaky output")] = 1,
     evaluator: Annotated[str, typer.Option(help="Evaluator to use to run the evaluation.")] = "semantic",
+    cache: Annotated[str, typer.Option(help="Type of cache to use.")] = "file",
 ) -> None:
     if not file_or_dir:
         file_or_dir = [Path.cwd()]
 
     success = run_suite(
         file_search_paths=file_or_dir,
         model=model,
         output_dir=output_dir,
         workers=workers,
         evaluator_name=evaluator,
         no_eval=not eval,
         retry_count=retry_count,
+        cache=cache,
     )
     if not success:
         raise typer.Exit(code=1)
 
 
 @app.command(help="Evaluate predictions")
 def eval(
@@ -57,21 +59,23 @@
     ],
     output_dir: Annotated[
         Path, typer.Option(help="Output directory to save evaluation reports into.", default_factory=output_dir_factory)
     ],
     model: Annotated[str, typer.Option(help="Model to use to run the evaluation.")] = "gpt-3",
     workers: Annotated[int, typer.Option(help="Number of workers to use to run the evaluation.")] = 1,
     evaluator: Annotated[str, typer.Option(help="Evaluator to use to run the evaluation.")] = "semantic",
+    cache: Annotated[str, typer.Option(help="Type of cache to use.")] = "file",
 ) -> None:
     success = evaluate_predictions(
         file_or_dir=file_or_dir,
         model=model,
         output_dir=output_dir,
         workers=workers,
         evaluator_name=evaluator,
+        cache=cache,
     )
     if not success:
         raise typer.Exit(code=1)
 
 
 @app.command(help="Add a new test case to a suite.")
 def add(
```

### Comparing `benchllm-0.1.0/benchllm/cli/utils.py` & `benchllm-0.2.0/benchllm/cli/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 from pathlib import Path
 
+from benchllm.cache import FileCache, MemoryCache
 from benchllm.cli.evaluator import InteractiveEvaluator, WebEvaluator
 from benchllm.evaluator import Evaluator, SemanticEvaluator, StringMatchEvaluator
 
 
 def output_dir_factory() -> Path:
     timestamp = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
     output_dir = Path.cwd() / "output" / str(timestamp)
@@ -24,7 +25,18 @@
         return InteractiveEvaluator()
     elif evaluator_name == "string-match":
         return StringMatchEvaluator(workers=workers)
     elif evaluator_name == "web":
         return WebEvaluator()
     else:
         raise ValueError(f"Unknown evaluator {evaluator_name}")
+
+
+def add_cache(cache_name: str, evaluator: Evaluator, cache_path: Path) -> Evaluator:
+    if cache_name == "file":
+        return FileCache(evaluator, cache_path)
+    elif cache_name == "memory":
+        return MemoryCache(evaluator)
+    elif cache_name == "none":
+        return evaluator
+    else:
+        raise ValueError(f"Unknown cache {cache_name}, valid values are 'file', 'memory', 'none'")
```

### Comparing `benchllm-0.1.0/benchllm/data_types.py` & `benchllm-0.2.0/benchllm/data_types.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.1.0/benchllm/listener.py` & `benchllm-0.2.0/benchllm/listener.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.1.0/benchllm/similarity.py` & `benchllm-0.2.0/benchllm/similarity.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,10 @@
     response = complete_text(
         f"""{{ 
         "answer_1": "{answer1}",
         "answer_2": "{answer2}"
     }}""",
         model=model,
     )
+    if response not in ["same", "different"]:
+        raise ValueError(f"Unexpected response: {response}")
     return response == "same"
```

### Comparing `benchllm-0.1.0/benchllm/singleton.py` & `benchllm-0.2.0/benchllm/singleton.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, Callable, Generic, Optional, Type, TypeVar
+from typing import Callable, Generic, Optional, Type, TypeVar
 
 T = TypeVar("T")
 
 
 class TestSingleton(Generic[T]):
     _instance = None
     func: Optional[Callable[[T], T]] = None
```

### Comparing `benchllm-0.1.0/benchllm/tester.py` & `benchllm-0.2.0/benchllm/tester.py`

 * *Files identical despite different names*

### Comparing `benchllm-0.1.0/benchllm/utils.py` & `benchllm-0.2.0/benchllm/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import ast
+import json
 from pathlib import Path
 
+import yaml
+
+from benchllm.data_types import Prediction
+
 
 class DecoratorFinder(ast.NodeVisitor):
     def __init__(self) -> None:
         self.has_decorator: bool = False
         self.module_aliases: list[str] = []
 
     def visit_Import(self, node: ast.Import) -> None:
@@ -55,7 +60,25 @@
             else:
                 continue
         else:
             for file in path.rglob("*"):
                 if file.suffix in (".yml", ".json", ".yaml"):
                     files.append(file)
     return list(set(files))
+
+
+def load_prediction_files(paths: list[Path]) -> list[Prediction]:
+    predictions = []
+    for path in paths:
+        for file_path in path.rglob("*"):
+            if not file_path.is_file():
+                continue
+            if file_path.suffix not in {".json", ".yml", ".yaml"}:
+                continue
+            with open(file_path, "r") as file:
+                if file_path.suffix == ".json":
+                    data = json.load(file)
+                    predictions.append(Prediction(**data))
+                elif file_path.suffix in {".yml", ".yaml"}:
+                    data = yaml.safe_load(file)
+                    predictions.append(Prediction(**data))
+    return predictions
```

### Comparing `benchllm-0.1.0/pyproject.toml` & `benchllm-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "benchllm"
-version = "0.1.0"
+version = "0.2.0"
 description = "Tool for testing LLMs"
 homepage = "https://github.com/v7labs/benchllm"
 authors = [ "Simon Edwardsson <simon@v7labs.com>", "Andrea Azzini <andrea@v7labs.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = []
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License",]
```

### Comparing `benchllm-0.1.0/setup.py` & `benchllm-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['benchllm', 'benchllm.cli', 'benchllm.cli.commands']
+['benchllm',
+ 'benchllm.cli',
+ 'benchllm.cli.commands',
+ 'benchllm.cli.evaluator',
+ 'benchllm.evaluator']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['openai', 'pydantic>=1.10.9,<2.0.0', 'pyyaml>=5.1', 'typer[all]']
 
@@ -16,17 +20,17 @@
  'test': ['pytest']}
 
 entry_points = \
 {'console_scripts': ['bench = benchllm.cli.main:main']}
 
 setup_kwargs = {
     'name': 'benchllm',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'Tool for testing LLMs',
-    'long_description': '# BenchLLM\n\nBenchLLM is a Python-based open-source library that streamlines the testing process for Large Language Models (LLMs) and AI-powered applications. It offers an intuitive and robust way to validate and score the output of your code with minimal boilerplate or configuration.\n\nBenchLLM is actively used at [V7](https://www.v7labs.com) for improving our LLM applications and now Open Sourced under MIT License to share with the wider community\n\nUse BenchLLM to:\n\n- Easily set up a comprehensive testing suite for your LLMs.\n- Continous integration for your langchain/agents/models.\n- Elimiate flaky chains and create confidence in your code.\n\n> **NOTE:** BenchLLM is in the early stage of development and will be subject to rapid changes.\n\nFor bug reporting, feature requests, or contributions, please open an issue or submit a pull request (PR) on our GitHub page.\n\n## BenchLLM Testing Methodology\n\nBenchLLM implements a distinct two-step methodology for validating your machine learning models:\n\n1. **Testing**: This stage involves running your code against various tests and capturing the predictions produced by your model without immediate judgment or comparison.\n\n2. **Evaluation**: During this phase, the recorded predictions are compared against the expected output. Detailed comparison reports, including pass/fail status and other metrics, are generated.\n\nThis methodical separation offers a comprehensive view of your model\'s performance and allows for better control and refinement of each step.\n\n## Install\n\nTo install BenchLLM we use pip\n\n```\npip install git+https://github.com/v7labs/benchllm\n```\n\n## Usage\n\nStart by importing the library and use the @benchllm.test decorator to mark the function you\'d like to test:\n\n```python\nimport benchllm\n\n# Your custom model implementation\ndef run_my_model(input):\n    # Your model\'s logic goes here.\n    return some_result\n\n@benchllm.test(suite="/path/to/test/suite") # If the tests are in the same directory, just use @benchllm.test.\ndef invoke_model(input: str):\n    return run_my_model(input)\n```\n\nNext, prepare your tests. These are YAML/JSON files structured as follows:\n\n```yml\ninput: What\'s 1+1? Be very terse, only numeric output\nexpected:\n  - 2\n  - 2.0\n```\n\nIn the above example, the `input` is the query or instruction that your model will process, and `expected` contains the potential responses that your model should return. It\'s important to note that `input` can be a simple `str` or a more complex nested dictionary; BenchLLM will extract the type of the `input` argument in the Python code and load the `input` field from the YAML file accordingly.\n\nBy default, BenchLLM uses OpenAI\'s GPT-3 model for the `semantic` evaluator. This requires setting the `OPENAI_API_KEY` environment variable. If you do not want to use this default evaluator, you can specify an alternative one (discussed in further detail below):\n\n```bash\nexport OPENAI_API_KEY=\'your-api-key\'\n```\n\nReplace \'your-api-key\' with your actual OpenAI API key.\n\nTo initiate testing, use the `bench run` command:\n\n```bash\n$ bench run\n```\n\nBy default, the bench run command looks for Python files implementing the @test decorator in the current directory. To target a specific file or folder, specify it directly:\n\n```bash\n$ bench run path/to/my/file.py or/path/to/folder/with/files\n```\n\nThe `--retry-count` parameter allows BenchLLM to run a test multiple times, useful for models that may have variability in their outputs:\n\n```bash\n$ bench run --retry-count 5\n```\n\nBenchLLM offers multiple evaluation methods to determine if the prediction matches the test case\'s expected values. You can use the `--evaluator` parameter to specify the evaluation method:\n\nThere are multiple ways to evaluate if the test functions prediction matches the test cases expected values.\nBy default GPT-3 is used to compare the output. You can use `--evaluator` to use a different method\n\n- `semantic`, checks semantic similarity using language models like GPT-3, GPT-3.5, or GPT-4 (`--model` parameter). Please note, for this evaluator, you need to set the `OPENAI_API_KEY` environment variable.\n- `string-match`, checks if the strings are matching (case insensitive)\n- `interactive`, user manually accepts or fails tests in the terminal\n- `web`, uses pywebio fora simple local web interface\n\nThe non interactive evaluators also supports `--workers N` to run in the evaluations in parallel\n\n```bash\n$ bench run --evaluator string-match --workers 5\n```\n\n### Eval\n\nWhile bench run runs each test function and then evaluates their output, it can often be beneficial to separate these into two steps. For example, if you want a person to manually do the evaluation or if you want to try multiple evaluation methods on the same function.\n\n```bash\n$ bench run --no-eval\n```\n\nThis will generate json files in `output/latest/predictions`\nThen later you can evaluate them with\n\n```bash\n$ bench eval output/latest/predictions\n```\n\n## API\n\nFor more detailed control, BenchLLM provides an API.\nYou are not required to add YML/JSON tests to be able to evaluate your model.\nYou can instead:\n\n- Instantiate `Test` objects\n- Use a `Tester` object to generate predictions\n- Use an `Evaluator` object to evaluate your model\n\n```python\nfrom benchllm import StringMatchEvaluator, Test, Tester\n\n# Instantiate your Test objects\ntests = [\n    Test(input="What\'s 1+1?", expected=["2", "It\'s 2"]),\n    Test(input="First rule of fight club?", expected=["Do not talk about fight club"]),\n]\n\n# Use a Tester object to generate predictions using any test functions\ntester = Tester(my_test_function)\ntester.add_tests(tests)\npredictions = tester.run()\n\n# Use an Evaluator object to evaluate your model\nevaluator = StringMatchEvaluator()\nevaluator.load(predictions)\nresults = evaluator.run()\n\nprint(results)\n```\n\n## Commands\n\n- `bench add`: Add a new test to a suite.\n- `bench tests`: List all tests in a suite.\n- `bench run`: Run all or target test suites.\n- `bench eval`: Runs the evaluation of an existing test run.\n\n## Contribute\n\nBenchLLM is developed for Python 3.10, although it may work with other Python versions as well. We recommend using a Python 3.10 environment. You can use conda or any other environment manager to set up the environment:\n\n```bash\n$ conda create --name benchllm python=3.10\n$ conda activate benchllm\n$ pip install -e ".[dev]"\n```\n\nTo run all the examples first install the examples extra dependencies\n\n```bash\n$ pip install -e ".[examples]"\n```\n\nContribution steps:\n\n1. Fork the repository.\n2. Create a new branch for your changes.\n3. Make your changes.\n4. Test your changes.\n5. Submit a pull request.\n\nWe adhere to PEP8 style guide. Please follow this guide when contributing.\n\nFor further information and advanced usage, please refer to the comprehensive BenchLLM documentation. If you need any support, feel free to open an issue on our GitHub page.\n',
+    'long_description': '# 🏋️\u200d♂️ BenchLLM 🏋️\u200d♀️\n\n🦾 Continuous Integration for LLM powered applications 🦙🦅🤖\n\n[![GitHub Repo stars](https://img.shields.io/github/stars/v7labs/BenchLLM?style=social)](https://github.com/v7labs/BenchLLM/stargazers)\n[![Twitter Follow](https://img.shields.io/twitter/follow/V7Labs?style=social)](https://twitter.com/V7Labs)\n[![Discord Follow](https://dcbadge.vercel.app/api/server/x7ExfHb3bG?style=flat)](https://discord.gg/x7ExfHb3bG)\n\n[**BenchLLM**](https://benchllm.com/) is a Python-based open-source library that streamlines the testing of Large Language Models (LLMs) and AI-powered applications. It measures the accuracy of your model, agents, or chains by validating responses on any number of tests via LLMs.\n\nBenchLLM is actively used at [V7](https://www.v7labs.com) for improving our LLM applications and is now Open Sourced under MIT License to share with the wider community\n\n## 💡 Get help on [Discord](https://discord.gg/x7ExfHb3bG) or [Tweet at us](https://twitter.com/V7Labs)\n\n<hr/>\n\nUse BenchLLM to:\n\n- Test the responses of your LLM across any number of prompts.\n- Continuous integration for chains like [Langchain](https://github.com/hwchase17/langchain), agents like [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT), or LLM models like [Llama](https://github.com/facebookresearch/llama) or GPT-4.\n- Eliminate flaky chains and create confidence in your code.\n- Spot inaccurate responses and hallucinations in your application at every version.\n\n<hr/>\n\n> ⚠️ **NOTE:** BenchLLM is in the early stage of development and will be subject to rapid changes.\n>\n> For bug reporting, feature requests, or contributions, please open an issue or submit a pull request (PR) on our GitHub page.\n\n## 🧪 BenchLLM Testing Methodology\n\nBenchLLM implements a distinct two-step methodology for validating your machine learning models:\n\n1. **Testing**: This stage involves running your code against any number of expected responses and capturing the predictions produced by your model without immediate judgment or comparison.\n\n2. **Evaluation**: The recorded predictions are compared against the expected output using LLMs to verify factual similarity (or optionally manually). Detailed comparison reports, including pass/fail status and other metrics, are generated.\n\nThis methodical separation offers a comprehensive view of your model\'s performance and allows for better control and refinement of each step.\n\n## 🚀 Install\n\nTo install BenchLLM we use pip\n\n```\npip install benchllm\n```\n\n## 💻 Usage\n\nStart by importing the library and use the @benchllm.test decorator to mark the function you\'d like to test:\n\n```python\nimport benchllm\n\n# Your custom model implementation\ndef run_my_model(input):\n    # Your model\'s logic goes here.\n    return some_result\n\n@benchllm.test(suite="/path/to/test/suite") # If the tests are in the same directory, just use @benchllm.test.\ndef invoke_model(input: str):\n    return run_my_model(input)\n```\n\nNext, prepare your tests. These are YAML/JSON files structured as follows:\n\n```yml\ninput: What\'s 1+1? Be very terse, only numeric output\nexpected:\n  - 2\n  - 2.0\n```\n\nIn the above example, the `input` is the query or instruction that your model will process, and `expected` contains the potential responses that your model should return. It\'s important to note that `input` can be a simple `str` or a more complex nested dictionary; BenchLLM will extract the type of the `input` argument in the Python code and load the `input` field from the YAML file accordingly.\n\nBy default, BenchLLM uses OpenAI\'s GPT-3 model for the `semantic` evaluator. This requires setting the `OPENAI_API_KEY` environment variable. If you do not want to use this default evaluator, you can specify an alternative one (discussed in further detail below):\n\n```bash\nexport OPENAI_API_KEY=\'your-api-key\'\n```\n\nReplace \'your-api-key\' with your actual OpenAI API key.\n\nTo initiate testing, use the `bench run` command:\n\n```bash\n$ bench run\n```\n\nBy default, the bench run command looks for Python files implementing the @test decorator in the current directory. To target a specific file or folder, specify it directly:\n\n```bash\n$ bench run path/to/my/file.py or/path/to/folder/with/files\n```\n\nThe `--retry-count` parameter allows BenchLLM to run a test multiple times, useful for models that may have variability in their outputs:\n\n```bash\n$ bench run --retry-count 5\n```\n\nBenchLLM offers multiple evaluation methods to determine if the prediction matches the test case\'s expected values. You can use the `--evaluator` parameter to specify the evaluation method:\n\nThere are multiple ways to evaluate if the test functions prediction matches the test cases expected values.\nBy default GPT-3 is used to compare the output. You can use `--evaluator` to use a different method\n\n- `semantic`, checks semantic similarity using language models like GPT-3, GPT-3.5, or GPT-4 (`--model` parameter). Please note, for this evaluator, you need to set the `OPENAI_API_KEY` environment variable.\n- `string-match`, checks if the strings are matching (case insensitive)\n- `interactive`, user manually accepts or fails tests in the terminal\n- `web`, uses pywebio fora simple local web interface\n\nThe non interactive evaluators also supports `--workers N` to run in the evaluations in parallel\n\n```bash\n$ bench run --evaluator string-match --workers 5\n```\n\nTo accelerate the evaluation process, BenchLLM uses a cache. If a (prediction, expected) pair has been evaluated in the past and a cache was used, the evaluation output will be saved for future evaluations. There are several types of caches:\n\n- `memory`, only caches output values during the current run. This is particularly useful when running with `--retry-count N`\n- `file`, stores the cache at the end of the run as a JSON file in output/cache.json. This is the default behavior.\n- `none`, does not use any cache.\n\n```bash\n$ bench run examples --cache memory\n```\n\n### 🧮 Eval\n\nWhile _bench run_ runs each test function and then evaluates their output, it can often be beneficial to separate these into two steps. For example, if you want a person to manually do the evaluation or if you want to try multiple evaluation methods on the same function.\n\n```bash\n$ bench run --no-eval\n```\n\nThis will generate json files in `output/latest/predictions`\nThen later you can evaluate them with\n\n```bash\n$ bench eval output/latest/predictions\n```\n\n## 🔌 API\n\nFor more detailed control, BenchLLM provides an API.\nYou are not required to add YML/JSON tests to be able to evaluate your model.\nYou can instead:\n\n- Instantiate `Test` objects\n- Use a `Tester` object to generate predictions\n- Use an `Evaluator` object to evaluate your model\n\n```python\nfrom benchllm import StringMatchEvaluator, Test, Tester\n\n# Instantiate your Test objects\ntests = [\n    Test(input="What\'s 1+1?", expected=["2", "It\'s 2"]),\n    Test(input="First rule of fight club?", expected=["Do not talk about fight club"]),\n]\n\n# Use a Tester object to generate predictions using any test functions\ntester = Tester(my_test_function)\ntester.add_tests(tests)\npredictions = tester.run()\n\n# Use an Evaluator object to evaluate your model\nevaluator = StringMatchEvaluator()\nevaluator.load(predictions)\nresults = evaluator.run()\n\nprint(results)\n```\n\nIf you want to incorporate caching and run multiple parallel evaluation jobs, you can modify your evaluator as follows:\n\n```python\nfrom benchllm.cache import FileCache\n\n...\n\nevaluator = FileCache(StringMatchEvaluator(workers=2), Path("path/to/cache.json"))\nevaluator.load(predictions)\nresults = evaluator.run()\n```\n\nIn this example, `FileCache` is used to enable caching, and the `workers` parameter of `StringMatchEvaluator` is set to `2` to allow for parallel evaluations. The cache results are saved in a file specified by `Path("path/to/cache.json")`.\n\n## ☕️ Commands\n\n- `bench add`: Add a new test to a suite.\n- `bench tests`: List all tests in a suite.\n- `bench run`: Run all or target test suites.\n- `bench eval`: Runs the evaluation of an existing test run.\n\n## 🙌 Contribute\n\nBenchLLM is developed for Python 3.10, although it may work with other Python versions as well. We recommend using a Python 3.10 environment and pip >= 23. You can use conda or any other environment manager to set up the environment:\n\n```bash\n$ conda create --name benchllm python=3.10\n$ conda activate benchllm\n$ pip install -e ".[dev]"\n```\n\nTo run all the examples first install the examples extra dependencies\n\n```bash\n$ pip install -e ".[examples]"\n```\n\nContribution steps:\n\n1. Fork the repository.\n2. Create a new branch for your changes.\n3. Make your changes.\n4. Test your changes.\n5. Submit a pull request.\n\nWe adhere to the PEP8 style guide. Please follow this guide when contributing.\n\nIf you need any support, feel free to open an issue on our GitHub page.\n',
     'author': 'Simon Edwardsson',
     'author_email': 'simon@v7labs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/v7labs/benchllm',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `benchllm-0.1.0/PKG-INFO` & `benchllm-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchllm
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tool for testing LLMs
 Home-page: https://github.com/v7labs/benchllm
 License: MIT
 Author: Simon Edwardsson
 Author-email: simon@v7labs.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -24,49 +24,62 @@
 Requires-Dist: pywebio
 Requires-Dist: pyyaml (>=5.1)
 Requires-Dist: tiktoken ; extra == "examples"
 Requires-Dist: typer[all]
 Requires-Dist: types-pyyaml ; extra == "dev"
 Description-Content-Type: text/markdown
 
-# BenchLLM
+# 🏋️‍♂️ BenchLLM 🏋️‍♀️
 
-BenchLLM is a Python-based open-source library that streamlines the testing process for Large Language Models (LLMs) and AI-powered applications. It offers an intuitive and robust way to validate and score the output of your code with minimal boilerplate or configuration.
+🦾 Continuous Integration for LLM powered applications 🦙🦅🤖
 
-BenchLLM is actively used at [V7](https://www.v7labs.com) for improving our LLM applications and now Open Sourced under MIT License to share with the wider community
+[![GitHub Repo stars](https://img.shields.io/github/stars/v7labs/BenchLLM?style=social)](https://github.com/v7labs/BenchLLM/stargazers)
+[![Twitter Follow](https://img.shields.io/twitter/follow/V7Labs?style=social)](https://twitter.com/V7Labs)
+[![Discord Follow](https://dcbadge.vercel.app/api/server/x7ExfHb3bG?style=flat)](https://discord.gg/x7ExfHb3bG)
 
-Use BenchLLM to:
+[**BenchLLM**](https://benchllm.com/) is a Python-based open-source library that streamlines the testing of Large Language Models (LLMs) and AI-powered applications. It measures the accuracy of your model, agents, or chains by validating responses on any number of tests via LLMs.
+
+BenchLLM is actively used at [V7](https://www.v7labs.com) for improving our LLM applications and is now Open Sourced under MIT License to share with the wider community
 
-- Easily set up a comprehensive testing suite for your LLMs.
-- Continous integration for your langchain/agents/models.
-- Elimiate flaky chains and create confidence in your code.
+## 💡 Get help on [Discord](https://discord.gg/x7ExfHb3bG) or [Tweet at us](https://twitter.com/V7Labs)
 
-> **NOTE:** BenchLLM is in the early stage of development and will be subject to rapid changes.
+<hr/>
 
-For bug reporting, feature requests, or contributions, please open an issue or submit a pull request (PR) on our GitHub page.
+Use BenchLLM to:
 
-## BenchLLM Testing Methodology
+- Test the responses of your LLM across any number of prompts.
+- Continuous integration for chains like [Langchain](https://github.com/hwchase17/langchain), agents like [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT), or LLM models like [Llama](https://github.com/facebookresearch/llama) or GPT-4.
+- Eliminate flaky chains and create confidence in your code.
+- Spot inaccurate responses and hallucinations in your application at every version.
+
+<hr/>
+
+> ⚠️ **NOTE:** BenchLLM is in the early stage of development and will be subject to rapid changes.
+>
+> For bug reporting, feature requests, or contributions, please open an issue or submit a pull request (PR) on our GitHub page.
+
+## 🧪 BenchLLM Testing Methodology
 
 BenchLLM implements a distinct two-step methodology for validating your machine learning models:
 
-1. **Testing**: This stage involves running your code against various tests and capturing the predictions produced by your model without immediate judgment or comparison.
+1. **Testing**: This stage involves running your code against any number of expected responses and capturing the predictions produced by your model without immediate judgment or comparison.
 
-2. **Evaluation**: During this phase, the recorded predictions are compared against the expected output. Detailed comparison reports, including pass/fail status and other metrics, are generated.
+2. **Evaluation**: The recorded predictions are compared against the expected output using LLMs to verify factual similarity (or optionally manually). Detailed comparison reports, including pass/fail status and other metrics, are generated.
 
 This methodical separation offers a comprehensive view of your model's performance and allows for better control and refinement of each step.
 
-## Install
+## 🚀 Install
 
 To install BenchLLM we use pip
 
 ```
-pip install git+https://github.com/v7labs/benchllm
+pip install benchllm
 ```
 
-## Usage
+## 💻 Usage
 
 Start by importing the library and use the @benchllm.test decorator to mark the function you'd like to test:
 
 ```python
 import benchllm
 
 # Your custom model implementation
@@ -128,30 +141,40 @@
 
 The non interactive evaluators also supports `--workers N` to run in the evaluations in parallel
 
 ```bash
 $ bench run --evaluator string-match --workers 5
 ```
 
-### Eval
+To accelerate the evaluation process, BenchLLM uses a cache. If a (prediction, expected) pair has been evaluated in the past and a cache was used, the evaluation output will be saved for future evaluations. There are several types of caches:
+
+- `memory`, only caches output values during the current run. This is particularly useful when running with `--retry-count N`
+- `file`, stores the cache at the end of the run as a JSON file in output/cache.json. This is the default behavior.
+- `none`, does not use any cache.
+
+```bash
+$ bench run examples --cache memory
+```
+
+### 🧮 Eval
 
-While bench run runs each test function and then evaluates their output, it can often be beneficial to separate these into two steps. For example, if you want a person to manually do the evaluation or if you want to try multiple evaluation methods on the same function.
+While _bench run_ runs each test function and then evaluates their output, it can often be beneficial to separate these into two steps. For example, if you want a person to manually do the evaluation or if you want to try multiple evaluation methods on the same function.
 
 ```bash
 $ bench run --no-eval
 ```
 
 This will generate json files in `output/latest/predictions`
 Then later you can evaluate them with
 
 ```bash
 $ bench eval output/latest/predictions
 ```
 
-## API
+## 🔌 API
 
 For more detailed control, BenchLLM provides an API.
 You are not required to add YML/JSON tests to be able to evaluate your model.
 You can instead:
 
 - Instantiate `Test` objects
 - Use a `Tester` object to generate predictions
@@ -175,24 +198,38 @@
 evaluator = StringMatchEvaluator()
 evaluator.load(predictions)
 results = evaluator.run()
 
 print(results)
 ```
 
-## Commands
+If you want to incorporate caching and run multiple parallel evaluation jobs, you can modify your evaluator as follows:
+
+```python
+from benchllm.cache import FileCache
+
+...
+
+evaluator = FileCache(StringMatchEvaluator(workers=2), Path("path/to/cache.json"))
+evaluator.load(predictions)
+results = evaluator.run()
+```
+
+In this example, `FileCache` is used to enable caching, and the `workers` parameter of `StringMatchEvaluator` is set to `2` to allow for parallel evaluations. The cache results are saved in a file specified by `Path("path/to/cache.json")`.
+
+## ☕️ Commands
 
 - `bench add`: Add a new test to a suite.
 - `bench tests`: List all tests in a suite.
 - `bench run`: Run all or target test suites.
 - `bench eval`: Runs the evaluation of an existing test run.
 
-## Contribute
+## 🙌 Contribute
 
-BenchLLM is developed for Python 3.10, although it may work with other Python versions as well. We recommend using a Python 3.10 environment. You can use conda or any other environment manager to set up the environment:
+BenchLLM is developed for Python 3.10, although it may work with other Python versions as well. We recommend using a Python 3.10 environment and pip >= 23. You can use conda or any other environment manager to set up the environment:
 
 ```bash
 $ conda create --name benchllm python=3.10
 $ conda activate benchllm
 $ pip install -e ".[dev]"
 ```
 
@@ -206,11 +243,11 @@
 
 1. Fork the repository.
 2. Create a new branch for your changes.
 3. Make your changes.
 4. Test your changes.
 5. Submit a pull request.
 
-We adhere to PEP8 style guide. Please follow this guide when contributing.
+We adhere to the PEP8 style guide. Please follow this guide when contributing.
 
-For further information and advanced usage, please refer to the comprehensive BenchLLM documentation. If you need any support, feel free to open an issue on our GitHub page.
+If you need any support, feel free to open an issue on our GitHub page.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

