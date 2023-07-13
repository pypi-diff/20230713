# Comparing `tmp/torchrec_nightly-2023.7.12-py39-none-any.whl.zip` & `tmp/torchrec_nightly-2023.7.13-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,146 +1,146 @@
 Zip file size: 361545 bytes, number of entries: 144
--rw-r--r--  2.0 unx      811 b- defN 23-Jul-12 19:25 torchrec/__init__.py
--rw-r--r--  2.0 unx     1638 b- defN 23-Jul-12 19:25 torchrec/streamable.py
--rw-r--r--  2.0 unx      854 b- defN 23-Jul-12 19:25 torchrec/types.py
--rw-r--r--  2.0 unx     1153 b- defN 23-Jul-12 19:25 torchrec/datasets/__init__.py
--rw-r--r--  2.0 unx    41469 b- defN 23-Jul-12 19:25 torchrec/datasets/criteo.py
--rw-r--r--  2.0 unx     4548 b- defN 23-Jul-12 19:25 torchrec/datasets/movielens.py
--rw-r--r--  2.0 unx     6539 b- defN 23-Jul-12 19:25 torchrec/datasets/random.py
--rw-r--r--  2.0 unx    10909 b- defN 23-Jul-12 19:25 torchrec/datasets/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 19:25 torchrec/datasets/scripts/__init__.py
--rw-r--r--  2.0 unx     2448 b- defN 23-Jul-12 19:25 torchrec/datasets/scripts/contiguous_preproc_criteo.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Jul-12 19:25 torchrec/datasets/scripts/npy_preproc_criteo.py
--rw-r--r--  2.0 unx     3077 b- defN 23-Jul-12 19:25 torchrec/datasets/scripts/shuffle_preproc_criteo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 19:25 torchrec/datasets/test_utils/__init__.py
--rw-r--r--  2.0 unx     5308 b- defN 23-Jul-12 19:25 torchrec/datasets/test_utils/criteo_test_utils.py
--rw-r--r--  2.0 unx     1912 b- defN 23-Jul-12 19:25 torchrec/distributed/__init__.py
--rw-r--r--  2.0 unx    37307 b- defN 23-Jul-12 19:25 torchrec/distributed/batched_embedding_kernel.py
--rw-r--r--  2.0 unx     2069 b- defN 23-Jul-12 19:25 torchrec/distributed/collective_utils.py
--rw-r--r--  2.0 unx     4988 b- defN 23-Jul-12 19:25 torchrec/distributed/comm.py
--rw-r--r--  2.0 unx    55918 b- defN 23-Jul-12 19:25 torchrec/distributed/comm_ops.py
--rw-r--r--  2.0 unx    36506 b- defN 23-Jul-12 19:25 torchrec/distributed/dist_data.py
--rw-r--r--  2.0 unx    32295 b- defN 23-Jul-12 19:25 torchrec/distributed/embedding.py
--rw-r--r--  2.0 unx     4947 b- defN 23-Jul-12 19:25 torchrec/distributed/embedding_kernel.py
--rw-r--r--  2.0 unx    29185 b- defN 23-Jul-12 19:25 torchrec/distributed/embedding_lookup.py
--rw-r--r--  2.0 unx    19035 b- defN 23-Jul-12 19:25 torchrec/distributed/embedding_sharding.py
--rw-r--r--  2.0 unx    36853 b- defN 23-Jul-12 19:25 torchrec/distributed/embedding_tower_sharding.py
--rw-r--r--  2.0 unx    15030 b- defN 23-Jul-12 19:25 torchrec/distributed/embedding_types.py
--rw-r--r--  2.0 unx    37214 b- defN 23-Jul-12 19:25 torchrec/distributed/embeddingbag.py
--rw-r--r--  2.0 unx     7373 b- defN 23-Jul-12 19:25 torchrec/distributed/fbgemm_qcomm_codec.py
--rw-r--r--  2.0 unx     6137 b- defN 23-Jul-12 19:25 torchrec/distributed/fp_embeddingbag.py
--rw-r--r--  2.0 unx     5243 b- defN 23-Jul-12 19:25 torchrec/distributed/fused_embedding.py
--rw-r--r--  2.0 unx     5080 b- defN 23-Jul-12 19:25 torchrec/distributed/fused_embeddingbag.py
--rw-r--r--  2.0 unx     2271 b- defN 23-Jul-12 19:25 torchrec/distributed/fused_params.py
--rw-r--r--  2.0 unx     3807 b- defN 23-Jul-12 19:25 torchrec/distributed/grouped_position_weighted.py
--rw-r--r--  2.0 unx    19750 b- defN 23-Jul-12 19:25 torchrec/distributed/model_parallel.py
--rw-r--r--  2.0 unx    20748 b- defN 23-Jul-12 19:25 torchrec/distributed/quant_embedding.py
--rw-r--r--  2.0 unx    15112 b- defN 23-Jul-12 19:25 torchrec/distributed/quant_embedding_kernel.py
--rw-r--r--  2.0 unx    12621 b- defN 23-Jul-12 19:25 torchrec/distributed/quant_embeddingbag.py
--rw-r--r--  2.0 unx    13928 b- defN 23-Jul-12 19:25 torchrec/distributed/quant_state.py
--rw-r--r--  2.0 unx     9261 b- defN 23-Jul-12 19:25 torchrec/distributed/shard.py
--rw-r--r--  2.0 unx    19646 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding_plan.py
--rw-r--r--  2.0 unx    32061 b- defN 23-Jul-12 19:25 torchrec/distributed/train_pipeline.py
--rw-r--r--  2.0 unx    27865 b- defN 23-Jul-12 19:25 torchrec/distributed/types.py
--rw-r--r--  2.0 unx    15470 b- defN 23-Jul-12 19:25 torchrec/distributed/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 19:25 torchrec/distributed/composable/__init__.py
--rw-r--r--  2.0 unx     3207 b- defN 23-Jul-12 19:25 torchrec/distributed/composable/table_batched_embedding_slice.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/__init__.py
--rw-r--r--  2.0 unx     3135 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/constants.py
--rw-r--r--  2.0 unx    11430 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/enumerators.py
--rw-r--r--  2.0 unx    12642 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/partitioners.py
--rw-r--r--  2.0 unx      835 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/perf_models.py
--rw-r--r--  2.0 unx    13530 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/planners.py
--rw-r--r--  2.0 unx    11236 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/proposers.py
--rw-r--r--  2.0 unx    41291 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/shard_estimators.py
--rw-r--r--  2.0 unx    23791 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/stats.py
--rw-r--r--  2.0 unx     9643 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/storage_reservations.py
--rw-r--r--  2.0 unx    14582 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/types.py
--rw-r--r--  2.0 unx     1119 b- defN 23-Jul-12 19:25 torchrec/distributed/planner/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/__init__.py
--rw-r--r--  2.0 unx     2479 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/cw_sequence_sharding.py
--rw-r--r--  2.0 unx    12945 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/cw_sharding.py
--rw-r--r--  2.0 unx     2802 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/dp_sequence_sharding.py
--rw-r--r--  2.0 unx     7681 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/dp_sharding.py
--rw-r--r--  2.0 unx     7640 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/rw_sequence_sharding.py
--rw-r--r--  2.0 unx    17911 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/rw_sharding.py
--rw-r--r--  2.0 unx     3627 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/sequence_sharding.py
--rw-r--r--  2.0 unx     7632 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/tw_sequence_sharding.py
--rw-r--r--  2.0 unx    16097 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/tw_sharding.py
--rw-r--r--  2.0 unx     1284 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/twcw_sharding.py
--rw-r--r--  2.0 unx    19871 b- defN 23-Jul-12 19:25 torchrec/distributed/sharding/twrw_sharding.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 19:25 torchrec/distributed/test_utils/__init__.py
--rw-r--r--  2.0 unx    11237 b- defN 23-Jul-12 19:25 torchrec/distributed/test_utils/infer_utils.py
--rw-r--r--  2.0 unx     4868 b- defN 23-Jul-12 19:25 torchrec/distributed/test_utils/multi_process.py
--rw-r--r--  2.0 unx    34091 b- defN 23-Jul-12 19:25 torchrec/distributed/test_utils/test_model.py
--rw-r--r--  2.0 unx    11197 b- defN 23-Jul-12 19:25 torchrec/distributed/test_utils/test_model_parallel.py
--rw-r--r--  2.0 unx    25310 b- defN 23-Jul-12 19:25 torchrec/distributed/test_utils/test_model_parallel_base.py
--rw-r--r--  2.0 unx    15367 b- defN 23-Jul-12 19:25 torchrec/distributed/test_utils/test_sharding.py
--rw-r--r--  2.0 unx      422 b- defN 23-Jul-12 19:25 torchrec/fx/__init__.py
--rw-r--r--  2.0 unx     6451 b- defN 23-Jul-12 19:25 torchrec/fx/tracer.py
--rw-r--r--  2.0 unx     4524 b- defN 23-Jul-12 19:25 torchrec/fx/utils.py
--rw-r--r--  2.0 unx     1223 b- defN 23-Jul-12 19:25 torchrec/inference/__init__.py
--rw-r--r--  2.0 unx     3614 b- defN 23-Jul-12 19:25 torchrec/inference/client.py
--rw-r--r--  2.0 unx     3957 b- defN 23-Jul-12 19:25 torchrec/inference/model_packager.py
--rw-r--r--  2.0 unx     8068 b- defN 23-Jul-12 19:25 torchrec/inference/modules.py
--rw-r--r--  2.0 unx     3797 b- defN 23-Jul-12 19:25 torchrec/inference/state_dict_transform.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 19:25 torchrec/metrics/__init__.py
--rw-r--r--  2.0 unx     4168 b- defN 23-Jul-12 19:25 torchrec/metrics/accuracy.py
--rw-r--r--  2.0 unx    12549 b- defN 23-Jul-12 19:25 torchrec/metrics/auc.py
--rw-r--r--  2.0 unx     3703 b- defN 23-Jul-12 19:25 torchrec/metrics/calibration.py
--rw-r--r--  2.0 unx     3465 b- defN 23-Jul-12 19:25 torchrec/metrics/ctr.py
--rw-r--r--  2.0 unx     3836 b- defN 23-Jul-12 19:25 torchrec/metrics/mae.py
--rw-r--r--  2.0 unx    17909 b- defN 23-Jul-12 19:25 torchrec/metrics/metric_module.py
--rw-r--r--  2.0 unx     6796 b- defN 23-Jul-12 19:25 torchrec/metrics/metrics_config.py
--rw-r--r--  2.0 unx     3731 b- defN 23-Jul-12 19:25 torchrec/metrics/metrics_namespace.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Jul-12 19:25 torchrec/metrics/model_utils.py
--rw-r--r--  2.0 unx     4631 b- defN 23-Jul-12 19:25 torchrec/metrics/mse.py
--rw-r--r--  2.0 unx     5605 b- defN 23-Jul-12 19:25 torchrec/metrics/multiclass_recall.py
--rw-r--r--  2.0 unx     6811 b- defN 23-Jul-12 19:25 torchrec/metrics/ne.py
--rw-r--r--  2.0 unx    33554 b- defN 23-Jul-12 19:25 torchrec/metrics/rec_metric.py
--rw-r--r--  2.0 unx    10490 b- defN 23-Jul-12 19:25 torchrec/metrics/recall_session.py
--rw-r--r--  2.0 unx     6057 b- defN 23-Jul-12 19:25 torchrec/metrics/throughput.py
--rw-r--r--  2.0 unx    11160 b- defN 23-Jul-12 19:25 torchrec/metrics/tower_qps.py
--rw-r--r--  2.0 unx     2867 b- defN 23-Jul-12 19:25 torchrec/metrics/weighted_avg.py
--rw-r--r--  2.0 unx    16441 b- defN 23-Jul-12 19:25 torchrec/metrics/test_utils/__init__.py
--rw-r--r--  2.0 unx      913 b- defN 23-Jul-12 19:25 torchrec/models/__init__.py
--rw-r--r--  2.0 unx    11410 b- defN 23-Jul-12 19:25 torchrec/models/deepfm.py
--rw-r--r--  2.0 unx    29965 b- defN 23-Jul-12 19:25 torchrec/models/dlrm.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 19:25 torchrec/models/experimental/__init__.py
--rw-r--r--  2.0 unx     9825 b- defN 23-Jul-12 19:25 torchrec/models/experimental/test_transformerdlrm.py
--rw-r--r--  2.0 unx     7434 b- defN 23-Jul-12 19:25 torchrec/models/experimental/transformerdlrm.py
--rw-r--r--  2.0 unx     1179 b- defN 23-Jul-12 19:25 torchrec/modules/__init__.py
--rw-r--r--  2.0 unx     1456 b- defN 23-Jul-12 19:25 torchrec/modules/activation.py
--rw-r--r--  2.0 unx    14636 b- defN 23-Jul-12 19:25 torchrec/modules/crossnet.py
--rw-r--r--  2.0 unx     8415 b- defN 23-Jul-12 19:25 torchrec/modules/deepfm.py
--rw-r--r--  2.0 unx     6468 b- defN 23-Jul-12 19:25 torchrec/modules/embedding_configs.py
--rw-r--r--  2.0 unx    14021 b- defN 23-Jul-12 19:25 torchrec/modules/embedding_modules.py
--rw-r--r--  2.0 unx     4858 b- defN 23-Jul-12 19:25 torchrec/modules/embedding_tower.py
--rw-r--r--  2.0 unx    12360 b- defN 23-Jul-12 19:25 torchrec/modules/feature_processor.py
--rw-r--r--  2.0 unx     4832 b- defN 23-Jul-12 19:25 torchrec/modules/feature_processor_.py
--rw-r--r--  2.0 unx     4403 b- defN 23-Jul-12 19:25 torchrec/modules/fp_embedding_modules.py
--rw-r--r--  2.0 unx    31545 b- defN 23-Jul-12 19:25 torchrec/modules/fused_embedding_modules.py
--rw-r--r--  2.0 unx    10541 b- defN 23-Jul-12 19:25 torchrec/modules/lazy_extension.py
--rw-r--r--  2.0 unx     6309 b- defN 23-Jul-12 19:25 torchrec/modules/mlp.py
--rw-r--r--  2.0 unx     3897 b- defN 23-Jul-12 19:25 torchrec/modules/utils.py
--rw-r--r--  2.0 unx     1639 b- defN 23-Jul-12 19:25 torchrec/optim/__init__.py
--rw-r--r--  2.0 unx     2012 b- defN 23-Jul-12 19:25 torchrec/optim/apply_optimizer_in_backward.py
--rw-r--r--  2.0 unx     1569 b- defN 23-Jul-12 19:25 torchrec/optim/clipping.py
--rw-r--r--  2.0 unx     1353 b- defN 23-Jul-12 19:25 torchrec/optim/fused.py
--rw-r--r--  2.0 unx    16069 b- defN 23-Jul-12 19:25 torchrec/optim/keyed.py
--rw-r--r--  2.0 unx     4420 b- defN 23-Jul-12 19:25 torchrec/optim/optimizers.py
--rw-r--r--  2.0 unx     7405 b- defN 23-Jul-12 19:25 torchrec/optim/rowwise_adagrad.py
--rw-r--r--  2.0 unx     4865 b- defN 23-Jul-12 19:25 torchrec/optim/warmup.py
--rw-r--r--  2.0 unx      560 b- defN 23-Jul-12 19:25 torchrec/optim/test_utils/__init__.py
--rw-r--r--  2.0 unx     1140 b- defN 23-Jul-12 19:25 torchrec/quant/__init__.py
--rw-r--r--  2.0 unx    26618 b- defN 23-Jul-12 19:25 torchrec/quant/embedding_modules.py
--rw-r--r--  2.0 unx     4292 b- defN 23-Jul-12 19:25 torchrec/quant/utils.py
--rw-r--r--  2.0 unx     1163 b- defN 23-Jul-12 19:25 torchrec/sparse/__init__.py
--rw-r--r--  2.0 unx    56412 b- defN 23-Jul-12 19:25 torchrec/sparse/jagged_tensor.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Jul-12 19:25 torchrec/sparse/test_utils/__init__.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Jul-12 19:25 torchrec/test_utils/__init__.py
--rw-r--r--  2.0 unx     1530 b- defN 23-Jul-12 19:30 torchrec_nightly-2023.7.12.dist-info/LICENSE
--rw-r--r--  2.0 unx     5012 b- defN 23-Jul-12 19:30 torchrec_nightly-2023.7.12.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-12 19:30 torchrec_nightly-2023.7.12.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 19:30 torchrec_nightly-2023.7.12.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    13446 b- defN 23-Jul-12 19:30 torchrec_nightly-2023.7.12.dist-info/RECORD
+-rw-r--r--  2.0 unx      811 b- defN 23-Jul-13 11:19 torchrec/__init__.py
+-rw-r--r--  2.0 unx     1638 b- defN 23-Jul-13 11:19 torchrec/streamable.py
+-rw-r--r--  2.0 unx      854 b- defN 23-Jul-13 11:19 torchrec/types.py
+-rw-r--r--  2.0 unx     1153 b- defN 23-Jul-13 11:19 torchrec/datasets/__init__.py
+-rw-r--r--  2.0 unx    41469 b- defN 23-Jul-13 11:19 torchrec/datasets/criteo.py
+-rw-r--r--  2.0 unx     4548 b- defN 23-Jul-13 11:19 torchrec/datasets/movielens.py
+-rw-r--r--  2.0 unx     6539 b- defN 23-Jul-13 11:19 torchrec/datasets/random.py
+-rw-r--r--  2.0 unx    10909 b- defN 23-Jul-13 11:19 torchrec/datasets/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-13 11:19 torchrec/datasets/scripts/__init__.py
+-rw-r--r--  2.0 unx     2448 b- defN 23-Jul-13 11:19 torchrec/datasets/scripts/contiguous_preproc_criteo.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jul-13 11:19 torchrec/datasets/scripts/npy_preproc_criteo.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Jul-13 11:19 torchrec/datasets/scripts/shuffle_preproc_criteo.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-13 11:19 torchrec/datasets/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5308 b- defN 23-Jul-13 11:19 torchrec/datasets/test_utils/criteo_test_utils.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-Jul-13 11:19 torchrec/distributed/__init__.py
+-rw-r--r--  2.0 unx    37307 b- defN 23-Jul-13 11:19 torchrec/distributed/batched_embedding_kernel.py
+-rw-r--r--  2.0 unx     2069 b- defN 23-Jul-13 11:19 torchrec/distributed/collective_utils.py
+-rw-r--r--  2.0 unx     4988 b- defN 23-Jul-13 11:19 torchrec/distributed/comm.py
+-rw-r--r--  2.0 unx    55918 b- defN 23-Jul-13 11:19 torchrec/distributed/comm_ops.py
+-rw-r--r--  2.0 unx    36506 b- defN 23-Jul-13 11:19 torchrec/distributed/dist_data.py
+-rw-r--r--  2.0 unx    32295 b- defN 23-Jul-13 11:19 torchrec/distributed/embedding.py
+-rw-r--r--  2.0 unx     4947 b- defN 23-Jul-13 11:19 torchrec/distributed/embedding_kernel.py
+-rw-r--r--  2.0 unx    29185 b- defN 23-Jul-13 11:19 torchrec/distributed/embedding_lookup.py
+-rw-r--r--  2.0 unx    19035 b- defN 23-Jul-13 11:19 torchrec/distributed/embedding_sharding.py
+-rw-r--r--  2.0 unx    36853 b- defN 23-Jul-13 11:19 torchrec/distributed/embedding_tower_sharding.py
+-rw-r--r--  2.0 unx    15030 b- defN 23-Jul-13 11:19 torchrec/distributed/embedding_types.py
+-rw-r--r--  2.0 unx    37214 b- defN 23-Jul-13 11:19 torchrec/distributed/embeddingbag.py
+-rw-r--r--  2.0 unx     7373 b- defN 23-Jul-13 11:19 torchrec/distributed/fbgemm_qcomm_codec.py
+-rw-r--r--  2.0 unx     6137 b- defN 23-Jul-13 11:19 torchrec/distributed/fp_embeddingbag.py
+-rw-r--r--  2.0 unx     5243 b- defN 23-Jul-13 11:19 torchrec/distributed/fused_embedding.py
+-rw-r--r--  2.0 unx     5080 b- defN 23-Jul-13 11:19 torchrec/distributed/fused_embeddingbag.py
+-rw-r--r--  2.0 unx     2271 b- defN 23-Jul-13 11:19 torchrec/distributed/fused_params.py
+-rw-r--r--  2.0 unx     3807 b- defN 23-Jul-13 11:19 torchrec/distributed/grouped_position_weighted.py
+-rw-r--r--  2.0 unx    19750 b- defN 23-Jul-13 11:19 torchrec/distributed/model_parallel.py
+-rw-r--r--  2.0 unx    20748 b- defN 23-Jul-13 11:19 torchrec/distributed/quant_embedding.py
+-rw-r--r--  2.0 unx    15112 b- defN 23-Jul-13 11:19 torchrec/distributed/quant_embedding_kernel.py
+-rw-r--r--  2.0 unx    12621 b- defN 23-Jul-13 11:19 torchrec/distributed/quant_embeddingbag.py
+-rw-r--r--  2.0 unx    13928 b- defN 23-Jul-13 11:19 torchrec/distributed/quant_state.py
+-rw-r--r--  2.0 unx     9261 b- defN 23-Jul-13 11:19 torchrec/distributed/shard.py
+-rw-r--r--  2.0 unx    19646 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding_plan.py
+-rw-r--r--  2.0 unx    32061 b- defN 23-Jul-13 11:19 torchrec/distributed/train_pipeline.py
+-rw-r--r--  2.0 unx    27865 b- defN 23-Jul-13 11:19 torchrec/distributed/types.py
+-rw-r--r--  2.0 unx    15470 b- defN 23-Jul-13 11:19 torchrec/distributed/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-13 11:19 torchrec/distributed/composable/__init__.py
+-rw-r--r--  2.0 unx     3207 b- defN 23-Jul-13 11:19 torchrec/distributed/composable/table_batched_embedding_slice.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/__init__.py
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/constants.py
+-rw-r--r--  2.0 unx    11430 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/enumerators.py
+-rw-r--r--  2.0 unx    12642 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/partitioners.py
+-rw-r--r--  2.0 unx      835 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/perf_models.py
+-rw-r--r--  2.0 unx    13530 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/planners.py
+-rw-r--r--  2.0 unx    11236 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/proposers.py
+-rw-r--r--  2.0 unx    41291 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/shard_estimators.py
+-rw-r--r--  2.0 unx    23791 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/stats.py
+-rw-r--r--  2.0 unx     9643 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/storage_reservations.py
+-rw-r--r--  2.0 unx    14582 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/types.py
+-rw-r--r--  2.0 unx     1119 b- defN 23-Jul-13 11:19 torchrec/distributed/planner/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/__init__.py
+-rw-r--r--  2.0 unx     2479 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/cw_sequence_sharding.py
+-rw-r--r--  2.0 unx    12945 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/cw_sharding.py
+-rw-r--r--  2.0 unx     2802 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/dp_sequence_sharding.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/dp_sharding.py
+-rw-r--r--  2.0 unx     7640 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/rw_sequence_sharding.py
+-rw-r--r--  2.0 unx    17911 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/rw_sharding.py
+-rw-r--r--  2.0 unx     3627 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/sequence_sharding.py
+-rw-r--r--  2.0 unx     7632 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/tw_sequence_sharding.py
+-rw-r--r--  2.0 unx    16097 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/tw_sharding.py
+-rw-r--r--  2.0 unx     1284 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/twcw_sharding.py
+-rw-r--r--  2.0 unx    19871 b- defN 23-Jul-13 11:19 torchrec/distributed/sharding/twrw_sharding.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-13 11:19 torchrec/distributed/test_utils/__init__.py
+-rw-r--r--  2.0 unx    11237 b- defN 23-Jul-13 11:19 torchrec/distributed/test_utils/infer_utils.py
+-rw-r--r--  2.0 unx     4868 b- defN 23-Jul-13 11:19 torchrec/distributed/test_utils/multi_process.py
+-rw-r--r--  2.0 unx    34091 b- defN 23-Jul-13 11:19 torchrec/distributed/test_utils/test_model.py
+-rw-r--r--  2.0 unx    11197 b- defN 23-Jul-13 11:19 torchrec/distributed/test_utils/test_model_parallel.py
+-rw-r--r--  2.0 unx    25310 b- defN 23-Jul-13 11:19 torchrec/distributed/test_utils/test_model_parallel_base.py
+-rw-r--r--  2.0 unx    15367 b- defN 23-Jul-13 11:19 torchrec/distributed/test_utils/test_sharding.py
+-rw-r--r--  2.0 unx      422 b- defN 23-Jul-13 11:19 torchrec/fx/__init__.py
+-rw-r--r--  2.0 unx     6451 b- defN 23-Jul-13 11:19 torchrec/fx/tracer.py
+-rw-r--r--  2.0 unx     4524 b- defN 23-Jul-13 11:19 torchrec/fx/utils.py
+-rw-r--r--  2.0 unx     1223 b- defN 23-Jul-13 11:19 torchrec/inference/__init__.py
+-rw-r--r--  2.0 unx     3614 b- defN 23-Jul-13 11:19 torchrec/inference/client.py
+-rw-r--r--  2.0 unx     3957 b- defN 23-Jul-13 11:19 torchrec/inference/model_packager.py
+-rw-r--r--  2.0 unx     8068 b- defN 23-Jul-13 11:19 torchrec/inference/modules.py
+-rw-r--r--  2.0 unx     3797 b- defN 23-Jul-13 11:19 torchrec/inference/state_dict_transform.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-13 11:19 torchrec/metrics/__init__.py
+-rw-r--r--  2.0 unx     4168 b- defN 23-Jul-13 11:19 torchrec/metrics/accuracy.py
+-rw-r--r--  2.0 unx    12549 b- defN 23-Jul-13 11:19 torchrec/metrics/auc.py
+-rw-r--r--  2.0 unx     3703 b- defN 23-Jul-13 11:19 torchrec/metrics/calibration.py
+-rw-r--r--  2.0 unx     3465 b- defN 23-Jul-13 11:19 torchrec/metrics/ctr.py
+-rw-r--r--  2.0 unx     3836 b- defN 23-Jul-13 11:19 torchrec/metrics/mae.py
+-rw-r--r--  2.0 unx    17909 b- defN 23-Jul-13 11:19 torchrec/metrics/metric_module.py
+-rw-r--r--  2.0 unx     6796 b- defN 23-Jul-13 11:19 torchrec/metrics/metrics_config.py
+-rw-r--r--  2.0 unx     3731 b- defN 23-Jul-13 11:19 torchrec/metrics/metrics_namespace.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-Jul-13 11:19 torchrec/metrics/model_utils.py
+-rw-r--r--  2.0 unx     4631 b- defN 23-Jul-13 11:19 torchrec/metrics/mse.py
+-rw-r--r--  2.0 unx     5605 b- defN 23-Jul-13 11:19 torchrec/metrics/multiclass_recall.py
+-rw-r--r--  2.0 unx     6811 b- defN 23-Jul-13 11:19 torchrec/metrics/ne.py
+-rw-r--r--  2.0 unx    33554 b- defN 23-Jul-13 11:19 torchrec/metrics/rec_metric.py
+-rw-r--r--  2.0 unx    10490 b- defN 23-Jul-13 11:19 torchrec/metrics/recall_session.py
+-rw-r--r--  2.0 unx     6057 b- defN 23-Jul-13 11:19 torchrec/metrics/throughput.py
+-rw-r--r--  2.0 unx    11160 b- defN 23-Jul-13 11:19 torchrec/metrics/tower_qps.py
+-rw-r--r--  2.0 unx     2867 b- defN 23-Jul-13 11:19 torchrec/metrics/weighted_avg.py
+-rw-r--r--  2.0 unx    16441 b- defN 23-Jul-13 11:19 torchrec/metrics/test_utils/__init__.py
+-rw-r--r--  2.0 unx      913 b- defN 23-Jul-13 11:19 torchrec/models/__init__.py
+-rw-r--r--  2.0 unx    11410 b- defN 23-Jul-13 11:19 torchrec/models/deepfm.py
+-rw-r--r--  2.0 unx    29965 b- defN 23-Jul-13 11:19 torchrec/models/dlrm.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-13 11:19 torchrec/models/experimental/__init__.py
+-rw-r--r--  2.0 unx     9825 b- defN 23-Jul-13 11:19 torchrec/models/experimental/test_transformerdlrm.py
+-rw-r--r--  2.0 unx     7434 b- defN 23-Jul-13 11:19 torchrec/models/experimental/transformerdlrm.py
+-rw-r--r--  2.0 unx     1179 b- defN 23-Jul-13 11:19 torchrec/modules/__init__.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-Jul-13 11:19 torchrec/modules/activation.py
+-rw-r--r--  2.0 unx    14636 b- defN 23-Jul-13 11:19 torchrec/modules/crossnet.py
+-rw-r--r--  2.0 unx     8415 b- defN 23-Jul-13 11:19 torchrec/modules/deepfm.py
+-rw-r--r--  2.0 unx     6468 b- defN 23-Jul-13 11:19 torchrec/modules/embedding_configs.py
+-rw-r--r--  2.0 unx    14021 b- defN 23-Jul-13 11:19 torchrec/modules/embedding_modules.py
+-rw-r--r--  2.0 unx     4858 b- defN 23-Jul-13 11:19 torchrec/modules/embedding_tower.py
+-rw-r--r--  2.0 unx    12360 b- defN 23-Jul-13 11:19 torchrec/modules/feature_processor.py
+-rw-r--r--  2.0 unx     4832 b- defN 23-Jul-13 11:19 torchrec/modules/feature_processor_.py
+-rw-r--r--  2.0 unx     4403 b- defN 23-Jul-13 11:19 torchrec/modules/fp_embedding_modules.py
+-rw-r--r--  2.0 unx    31545 b- defN 23-Jul-13 11:19 torchrec/modules/fused_embedding_modules.py
+-rw-r--r--  2.0 unx    10541 b- defN 23-Jul-13 11:19 torchrec/modules/lazy_extension.py
+-rw-r--r--  2.0 unx     6309 b- defN 23-Jul-13 11:19 torchrec/modules/mlp.py
+-rw-r--r--  2.0 unx     3897 b- defN 23-Jul-13 11:19 torchrec/modules/utils.py
+-rw-r--r--  2.0 unx     1639 b- defN 23-Jul-13 11:19 torchrec/optim/__init__.py
+-rw-r--r--  2.0 unx     2012 b- defN 23-Jul-13 11:19 torchrec/optim/apply_optimizer_in_backward.py
+-rw-r--r--  2.0 unx     1569 b- defN 23-Jul-13 11:19 torchrec/optim/clipping.py
+-rw-r--r--  2.0 unx     1353 b- defN 23-Jul-13 11:19 torchrec/optim/fused.py
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jul-13 11:19 torchrec/optim/keyed.py
+-rw-r--r--  2.0 unx     4420 b- defN 23-Jul-13 11:19 torchrec/optim/optimizers.py
+-rw-r--r--  2.0 unx     7405 b- defN 23-Jul-13 11:19 torchrec/optim/rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4865 b- defN 23-Jul-13 11:19 torchrec/optim/warmup.py
+-rw-r--r--  2.0 unx      560 b- defN 23-Jul-13 11:19 torchrec/optim/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1140 b- defN 23-Jul-13 11:19 torchrec/quant/__init__.py
+-rw-r--r--  2.0 unx    26618 b- defN 23-Jul-13 11:19 torchrec/quant/embedding_modules.py
+-rw-r--r--  2.0 unx     4292 b- defN 23-Jul-13 11:19 torchrec/quant/utils.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-Jul-13 11:19 torchrec/sparse/__init__.py
+-rw-r--r--  2.0 unx    56412 b- defN 23-Jul-13 11:19 torchrec/sparse/jagged_tensor.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Jul-13 11:19 torchrec/sparse/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jul-13 11:19 torchrec/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1530 b- defN 23-Jul-13 11:23 torchrec_nightly-2023.7.13.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5012 b- defN 23-Jul-13 11:23 torchrec_nightly-2023.7.13.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-13 11:23 torchrec_nightly-2023.7.13.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-13 11:23 torchrec_nightly-2023.7.13.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    13446 b- defN 23-Jul-13 11:23 torchrec_nightly-2023.7.13.dist-info/RECORD
 144 files, 1491636 bytes uncompressed, 340035 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -411,23 +411,23 @@
 
 Filename: torchrec/sparse/test_utils/__init__.py
 Comment: 
 
 Filename: torchrec/test_utils/__init__.py
 Comment: 
 
