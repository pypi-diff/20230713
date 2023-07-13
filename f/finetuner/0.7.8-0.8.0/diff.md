# Comparing `tmp/finetuner-0.7.8.tar.gz` & `tmp/finetuner-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetuner-0.7.8.tar", last modified: Thu Jun  8 13:51:59 2023, max compression
+gzip compressed data, was "finetuner-0.8.0.tar", last modified: Thu Jul 13 13:59:27 2023, max compression
```

## Comparing `finetuner-0.7.8.tar` & `finetuner-0.8.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:51:59.280786 finetuner-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-06-08 13:51:50.000000 finetuner-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 13:51:50.000000 finetuner-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-08 13:51:59.280786 finetuner-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-06-08 13:51:50.000000 finetuner-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:51:59.280786 finetuner-0.7.8/finetuner/
--rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:51:59.280786 finetuner-0.7.8/finetuner/client/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/excepts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/finetuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:51:59.280786 finetuner-0.7.8/finetuner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-08 13:51:58.000000 finetuner-0.7.8/finetuner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-08 13:51:59.000000 finetuner-0.7.8/finetuner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:51:58.000000 finetuner-0.7.8/finetuner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:51:58.000000 finetuner-0.7.8/finetuner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 13:51:58.000000 finetuner-0.7.8/finetuner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 13:51:58.000000 finetuner-0.7.8/finetuner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-08 13:51:50.000000 finetuner-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 13:51:59.280786 finetuner-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-08 13:51:50.000000 finetuner-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:59:27.600880 finetuner-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-07-13 13:59:18.000000 finetuner-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 13:59:18.000000 finetuner-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-07-13 13:59:27.600880 finetuner-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-13 13:59:18.000000 finetuner-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:59:27.600880 finetuner-0.8.0/finetuner/
+-rw-r--r--   0 runner    (1001) docker     (123)    28180 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:59:27.600880 finetuner-0.8.0/finetuner/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/excepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/finetuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-13 13:59:18.000000 finetuner-0.8.0/finetuner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:59:27.600880 finetuner-0.8.0/finetuner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 13:59:27.000000 finetuner-0.8.0/finetuner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 13:59:18.000000 finetuner-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 13:59:27.600880 finetuner-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-13 13:59:18.000000 finetuner-0.8.0/setup.py
```

### Comparing `finetuner-0.7.8/LICENSE` & `finetuner-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/PKG-INFO` & `finetuner-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.7.8
+Version: 0.8.0
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
@@ -157,17 +157,15 @@
         
         Make sure you have Python 3.8+ installed. Finetuner can be installed via `pip` by executing:
         
         ```bash
         pip install -U finetuner
         ```
         
-        If you want to encode local data with the `finetuner.encode` function, you need to install 
-        `"finetuner[full]"`. This includes a number of additional dependencies, which are necessary for encoding: Torch, 
-        Torchvision and OpenCLIP:
+        If you want to submit a fine-tuning job on the cloud, please use
         
         ```bash
         pip install "finetuner[full]"
         ```
         
         <!-- end install-instruction -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.7.8 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.8.0 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
 
