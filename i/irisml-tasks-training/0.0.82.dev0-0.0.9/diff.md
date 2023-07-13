# Comparing `tmp/irisml-tasks-training-0.0.82.dev0.tar.gz` & `tmp/irisml-tasks-training-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-training-0.0.82.dev0.tar", last modified: Thu Jul 13 08:55:41 2023, max compression
+gzip compressed data, was "irisml-tasks-training-0.0.9.tar", last modified: Wed Aug 10 05:23:37 2022, max compression
```

## Comparing `irisml-tasks-training-0.0.82.dev0.tar` & `irisml-tasks-training-0.0.9.tar`

### file list

```diff
@@ -1,113 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:41.617675 irisml-tasks-training-0.0.82.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-07-13 08:55:41.617675 irisml-tasks-training-0.0.82.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:41.601674 irisml-tasks-training-0.0.82.dev0/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:41.609675 irisml-tasks-training-0.0.82.dev0/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/append_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/benchmark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/benchmark_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/benchmark_model_with_grad_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/build_classification_prompt_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/build_zero_shot_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/concatenate_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/create_classification_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/evaluate_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/evaluate_detection_average_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/exclude_negative_samples_from_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/find_incorrect_classification_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/find_incorrect_classification_multilabel_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/get_subclass_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/get_targets_from_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/load_simple_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_classification_dataset_from_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_classification_dataset_from_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_classification_dataset_with_extra_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_feature_extractor_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_fixed_prompt_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_fixed_text_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_image_text_contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_image_text_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_oversampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_prompt_image_list_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_prompt_list_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/num_iters_to_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/remove_empty_images_from_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/sample_few_shot_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/split_image_text_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:41.609675 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/build_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/build_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/build_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/ddp_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/ddp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugin_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugin_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:41.613675 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/clip_grad_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/detect_anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/fp16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/freeze_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/freeze_modules_upto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/log_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/log_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/nop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/scale_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/step_decay_ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/irisml/tasks/train_with_gradient_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:41.613675 irisml-tasks-training-0.0.82.dev0/irisml_tasks_training.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-07-13 08:55:41.000000 irisml-tasks-training-0.0.82.dev0/irisml_tasks_training.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-13 08:55:41.000000 irisml-tasks-training-0.0.82.dev0/irisml_tasks_training.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:55:41.000000 irisml-tasks-training-0.0.82.dev0/irisml_tasks_training.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 08:55:41.000000 irisml-tasks-training-0.0.82.dev0/irisml_tasks_training.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 08:55:41.000000 irisml-tasks-training-0.0.82.dev0/irisml_tasks_training.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-13 08:55:41.621676 irisml-tasks-training-0.0.82.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:41.617675 irisml-tasks-training-0.0.82.dev0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_append_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_benchmark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_benchmark_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_build_classification_prompt_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_build_zero_shot_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_concatenate_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_create_classification_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_ddp_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_evaluate_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_evaluate_detection_average_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_exclude_negative_samples_from_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_find_incorrect_classification_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_find_incorrect_classification_multilabel_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_get_subclass_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_get_targets_from_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_irisml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_load_simple_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_make_classification_dataset_from_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_make_classification_dataset_from_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_make_feature_extractor_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_make_fixed_prompt_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_make_fixed_text_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_make_image_text_contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_make_image_text_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_make_oversampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_make_prompt_list_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_num_iters_to_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_remove_empty_images_from_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_sample_few_shot_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_split_image_text_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-13 08:52:36.000000 irisml-tasks-training-0.0.82.dev0/test/test_train_with_gradient_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4897 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4612 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.804559 irisml-tasks-training-0.0.9/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.804559 irisml-tasks-training-0.0.9/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/append_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/build_classification_prompt_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/build_zero_shot_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/create_classification_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/evaluate_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/evaluate_detection_average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/get_targets_from_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2160 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/make_feature_extractor_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/make_image_text_contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2563 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/make_image_text_transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/predict.py
+-rw-r--r--   0 runner    (1001) docker     (121)      939 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/split_image_text_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.804559 irisml-tasks-training-0.0.9/irisml/tasks/train/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/build_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/build_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/build_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4622 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/ddp_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/ddp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugin_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/log_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/log_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)      879 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4897 2022-08-10 05:23:37.000000 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-08-10 05:23:37.000000 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 05:23:37.000000 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-10 05:23:37.000000 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-10 05:23:37.000000 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_append_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_build_classification_prompt_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_build_zero_shot_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_create_classification_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4247 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_ddp_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_evaluate_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_evaluate_detection_average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_get_targets_from_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_make_feature_extractor_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_make_image_text_contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_make_image_text_transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_split_image_text_model.py
```

### Comparing `irisml-tasks-training-0.0.82.dev0/LICENSE` & `irisml-tasks-training-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/PKG-INFO` & `irisml-tasks-training-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-training
-Version: 0.0.82.dev0
+Version: 0.0.9
 Summary: IrisML tasks for pytorch training
 Home-page: https://github.com/microsoft/irisml-tasks-training
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,17 +22,14 @@
 
 ### predict
 Run inference with a given pytorch model. Returns prediction results.
 
 ### append_classifier
 Append a classifier layer to an encoder model.
 
-### benchmark_model
-Benchmark a given model.
-
 ### build_classification_prompt_dataset
 Convert a multiclass classification Image Dataset into a dataset with text prompts.
 
 ### build_zero_shot_classifier
 Build a classifier FC layer from text features. See the CLIP repo for the detail.
 
 ### create_classification_prompt_generator
@@ -46,42 +43,27 @@
 
 ### evaluate_detection_average_precision
 Calculate mAP for object detection results.
 
 ### get_targets_from_dataset
 Get a list or a tensor of targets from a Dataset.
 
-### get_subclass_dataset
-Given a list of class ids, extract the sub-dataset of those classes.
-
 ### make_feature_extractor_model
 Make a new model to extract intermediate features from the given model. Use the predict task to run the extractor model.
 
 ### make_image_text_contrastive_model
 Make a new model to run image-text contrastive training like CLIP.
 
 ### make_image_text_transform
 Make a transform function that can be used for a contrastive training
 
-### make_oversampled_dataset
-Oversample from a dataset and return a new dataset
-
 ### split_image_text_model
 Extract image_model and text_model from a image-text model.
 
-### sample_few_shot_dataset
-Sample few-shot dataset from given a shot number and random seed.
-
-### train_with_gradient_cache
-Train a pytorch model using gradient cache. Useful for training a large contrastive model.
-
 # Available plugins for train task.
-- amp
-- clip_grad_norm
-- ema
 - log_summary
 - log_tensorboard
 - progressbar
 
 # Interfaces for training and prediction
 The tasks in this package expects the following interfaces
