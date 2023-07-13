# Comparing `tmp/trl-0.4.6.tar.gz` & `tmp/trl-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trl-0.4.6.tar", last modified: Fri Jun 23 09:18:14 2023, max compression
+gzip compressed data, was "trl-0.4.7.tar", last modified: Thu Jul 13 08:26:56 2023, max compression
```

## Comparing `trl-0.4.6.tar` & `trl-0.4.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.319674 trl-0.4.6/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2445 2023-05-03 09:18:40.000000 trl-0.4.6/CONTRIBUTING.md
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11357 2023-05-03 09:18:40.000000 trl-0.4.6/LICENSE
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      111 2023-05-03 09:18:40.000000 trl-0.4.6/MANIFEST.in
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6443 2023-06-23 09:18:14.319674 trl-0.4.6/PKG-INFO
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5413 2023-05-03 09:18:40.000000 trl-0.4.6/README.md
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      315 2023-06-23 09:18:14.319674 trl-0.4.6/setup.cfg
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3779 2023-06-23 09:17:08.000000 trl-0.4.6/setup.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.311673 trl-0.4.6/tests/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-05-03 09:18:40.000000 trl-0.4.6/tests/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3162 2023-06-21 08:50:41.000000 trl-0.4.6/tests/test_best_of_n_sampler.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1561 2023-05-03 09:18:40.000000 trl-0.4.6/tests/test_core.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      152 2023-06-21 08:50:41.000000 trl-0.4.6/tests/test_e2e.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23191 2023-05-03 09:18:40.000000 trl-0.4.6/tests/test_modeling_value_head.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5439 2023-05-03 09:18:40.000000 trl-0.4.6/tests/test_no_peft.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9515 2023-06-19 11:54:46.000000 trl-0.4.6/tests/test_peft_models.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    41226 2023-06-23 08:12:16.000000 trl-0.4.6/tests/test_ppo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9931 2023-06-21 08:50:41.000000 trl-0.4.6/tests/test_reward_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    18911 2023-06-23 08:12:16.000000 trl-0.4.6/tests/test_sft_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      799 2023-05-03 09:18:40.000000 trl-0.4.6/tests/testing_constants.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1555 2023-05-03 09:18:40.000000 trl-0.4.6/tests/testing_utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.315673 trl-0.4.6/trl/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      407 2023-06-23 09:17:04.000000 trl-0.4.6/trl/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7920 2023-05-03 09:18:40.000000 trl-0.4.6/trl/core.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.315673 trl-0.4.6/trl/extras/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      668 2023-06-21 08:50:41.000000 trl-0.4.6/trl/extras/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5190 2023-06-21 08:50:41.000000 trl-0.4.6/trl/extras/best_of_n_sampler.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1120 2023-05-03 09:18:40.000000 trl-0.4.6/trl/import_utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.315673 trl-0.4.6/trl/models/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      910 2023-05-03 09:18:40.000000 trl-0.4.6/trl/models/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23627 2023-06-23 08:12:16.000000 trl-0.4.6/trl/models/modeling_base.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    17967 2023-05-17 09:28:26.000000 trl-0.4.6/trl/models/modeling_value_head.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.319674 trl-0.4.6/trl/trainer/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1035 2023-06-21 09:04:57.000000 trl-0.4.6/trl/trainer/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1772 2023-05-03 09:18:40.000000 trl-0.4.6/trl/trainer/base.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8312 2023-06-23 09:13:55.000000 trl-0.4.6/trl/trainer/ppo_config.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    52510 2023-06-23 08:12:16.000000 trl-0.4.6/trl/trainer/ppo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    10115 2023-06-23 08:12:16.000000 trl-0.4.6/trl/trainer/reward_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    14717 2023-06-23 08:12:16.000000 trl-0.4.6/trl/trainer/sft_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11523 2023-06-23 08:12:16.000000 trl-0.4.6/trl/trainer/utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-06-23 09:18:14.315673 trl-0.4.6/trl.egg-info/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6443 2023-06-23 09:18:14.000000 trl-0.4.6/trl.egg-info/PKG-INFO
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      887 2023-06-23 09:18:14.000000 trl-0.4.6/trl.egg-info/SOURCES.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-06-23 09:18:14.000000 trl-0.4.6/trl.egg-info/dependency_links.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-05-17 08:26:30.000000 trl-0.4.6/trl.egg-info/not-zip-safe
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      225 2023-06-23 09:18:14.000000 trl-0.4.6/trl.egg-info/requires.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       10 2023-06-23 09:18:14.000000 trl-0.4.6/trl.egg-info/top_level.txt
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.241035 trl-0.4.7/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2522 2023-07-12 12:43:13.000000 trl-0.4.7/CONTRIBUTING.md
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11357 2023-05-03 09:18:40.000000 trl-0.4.7/LICENSE
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      111 2023-05-03 09:18:40.000000 trl-0.4.7/MANIFEST.in
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9620 2023-07-13 08:26:56.241035 trl-0.4.7/PKG-INFO
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8590 2023-07-12 12:43:13.000000 trl-0.4.7/README.md
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      257 2023-07-13 08:26:56.241035 trl-0.4.7/setup.cfg
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3759 2023-07-13 08:17:28.000000 trl-0.4.7/setup.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.237035 trl-0.4.7/tests/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-05-03 09:18:40.000000 trl-0.4.7/tests/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3162 2023-06-21 08:50:41.000000 trl-0.4.7/tests/test_best_of_n_sampler.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1561 2023-05-03 09:18:40.000000 trl-0.4.7/tests/test_core.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      152 2023-06-21 08:50:41.000000 trl-0.4.7/tests/test_e2e.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23191 2023-05-03 09:18:40.000000 trl-0.4.7/tests/test_modeling_value_head.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5439 2023-05-03 09:18:40.000000 trl-0.4.7/tests/test_no_peft.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9515 2023-06-19 11:54:46.000000 trl-0.4.7/tests/test_peft_models.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    42825 2023-07-12 12:43:13.000000 trl-0.4.7/tests/test_ppo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9931 2023-07-11 07:11:15.000000 trl-0.4.7/tests/test_reward_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    18911 2023-06-23 08:12:16.000000 trl-0.4.7/tests/test_sft_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      799 2023-05-03 09:18:40.000000 trl-0.4.7/tests/testing_constants.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1555 2023-05-03 09:18:40.000000 trl-0.4.7/tests/testing_utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.237035 trl-0.4.7/trl/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      407 2023-07-13 08:17:35.000000 trl-0.4.7/trl/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7920 2023-05-03 09:18:40.000000 trl-0.4.7/trl/core.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.241035 trl-0.4.7/trl/extras/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      668 2023-06-21 08:50:41.000000 trl-0.4.7/trl/extras/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5190 2023-06-21 08:50:41.000000 trl-0.4.7/trl/extras/best_of_n_sampler.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1120 2023-05-03 09:18:40.000000 trl-0.4.7/trl/import_utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.241035 trl-0.4.7/trl/models/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      910 2023-05-03 09:18:40.000000 trl-0.4.7/trl/models/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    23980 2023-07-12 12:43:13.000000 trl-0.4.7/trl/models/modeling_base.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    18277 2023-07-12 12:43:13.000000 trl-0.4.7/trl/models/modeling_value_head.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.241035 trl-0.4.7/trl/trainer/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1035 2023-07-07 10:32:34.000000 trl-0.4.7/trl/trainer/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1772 2023-05-03 09:18:40.000000 trl-0.4.7/trl/trainer/base.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8751 2023-07-12 12:43:13.000000 trl-0.4.7/trl/trainer/ppo_config.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    53529 2023-07-12 12:43:13.000000 trl-0.4.7/trl/trainer/ppo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    10115 2023-07-12 12:37:45.000000 trl-0.4.7/trl/trainer/reward_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    13740 2023-07-13 08:15:02.000000 trl-0.4.7/trl/trainer/sft_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    12711 2023-07-12 12:43:13.000000 trl-0.4.7/trl/trainer/utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-07-13 08:26:56.241035 trl-0.4.7/trl.egg-info/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9620 2023-07-13 08:26:56.000000 trl-0.4.7/trl.egg-info/PKG-INFO
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      887 2023-07-13 08:26:56.000000 trl-0.4.7/trl.egg-info/SOURCES.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-07-13 08:26:56.000000 trl-0.4.7/trl.egg-info/dependency_links.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-05-17 08:26:30.000000 trl-0.4.7/trl.egg-info/not-zip-safe
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      210 2023-07-13 08:26:56.000000 trl-0.4.7/trl.egg-info/requires.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       10 2023-07-13 08:26:56.000000 trl-0.4.7/trl.egg-info/top_level.txt
```

### Comparing `trl-0.4.6/CONTRIBUTING.md` & `trl-0.4.7/CONTRIBUTING.md`

 * *Files 14% similar despite different names*

```diff
@@ -32,17 +32,22 @@
 
 First you want to make sure that all the tests pass:
 
 ```bash
 make test
 ```
 
