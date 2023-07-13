# Comparing `tmp/cerebrium-1.1.8.tar.gz` & `tmp/cerebrium-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.1.8.tar", max compression
+gzip compressed data, was "cerebrium-1.1.9.tar", max compression
```

## Comparing `cerebrium-1.1.8.tar` & `cerebrium-1.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      371 2023-07-11 19:14:14.273791 cerebrium-1.1.8/EXTERNAL_README.md
--rw-r--r--   0        0        0    34594 2023-07-11 19:14:14.273791 cerebrium-1.1.8/LICENSE
--rw-r--r--   0        0        0      360 2023-07-11 19:16:39.200396 cerebrium-1.1.8/cerebrium/__init__.py
--rwxr-xr-x   0        0        0    25081 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/cli.py
--rw-r--r--   0        0        0    33936 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/conduit.py
--rw-r--r--   0        0        0     5048 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/core.py
--rw-r--r--   0        0        0     2488 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/errors.py
--rw-r--r--   0        0        0    10182 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/flow.py
--rw-r--r--   0        0        0     3070 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3990 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      600 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/models/base.py
--rw-r--r--   0        0        0      550 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      411 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/models/onnx.py
--rw-r--r--   0        0        0      793 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      270 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      273 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8545 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/requests.py
--rw-r--r--   0        0        0    11285 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/README_Diffusers.md
--rw-r--r--   0        0        0     5592 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/README_Transformers.md
--rw-r--r--   0        0        0      110 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/__init__.py
--rw-r--r--   0        0        0     2174 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/diffuser_config.yaml
--rw-r--r--   0        0        0    14933 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/diffuser_tuner.py
--rw-r--r--   0        0        0     9079 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/fine_tuner.py
--rw-r--r--   0        0        0     1716 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/finetune_LLM/finetuning_model.py
--rw-r--r--   0        0        0        0 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
--rw-r--r--   0        0        0     2647 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
--rw-r--r--   0        0        0     4040 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
--rw-r--r--   0        0        0     1614 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/trainer/transformer_config.yaml
--rw-r--r--   0        0        0     1048 2023-07-11 19:14:14.273791 cerebrium-1.1.8/cerebrium/utils.py
--rw-r--r--   0        0        0     2378 2023-07-11 19:16:39.200396 cerebrium-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 cerebrium-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0      371 2023-07-13 16:29:26.693686 cerebrium-1.1.9/EXTERNAL_README.md
+-rw-r--r--   0        0        0    34594 2023-07-13 16:29:26.693686 cerebrium-1.1.9/LICENSE
+-rw-r--r--   0        0        0      360 2023-07-13 16:32:25.612339 cerebrium-1.1.9/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0    25216 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/cli.py
+-rw-r--r--   0        0        0    33936 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5048 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/core.py
+-rw-r--r--   0        0        0     2488 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/errors.py
+-rw-r--r--   0        0        0    10182 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/flow.py
+-rw-r--r--   0        0        0     3070 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3990 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      600 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/models/base.py
+-rw-r--r--   0        0        0      550 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      411 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0      793 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      270 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      273 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8545 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/requests.py
+-rw-r--r--   0        0        0    11285 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/README_Diffusers.md
+-rw-r--r--   0        0        0     5592 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/README_Transformers.md
+-rw-r--r--   0        0        0      110 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/__init__.py
+-rw-r--r--   0        0        0     1825 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/diffuser_config.yaml
+-rw-r--r--   0        0        0    14934 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/diffuser_tuner.py
+-rw-r--r--   0        0        0     9079 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/fine_tuner.py
+-rw-r--r--   0        0        0     1716 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/finetuning_model.py
+-rw-r--r--   0        0        0        0 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
+-rw-r--r--   0        0        0     2647 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
+-rw-r--r--   0        0        0     4040 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
+-rw-r--r--   0        0        0     1614 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/transformer_config.yaml
+-rw-r--r--   0        0        0     1048 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/utils.py
+-rw-r--r--   0        0        0     2378 2023-07-13 16:32:25.612339 cerebrium-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 cerebrium-1.1.9/PKG-INFO
```

### Comparing `cerebrium-1.1.8/LICENSE` & `cerebrium-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/cli.py` & `cerebrium-1.1.9/cerebrium/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,22 @@
         zip_path = os.path.join(temp_dir, zip_file_name)
         dir_name = os.path.dirname(zip_path)
         os.makedirs(dir_name, exist_ok=True)
         with zipfile.ZipFile(zip_path, "w") as zip_file:
             # include files
             include_set = include.strip("[]").split(",")
             # Force include main.py, requirements.txt, pkglist.txt and conda_pkglist.txt
