# Comparing `tmp/uniem-0.3.0.tar.gz` & `tmp/uniem-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniem-0.3.0.tar", max compression
+gzip compressed data, was "uniem-0.3.1.tar", max compression
```

## Comparing `uniem-0.3.0.tar` & `uniem-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-07-11 11:08:20.264987 uniem-0.3.0/LICENSE
--rw-r--r--   0        0        0     6213 2023-07-11 11:08:20.264987 uniem-0.3.0/README.md
--rw-r--r--   0        0        0      813 2023-07-11 11:08:20.276987 uniem-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       92 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/__init__.py
--rw-r--r--   0        0        0     7166 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/criteria.py
--rw-r--r--   0        0        0    12450 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/data.py
--rw-r--r--   0        0        0     1109 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/data_structures.py
--rw-r--r--   0        0        0    14276 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/finetuner.py
--rw-r--r--   0        0        0        0 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/integration/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/integration/sentence_transformers_wrapper.py
--rw-r--r--   0        0        0    13360 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/model.py
--rw-r--r--   0        0        0     6331 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/trainer.py
--rw-r--r--   0        0        0     3678 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/training_strategy.py
--rw-r--r--   0        0        0      658 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/types.py
--rw-r--r--   0        0        0     6193 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/utils.py
--rw-r--r--   0        0        0       22 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/version.py
--rw-r--r--   0        0        0     6848 1970-01-01 00:00:00.000000 uniem-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-13 03:55:28.481386 uniem-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6369 2023-07-13 03:55:28.481386 uniem-0.3.1/README.md
+-rw-r--r--   0        0        0      813 2023-07-13 03:55:28.489386 uniem-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       92 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/__init__.py
+-rw-r--r--   0        0        0     7166 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/criteria.py
+-rw-r--r--   0        0        0    12450 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/data.py
+-rw-r--r--   0        0        0     1109 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/data_structures.py
+-rw-r--r--   0        0        0    14419 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/finetuner.py
+-rw-r--r--   0        0        0        0 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/integration/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/integration/sentence_transformers_wrapper.py
+-rw-r--r--   0        0        0    13360 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/model.py
+-rw-r--r--   0        0        0     6478 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/trainer.py
+-rw-r--r--   0        0        0     3678 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/training_strategy.py
+-rw-r--r--   0        0        0      658 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/types.py
+-rw-r--r--   0        0        0     6193 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/utils.py
+-rw-r--r--   0        0        0       22 2023-07-13 03:55:28.581388 uniem-0.3.1/uniem/version.py
+-rw-r--r--   0        0        0     7004 1970-01-01 00:00:00.000000 uniem-0.3.1/PKG-INFO
```

### Comparing `uniem-0.3.0/LICENSE` & `uniem-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uniem-0.3.0/README.md` & `uniem-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,30 @@
 ```python
 from datasets import load_dataset
 
 from uniem.finetuner import FineTuner
 
 dataset = load_dataset('shibing624/nli_zh', 'STS-B')
 # 指定训练的模型为 m3e-small
-finetuner = FineTuner('moka-ai/m3e-small', dataset=dataset)
-finetuner.run(epochs=1)
+finetuner = FineTuner.from_pretrained('moka-ai/m3e-small', dataset=dataset)
+finetuner.run(epochs=3)
 ```
 