-Then before submitting your PR make sure the code quality follows the standards. You can run the following command to format and test:
+Then before submitting your PR make sure the code quality follows the standards. You can run the following command to format:
 
 ```bash
-make style && make quality
+make precommit
+```
+
+Make sure to install `pre-commit` before running the command:
+```bash
+pip install pre-commit
 ```
 
 ## Do you want to contribute to the documentation?
 
 * Docs are in the `docs/` folder and can be updated there.
```

### Comparing `trl-0.4.6/LICENSE` & `trl-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/setup.py` & `trl-0.4.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,29 +50,30 @@
 
 7. Fill release notes in the tag in github once everything is looking hunky-dory.
 
 8. Change the version in __init__.py and setup.py to X.X.X+1.dev0 (e.g. VERSION=1.18.3 -> 1.18.4.dev0).
    Then push the change with a message 'set dev version'
 """
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-__version__ = "0.4.6"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+
+__version__ = "0.4.7"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
 
 REQUIRED_PKGS = [
     "torch>=1.4.0",
     "transformers>=4.18.0",
     "numpy>=1.18.2",
     "accelerate",
     "datasets",
 ]
 EXTRAS = {
     "test": ["parameterized", "pytest", "pytest-xdist", "accelerate", "peft"],
     "peft": ["peft>=0.2.0"],
-    "dev": ["parameterized", "pytest", "pytest-xdist", "black", "isort", "flake8>=3.8.3", "peft>=0.2.0"],
+    "dev": ["parameterized", "pytest", "pytest-xdist", "pre-commit", "peft>=0.2.0"],
 }
 
 setup(
     name="trl",
     license="Apache 2.0",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
```

### Comparing `trl-0.4.6/tests/test_best_of_n_sampler.py` & `trl-0.4.7/tests/test_best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/tests/test_core.py` & `trl-0.4.7/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/tests/test_modeling_value_head.py` & `trl-0.4.7/tests/test_modeling_value_head.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/tests/test_no_peft.py` & `trl-0.4.7/tests/test_no_peft.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/tests/test_peft_models.py` & `trl-0.4.7/tests/test_peft_models.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/tests/test_ppo_trainer.py` & `trl-0.4.7/tests/test_ppo_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,14 +675,55 @@
         for name, param in ppo_trainer.model.named_parameters():
             self.assertTrue(param.grad is not None, f"Parameter {name} has no gradient")
             self.assertTrue(
                 torch.all(param.grad.abs() <= self.ppo_config.max_grad_norm),
                 f"Parameter {name} has a gradient larger than max_grad_norm",
             )
 
+    def test_ppo_trainer_kl_penalty(self):
+        dummy_dataset = self._init_dummy_dataset()
+
+        log_probs = torch.Tensor([[0.5, 0.2, 0.1], [0.6, 0.2, 0.1]])
+        ref_log_probs = torch.Tensor([[0.4, 0.3, 0.0], [0.7, 0.1, 0.3]])
+
+        ppo_trainer = PPOTrainer(
+            config=self.ppo_config,
+            model=self.gpt2_model,
+            ref_model=None,
+            tokenizer=self.gpt2_tokenizer,
+            dataset=dummy_dataset,
+        )
+
+        expected_output = torch.Tensor([[0.1000, -0.1000, 0.1000], [-0.1000, 0.1000, -0.2000]])
+        self.assertTrue(torch.allclose(ppo_trainer._kl_penalty(log_probs, ref_log_probs), expected_output))
+
+        self.ppo_config.kl_penalty = "abs"
+        ppo_trainer = PPOTrainer(
+            config=self.ppo_config,
+            model=self.gpt2_model,
+            ref_model=None,
+            tokenizer=self.gpt2_tokenizer,
+            dataset=dummy_dataset,
+        )
+
+        expected_output = torch.Tensor([[0.1000, 0.1000, 0.1000], [0.1000, 0.1000, 0.2000]])
+        self.assertTrue(torch.allclose(ppo_trainer._kl_penalty(log_probs, ref_log_probs), expected_output))
+
+        self.ppo_config.kl_penalty = "mse"
+        ppo_trainer = PPOTrainer(
+            config=self.ppo_config,
+            model=self.gpt2_model,
+            ref_model=None,
+            tokenizer=self.gpt2_tokenizer,
+            dataset=dummy_dataset,
+        )
+
+        expected_output = torch.Tensor([[0.0050, 0.0050, 0.0050], [0.0050, 0.0050, 0.0200]])
+        self.assertTrue(torch.allclose(ppo_trainer._kl_penalty(log_probs, ref_log_probs), expected_output))
+
     @require_peft
     @mark.peft_test
     def test_peft_model_ppo_trainer(self):
         from peft import LoraConfig, get_peft_model
         from transformers import AutoModelForCausalLM
 
         lora_config = LoraConfig(
```

### Comparing `trl-0.4.6/tests/test_reward_trainer.py` & `trl-0.4.7/tests/test_reward_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,17 @@
             lora_dropout=0.1,
         )
 
         with tempfile.TemporaryDirectory() as tmp_dir:
             training_args = TrainingArguments(
                 output_dir=tmp_dir,
                 per_device_train_batch_size=2,
-                max_steps=3,
+                max_steps=6,
                 remove_unused_columns=False,
-                gradient_accumulation_steps=4,
+                gradient_accumulation_steps=2,
                 learning_rate=9e-1,
                 evaluation_strategy="steps",
             )
 
             # fmt: off
             dummy_dataset_dict = {
                 "input_ids_chosen": [
```

### Comparing `trl-0.4.6/tests/test_sft_trainer.py` & `trl-0.4.7/tests/test_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/tests/testing_constants.py` & `trl-0.4.7/tests/testing_constants.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/tests/testing_utils.py` & `trl-0.4.7/tests/testing_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/trl/core.py` & `trl-0.4.7/trl/core.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/trl/extras/__init__.py` & `trl-0.4.7/trl/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/trl/extras/best_of_n_sampler.py` & `trl-0.4.7/trl/extras/best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/trl/import_utils.py` & `trl-0.4.7/trl/import_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/trl/models/__init__.py` & `trl-0.4.7/trl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/trl/models/modeling_base.py` & `trl-0.4.7/trl/models/modeling_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 if is_peft_available():
     from peft import (
         LoraConfig,
         PeftConfig,
         PeftModel,
         PeftModelForCausalLM,
         PeftModelForSeq2SeqLM,
+        PromptLearningConfig,
         get_peft_model,
         prepare_model_for_int8_training,
     )
     from peft.peft_model import set_peft_model_state_dict
 
 LAYER_PATTERNS = [
     "transformer.h.{layer}",
@@ -123,14 +124,15 @@
 
         if reward_adapter is not None and not isinstance(reward_adapter, str):
             raise ValueError(
                 "The `reward_adapter` argument should be a string representing the name of local path or the Hub id to the Reward Modeling adapter."
             )
 
         is_peft_model = False
+
         current_device = cls._get_current_device()
         if isinstance(pretrained_model_name_or_path, str):
             is_loaded_in_8bit = pretrained_kwargs["load_in_8bit"] if "load_in_8bit" in pretrained_kwargs else False
             is_loaded_in_4bit = pretrained_kwargs["load_in_4bit"] if "load_in_4bit" in pretrained_kwargs else False
         else:
             is_loaded_in_8bit = getattr(pretrained_model_name_or_path, "is_loaded_in_8bit", False)
             is_loaded_in_4bit = getattr(pretrained_model_name_or_path, "is_loaded_in_4bit", False)
@@ -217,14 +219,19 @@
                 "pretrained_model_name_or_path should be a string or a PreTrainedModel, "
                 f"but is {type(pretrained_model_name_or_path)}"
             )
 
         if is_peft_available():
             if isinstance(pretrained_model, PeftModel):
                 is_peft_model = True
+                # for backward compatibility
+                if hasattr(pretrained_model, "active_peft_config") and isinstance(
+                    pretrained_model.active_peft_config, PromptLearningConfig
+                ):
+                    raise ValueError("PromptLearningConfig is not supported for PPO training.")
         # Then, create the full model by instantiating the wrapper class
         model = cls(pretrained_model, **trl_model_args)
 
         # if resume_training, load the state_dict again - this is ok since the
         # state_dict is removed from the model after loading it.
         is_resuming_training = True
         if isinstance(pretrained_model_name_or_path, str):
@@ -270,14 +277,15 @@
                 else:
                     state_dict = torch.load(filename, map_location="cpu")
 
         else:
             state_dict = pretrained_model_name_or_path.state_dict()
 
         model.is_peft_model = is_peft_model
+
         model.current_device = current_device
 
         if is_resuming_training:
             model.post_init(state_dict=state_dict)
 
         if not is_peft_model and reward_adapter is not None:
             raise ValueError("reward_adapter can only be used with a PeftModel. ")
```

### Comparing `trl-0.4.6/trl/models/modeling_value_head.py` & `trl-0.4.7/trl/models/modeling_value_head.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,18 +153,21 @@
                 Mask to avoid performing attention on padding token indices. Mask values selected in ``[0, 1]``:
                 - 1 for tokens that are **not masked**,
                 - 0 for tokens that are **masked**.
             kwargs (`dict`, `optional`):
                 Additional keyword arguments, that are passed to the wrapped model.
         """
         kwargs["output_hidden_states"] = True  # this had already been set in the LORA / PEFT examples