-            include_set.extend(["./main.py", "./requirements.txt", "./pkglist.txt", "./conda_pkglist.txt"])
+            include_set.extend(
+                [
+                    "./main.py",
+                    "./requirements.txt",
+                    "./pkglist.txt",
+                    "./conda_pkglist.txt",
+                ]
+            )
             include_set = set(ensure_pattern_format(pattern) for pattern in include_set)
             exclude_set = exclude.strip("[]").split(",")
             exclude_set = set(ensure_pattern_format(pattern) for pattern in exclude_set)
             file_list = []
             for root, _, files in os.walk("./"):
                 for file in files:
                     full_path = os.path.join(root, file)
@@ -386,23 +393,23 @@
 @app.command()
 def get_training_logs(
     job_id: str = typer.Argument(
         ..., help="Job ID returned for your training instance."
     ),
     api_key: str = typer.Option("", help="Private API key for the user."),
     max_polling_duration: int = typer.Option(
-        6000, help="Number of seconds to poll the training. Maximum of 15min."
+        6000, help="Number of seconds to poll the training. Maximum of 60min."
     ),
 ):
     print(f"Retrieving training logs for {job_id}...")
     if not api_key:
         api_key = get_api_key()
 
-    interval = 5  # seconds between polling.
-    max_polling_duration = min(max_polling_duration, 60 * 15)
+    interval = 1  # seconds between polling.
+    max_polling_duration = min(max_polling_duration, 60 * 60)
 
     # Poll the trainingLogs and make the output pretty
     seen_index = 0
     t_start = time.time()
     with yaspin.yaspin(text="CHECKING...", color="green") as spinner:
         train_status = "CHECKING..."
         while train_status != "succeeded":
@@ -580,25 +587,25 @@
         config = {}
 
     if config_string:
         config_json = json.loads(config_string)
         config.update(config_json)
 
     # check if training type is specified in config
-    training_type = (
-        training_type or config.get("training_type")
-    )
+    training_type = training_type or config.get("training_type")
     assert (
         training_type is not None
     ), "Training type must be specified in config or command line args."
 
     # overwrite with command line args if present
     name = name or config["name"]
     if not api_key:
-        api_key = config.get("api_key")  # default to config from either the file or the string
+        api_key = config.get(
+            "api_key"
+        )  # default to config from either the file or the string
 
     # If api key is not provided in any parameter or config, check if it is in the login config file
     if not api_key:
         api_key = get_api_key()
 
     # get log level
     log_level = log_level or config.get("log_level", "INFO")
```

### Comparing `cerebrium-1.1.8/cerebrium/conduit.py` & `cerebrium-1.1.9/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/core.py` & `cerebrium-1.1.9/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/errors.py` & `cerebrium-1.1.9/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/flow.py` & `cerebrium-1.1.9/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/logging/arize.py` & `cerebrium-1.1.9/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/logging/base.py` & `cerebrium-1.1.9/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/logging/censius.py` & `cerebrium-1.1.9/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/models/base.py` & `cerebrium-1.1.9/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/models/hf_pipeline.py` & `cerebrium-1.1.9/cerebrium/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/models/sklearn.py` & `cerebrium-1.1.9/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/requests.py` & `cerebrium-1.1.9/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/trainer/README_Diffusers.md` & `cerebrium-1.1.9/cerebrium/trainer/README_Diffusers.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/trainer/README_Transformers.md` & `cerebrium-1.1.9/cerebrium/trainer/README_Transformers.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/trainer/diffuser_config.yaml` & `cerebrium-1.1.9/cerebrium/trainer/diffuser_config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,47 @@
 %YAML 1.2
 ---
 training_type: "diffuser" # Type of training to run. Either "diffuser" or "transformer".
 name: "test-config-file" # Name of the experiment.