-Filename: torchrec_nightly-2023.7.12.dist-info/LICENSE
+Filename: torchrec_nightly-2023.7.13.dist-info/LICENSE
 Comment: 
 
-Filename: torchrec_nightly-2023.7.12.dist-info/METADATA
+Filename: torchrec_nightly-2023.7.13.dist-info/METADATA
 Comment: 
 
-Filename: torchrec_nightly-2023.7.12.dist-info/WHEEL
+Filename: torchrec_nightly-2023.7.13.dist-info/WHEEL
 Comment: 
 
-Filename: torchrec_nightly-2023.7.12.dist-info/top_level.txt
+Filename: torchrec_nightly-2023.7.13.dist-info/top_level.txt
 Comment: 
 
-Filename: torchrec_nightly-2023.7.12.dist-info/RECORD
+Filename: torchrec_nightly-2023.7.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `torchrec_nightly-2023.7.12.dist-info/LICENSE` & `torchrec_nightly-2023.7.13.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchrec_nightly-2023.7.12.dist-info/METADATA` & `torchrec_nightly-2023.7.13.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchrec-nightly
-Version: 2023.7.12
+Version: 2023.7.13
 Summary: Pytorch domain library for recommendation systems
 Home-page: https://github.com/pytorch/torchrec
 Author: TorchRec Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: pytorch,recommendation systems,sharding
 Classifier: Development Status :: 4 - Beta
```