+        kwargs["past_key_values"] = past_key_values
+
+        if self.is_peft_model and self.pretrained_model.active_peft_config.peft_type == "PREFIX_TUNING":
+            kwargs.pop("past_key_values")
 
         base_model_output = self.pretrained_model(
             input_ids=input_ids,
-            past_key_values=past_key_values,
             attention_mask=attention_mask,
             **kwargs,
         )
 
         last_hidden_state = base_model_output.hidden_states[-1]
         lm_logits = base_model_output.logits
         loss = base_model_output.loss
@@ -388,17 +391,20 @@
     def forward(
         self,
         input_ids=None,
         past_key_values=None,
         attention_mask=None,
         **kwargs,
     ):
+        kwargs["past_key_values"] = past_key_values
+        if self.is_peft_model and self.pretrained_model.active_peft_config.peft_type == "PREFIX_TUNING":
+            kwargs.pop("past_key_values")
+
         base_model_output = self.pretrained_model(
             input_ids=input_ids,
-            past_key_values=past_key_values,
             attention_mask=attention_mask,
             output_hidden_states=True,  # We force the model to output hidden states
             **kwargs,
         )
 
         last_hidden_state = base_model_output.decoder_hidden_states[-1]
         lm_logits = base_model_output.logits
```

### Comparing `trl-0.4.6/trl/trainer/__init__.py` & `trl-0.4.7/trl/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/trl/trainer/base.py` & `trl-0.4.7/trl/trainer/base.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/trl/trainer/ppo_config.py` & `trl-0.4.7/trl/trainer/ppo_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,20 @@
     steps: Optional[int] = field(default=20000, metadata={"help": "Number of training steps"})
     learning_rate: Optional[float] = field(default=1e-5, metadata={"help": "Adam learning rate"})
     adap_kl_ctrl: Optional[bool] = field(default=True, metadata={"help": "Use adaptive KL control, otherwise linear"})
     init_kl_coef: Optional[float] = field(
         default=0.2,
         metadata={"help": "Initial KL penalty coefficient (used for adaptive and linear control)"},
     )