-api-key: "dev-private-4f293d340d112179542f" # Your Cerebrium API key.
+api-key: "YOUR API KEY HERE" # Your Cerebrium API key.
 hf_model_path: "runwayml/stable-diffusion-v1-5"
 revision: "main" # Revision of the diffuser model to use.
 train_prompt: "Photo of a tsdf dog." 
 validation_prompt: ~ # an optional validation prompt to use. If ~, will use the training prompt.
 custom_tokenizer: "" # custom tokenizer from AutoTokenizer if required.
 log_level: "WARNING" # log_level level for logging.
 
 
-# Dataset params
-train_image_dir: /Users/michaelkatsoulis/Documents/Cerebrium/FineTuningData/StableDiffusion/trainingImages/doberman # data/training_class_images/ # Directory of training images.
-prior_class_image_dir: /Users/michaelkatsoulis/Documents/Cerebrium/FineTuningData/StableDiffusion/trainingImages/dog # ~ # "data/prior_class_images" # Optional directory of images to use for prior class.
+train_image_dir: data/training_class_images/ # Directory of training images.
+prior_class_image_dir: ~ # "data/prior_class_images" # Optional directory of images to use for prior class.
 prior_class_prompt: "Photo of a dog."
 
 # Training params
 training_args:
   # General training params
   num_validation_images: 4 # Number of images to generate in validation.
-  learning_rate: 1e-4
-  num_train_epochs: 10
+  learning_rate: 1.0E-4
+  num_train_epochs: 30
   seed: ~
   resolution: 512 # Resolution to train images at.
   center_crop: False # Whether to center crop images to resolution.
   train_batch_size: 2
   num_prior_class_images: 10
   prior_class_generation_batch_size: 2
   prior_loss_weight: 1.0 # Weight of prior loss in the total loss.
   max_train_steps: ~ # maximum training steps which overrides number of training epochs
-  validation_epochs: 5 # number of epochs before running validation and checkpointing
+  validation_epochs: 10 # number of epochs before running validation and checkpointing
 
   
   # Training loop params
   gradient_accumulation_steps: 1
-  learning_rate: 0.0005
   lr_scheduler: "constant"
   lr_warmup_steps: 5
   lr_num_cycles: 1
   lr_power: 1.0
   allow_tf32: False
   max_grad_norm: 1.0
-  mixed_precision: "fp16"
+  mixed_precision: 'no' # "fp16 or "bf16"
   prior_generation_precision: ~
   scale_lr: False 
   use_8bit_adam: True
   use_xformers: True # Whether to use xformers memory efficient attention or not.
-
-# Reporting params #TODO not implemented yet.
-  report_to: ~
-  hub_token: ~
-  hub_model_id: ~
-  push_to_hub: False
```

### Comparing `cerebrium-1.1.8/cerebrium/trainer/diffuser_tuner.py` & `cerebrium-1.1.9/cerebrium/trainer/diffuser_tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,15 @@
                     )
                     print("Error uploading to Cerebrium:", upload_response.text)
                     raise Exception("Error uploading to Cerebrium")
                 else:
                     print(f"✅ Resources uploaded successfully for {job_id}")
             print(
                 f"You can query the training status with `cerebrium get-training-jobs --api-key {api_key}` \n",
-                f"Your training logs can be found at `cerebrium get-training-logs {job_id} --api-key{api_key}` ",
+                f"Your training logs can be found at `cerebrium get-training-logs {job_id} --api-key {api_key}` ",
             )
 
     def __iter__(self):
         yield from self.__dict__.items()
 
     def __str__(self):
         return json.dumps(dict(self), ensure_ascii=False)
```

### Comparing `cerebrium-1.1.8/cerebrium/trainer/fine_tuner.py` & `cerebrium-1.1.9/cerebrium/trainer/fine_tuner.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/trainer/finetune_LLM/finetuning_model.py` & `cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/finetuning_model.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py` & `cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py` & `cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/trainer/transformer_config.yaml` & `cerebrium-1.1.9/cerebrium/trainer/transformer_config.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/cerebrium/utils.py` & `cerebrium-1.1.9/cerebrium/utils.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.8/pyproject.toml` & `cerebrium-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.1.8"
+version = "1.1.9"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "EXTERNAL_README.md"
 exclude = ["tests/*", "dist/*", "webhook/*", "builder/*", "prebuilt/*", "common/*", "examples/*", "trainer/*", "README.md"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.1.8/PKG-INFO` & `cerebrium-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.1.8
+Version: 1.1.9
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