-微调的模型详见 [uniem 微调教程](https://github.com/wangyuxinwhy/uniem/blob/main/examples/finetune.ipynb) or <a target="_blank" href="https://colab.research.google.com/github/wangyuxinwhy/uniem/blob/main/examples/finetune.ipynb">
+微调模型详见 [uniem 微调教程](https://github.com/wangyuxinwhy/uniem/blob/main/examples/finetune.ipynb) or <a target="_blank" href="https://colab.research.google.com/github/wangyuxinwhy/uniem/blob/main/examples/finetune.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
+
+如果您想要在本地运行，您需要运行如下命令，准备环境
+
+```bash
+conda create -n uniem python=3.10
+pip install uniem
+```
+
 ## 💯 MTEB-zh
 
 中文 Embedding 模型缺少统一的评测标准，所以我们参考了 [MTEB](https://huggingface.co/spaces/mteb/leaderboard) ，构建了中文评测标准 MTEB-zh，目前已经对 6 种模型在各种数据集上进行了横评，详细的评测方式和代码请参考 [MTEB-zh](https://github.com/wangyuxinwhy/uniem/tree/main/mteb-zh) 。
 
 
 ### 文本分类
```

### Comparing `uniem-0.3.0/pyproject.toml` & `uniem-0.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniem"
-version = "0.3.0"
+version = "0.3.1"
 description = "unified embedding model"
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `uniem-0.3.0/uniem/criteria.py` & `uniem-0.3.1/uniem/criteria.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.0/uniem/data.py` & `uniem-0.3.1/uniem/data.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.0/uniem/data_structures.py` & `uniem-0.3.1/uniem/data_structures.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.0/uniem/finetuner.py` & `uniem-0.3.1/uniem/finetuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 from enum import Enum
 from pathlib import Path
-from typing import Iterable, Sequence, Sized, cast
+from typing import Callable, Iterable, Sequence, Sized, cast
 
 import torch
 from accelerate import Accelerator
 from accelerate.tracking import GeneralTracker
 from accelerate.utils import LoggerType, ProjectConfiguration, set_seed
 from datasets import Dataset as HFDataset
 from datasets import IterableDataset as HFIterableDataset
@@ -230,23 +230,24 @@
         weight_decay: float = 1e-3,
         num_warmup_steps: float | None = None,
         # Data
         batch_size: int = 256,
         max_length: int = 512,
         drop_last: bool = False,
         shuffle: bool = False,
+        num_workers: int = 0,
         # Trainer
         epochs: int = 3,
         mixed_precision: MixedPrecisionType = MixedPrecisionType.no,
         gradient_accumulation_steps: int = 1,
         save_on_epoch_end: bool = False,
         num_max_checkpoints: int = 1,
         log_with: str | LoggerType | GeneralTracker | list[str | LoggerType | GeneralTracker] | None = None,
-        num_workers: int = 0,
         seed: int = 42,
+        epoch_end_callbacks: Sequence[Callable[[Trainer], None]] | None = None,
         output_dir: Path | str | None = None,
     ):
 
         os.environ.setdefault('TRANSFORMERS_NO_ADVISORY_WARNINGS', '1')
         if num_workers >= 1:
             os.environ.setdefault('TOKENIZERS_PARALLELISM', 'false')
 
@@ -321,14 +322,15 @@
             train_dataloader=train_dataloader,
             validation_dataloader=validation_dataloader,
             accelerator=accelerator,
             epochs=epochs,
             lr_scheduler=lr_scheduler,
             log_interval=10,
             save_on_epoch_end=save_on_epoch_end,
+            epoch_end_callbacks=epoch_end_callbacks,
         )
         accelerator.print(f'Start training for {epochs} epochs')
         trainer.train()
 
         accelerator.wait_for_everyone()
         accelerator.print('Training finished')
```

### Comparing `uniem-0.3.0/uniem/integration/sentence_transformers_wrapper.py` & `uniem-0.3.1/uniem/integration/sentence_transformers_wrapper.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.0/uniem/model.py` & `uniem-0.3.1/uniem/model.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.0/uniem/trainer.py` & `uniem-0.3.1/uniem/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from __future__ import annotations
 
-from typing import Any, Sized
+from typing import Any, Callable, Sequence, Sized
 
 import torch
 from accelerate import Accelerator
 from torch.optim import Optimizer
-from torch.optim.lr_scheduler import LRScheduler
 from torch.utils.data import DataLoader
 from tqdm.auto import tqdm
 
+try:
+    from torch.optim.lr_scheduler import LRScheduler
+except ImportError:
+    from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
+
 
 class Trainer:
     def __init__(
         self,
         *,
         model: torch.nn.Module,
         train_dataloader: DataLoader,
         optimizer: Optimizer,
         accelerator: Accelerator,
         validation_dataloader: DataLoader | None = None,
         epochs: int = 3,
         lr_scheduler: LRScheduler | None = None,
         log_interval: int = 50,
         save_on_epoch_end: bool = True,
-        epoch_end_callbacks: list[Any] | None = None,
+        epoch_end_callbacks: Sequence[Callable[['Trainer'], None]] | None = None,
     ):
         self.model = model
         self.optimizer = optimizer
         self.train_dataloader = train_dataloader
         self.validation_dataloader = validation_dataloader
         self.lr_scheduler = lr_scheduler
         self.accelerator = accelerator
```

### Comparing `uniem-0.3.0/uniem/training_strategy.py` & `uniem-0.3.1/uniem/training_strategy.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.0/uniem/types.py` & `uniem-0.3.1/uniem/types.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.0/uniem/utils.py` & `uniem-0.3.1/uniem/utils.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.0/PKG-INFO` & `uniem-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniem
-Version: 0.3.0
+Version: 0.3.1
 Summary: unified embedding model
 License: MIT
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -60,22 +60,30 @@
 ```python
 from datasets import load_dataset
 
 from uniem.finetuner import FineTuner
 
 dataset = load_dataset('shibing624/nli_zh', 'STS-B')
 # 指定训练的模型为 m3e-small
-finetuner = FineTuner('moka-ai/m3e-small', dataset=dataset)
-finetuner.run(epochs=1)
+finetuner = FineTuner.from_pretrained('moka-ai/m3e-small', dataset=dataset)
+finetuner.run(epochs=3)
 ```
 
-微调的模型详见 [uniem 微调教程](https://github.com/wangyuxinwhy/uniem/blob/main/examples/finetune.ipynb) or <a target="_blank" href="https://colab.research.google.com/github/wangyuxinwhy/uniem/blob/main/examples/finetune.ipynb">
+微调模型详见 [uniem 微调教程](https://github.com/wangyuxinwhy/uniem/blob/main/examples/finetune.ipynb) or <a target="_blank" href="https://colab.research.google.com/github/wangyuxinwhy/uniem/blob/main/examples/finetune.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
+
+如果您想要在本地运行，您需要运行如下命令，准备环境
+
+```bash
+conda create -n uniem python=3.10
+pip install uniem
+```
+
 ## 💯 MTEB-zh
 
 中文 Embedding 模型缺少统一的评测标准，所以我们参考了 [MTEB](https://huggingface.co/spaces/mteb/leaderboard) ，构建了中文评测标准 MTEB-zh，目前已经对 6 种模型在各种数据集上进行了横评，详细的评测方式和代码请参考 [MTEB-zh](https://github.com/wangyuxinwhy/uniem/tree/main/mteb-zh) 。
 
 
 ### 文本分类
```