## Comparing `torchrec_nightly-2023.7.12.dist-info/RECORD` & `torchrec_nightly-2023.7.13.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -133,12 +133,12 @@
 torchrec/quant/__init__.py,sha256=A6NIA6ztq6iP1JTLRLNzlgnCcd-LaN8efnxGub3Ii4A,1140
 torchrec/quant/embedding_modules.py,sha256=-_5_HaoNpt3AmL7fapO2Wj2r6WPjbq2VvATNmGhrai0,26618
 torchrec/quant/utils.py,sha256=rcyo5LDcLK49VLs6ZFxOHeutblWZunDAM_T-0NsraDE,4292
 torchrec/sparse/__init__.py,sha256=dLqSye4Jo6obnNNTUKdPDxPQb9sL2U4weemSn-DjpYk,1163
 torchrec/sparse/jagged_tensor.py,sha256=__iBD2tBQE9ZZpxcOn8RVmDF9gognnyUlmMjedHxJ4E,56412
 torchrec/sparse/test_utils/__init__.py,sha256=BLxfGKJvwjjCiQM64O5wGAA_Cea0sG-buw9lTDWuqug,1430
 torchrec/test_utils/__init__.py,sha256=JncJcXS4N3gI7-fsizQ2-qiWM6MhIrpvskF_9gDf0Go,5661
-torchrec_nightly-2023.7.12.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
-torchrec_nightly-2023.7.12.dist-info/METADATA,sha256=Drcu22wuU2soSfL1jjyGPoi-2fip_mG4L1RJPsACGEs,5012
-torchrec_nightly-2023.7.12.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
-torchrec_nightly-2023.7.12.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
-torchrec_nightly-2023.7.12.dist-info/RECORD,,
+torchrec_nightly-2023.7.13.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
+torchrec_nightly-2023.7.13.dist-info/METADATA,sha256=BfEAT67_FM4luQqI0jlFfk-3jfzwkQOO-ZBouH8i98A,5012
+torchrec_nightly-2023.7.13.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
+torchrec_nightly-2023.7.13.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
+torchrec_nightly-2023.7.13.dist-info/RECORD,,
```