+    kl_penalty: Optional[str] = field(
+        default="kl",
+        metadata={
+            "help": "kl penalty options: 'kl': model_logp - ref_logp,  'abs': abs(kl) and 'mse': mean squared error mse(kl)."
+        },
+    )
     target: Optional[float] = field(default=6, metadata={"help": "Target KL value for adaptive KL control"})
     horizon: Optional[float] = field(default=10000, metadata={"help": "Horizon for adaptive KL control"})
     gamma: Optional[float] = field(default=1, metadata={"help": "Gamma parameter for advantage calculation"})
     lam: Optional[float] = field(default=0.95, metadata={"help": "Lambda parameter for advantage calculation"})
     cliprange: Optional[float] = field(
         default=0.2, metadata={"help": "Range for clipping in PPO policy gradient loss"}
     )
@@ -146,14 +152,17 @@
         default_factory=dict,
         metadata={"help": "Keyword arguments for pushing model to the hub during training (e.g. repo_id)"},
     )
     compare_steps: Optional[int] = field(
         default=1,
         metadata={"help": "Number of steps between comparison of the current reward with the best seen so far"},
     )
+    ratio_threshold: Optional[float] = field(
+        default=10.0, metadata={"help": "Skip mini-batches with high PPO ratios that can cause loss spikes"}
+    )
 
     def __post_init__(self):
         if self.forward_batch_size is not None:
             warnings.warn(
                 "Note that using `forward_batch_size` is deprecated, use `mini_batch_size` instead. By setting it you overwrite `mini_batch_size` which affects both the batch size during forward passes and also the mini batch size for PPO optimization."
             )
             self.mini_batch_size = self.forward_batch_size