```

### Comparing `irisml-tasks-training-0.0.82.dev0/README.md` & `irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: irisml-tasks-training
+Version: 0.0.9
+Summary: IrisML tasks for pytorch training
+Home-page: https://github.com/microsoft/irisml-tasks-training
+Author: irisdev
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # irisml-tasks-training
 
 This is a package for IrisML training-related tasks.
 
 See [irisml repository](https://github.com/microsoft/irisml) for the detail of irisml framework.
 
 ## Tasks
@@ -11,17 +22,14 @@
 
 ### predict
 Run inference with a given pytorch model. Returns prediction results.
 
 ### append_classifier
 Append a classifier layer to an encoder model.
 
-### benchmark_model
-Benchmark a given model.
-
 ### build_classification_prompt_dataset
 Convert a multiclass classification Image Dataset into a dataset with text prompts.
 
 ### build_zero_shot_classifier
 Build a classifier FC layer from text features. See the CLIP repo for the detail.
 
 ### create_classification_prompt_generator
@@ -35,42 +43,27 @@
 
 ### evaluate_detection_average_precision
 Calculate mAP for object detection results.
 
 ### get_targets_from_dataset
 Get a list or a tensor of targets from a Dataset.
 
-### get_subclass_dataset
-Given a list of class ids, extract the sub-dataset of those classes.
-
 ### make_feature_extractor_model
 Make a new model to extract intermediate features from the given model. Use the predict task to run the extractor model.
 
 ### make_image_text_contrastive_model
 Make a new model to run image-text contrastive training like CLIP.
 
 ### make_image_text_transform
 Make a transform function that can be used for a contrastive training
 
-### make_oversampled_dataset
-Oversample from a dataset and return a new dataset
-
 ### split_image_text_model
 Extract image_model and text_model from a image-text model.
 
-### sample_few_shot_dataset
-Sample few-shot dataset from given a shot number and random seed.
-
-### train_with_gradient_cache
-Train a pytorch model using gradient cache. Useful for training a large contrastive model.
-
 # Available plugins for train task.
-- amp
-- clip_grad_norm
-- ema
 - log_summary
 - log_tensorboard
 - progressbar
 
 # Interfaces for training and prediction
 The tasks in this package expects the following interfaces
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/append_classifier.py` & `irisml-tasks-training-0.0.9/irisml/tasks/append_classifier.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/build_classification_prompt_dataset.py` & `irisml-tasks-training-0.0.9/irisml/tasks/build_classification_prompt_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 
     def execute(self, inputs):
         text_lists = [(t, i) for i, label in enumerate(inputs.class_names) for t in inputs.prompt_generator(label)]
         logger.debug(f"Created a text dataset. The number of examples: {len(text_lists)}. The number of classes: {len(inputs.class_names)}")
         return self.Outputs(TextListDataset(text_lists))
 
     def dry_run(self, inputs):
-        class_names = inputs.class_names or ['fake_label0', 'fake_label1']
-        text_lists = [(t, i) for i, label in enumerate(class_names) for t in inputs.prompt_generator(label)]
-        return self.Outputs(TextListDataset(text_lists))
+        return self.execute(inputs)
 
 
 class TextListDataset(torch.utils.data.Dataset):
     def __init__(self, text_list: typing.List[typing.Tuple[str, int]]):
         self._data = text_list
 
     def __len__(self):
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/build_zero_shot_classifier.py` & `irisml-tasks-training-0.0.9/irisml/tasks/build_zero_shot_classifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 import irisml.core
 
 logger = logging.getLogger(__name__)
 
 
 class Task(irisml.core.TaskBase):
     """Create a zero-shot classification layer."""
-    VERSION = '0.1.1'
+    VERSION = '0.1.0'
 
     @dataclasses.dataclass
     class Inputs:
         text_features: typing.List[torch.Tensor]
         text_classes: typing.Union[typing.List[int], torch.Tensor]
-        logit_scale: typing.Optional[torch.Tensor] = None
 
     @dataclasses.dataclass
     class Config:
         num_classes: int
 
     @dataclasses.dataclass
     class Outputs:
@@ -40,25 +39,21 @@
                 raise RuntimeError(f"Unexpected class index: {index}")
             features_per_class[index].append(f)
 
         embeddings_per_class = []
         for c in range(self.config.num_classes):
             if features_per_class[c]:
                 class_embeddings = torch.stack(features_per_class[c])
+                class_embeddings /= class_embeddings.norm(dim=-1, keepdim=True)
                 class_embedding = class_embeddings.mean(dim=0)
                 class_embedding /= class_embedding.norm()
             else:
                 logger.warning(f"No features are provided for class {c}. Initializing with zeros.")
                 class_embedding = torch.zeros(*feature_shape)
 
             embeddings_per_class.append(class_embedding)
 
-        weights = torch.stack(embeddings_per_class, dim=1).transpose(0, 1)
-        if inputs.logit_scale:
-            if inputs.logit_scale.nelement() != 1:
-                raise RuntimeError("Unexpected shape of logit_scale")
-            weights *= inputs.logit_scale.exp()
-
+        weights = torch.stack(embeddings_per_class, dim=1).transpose(0, 1)  # TODO: Multiply with logit_scale?
         with torch.no_grad():
             classifier = torch.nn.Linear(weights.shape[1], weights.shape[0], bias=False)
             classifier.weight.copy_(weights)
         return self.Outputs(classifier)
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/evaluate_detection_average_precision.py` & `irisml-tasks-training-0.0.9/irisml/tasks/evaluate_detection_average_precision.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/export_onnx.py` & `irisml-tasks-training-0.0.9/irisml/tasks/export_onnx.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 import torch
 import irisml.core
 
 
 class Task(irisml.core.TaskBase):
     """Export the given model as ONNX."""
-    VERSION = '0.1.1'
+    VERSION = '0.1.0'
 
     @dataclasses.dataclass
     class Inputs:
         model: torch.nn.Module
 
     @dataclasses.dataclass
     class Config:
@@ -22,20 +22,15 @@
 
     class PredictionModel(torch.nn.Module):
         def __init__(self, model):
             super().__init__()
             self._model = model
 
         def forward(self, x):
-            if hasattr(self._model, 'prediction_step'):
-                return self._model.prediction_step(x)
-            elif hasattr(self._model, 'predictor'):
-                return self._model.predictor(self._model(x))
-            else:
-                return self._model(x)
+            return self._model.prediction_step(x)
 
     def execute(self, inputs):
         model = Task.PredictionModel(inputs.model)
         x = torch.randn(1, 3, self.config.input_size, self.config.input_size)
         with io.BytesIO() as bytes_io:
             torch.onnx.export(model, x, bytes_io)
             return self.Outputs(bytes(bytes_io.getbuffer()))
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_feature_extractor_model.py` & `irisml-tasks-training-0.0.9/irisml/tasks/make_feature_extractor_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import irisml.core
 
 
 class Task(irisml.core.TaskBase):
     """Make a wrapper model to extract a feature vector from a vision model.
 
     """
-    VERSION = '0.1.1'
+    VERSION = '0.1.0'
 
     @dataclasses.dataclass
     class Inputs:
         model: torch.nn.Module
 
     @dataclasses.dataclass
     class Config:
@@ -45,28 +45,22 @@
             output_module_name: The name of the module to extract feature vectors.
         """
         super().__init__()
         self._model = model
         self._output_module_name = output_module_name
 
         if output_module_name:
-            self._find_module(self._model, output_module_name)  # Check if the module exists.
+            module = self._find_module(self._model, output_module_name)
+            # Instead of having a plugin to remove the hook, we forget about it. The model shouldn't be reused.
+            module.register_forward_hook(self._save_outputs)
 
     def prediction_step(self, inputs):
         self._features = None
-
-        # Add a forward_hook to extract the feature. The performance overhead should be small.
-        handle = self._find_module(self._model, self._output_module_name).register_forward_hook(self._save_outputs) if self._output_module_name else None
-
         outputs = self._model(inputs)
         outputs = self._features if self._output_module_name else outputs
-
-        if handle:
-            handle.remove()
-
         self._features = None
         return outputs
 
     def _save_outputs(self, module, inputs, outputs):
         if self._features is None:
             self._features = copy.deepcopy(outputs.detach())
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_image_text_contrastive_model.py` & `irisml-tasks-training-0.0.9/irisml/tasks/make_image_text_contrastive_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,18 +92,14 @@
         if loss_name == 'clip':
             self._criterion = CLIPContrastiveCriterion()
         elif loss_name == 'unicl':
             self._criterion = UnifiedContrastiveCriterion()
         else:
             raise RuntimeError
 
-    @property
-    def criterion(self):
-        return self._criterion
-
     def forward(self, inputs):
         image_features = self.image_projection(self.image_model(inputs[0]))
         text_features = self.text_projection(self.text_model(inputs[1]))
 
         image_features = image_features / image_features.norm(p=2, dim=-1, keepdim=True)
         text_features = text_features / text_features.norm(p=2, dim=-1, keepdim=True)
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/make_image_text_transform.py` & `irisml-tasks-training-0.0.9/irisml/tasks/make_image_text_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/num_iters_to_epochs.py` & `irisml-tasks-training-0.0.9/irisml/tasks/get_targets_from_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import dataclasses
-import logging
-import math
-import irisml.core
+import typing
 import torch
-
-logger = logging.getLogger(__name__)
+import irisml.core
 
 
 class Task(irisml.core.TaskBase):
-    """Convert number of iterations to number of epochs. Min value is 1."""
+    """Extract only targets from a given Dataset.
+
+    If the targets are integers or tensors with same shape, a tensor will be returned. Otherwise, returns a list of targets.
+    """
     VERSION = '0.1.0'
 
     @dataclasses.dataclass
     class Inputs:
-        batch_size: int
-        num_iterations: int
         dataset: torch.utils.data.Dataset
 
     @dataclasses.dataclass
     class Outputs:
-        num_epochs: int
+        targets: typing.Union[typing.List, torch.Tensor] = dataclasses.field(default_factory=list)
 
     def execute(self, inputs):
-        num_epochs = max(math.ceil(inputs.batch_size * inputs.num_iterations / len(inputs.dataset)), 1)
-
-        return self.Outputs(num_epochs)
+        targets = [t for _, t in inputs.dataset]
+        if torch.is_tensor(targets[0]):
+            shape = targets[0].shape
+            if all(t.shape == shape for t in targets):
+                targets = torch.stack(targets)
+        elif isinstance(targets[0], int):
+            targets = torch.tensor(targets)
 
-    def dry_run(self, inputs):
-        return self.execute(inputs)
+        return self.Outputs(targets)
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/predict.py` & `irisml-tasks-training-0.0.9/irisml/tasks/predict.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,78 +6,63 @@
 import queue
 import typing
 import torch.nn
 import torch.utils.data
 import irisml.core
 from irisml.tasks.train.build_dataloader import build_dataloader
 from irisml.tasks.train.ddp_utils import spawn_processes, recreate_dataloader_with_new_sampler
-from irisml.tasks.train.plugin_list import PluginList
-from irisml.tasks.train.plugin_loader import load_plugin
-
 
 logger = logging.getLogger(__name__)
 
 
 class Predictor:
-    def __init__(self, model, plugins, device=torch.device('cpu')):
+    def __init__(self, model, device=torch.device('cpu')):
         self._model = model
         self._device = device
         self._predictor = getattr(model, 'predictor', None)
-        self._plugins = plugins
 
     @property
     def device(self):
         return self._device
 
     @torch.no_grad()
     def predict(self, dataloader):
         self._model.to(self.device)
 
         was_training = self._model.training
         self._model.eval()
 
         results = []
         targets = []
-        self._model = self._plugins.on_prediction_start(self, self._model)
-
         for batch_index, batch in enumerate(dataloader):
-            batch = self._plugins.on_prediction_batch_start(self, self._model, batch, batch_index)
             batch_results, batch_targets = self.prediction_step(batch, batch_index)
             results.append(batch_results)
             targets.append(batch_targets)
-            self._plugins.on_prediction_batch_end(self, self._model, batch, batch_index)
-
-        self._model = self._plugins.on_prediction_end(self, self._model)
 
         if was_training:
             self._model.train()
 
         self._model.to(torch.device('cpu'))
-        return self._aggregate_results(results), self._aggregate_results(targets)
+        return self._move_to_cpu(self._aggregate_results(results)), self._move_to_cpu(self._aggregate_results(targets))
 
     def prediction_step(self, batch, batch_index):
         inputs, targets = batch
         inputs = self._to_device(inputs)
-        with self._plugins.forward_context():
-            if hasattr(self._model, 'prediction_step'):
-                batch_results = self._model.prediction_step(inputs)
-            elif self._predictor is not None:
-                outputs = self._model(inputs)
-                batch_results = self._predictor(outputs)
-            else:
-                batch_results = self._model(inputs)
-        batch_results = self._move_to_cpu(batch_results)
+        if hasattr(self._model, 'prediction_step'):
+            batch_results = self._model.prediction_step(inputs)
+        elif self._predictor is not None:
+            outputs = self._model(inputs)
+            batch_results = self._predictor(outputs)
+        else:
+            batch_results = self._model(inputs)
         return batch_results, targets
 
-    def _aggregate_results(self, results: typing.List):
+    def _aggregate_results(self, results):
         if torch.is_tensor(results[0]):
-            if all(results[0].shape[1:] == r.shape[1:] for r in results):
-                return torch.cat(results)
-            else:
-                return list(itertools.chain.from_iterable(list(x) for x in results))
+            return torch.cat(results)
         elif isinstance(results[0], list):
             return list(itertools.chain(*results))
         else:
             raise RuntimeError(f"Unexpected result types: {results[0]}")
 
     def _to_device(self, data):
         if isinstance(data, list):
@@ -87,15 +72,15 @@
         elif hasattr(data, 'to'):
             return data.to(self.device, non_blocking=True)
         return data
 
     @staticmethod
     def _move_to_cpu(value):
         if torch.is_tensor(value):
-            return value.to(torch.device('cpu'), non_blocking=True)
+            return value.to(torch.device('cpu'))
         elif isinstance(value, list):
             return [Predictor._move_to_cpu(x) for x in value]
         elif isinstance(value, (int, float, str)):
             return value
         else:
             raise ValueError(f"Unexpected value type: {type(value)}")
 
@@ -111,17 +96,17 @@
         return self._end_index - self._start_index
 
     def __iter__(self):
         return iter(range(self._start_index, self._end_index))
 
 
 class DistributedPredictor(Predictor):
-    def __init__(self, model, num_processes, plugins, device=torch.device('cpu')):
+    def __init__(self, model, num_processes, device=torch.device('cpu')):
         self._num_processes = num_processes
-        super().__init__(model, plugins, device)
+        super().__init__(model, device)
 
     def predict(self, dataloader):
         mp_queue = multiprocessing.get_context('spawn').JoinableQueue(self._num_processes)
         num_examples_per_process = math.ceil(len(dataloader.dataset) / self._num_processes)
         context = spawn_processes(self._predict_on_new_process, args=(dataloader, num_examples_per_process, mp_queue), nprocs=self._num_processes)
         all_results = {}
 
@@ -164,52 +149,41 @@
         mp_queue.join()
 
 
 class Task(irisml.core.TaskBase):
     """Predict using a given model.
 
     This class assumes that the model.predictor returns a Tensor or a list of results.
-
-    Config:
-        batch_size (int): The batch size
-        device (Optional['cpu' or 'cuda']): The device to run inference
-        num_processes (int): The number of processes to use
-        plugins (List[str]): List of plugins to use
     """
-    VERSION = '0.2.0'
+    VERSION = '0.1.0'
 
     @dataclasses.dataclass
     class Inputs:
         dataset: torch.utils.data.Dataset
+        transform: torch.nn.Module
         model: torch.nn.Module
-        transform: typing.Optional[typing.Callable] = None
 
     @dataclasses.dataclass
     class Config:
         batch_size: int = 1
         device: typing.Optional[typing.Literal['cpu', 'cuda']] = None
         num_processes: int = 1
-        plugins: typing.List[str] = dataclasses.field(default_factory=list)
 
     @dataclasses.dataclass
     class Outputs:
-        predictions: typing.Union[typing.List, torch.Tensor] = dataclasses.field(default_factory=list)
-        targets: typing.Optional[typing.Union[typing.List, torch.Tensor]] = None
+        predictions: typing.List = dataclasses.field(default_factory=list)
+        targets: typing.Optional[typing.List] = None
 
     def execute(self, inputs):
         results = self._predict(inputs)
         return self.Outputs(results[0], results[1])
 
     def _predict(self, inputs):
-        plugins = PluginList([load_plugin(p, self.context) for p in self.config.plugins])
         dataloader = build_dataloader(inputs.dataset, inputs.transform, batch_size=self.config.batch_size, shuffle=False, drop_last=False)
-        if self.config.num_processes == 1:
-            predictor = Predictor(inputs.model, plugins, self._get_device())
-        else:
-            predictor = DistributedPredictor(inputs.model, self.config.num_processes, plugins, self._get_device())
+        predictor = Predictor(inputs.model, self._get_device()) if self.config.num_processes == 1 else DistributedPredictor(inputs.model, self.config.num_processes, self._get_device())
         results = predictor.predict(dataloader)
         if len(inputs.dataset) != len(results[0]):
             raise RuntimeError(f"Couldn't get the expected number of prediction results. Expected: {len(inputs.dataset)}. Actual: {len(results[0])}")
         return results
 
     def _get_device(self) -> torch.device:
         """Get a torch device based on the configuration. If not specified explicitly, it uses cuda if available."""
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/build_dataloader.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/build_dataloader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 import inspect
 import typing
-import torch.multiprocessing
 import torch.utils.data
 
 
 class Dataset(torch.utils.data.Dataset):
     """Dataset wrapper to support both image-only transforms and image-and-targets transforms."""
     def __init__(self, dataset, transform):
         self._dataset = dataset
         self._transform = transform
-        if transform is not None:
-            self._num_transform_args = self._get_num_args(transform)
-            assert 1 <= self._num_transform_args <= 2
-        else:
-            self._num_transform_args = 0
+        self._num_transform_args = self._get_num_args(transform)
+        assert 1 <= self._num_transform_args <= 2
 
     def __len__(self):
         return len(self._dataset)
 
     def __getitem__(self, index):
         item = self._dataset[index]
         assert len(item) == 2
         if self._num_transform_args == 1:
             return self._transform(item[0]), item[1]
         elif self._num_transform_args == 2:
             return self._transform(*item)
-        elif self._num_transform_args == 0:
-            return item
 
     @staticmethod
     def _get_num_args(function):
         args = inspect.getfullargspec(function).args
         if args[0] == 'self':
             return len(args) - 1
         return len(args)
@@ -39,39 +33,32 @@
 def collate(batch) -> typing.List:
     """Handle batching.
 
     Supported batch formats are:
         [(Tensor[C, H, W], int), ...]  # multiclass classification
         [(Tensor[C, H, W], [int, ...]), ...]  # multiclass or multilabel classification
         [(Tensor[C, H, W], Tensor[T]), ...]  # multiclass or multilabel classification
-        [(Tensor[C, H, W], [float, ...]), ...]  # regression
         [(Tensor[C, H, W], [[tag, x, y, x2, y2], ...]), ...]  # object detection
         [(Tensor[C, H, W], Tensor[T, 5]), ...]  # object detection
         [Tensor[C, H, W], ...]  # prediction
-        [((str, [Tensor[C, H, W], ...]), *), ...]  # text generation
     """
 
     if isinstance(batch[0], tuple):
-        if isinstance(batch[0][0], tuple) and isinstance(batch[0][0][0], str):
-            return [[b[0] for b in batch], _collate_targets([b[1] for b in batch])]
-        else:
-            return [_collate_tensor([b[0] for b in batch]), _collate_targets([b[1] for b in batch])]
+        return [_collate_tensor([b[0] for b in batch]), _collate_targets([b[1] for b in batch])]
     elif isinstance(batch[0], torch.Tensor):
         return [_collate_tensor(batch), None]
-    elif isinstance(batch[0], str):
-        return batch
 
     raise TypeError(f"Unexpected type: {type(batch[0])}")
 
 
 def _collate_tensor(batch: typing.List):
     """
-    Expected input types are:
-    - List[Tensor[C, H, W]]
-    - List[Tuple[Tensor[C, H, W], Tensor]]
+    Inputs are:
+        A list of Tensor[C, H, W] or
+        A list of (Tensor[C, H, W], Tensor)
     """
     if isinstance(batch[0], torch.Tensor):
         if all(b.shape == (1,) for b in batch):
             return torch.cat(batch)
 
         if all(batch[0].shape == b.shape for b in batch):
             return torch.stack(batch, 0)
@@ -81,40 +68,26 @@
         # For image-text dataset.
         return _collate_tensor([b[0] for b in batch]), _collate_tensor([b[1] for b in batch])
 
     raise TypeError(f"Unexpected type: {type(batch[0])}")
 
 
 def _collate_targets(batch: typing.List):
-    if all(b is None for b in batch):
-        return batch
-
     if isinstance(batch[0], torch.Tensor):
         return _collate_tensor(batch)
 
     if isinstance(batch[0], list):
         if any(b and isinstance(b[0], (list, tuple)) for b in batch):  # batch = [[[...], ...], ...]
             return [torch.tensor(b).reshape(-1, 5) for b in batch]
-        elif any(b and isinstance(b[0], (int, float)) for b in batch):  # batch = [[int, ...], ...]
+        elif any(b and isinstance(b[0], int) for b in batch):  # batch = [[int, ...], ...]
             return _collate_tensor([torch.tensor(b) for b in batch])
-        elif any(x and all(isinstance(y, str) for y in x) for x in batch):  # caption
-            return batch
-        elif any(x and all(len(y) == 2 and isinstance(y[0], str) and isinstance(y[1], int) for y in x) for x in batch):  # image-text matching
-            return batch
         elif not any(batch):
             return batch
     elif isinstance(batch[0], int):
         return torch.tensor(batch)
 
     raise TypeError(f"Unexpected target type: {batch}")
 
 
-def build_dataloader(dataset, transform, batch_size: int, num_processes: int = 1, num_workers: int = 4, shuffle=True, drop_last=True):
-    """Build a DataLoader class.
-
-    If the dataset is smaller than batch_size*num_processes, it will oversample the dataset so that there is at least one batch per epoch.
-    """
+def build_dataloader(dataset, transform, batch_size: int, shuffle=True, drop_last=True):
     my_dataset = Dataset(dataset, transform)
-    sampler = (torch.utils.data.RandomSampler(my_dataset, replacement=(batch_size * num_processes) > len(dataset), num_samples=max(batch_size * num_processes, len(dataset))) if shuffle
-               else torch.utils.data.SequentialSampler(my_dataset))
-    return torch.utils.data.DataLoader(my_dataset, batch_size=batch_size, num_workers=num_workers, sampler=sampler, drop_last=drop_last,
-                                       pin_memory=True, collate_fn=collate, multiprocessing_context=torch.multiprocessing.get_context('fork'))
+    return torch.utils.data.DataLoader(my_dataset, batch_size=batch_size, num_workers=4, shuffle=shuffle, drop_last=drop_last, pin_memory=True, collate_fn=collate)
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/ddp_trainer.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/ddp_trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,86 @@
 import logging
 import multiprocessing
 import os
 import queue
 import torch
-from .ddp_utils import create_distributed_data_parallel_model, spawn_and_wait, recreate_dataloader_with_distributed_sampler
+from .ddp_utils import spawn_and_wait, recreate_dataloader_with_distributed_sampler
 from .trainer import Trainer
 from .plugins.ddp import Plugin as DDPPlugin
 
 logger = logging.getLogger(__name__)
 
 
 class DDPTrainer(Trainer):
     """Train with DistributedDataParallel.
 
     This class assumes single-node multi-device environment.
     """
-    def __init__(self, model, lr_scheduler_factory, optimizer_factory, plugins=None, device=torch.device('cpu'), val_check_interval=None, accumulate_grad_batches=None, num_processes=2,
-                 find_unused_parameters=False):
+    def __init__(self, model, lr_scheduler_factory, optimizer_factory, plugins=None, device=torch.device('cpu'), val_check_interval=None, num_processes=2):
         plugins = plugins or []
         plugins.append(DDPPlugin())
-        super().__init__(model, lr_scheduler_factory, optimizer_factory, plugins, device, val_check_interval, accumulate_grad_batches)
+        super().__init__(model, lr_scheduler_factory, optimizer_factory, plugins, device, val_check_interval)
         if device.type == 'cuda' and torch.cuda.is_available() and num_processes > torch.cuda.device_count():
             raise RuntimeError(f"Distributed training is used with {num_processes} processes, but there are only {torch.cuda.device_count()} devices.")
         if num_processes == 1:
             raise RuntimeError("At least 2 processes are required for DDP training.")
 
         if device.type == 'cuda':
             # Crashes the process on errors. This setting has very little performance overhead.
             os.environ['NCCL_ASYNC_ERROR_HANDLING'] = '1'
 
         logger.info(f"Distributed training with {num_processes} processes.")
         self._num_processes = num_processes
-        self._find_unused_parameters = find_unused_parameters
 
     def train(self, train_dataloader, val_dataloader, num_epochs):
         """Spawn processes and run training on each process.
 
         To send tensors from a child process, the process must be kept alive until the tensors are loaded on the main process.
         """
         mp_queue = multiprocessing.get_context('spawn').JoinableQueue(1)
 
-        if self.device.type == 'cuda':
-            torch.cuda.empty_cache()  # Needs to remove the cache on this process since it is not usable from the new processes.
-
         context = spawn_and_wait(self._train_on_new_process, args=(train_dataloader, val_dataloader, num_epochs, mp_queue), nprocs=self._num_processes)
 
         logger.info("At least one of the child processes has completed. Now waiting for the outputs.")
 
         try:
             state_dict = mp_queue.get(timeout=60)  # If it couldn't get the state_dict in 60 seconds, something wrong must have happend.
-            try:
-                logger.info(list(state_dict.keys()))
-                self.model.load_state_dict(state_dict)
-            finally:
-                mp_queue.task_done()  # Terminate the child process after loading the state_dict.
+            self.model.load_state_dict(state_dict)
+            mp_queue.task_done()  # Terminate the child process after loading the state_dict.
         except queue.Empty:
             context.join(1)  # If there was an exception information, let the library handle it.
             raise RuntimeError("Failed to get a trained model from the child process.")
 
         context.join()
 
     def _train_on_new_process(self, process_index, train_dataloader, val_dataloader, num_epochs, mp_queue):
         """Method that runs on a new process.
 
         This method returns immediately after the training if process_index != 0. If process_index == 0, it will wait for the main process to read the trained state_dict.
         """
         device_id = [process_index] if self._device.type == 'cuda' else None
         if self._device.type == 'cuda':
             self._device = torch.device('cuda', process_index)
-            torch.cuda.set_device(process_index)
 
         backend = 'gloo' if device_id is None else 'nccl'
         logger.info(f"New process started on device {self._device}. backend={backend}, rank={process_index}")
         torch.distributed.init_process_group(backend, rank=process_index, world_size=self._num_processes)
         logger.info(f"Initialized the process group on rank {process_index}.")
 
         # The model needs to be on the target device. Otherwise, DistributedDataParallel() will stuck.
         self._model.to(self._device)
 
-        self._model = create_distributed_data_parallel_model(self.model, device_id, find_unused_parameters=self._find_unused_parameters)
+        # TODO: we might need to set find_unused_parameters=True if there are models that require such settings.
+        self._model = torch.nn.parallel.DistributedDataParallel(self.model, device_ids=device_id)
 
         distributed_train_dataloader = recreate_dataloader_with_distributed_sampler(train_dataloader)
         distributed_val_dataloader = val_dataloader and recreate_dataloader_with_distributed_sampler(val_dataloader)
 
         super().train(distributed_train_dataloader, distributed_val_dataloader, num_epochs)
 
         if process_index == 0:
             # All processes have the same model at this point. Sending it to the main process from the 0th process.
-            state_dict = self._model.module.to(torch.device('cpu')).state_dict()
+            state_dict = self._model.to(torch.device('cpu')).state_dict()
+            torch.nn.modules.utils.consume_prefix_in_state_dict_if_present(state_dict, 'module.')
             logger.debug("Sending the state_dict from the process 0")
             mp_queue.put(state_dict)
             mp_queue.join()  # Wait until the state_dict is loaded by the main process.
-
-        logger.info(f"Process {process_index} is completed.")
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugin_list.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/plugin_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,61 @@
-import contextlib
-
-
 class PluginList:
-    """Provides a single Plugin interface for a list of plugins."""
     def __init__(self, plugins):
         self._plugins = plugins
 
     def on_train_start(self, trainer, model):
         for plugin in self._plugins:
-            maybe_model = plugin.on_train_start(trainer, model)
-            if maybe_model is not None:
-                model = maybe_model
-        return model
+            if hasattr(plugin, 'on_train_start'):
+                plugin.on_train_start(trainer, model)
 
     def on_train_end(self, trainer, model):
         for plugin in self._plugins:
-            maybe_model = plugin.on_train_end(trainer, model)
-            if maybe_model is not None:
-                model = maybe_model
-        return model
+            if hasattr(plugin, 'on_train_end'):
+                plugin.on_train_end(trainer, model)
 
     def on_train_epoch_start(self, trainer, model, epoch_index):
-        flag = True
         for plugin in self._plugins:
-            flag &= plugin.on_train_epoch_start(trainer, model, epoch_index)
-        return flag
+            if hasattr(plugin, 'on_train_epoch_start'):
+                plugin.on_train_epoch_start(trainer, model, epoch_index)
 
     def on_train_epoch_end(self, trainer, model, epoch_index):
         for plugin in self._plugins:
-            plugin.on_train_epoch_end(trainer, model, epoch_index)
+            if hasattr(plugin, 'on_train_epoch_end'):
+                plugin.on_train_epoch_end(trainer, model, epoch_index)
 
     def on_train_batch_start(self, trainer, model, batch, batch_index):
         for plugin in self._plugins:
-            batch = plugin.on_train_batch_start(trainer, model, batch, batch_index)
+            if hasattr(plugin, 'on_train_batch_start'):
+                batch = plugin.on_train_batch_start(trainer, model, batch, batch_index)
         return batch
 
     def on_train_batch_end(self, trainer, model, loss, batch, batch_index):
         for plugin in self._plugins:
-            plugin.on_train_batch_end(trainer, model, loss, batch, batch_index)
+            if hasattr(plugin, 'on_train_batch_end'):
+                plugin.on_train_batch_end(trainer, model, loss, batch, batch_index)
 
     def on_train_backward_start(self, trainer, model, loss):
         for plugin in self._plugins:
-            loss = plugin.on_train_backward_start(trainer, model, loss)
+            if hasattr(plugin, 'on_train_backward_start'):
+                loss = plugin.on_train_backward_start(trainer, model, loss)
         return loss
 
-    def on_train_backward_end(self, trainer, model):
-        for plugin in self._plugins:
-            plugin.on_train_backward_end(trainer, model)
-
-    def on_optimizer_step_start(self, trainer, model, optimizer):
-        for plugin in self._plugins:
-            optimizer = plugin.on_optimizer_step_start(trainer, model, optimizer)
-        return optimizer
-
     def on_validation_start(self, trainer, model):
         for plugin in self._plugins:
-            plugin.on_validation_start(trainer, model)
+            if hasattr(plugin, 'on_validation_start'):
+                plugin.on_validation_start(trainer, model)
 
     def on_validation_end(self, trainer, model):
         for plugin in self._plugins:
-            plugin.on_validation_end(trainer, model)
+            if hasattr(plugin, 'on_validation_end'):
+                plugin.on_validation_end(trainer, model)
 
     def on_validation_batch_start(self, trainer, model, batch, batch_index):
         for plugin in self._plugins:
-            batch = plugin.on_validation_batch_start(trainer, model, batch, batch_index)
+            if hasattr(plugin, 'on_validation_batch_start'):
+                batch = plugin.on_validation_batch_start(trainer, model, batch, batch_index)
         return batch
 
     def on_validation_batch_end(self, trainer, model, loss, batch, batch_index):
         for plugin in self._plugins:
-            plugin.on_validation_batch_end(trainer, model, loss, batch, batch_index)
-
-    def on_prediction_start(self, trainer, model):
-        for plugin in self._plugins:
-            maybe_model = plugin.on_prediction_start(trainer, model)
-            if maybe_model is not None:
-                model = maybe_model
-        return model
-
-    def on_prediction_end(self, trainer, model):
-        for plugin in self._plugins:
-            maybe_model = plugin.on_prediction_end(trainer, model)
-            if maybe_model is not None:
-                model = maybe_model
-        return model
-
-    def on_prediction_batch_start(self, trainer, model, batch, batch_index):
-        for plugin in self._plugins:
-            batch = plugin.on_prediction_batch_start(trainer, model, batch, batch_index)
-        return batch
-
-    def on_prediction_batch_end(self, trainer, model, batch, batch_index):
-        for plugin in self._plugins:
-            plugin.on_prediction_batch_end(trainer, model, batch, batch_index)
-
-    @contextlib.contextmanager
-    def forward_context(self):
-        with contextlib.ExitStack() as stack:
-            for plugin in self._plugins:
-                if hasattr(plugin, 'forward_context'):
-                    ctx = plugin.forward_context()
-                    if ctx:
-                        stack.enter_context(ctx)
-            yield
+            if hasattr(plugin, 'on_validation_batch_end'):
+                plugin.on_validation_batch_end(trainer, model, loss, batch, batch_index)
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/log_summary.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/log_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,51 +8,38 @@
 
 class Plugin(PluginBase):
     def on_train_epoch_start(self, trainer, model, epoch_index):
         self._epoch_sum_loss = 0
         self._epoch_num_samples = 0
         self._num_iters = 0
         self._epoch_start = time.time()
-        return True
 
     def on_train_epoch_end(self, trainer, model, epoch_index):
-        if not self._epoch_num_samples:
-            logger.info(f"Epoch {epoch_index}: No iterations.")
-            return
-
         loss = self._epoch_sum_loss / self._epoch_num_samples
         training_time = time.time() - self._epoch_start
         log = f"Epoch {epoch_index}: Training loss: {loss:.4f}, time: {training_time:.2f}s, iteration: {self._num_iters}"
         if trainer.device.type == 'cuda':
             total_memory = torch.cuda.get_device_properties(trainer.device).total_memory // (1024 * 1024)
             max_allocated = torch.cuda.max_memory_allocated(trainer.device) // (1024 * 1024)
             torch.cuda.reset_peak_memory_stats(trainer.device)
             log += f", CUDA max memory: {max_allocated}/{total_memory} MB"
         logger.info(log)
 
-    def on_train_backward_start(self, trainer, model, loss):
-        # Get a loss in this method since some other plugins can modify the loss.
-        self._batch_loss = float(loss.item())
-        return loss
-
     def on_train_batch_end(self, trainer, model, loss, batch, batch_index):
-        self._epoch_sum_loss += self._batch_loss * len(batch[0])
+        self._epoch_sum_loss += float(loss.item()) * len(batch[0])
         self._epoch_num_samples += len(batch[0])
         self._num_iters += 1
+        return loss
 
     def on_validation_start(self, trainer, model):
         self._validation_sum_loss = 0
         self._validation_num_samples = 0
         self._validation_num_iters = 0
 
     def on_validation_batch_end(self, trainer, model, loss, batch, batch_index):
         self._validation_sum_loss += float(loss.item()) * len(batch[0])
         self._validation_num_samples += len(batch[0])
         self._validation_num_iters += 1
 
     def on_validation_end(self, trainer, model):
-        if not self._validation_num_samples:
-            logger.info("Validation: No iterations.")
-            return
-
         loss = self._validation_sum_loss / self._validation_num_samples
         logger.info(f"Validation loss: {loss:.4f}, iteration: {self._validation_num_iters}")
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/log_tensorboard.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/log_tensorboard.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/plugins/progressbar.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/progressbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,12 +39,11 @@
         if not self._disabled:
             self._epoch_progressbar.close()
             self._training_progressbar.update(1)
 
     def on_train_epoch_start(self, trainer, model, epoch_index):
         if not self._disabled:
             self._epoch_progressbar = tqdm.tqdm(total=len(trainer.train_dataloader), position=1, leave=None, disable=None)
-        return True
 
     def on_train_batch_end(self, trainer, model, loss, batch, batch_index):
         if not self._disabled:
             self._epoch_progressbar.update(1)
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml/tasks/train/trainer.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/trainer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import logging
-import math
 import torch
 from .plugin_list import PluginList
 
 logger = logging.getLogger(__name__)
 
 
 class Trainer:
-    N_LOSS_NAN_TOLERANCE = 5
-
-    def __init__(self, model, lr_scheduler_factory, optimizer_factory, plugins=None, device=torch.device('cpu'), val_check_interval=None, accumulate_grad_batches=None):
+    def __init__(self, model, lr_scheduler_factory, optimizer_factory, plugins=None, device=torch.device('cpu'), val_check_interval=None):
         """Initialize the trainer class.
 
         Args:
             model (torch.nn.Module): Target model.
             optimizer_factory ((parameters) => torch.optim.Optimizer): A function to instantiate an optimizer.
             val_check_interval (int or float): validate() will be called every N epochs. If val_check_interval is float, N = int(num_epochs * val_check_interval).
         """
@@ -21,19 +18,18 @@
         self._lr_scheduler_factory = lr_scheduler_factory
         self._optimizer_factory = optimizer_factory
         self._optimizer = None
         model_plugins = model.plugins if hasattr(model, 'plugins') else []
         self._plugins = PluginList(model_plugins + (plugins or []))
         self._device = device
         self._val_check_interval = val_check_interval
-        self._accumulate_grad_batches = accumulate_grad_batches
         self.criterion = getattr(model, 'criterion', None)
-        self._nan_loss_cnt = 0
+
         if not hasattr(self.model, 'training_step') and not self.criterion:
-            raise RuntimeError(f"A model must provide training_step() method or a criterion property. model={type(self.model)}")
+            raise RuntimeError("A model must provide training_step() method or a criterion property.")
 
     @property
     def model(self):
         """Returns a model instance. It is on the target device during a training phase."""
         return self._model
 
     @property
@@ -48,100 +44,72 @@
     def train(self, train_dataloader, val_dataloader, num_epochs):
         # Saving to instance varialbes so that the plugins can access them.
         self.num_epochs = num_epochs
         self.train_dataloader = train_dataloader
         self.val_dataloader = val_dataloader
 
         self.model.to(self.device)
+        self.model.train()
 
-        self._optimizer = self._optimizer_factory(self.model)
+        self._optimizer = self._optimizer_factory(self.model.parameters())
         self._lr_scheduler = self._lr_scheduler_factory(self._optimizer)
 
         if self.criterion:
             self.criterion.to(self.device)
 
         val_interval = 0 if not self._val_check_interval else (self._val_check_interval if isinstance(self._val_check_interval, int) else num_epochs * self._val_check_interval)
 
-        self._model = self._plugins.on_train_start(self, self.model)
+        self._plugins.on_train_start(self, self.model)
         for epoch in range(num_epochs):
-            self.model.train()
-            if not self.train_epoch(train_dataloader, epoch):
-                break
+            self._train_epoch(train_dataloader, epoch)
             if val_interval and epoch % val_interval == 0:
-                self.model.eval()
                 self.validate(val_dataloader)
 
         self._plugins.on_train_end(self, self.model)
         self.model.to(torch.device('cpu'))
-        self.model.train()
         self._optimizer = None
         self._lr_scheduler = None
 
     @torch.no_grad()
     def validate(self, val_dataloader):
+        self.model.eval()
         outputs = []
         self._plugins.on_validation_start(self, self.model)
         for batch_index, batch in enumerate(val_dataloader):
             batch = self._plugins.on_validation_batch_start(self, self.model, batch, batch_index)
             loss = self.training_step(batch, batch_index)
             outputs.append(loss)
             self._plugins.on_validation_batch_end(self, self.model, loss, batch, batch_index)
 
         self._plugins.on_validation_end(self, self.model)
+        self.model.train()
         return outputs
 
-    def train_epoch(self, dataloader, epoch):
-        """Train for an epoch.
-
-        Returns: False if the training should be stopped.
-        """
-        if not self._plugins.on_train_epoch_start(self, self.model, epoch):
-            self._plugins.on_train_epoch_end(self, self.model, epoch)
-            return False
-
-        # Resetting the gradients at every epoch.
-        self._optimizer.zero_grad()
-
-        if self._nan_loss_cnt > self.N_LOSS_NAN_TOLERANCE:  # there is a bug where loss occasionally becomes nan, and grad clip recovers it
-            logger.warning(f'Training has diverged and failed: loss stuck in NaN for more than {self.N_LOSS_NAN_TOLERANCE} epochs.')
-            self._plugins.on_train_epoch_end(self, self.model, epoch)
-            return False
+    def _train_epoch(self, dataloader, epoch):
+        self._plugins.on_train_epoch_start(self, self.model, epoch)
 
         for batch_index, batch in enumerate(dataloader):
+            self._optimizer.zero_grad()
             batch = self._plugins.on_train_batch_start(self, self.model, batch, batch_index)
             loss = self.training_step(batch, batch_index)
             loss = self._plugins.on_train_backward_start(self, self.model, loss)
             loss.backward()
-            self._plugins.on_train_backward_end(self, self.model)
-
-            if not self._accumulate_grad_batches or (batch_index + 1) % self._accumulate_grad_batches == 0:
-                # On gradient accumulation, ignore the remainder batches for implementation simplicity.
-                optimizer = self._plugins.on_optimizer_step_start(self, self.model, self._optimizer)
-                optimizer.step()
-                self._optimizer.zero_grad()
-
+            self._optimizer.step()
             self._plugins.on_train_batch_end(self, self.model, loss, batch, batch_index)
-            self._lr_scheduler.step()
-
-            if math.isnan(loss):
-                self._nan_loss_cnt += 1
-            else:
-                self._nan_loss_cnt = 0
 
+        self._lr_scheduler.step()
         self._plugins.on_train_epoch_end(self, self.model, epoch)
-        return True
 
     def training_step(self, batch, batch_index) -> torch.Tensor:
         inputs, targets = self._to_device(batch)
-        with self._plugins.forward_context():
-            if hasattr(self.model, 'training_step'):
-                loss = self.model.training_step(inputs, targets)['loss']
-            else:
-                outputs = self.model(inputs)
-                loss = self.criterion(outputs, targets)
+        if hasattr(self.model, 'training_step'):
+            loss = self.model.training_step(inputs, targets)['loss']
+        else:
+            outputs = self.model(inputs)
+            loss = self.criterion(outputs, targets)
         return loss
 
     def _to_device(self, data):
         if isinstance(data, list):
             return [self._to_device(d) for d in data]
         elif isinstance(data, tuple):
             return tuple(self._to_device(d) for d in data)
```

### Comparing `irisml-tasks-training-0.0.82.dev0/irisml_tasks_training.egg-info/PKG-INFO` & `irisml-tasks-training-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: irisml-tasks-training
-Version: 0.0.82.dev0
-Summary: IrisML tasks for pytorch training
-Home-page: https://github.com/microsoft/irisml-tasks-training
-Author: irisdev
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # irisml-tasks-training
 
 This is a package for IrisML training-related tasks.
 
 See [irisml repository](https://github.com/microsoft/irisml) for the detail of irisml framework.
 
 ## Tasks
@@ -22,17 +11,14 @@
 
 ### predict
 Run inference with a given pytorch model. Returns prediction results.
 
 ### append_classifier
 Append a classifier layer to an encoder model.
 
-### benchmark_model
-Benchmark a given model.
-
 ### build_classification_prompt_dataset
 Convert a multiclass classification Image Dataset into a dataset with text prompts.
 
 ### build_zero_shot_classifier
 Build a classifier FC layer from text features. See the CLIP repo for the detail.
 
 ### create_classification_prompt_generator
@@ -46,42 +32,27 @@
 
 ### evaluate_detection_average_precision
 Calculate mAP for object detection results.
 
 ### get_targets_from_dataset
 Get a list or a tensor of targets from a Dataset.
 
-### get_subclass_dataset
-Given a list of class ids, extract the sub-dataset of those classes.
-
 ### make_feature_extractor_model
 Make a new model to extract intermediate features from the given model. Use the predict task to run the extractor model.
 
 ### make_image_text_contrastive_model
 Make a new model to run image-text contrastive training like CLIP.
 
 ### make_image_text_transform
 Make a transform function that can be used for a contrastive training
 
-### make_oversampled_dataset
-Oversample from a dataset and return a new dataset
-
 ### split_image_text_model
 Extract image_model and text_model from a image-text model.
 
-### sample_few_shot_dataset
-Sample few-shot dataset from given a shot number and random seed.
-
-### train_with_gradient_cache
-Train a pytorch model using gradient cache. Useful for training a large contrastive model.
-
 # Available plugins for train task.
-- amp
-- clip_grad_norm
-- ema
 - log_summary
 - log_tensorboard
 - progressbar
 
 # Interfaces for training and prediction
 The tasks in this package expects the following interfaces
```

### Comparing `irisml-tasks-training-0.0.82.dev0/test/test_append_classifier.py` & `irisml-tasks-training-0.0.9/test/test_append_classifier.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/test/test_build_classification_prompt_dataset.py` & `irisml-tasks-training-0.0.9/test/test_build_classification_prompt_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/test/test_build_zero_shot_classifier.py` & `irisml-tasks-training-0.0.9/test/test_build_zero_shot_classifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,29 +14,14 @@
         text_classes = [1, 0, 1, 0]
         inputs = Task.Inputs(text_features, text_classes)
         outputs = Task(Task.Config(num_classes=2)).execute(inputs)
 
         self.assertEqual(torch.argmax(outputs.classifier(one_feature)), 1)
         self.assertEqual(torch.argmax(outputs.classifier(zero_feature)), 0)
 
-    def test_simple_with_logit_scale(self):
-        zero_feature = torch.ones(32)
-        zero_feature[0] = 10
-        one_feature = torch.ones(32)
-        one_feature[1] = 10
-
-        text_features = [one_feature, zero_feature, one_feature, zero_feature]
-        text_classes = [1, 0, 1, 0]
-        logit_scale = torch.ones([])
-        inputs = Task.Inputs(text_features, text_classes, logit_scale)
-        outputs = Task(Task.Config(num_classes=2)).execute(inputs)
-
-        self.assertEqual(torch.argmax(outputs.classifier(one_feature)), 1)
-        self.assertEqual(torch.argmax(outputs.classifier(zero_feature)), 0)
-
     def test_tensor_classes(self):
         zero_feature = torch.ones(32)
         zero_feature[0] = 10
         one_feature = torch.ones(32)
         one_feature[1] = 10
 
         text_features = [one_feature, zero_feature, one_feature, zero_feature]
```

### Comparing `irisml-tasks-training-0.0.82.dev0/test/test_ddp_trainer.py` & `irisml-tasks-training-0.0.9/test/test_ddp_trainer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import copy
 import unittest
 import torch
 from irisml.tasks.train.ddp_trainer import DDPTrainer
 
-from utils import FakeDataset
+
+class FakeDataset(torch.utils.data.Dataset):
+    def __init__(self, data):
+        self._data = data
+
+    def __getitem__(self, index):
+        return self._data[index]
+
+    def __len__(self):
+        return len(self._data)
 
 
 class FakeModel(torch.nn.Module):
     def __init__(self):
         super().__init__()
         self.model = torch.nn.Conv2d(3, 3, 3)
 
@@ -15,16 +24,16 @@
         return torch.flatten(torch.nn.AdaptiveAvgPool2d(1)(self.model(x)), start_dim=1)
 
     @property
     def criterion(self):
         return torch.nn.CrossEntropyLoss()
 
 
-def fake_optimizer_factory(model):
-    return torch.optim.SGD(model.parameters(), lr=0.01)
+def fake_optimizer_factory(parameters):
+    return torch.optim.SGD(parameters, lr=0.01)
 
 
 def fake_lr_scheduler_factory(optimizer):
     return torch.optim.lr_scheduler.CosineAnnealingWarmRestarts(optimizer, 1)
 
 
 class TestDDPTrainer(unittest.TestCase):
```

### Comparing `irisml-tasks-training-0.0.82.dev0/test/test_evaluate_accuracy.py` & `irisml-tasks-training-0.0.9/test/test_evaluate_accuracy.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,27 +11,13 @@
 
         self.assertEqual(outputs.accuracy, 1.0)
 
         targets = torch.Tensor([2, 1, 1])
         outputs = Task(Task.Config()).execute(Task.Inputs(predictions, targets))
         self.assertEqual(outputs.accuracy, 0.0)
 
-    def test_2d_targets(self):
+    def test_list_targets(self):
         predictions = torch.Tensor([[0.1, 0.2, 0.1], [0.9, 0.2, 0.2], [0.4, 0.4, 0.8]])
         targets = torch.Tensor([[1], [0], [2]])
         outputs = Task(Task.Config()).execute(Task.Inputs(predictions, targets))
 
         self.assertEqual(outputs.accuracy, 1.0)
-
-    def test_1d_predictions(self):
-        predictions = torch.Tensor([1, 0, 2])
-        targets = torch.Tensor([1, 0, 2])
-        outputs = Task(Task.Config()).execute(Task.Inputs(predictions, targets))
-
-        self.assertEqual(outputs.accuracy, 1.0)
-
-    def test_1d_predictions_2d_targets(self):
-        predictions = torch.Tensor([1, 0, 2])
-        targets = torch.Tensor([[1], [0], [2]])
-        outputs = Task(Task.Config()).execute(Task.Inputs(predictions, targets))
-
-        self.assertEqual(outputs.accuracy, 1.0)
```

### Comparing `irisml-tasks-training-0.0.82.dev0/test/test_evaluate_detection_average_precision.py` & `irisml-tasks-training-0.0.9/test/test_evaluate_detection_average_precision.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/test/test_make_feature_extractor_model.py` & `irisml-tasks-training-0.0.9/test/test_make_feature_extractor_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/test/test_make_image_text_contrastive_model.py` & `irisml-tasks-training-0.0.9/test/test_make_image_text_contrastive_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/test/test_make_image_text_transform.py` & `irisml-tasks-training-0.0.9/test/test_make_image_text_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.82.dev0/test/test_split_image_text_model.py` & `irisml-tasks-training-0.0.9/irisml/tasks/split_image_text_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,30 @@
-import unittest
+import copy
+import dataclasses
 import torch.nn
-from irisml.tasks.split_image_text_model import Task
+import irisml.core
 
 
-class TestSplitImageTextModel(unittest.TestCase):
-    def test_simple(self):
-        class FakeModel(torch.nn.Module):
-            def __init__(self):
-                super().__init__()
-                self.image_model = torch.nn.Conv2d(3, 3, 3)
-                self.text_model = torch.nn.Conv2d(3, 3, 3)
-                self.logit_scale = torch.nn.Parameter(torch.ones([]))
-                self.image_projection = torch.nn.Identity()
-                self.text_projection = torch.nn.Identity()
-
-        inputs = Task.Inputs(FakeModel())
-        outputs = Task(Task.Config()).execute(inputs)
-        self.assertIsNotNone(outputs.image_model)
-        self.assertIsNotNone(outputs.text_model)
-        self.assertIsNotNone(outputs.logit_scale)
+class Task(irisml.core.TaskBase):
+    """Split a image-text model into an image model and a text model.
+
+    Inputs:
+        model (torch.nn.Module): An input model. It must have 'image_model' and 'text_model' attributes.
+    """
+    VERSION = '0.1.0'
+
+    @dataclasses.dataclass
+    class Inputs:
+        model: torch.nn.Module
+
+    @dataclasses.dataclass
+    class Outputs:
+        image_model: torch.nn.Module = None
+        text_model: torch.nn.Module = None
+
+    def execute(self, inputs):
+        image_model = torch.nn.Sequential(copy.deepcopy(inputs.model.image_model), copy.deepcopy(inputs.model.image_projection))
+        text_model = torch.nn.Sequential(copy.deepcopy(inputs.model.text_model), copy.deepcopy(inputs.model.text_projection))
+        return self.Outputs(image_model, text_model)
+
+    def dry_run(self, inputs):
+        return self.execute(inputs)
```