@@ -51,29 +51,27 @@
            (German)
 PointNet++ ModelNet40 3D   mRR    0.791      0.891     12.7%  [Open_In_Colab]
            Mesh Search     Recall 0.154      0.242     57.1%
 All metrics were evaluated for k@20 after training for 5 epochs using the Adam
 optimizer with learning rates of 1e-4 for ResNet, 1e-7 for CLIP and 1e-5 for
 the BERT models, 5e-4 for PointNet++  ## Install Make sure you have Python 3.8+
 installed. Finetuner can be installed via `pip` by executing: ```bash pip
-install -U finetuner ``` If you want to encode local data with the
-`finetuner.encode` function, you need to install `"finetuner[full]"`. This
-includes a number of additional dependencies, which are necessary for encoding:
-Torch, Torchvision and OpenCLIP: ```bash pip install "finetuner[full]" ```  >
-â ï¸ Starting with version 0.5.0, Finetuner computing is performed on Jina AI
-Cloud. The last local version is `0.4.1`. > This version is still available for
-installation via `pip`. See [Finetuner git tags and releases](https://
-github.com/jina-ai/finetuner/releases).  ## Articles about Finetuner Check out
-our published blogposts and tutorials to see Finetuner in action! - [Fine-
-tuning with Low Budget and High Expectations](https://jina.ai/news/fine-tuning-
-with-low-budget-and-high-expectations/) - [Hype and Hybrids: Search is more
-than Keywords and Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-
-search-means-more-than-keywords-and-vectors-2/) - [Improving Search Quality for
-Non-English Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/
-news/improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
+install -U finetuner ``` If you want to submit a fine-tuning job on the cloud,
+please use ```bash pip install "finetuner[full]" ```  > â ï¸ Starting with
+version 0.5.0, Finetuner computing is performed on Jina AI Cloud. The last
+local version is `0.4.1`. > This version is still available for installation
+via `pip`. See [Finetuner git tags and releases](https://github.com/jina-ai/
+finetuner/releases).  ## Articles about Finetuner Check out our published
+blogposts and tutorials to see Finetuner in action! - [Fine-tuning with Low
+Budget and High Expectations](https://jina.ai/news/fine-tuning-with-low-budget-
+and-high-expectations/) - [Hype and Hybrids: Search is more than Keywords and
+Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-search-means-more-
+than-keywords-and-vectors-2/) - [Improving Search Quality for Non-English
+Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/news/
+improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
 models/) - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/
 applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/
 )   ## Support - Use [Discussions](https://github.com/jina-ai/finetuner/
 discussions) to talk about your use cases, questions, and support queries. -
 Join our [Discord community](https://discord.jina.ai) and chat with other
 community members about ideas. - Join our [Engineering All Hands](https://
 youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to
```

### Comparing `finetuner-0.7.8/README.md` & `finetuner-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -145,17 +145,15 @@
 
 Make sure you have Python 3.8+ installed. Finetuner can be installed via `pip` by executing:
 
 ```bash
 pip install -U finetuner
 ```
 
-If you want to encode local data with the `finetuner.encode` function, you need to install 
-`"finetuner[full]"`. This includes a number of additional dependencies, which are necessary for encoding: Torch, 
-Torchvision and OpenCLIP:
+If you want to submit a fine-tuning job on the cloud, please use
 
 ```bash
 pip install "finetuner[full]"
 ```
 
 <!-- end install-instruction -->
```

#### html2text {}

```diff
@@ -45,29 +45,27 @@
            (German)
 PointNet++ ModelNet40 3D   mRR    0.791      0.891     12.7%  [Open_In_Colab]
            Mesh Search     Recall 0.154      0.242     57.1%
 All metrics were evaluated for k@20 after training for 5 epochs using the Adam
 optimizer with learning rates of 1e-4 for ResNet, 1e-7 for CLIP and 1e-5 for
 the BERT models, 5e-4 for PointNet++  ## Install Make sure you have Python 3.8+
 installed. Finetuner can be installed via `pip` by executing: ```bash pip
-install -U finetuner ``` If you want to encode local data with the
-`finetuner.encode` function, you need to install `"finetuner[full]"`. This
-includes a number of additional dependencies, which are necessary for encoding:
-Torch, Torchvision and OpenCLIP: ```bash pip install "finetuner[full]" ```  >
-â ï¸ Starting with version 0.5.0, Finetuner computing is performed on Jina AI
-Cloud. The last local version is `0.4.1`. > This version is still available for
-installation via `pip`. See [Finetuner git tags and releases](https://
-github.com/jina-ai/finetuner/releases).  ## Articles about Finetuner Check out
-our published blogposts and tutorials to see Finetuner in action! - [Fine-
-tuning with Low Budget and High Expectations](https://jina.ai/news/fine-tuning-
-with-low-budget-and-high-expectations/) - [Hype and Hybrids: Search is more
-than Keywords and Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-
-search-means-more-than-keywords-and-vectors-2/) - [Improving Search Quality for
-Non-English Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/
-news/improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
+install -U finetuner ``` If you want to submit a fine-tuning job on the cloud,
+please use ```bash pip install "finetuner[full]" ```  > â ï¸ Starting with
+version 0.5.0, Finetuner computing is performed on Jina AI Cloud. The last
+local version is `0.4.1`. > This version is still available for installation
+via `pip`. See [Finetuner git tags and releases](https://github.com/jina-ai/
+finetuner/releases).  ## Articles about Finetuner Check out our published
+blogposts and tutorials to see Finetuner in action! - [Fine-tuning with Low
+Budget and High Expectations](https://jina.ai/news/fine-tuning-with-low-budget-
+and-high-expectations/) - [Hype and Hybrids: Search is more than Keywords and
+Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-search-means-more-
+than-keywords-and-vectors-2/) - [Improving Search Quality for Non-English
+Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/news/
+improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
 models/) - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/
 applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/
 )   ## Support - Use [Discussions](https://github.com/jina-ai/finetuner/
 discussions) to talk about your use cases, questions, and support queries. -
 Join our [Discord community](https://discord.jina.ai) and chat with other
 community members about ideas. - Join our [Engineering All Hands](https://
 youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to
```

### Comparing `finetuner-0.7.8/finetuner/__init__.py` & `finetuner-0.8.0/finetuner/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
 import os
 import warnings
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, TextIO, Union
 from urllib.parse import urlparse
 
+import numpy as np
 from _finetuner.runner.stubs import model as model_stub
 from docarray import Document, DocumentArray  # noqa F401
 
 from finetuner.constants import (
     DEFAULT_FINETUNER_HOST,
     DEFAULT_HUBBLE_REGISTRY,
     HOST,
@@ -29,15 +30,14 @@
 from finetuner.constants import HF_ORG_PREFIX, HF_URL_PREFIX
 from finetuner.data import build_encoding_dataset
 from finetuner.experiment import Experiment
 from finetuner.finetuner import Finetuner
 from finetuner.model import list_model_classes
 
 if TYPE_CHECKING:
-    import numpy as np
     from _finetuner.models.inference import InferenceEngine
 
 ft = Finetuner()
 
 
 def login(force: bool = False, interactive: Optional[bool] = None):
     """
@@ -665,7 +665,17 @@
             inputs = model._flatten_inputs(inputs)
             model._check_input_names(inputs)
             inputs = model._move_to_device(inputs)
             output = model.run(inputs)
             batch.embeddings = output.detach().cpu().numpy()
 
     return data if return_da else data.embeddings
+
+
+def cos_sim(a: np.ndarray, b: np.ndarray) -> float:
+    """Cosine similarity between two vectors.
+
+    :param a: The first vector.
+    :param b: The second vector.
+    :return: Cosine similarity between two vectors.
+    """
+    return np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b))
```

### Comparing `finetuner-0.7.8/finetuner/client/base.py` & `finetuner-0.8.0/finetuner/client/base.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/client/client.py` & `finetuner-0.8.0/finetuner/client/client.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/client/session.py` & `finetuner-0.8.0/finetuner/client/session.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/console.py` & `finetuner-0.8.0/finetuner/console.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/constants.py` & `finetuner-0.8.0/finetuner/constants.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/data.py` & `finetuner-0.8.0/finetuner/data.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/experiment.py` & `finetuner-0.8.0/finetuner/experiment.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/finetuner.py` & `finetuner-0.8.0/finetuner/finetuner.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/hubble.py` & `finetuner-0.8.0/finetuner/hubble.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/model.py` & `finetuner-0.8.0/finetuner/model.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/names.py` & `finetuner-0.8.0/finetuner/names.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner/run.py` & `finetuner-0.8.0/finetuner/run.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/finetuner.egg-info/PKG-INFO` & `finetuner-0.8.0/finetuner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.7.8
+Version: 0.8.0
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
@@ -157,17 +157,15 @@
         
         Make sure you have Python 3.8+ installed. Finetuner can be installed via `pip` by executing:
         
         ```bash
         pip install -U finetuner
         ```
         
-        If you want to encode local data with the `finetuner.encode` function, you need to install 
-        `"finetuner[full]"`. This includes a number of additional dependencies, which are necessary for encoding: Torch, 
-        Torchvision and OpenCLIP:
+        If you want to submit a fine-tuning job on the cloud, please use
         
         ```bash
         pip install "finetuner[full]"
         ```
         
         <!-- end install-instruction -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.7.8 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.8.0 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
 
@@ -51,29 +51,27 @@
            (German)
 PointNet++ ModelNet40 3D   mRR    0.791      0.891     12.7%  [Open_In_Colab]
            Mesh Search     Recall 0.154      0.242     57.1%
 All metrics were evaluated for k@20 after training for 5 epochs using the Adam
 optimizer with learning rates of 1e-4 for ResNet, 1e-7 for CLIP and 1e-5 for
 the BERT models, 5e-4 for PointNet++  ## Install Make sure you have Python 3.8+
 installed. Finetuner can be installed via `pip` by executing: ```bash pip
-install -U finetuner ``` If you want to encode local data with the
-`finetuner.encode` function, you need to install `"finetuner[full]"`. This
-includes a number of additional dependencies, which are necessary for encoding:
-Torch, Torchvision and OpenCLIP: ```bash pip install "finetuner[full]" ```  >
-â ï¸ Starting with version 0.5.0, Finetuner computing is performed on Jina AI
-Cloud. The last local version is `0.4.1`. > This version is still available for
-installation via `pip`. See [Finetuner git tags and releases](https://
-github.com/jina-ai/finetuner/releases).  ## Articles about Finetuner Check out
-our published blogposts and tutorials to see Finetuner in action! - [Fine-
-tuning with Low Budget and High Expectations](https://jina.ai/news/fine-tuning-
-with-low-budget-and-high-expectations/) - [Hype and Hybrids: Search is more
-than Keywords and Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-
-search-means-more-than-keywords-and-vectors-2/) - [Improving Search Quality for
-Non-English Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/
-news/improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
+install -U finetuner ``` If you want to submit a fine-tuning job on the cloud,
+please use ```bash pip install "finetuner[full]" ```  > â ï¸ Starting with
+version 0.5.0, Finetuner computing is performed on Jina AI Cloud. The last
+local version is `0.4.1`. > This version is still available for installation
+via `pip`. See [Finetuner git tags and releases](https://github.com/jina-ai/
+finetuner/releases).  ## Articles about Finetuner Check out our published
+blogposts and tutorials to see Finetuner in action! - [Fine-tuning with Low
+Budget and High Expectations](https://jina.ai/news/fine-tuning-with-low-budget-
+and-high-expectations/) - [Hype and Hybrids: Search is more than Keywords and
+Vectors](https://jina.ai/news/hype-and-hybrids-multimodal-search-means-more-
+than-keywords-and-vectors-2/) - [Improving Search Quality for Non-English
+Queries with Fine-tuned Multilingual CLIP Models](https://jina.ai/news/
+improving-search-quality-non-english-queries-fine-tuned-multilingual-clip-
 models/) - [How Much Do We Get by Finetuning CLIP?](https://jina.ai/news/
 applying-jina-ai-finetuner-to-clip-less-data-smaller-models-higher-performance/
 )   ## Support - Use [Discussions](https://github.com/jina-ai/finetuner/
 discussions) to talk about your use cases, questions, and support queries. -
 Join our [Discord community](https://discord.jina.ai) and chat with other
 community members about ideas. - Join our [Engineering All Hands](https://
 youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to
```

### Comparing `finetuner-0.7.8/finetuner.egg-info/SOURCES.txt` & `finetuner-0.8.0/finetuner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.8/setup.py` & `finetuner-0.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,21 +24,21 @@
         download_url='https://github.com/jina-ai/finetuner/tags',
         long_description=_long_description,
         long_description_content_type='text/markdown',
         zip_safe=False,
         setup_requires=['setuptools>=18.0', 'wheel'],
         install_requires=[
             'docarray[common]<0.30.0',
-            'trimesh==3.16.4',
-            'finetuner-stubs==0.13.7',
-            'jina-hubble-sdk==0.33.1',
+            'finetuner-stubs==0.13.9',
+            'finetuner-commons==0.13.9',
         ],
         extras_require={
             'full': [
-                'finetuner-commons==0.13.7',
+                'jina-hubble-sdk==0.33.1',
+                'trimesh==3.16.4',
             ],
             'test': [
                 'black==23.3.0',
                 'flake8==6.0.0',
                 'isort==5.12.0',
                 'pytest==7.0.0',
                 'pytest-cov==3.0.0',
```