@@ -174,13 +183,14 @@
                     logging.info(f"the following tags will be used for wandb logging: {os.environ['WANDB_TAGS']}")
             except ImportError:
                 raise ImportError(
                     "Please install wandb to use wandb logging. You can do this by running `pip install wandb`."
                 )
 
         self.total_ppo_epochs = int(np.ceil(self.steps / self.batch_size))
+        assert self.kl_penalty in ["kl", "abs", "mse"]
 
     def to_dict(self):
         output_dict = {}
         for key, value in self.__dict__.items():
             output_dict[key] = value
         return flatten_dict(output_dict)
```

### Comparing `trl-0.4.6/trl/trainer/ppo_trainer.py` & `trl-0.4.7/trl/trainer/ppo_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,14 +450,15 @@
     def _generate_batched(
         self,
         query_tensors: List[torch.Tensor],
         length_sampler: Callable = None,
         batch_size: int = 4,
         return_prompt: bool = True,
         pad_to_multiple_of: int = None,
+        remove_padding: bool = True,
         **generation_kwargs,
     ):
         outputs = []
 
         padding_side_default = self.tokenizer.padding_side
         if not self.is_encoder_decoder:
             self.tokenizer.padding_side = "left"
@@ -490,14 +491,20 @@
                 if not self.is_encoder_decoder:
                     output = generation[(1 - mask).sum() :]  # remove padding
                 else:
                     output = generation
 
                 if not return_prompt and not self.is_encoder_decoder:
                     output = output[(mask).sum() :]  # remove prompt
+
+                if remove_padding and self.tokenizer.eos_token_id in output:
+                    pad_mask = output == self.tokenizer.eos_token_id
+                    pad_start = torch.nonzero(pad_mask, as_tuple=False)[0, 0].item()
+                    output = output[: pad_start + 1]  # keep the eos token at the end
+
                 outputs.append(output)
 
         self.tokenizer.padding_side = padding_side_default
         return outputs
 
     def _step_safety_checker(
         self,
@@ -879,17 +886,14 @@
                     end = attention_mask[j, :].sum() - 1
                 else:
                     start = len(query_batch[j]) - 1
                     if attention_mask[j, 0] == 0:  # offset left padding
                         start += attention_mask[j, :].nonzero()[0]
                     end = start + len(response_batch[j])
 
-                if len(logprobs[j, start:end]) < 2:
-                    raise ValueError("Responses are too short. Make sure they are at least 4 tokens long.")
-
                 masks[j, :start] = 0
                 masks[j, end:] = 0
 
             if return_logits:
                 all_logits.append(logits)
             else:
                 del logits
@@ -967,25 +971,37 @@
                 Log probabilities of the model, shape (`batch_size`, `response_length`)
             ref_logprobs (`torch.FloatTensor`):
                 Log probabilities of the reference model, shape (`batch_size`, `response_length`)
         """
         rewards, non_score_rewards = [], []
         for score, logprob, ref_logprob, mask in zip(scores, logprobs, ref_logprobs, masks):
             # compute KL penalty (from difference in logprobs)
-            kl = logprob - ref_logprob
+            kl = self._kl_penalty(logprob, ref_logprob)
             non_score_reward = -self.kl_ctl.value * kl
             non_score_rewards.append(non_score_reward)
             reward = non_score_reward.clone()
             last_non_masked_index = mask.nonzero()[-1]
 
             # reward is preference model score + KL penalty
             reward[last_non_masked_index] += score
             rewards.append(reward)
         return torch.stack(rewards), torch.stack(non_score_rewards)
 
+    def _kl_penalty(self, logprob: torch.FloatTensor, ref_logprob: torch.FloatTensor) -> torch.FloatTensor:
+        if self.config.kl_penalty == "kl":
+            return logprob - ref_logprob
+
+        if self.config.kl_penalty == "abs":
+            return (logprob - ref_logprob).abs()
+
+        if self.config.kl_penalty == "mse":
+            return 0.5 * (logprob - ref_logprob).square()
+
+        raise NotImplementedError
+
     def loss(
         self,
         old_logprobs: torch.FloatTensor,
         values: torch.FloatTensor,
         rewards: torch.FloatTensor,
         logits: torch.FloatTensor,
         vpreds: torch.FloatTensor,
@@ -1030,28 +1046,40 @@
         vpredclipped = clip_by_value(
             vpreds, values - self.config.cliprange_value, values + self.config.cliprange_value
         )
 
         vf_losses1 = (vpreds - returns) ** 2
         vf_losses2 = (vpredclipped - returns) ** 2
         vf_loss = 0.5 * masked_mean(torch.max(vf_losses1, vf_losses2), mask)
-        vf_clipfrac = masked_mean(torch.gt(vf_losses2, vf_losses1).double(), mask)
+        vf_clipfrac = masked_mean(torch.gt(vf_losses2, vf_losses1).float(), mask)
 
         ratio = torch.exp(logprobs - old_logprobs)
+
         pg_losses = -advantages * ratio
         pg_losses2 = -advantages * torch.clamp(ratio, 1.0 - self.config.cliprange, 1.0 + self.config.cliprange)
 
         pg_loss = masked_mean(torch.max(pg_losses, pg_losses2), mask)
-        pg_clipfrac = masked_mean(torch.gt(pg_losses2, pg_losses).double(), mask)
+        pg_clipfrac = masked_mean(torch.gt(pg_losses2, pg_losses).float(), mask)
 
         loss = pg_loss + self.config.vf_coef * vf_loss
 
+        avg_ratio = masked_mean(ratio, mask).item()
+        if avg_ratio > self.config.ratio_threshold:
+            warnings.warn(
+                f"The average ratio of batch ({avg_ratio:.2f}) exceeds threshold {self.config.ratio_threshold:.2f}. Skipping batch."
+            )
+            pg_loss = pg_loss * 0.0
+            vf_loss = vf_loss * 0.0
+            loss = loss * 0.0
+
         entropy = masked_mean(entropy_from_logits(logits), mask)
+
         approxkl = 0.5 * masked_mean((logprobs - old_logprobs) ** 2, mask)
         policykl = masked_mean(old_logprobs - logprobs, mask)
+
         return_mean, return_var = masked_mean(returns, mask), masked_var(returns, mask)
         value_mean, value_var = masked_mean(values, mask), masked_var(values, mask)
 
         stats = dict(
             loss=dict(policy=pg_loss.detach(), value=vf_loss.detach(), total=loss.detach()),
             policy=dict(
                 entropy=entropy.detach(),
```

### Comparing `trl-0.4.6/trl/trainer/reward_trainer.py` & `trl-0.4.7/trl/trainer/reward_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.4.6/trl/trainer/sft_trainer.py` & `trl-0.4.7/trl/trainer/sft_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                 if getattr(model, "is_loaded_in_8bit", False) or getattr(model, "is_loaded_in_4bit", False):
                     model = prepare_model_for_int8_training(model)
 
                 model = get_peft_model(model, peft_config)
 
             if callbacks is None:
                 callbacks = [PeftSavingCallback]
-        elif not isinstance(model, PreTrainedModel):
+        elif not isinstance(model, (PreTrainedModel, PeftModel)):
             model = AutoModelForCausalLM.from_pretrained(model)
 
         if tokenizer is None:
             tokenizer = AutoTokenizer.from_pretrained(model.config._name_or_path)
             if getattr(tokenizer, "pad_token", None) is None:
                 tokenizer.pad_token = tokenizer.eos_token
 
@@ -224,98 +224,71 @@
         dataset_text_field,
         max_seq_length,
         formatting_func,
         infinite,
         num_of_sequences,
         chars_per_token,
     ):
+        if dataset is None:
+            raise ValueError("The dataset should not be None")
+
         # check if torch dataset / dataloader and do nothing
-        if dataset is not None and (
-            isinstance(
-                dataset,
-                (torch.utils.data.IterableDataset, torch.utils.data.Dataset),
-            )
-        ):
-            is_already_dataset = True
-        elif dataset is not None and isinstance(dataset, ConstantLengthDataset):
-            is_already_dataset = True
-            packing = True
-        else:
-            is_already_dataset = False
+        if isinstance(dataset, (torch.utils.data.IterableDataset, torch.utils.data.Dataset, ConstantLengthDataset)):
+            return dataset
 
         if not packing:
-            dataset = self._prepare_non_packed_dataloader(
+            return self._prepare_non_packed_dataloader(
                 tokenizer, dataset, dataset_text_field, max_seq_length, formatting_func
             )
 
-            is_already_dataset = True
-
-        if not is_already_dataset and (dataset_text_field is not None or formatting_func is not None):
+        if dataset_text_field is not None or formatting_func is not None:
             if tokenizer is None:
                 raise ValueError(
                     "You need to pass a tokenizer when using the SFT Trainer when passing a `dataset_text_field`."
                 )
 
-            dataset = ConstantLengthDataset(
+            return ConstantLengthDataset(
                 tokenizer,
                 dataset,
                 dataset_text_field=dataset_text_field,
                 formatting_func=formatting_func,
                 seq_length=max_seq_length,
                 infinite=infinite,
                 num_of_sequences=num_of_sequences,
                 chars_per_token=chars_per_token,
                 eos_token_id=tokenizer.eos_token_id,
             )
 
-        elif not is_already_dataset and (dataset_text_field is None and formatting_func is None):
-            raise ValueError(
-                "You need to pass a `dataset_text_field` or `formatting_func` argument to the SFTTrainer if you want to use the `ConstantLengthDataset`."
-            )
-
-        return dataset
+        raise ValueError(
+            "You need to pass a `dataset_text_field` or `formatting_func` argument to the SFTTrainer if you want to use the `ConstantLengthDataset`."
+        )
 
     def _prepare_non_packed_dataloader(
         self, tokenizer, dataset, dataset_text_field, max_seq_len, formatting_func=None
     ):
         use_formatting_func = formatting_func is not None and dataset_text_field is None
         self._dataset_sanity_checked = False
 
         # Inspired from: https://huggingface.co/learn/nlp-course/chapter7/6?fw=pt
         def tokenize(element):
-            input_batch = []
-            attention_masks = []
-
             outputs = tokenizer(
                 element[dataset_text_field] if not use_formatting_func else formatting_func(element),
                 truncation=True,
-                padding=True,
+                padding=False,
                 max_length=max_seq_len,
                 return_overflowing_tokens=False,
-                return_length=True,
+                return_length=False,
             )
 
             if use_formatting_func and not self._dataset_sanity_checked:
                 if not isinstance(formatting_func(element), list):
                     raise ValueError(
                         "The `formatting_func` should return a list of processed strings since it can lead to silent bugs."
                     )
                 else:
                     self._dataset_sanity_checked = True
 
-            for length, input_ids, attention_mask in zip(
-                outputs["length"], outputs["input_ids"], outputs["attention_mask"]
-            ):
-                if length == max_seq_len:
-                    input_batch.append(input_ids)
-                    attention_masks.append(attention_mask)
-
-            if len(input_batch) == 0:
-                # warn users
-                warnings.warn(
-                    f"Found 0 samples with a length of {max_seq_len}. You might want to decrease the `max_seq_len` argument."
-                )
-            return {"input_ids": input_batch, "attention_mask": attention_masks}
+            return {"input_ids": outputs["input_ids"], "attention_mask": outputs["attention_mask"]}
 
         tokenized_dataset = dataset.map(tokenize, batched=True, remove_columns=dataset.column_names)
 
         return tokenized_dataset
```

### Comparing `trl-0.4.6/trl/trainer/utils.py` & `trl-0.4.7/trl/trainer/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,17 +48,33 @@
         self.value = kl_coef
 
     def update(self, current, n_steps):
         pass
 
 
 class DataCollatorForCompletionOnlyLM(DataCollatorForLanguageModeling):
-    def __init__(self, response_template, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    """
+    Data collator used for completion tasks. It ensures that all the tokens of the labels are set to an 'ignore_index'
+     up to the prompt response template tokens ('response_template'). This ensure that the loss is only
+     calculated on the completion of the reponse.
+
+    Args:
+        response_template (`str`): the template form that indicates the start of the response, typically something like
+            '### Response:\n'
+        mlm (`bool`, *optional*, defaults to `False`): Whether or not to use masked language modeling in the underlying
+            `DataCollatorForLanguageModeling` class. Note that this option currently has no effect but is present
+             for flexibility and backwards-compatibility.
+        ignore_index (`int`, *optional*, defaults to `-100`):
+            The index to use to ignore the initial tokens with
+    """
+
+    def __init__(self, response_template: str, *args, mlm: bool = False, ignore_index: int = -100, **kwargs):
+        super().__init__(*args, mlm=mlm, **kwargs)
         self.response_template = response_template
+        self.ignore_index = ignore_index
 
     def torch_call(self, examples: List[Union[List[int], Any, Dict[str, Any]]]) -> Dict[str, Any]:
         batch = super().torch_call(examples)
 
         # The prompt ends with the response key plus a newline.  We encode this and then try to find it in the
         # sequence of tokens.  This should just be a single token.
         response_token_ids = self.tokenizer.encode(self.response_template, add_special_tokens=False)
@@ -77,15 +93,15 @@
                 raise RuntimeError(
                     f'Could not find response key {response_token_ids} in token IDs {batch["labels"][i]}'
                 )
 
             response_token_ids_end_idx = response_token_ids_start_idx + len(response_token_ids)
 
             # Make pytorch loss function ignore all tokens up through the end of the response key
-            labels[i, :response_token_ids_end_idx] = -100
+            labels[i, :response_token_ids_end_idx] = self.ignore_index
 
         batch["labels"] = labels
 
         return batch
 
 
 @dataclass
@@ -183,27 +199,30 @@
                 Length of token sequences to return.
             num_of_sequences (`int`, *optional*, defaults to `1024`):
                 Number of token sequences to keep in buffer.
             chars_per_token (`int`, *optional*, defaults to `3.6`):
                 Number of characters per token used to estimate number of tokens in text buffer.
             eos_token_id (`int`, *optional*, defaults to `0`):
                 Id of the end of sequence token if the passed tokenizer does not have an EOS token.
+            shuffle ('bool', *optional*, defaults to True)
+                Shuffle the examples before they are returned
     """
 
     def __init__(
         self,
         tokenizer,
         dataset,
         dataset_text_field=None,
         formatting_func=None,
         infinite=False,
         seq_length=1024,
         num_of_sequences=1024,
         chars_per_token=3.6,
         eos_token_id=0,
+        shuffle=True,
     ):
         self.tokenizer = tokenizer
 
         if tokenizer.eos_token_id is None:
             warnings.warn(
                 "The passed tokenizer does not have an EOS token. We will use the passed eos_token_id instead which corresponds"
                 f" to {eos_token_id}. If this is not the correct EOS token, make sure to pass the correct eos_token_id."
@@ -211,14 +230,15 @@
 
         self.concat_token_id = tokenizer.eos_token_id if tokenizer.eos_token_id else eos_token_id
         self.dataset = dataset
         self.seq_length = seq_length
         self.infinite = infinite
         self.current_size = 0
         self.max_buffer_size = seq_length * chars_per_token * num_of_sequences
+        self.shuffle = shuffle
         if formatting_func is None:
             self.formatting_func = lambda x: x[dataset_text_field]
         else:
             self.formatting_func = formatting_func
 
         if formatting_func is not None:
             formatting_func_signature = formatting_func.__code__.co_varnames
@@ -254,15 +274,16 @@
             for tokenized_input in tokenized_inputs:
                 all_token_ids.extend(tokenized_input + [self.concat_token_id])
             examples = []
             for i in range(0, len(all_token_ids), self.seq_length):
                 input_ids = all_token_ids[i : i + self.seq_length]
                 if len(input_ids) == self.seq_length:
                     examples.append(input_ids)
-            random.shuffle(examples)
+            if self.shuffle:
+                random.shuffle(examples)
             for example in examples:
                 self.current_size += 1
                 yield {
                     "input_ids": torch.LongTensor(example),
                     "labels": torch.LongTensor(example),
                 }
```

### Comparing `trl-0.4.6/trl.egg-info/SOURCES.txt` & `trl-0.4.7/trl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

