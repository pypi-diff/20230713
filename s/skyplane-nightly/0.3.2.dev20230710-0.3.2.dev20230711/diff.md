# Comparing `tmp/skyplane_nightly-0.3.2.dev20230710.tar.gz` & `tmp/skyplane_nightly-0.3.2.dev20230711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyplane_nightly-0.3.2.dev20230710.tar", max compression
+gzip compressed data, was "skyplane_nightly-0.3.2.dev20230711.tar", max compression
```

## Comparing `skyplane_nightly-0.3.2.dev20230710.tar` & `skyplane_nightly-0.3.2.dev20230711.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0    11357 2023-07-10 23:44:26.001998 skyplane_nightly-0.3.2.dev20230710/LICENSE
--rw-r--r--   0        0        0     7221 2023-07-10 23:44:26.001998 skyplane_nightly-0.3.2.dev20230710/README.md
--rw-r--r--   0        0        0     3669 2023-07-10 23:45:14.590367 skyplane_nightly-0.3.2.dev20230710/pyproject.toml
--rw-r--r--   0        0        0      649 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/__init__.py
--rw-r--r--   0        0        0     4331 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/api/client.py
--rw-r--r--   0        0        0     3040 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/api/config.py
--rw-r--r--   0        0        0    14831 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/api/dataplane.py
--rw-r--r--   0        0        0     2081 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/api/obj_store.py
--rw-r--r--   0        0        0     6616 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/api/pipeline.py
--rw-r--r--   0        0        0    15091 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/api/provisioner.py
--rw-r--r--   0        0        0    17597 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/api/tracker.py
--rw-r--r--   0        0        0    39196 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/api/transfer_job.py
--rw-r--r--   0        0        0    14790 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/api/usage.py
--rw-r--r--   0        0        0     5726 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/chunk.py
--rw-r--r--   0        0        0     3317 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/cli.py
--rw-r--r--   0        0        0    18045 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/cli_cloud.py
--rw-r--r--   0        0        0     1678 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/cli_config.py
--rw-r--r--   0        0        0    27030 2023-07-10 23:44:26.013998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/cli_init.py
--rw-r--r--   0        0        0    24587 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/cli_transfer.py
--rw-r--r--   0        0        0      461 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/experiments/__init__.py
--rw-r--r--   0        0        0    23462 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/experiments/cli_profile.py
--rw-r--r--   0        0        0     1757 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/experiments/cli_query.py
--rw-r--r--   0        0        0     9215 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/experiments/provision.py
--rw-r--r--   0        0        0     3100 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/impl/common.py
--rw-r--r--   0        0        0     4678 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/impl/cp_replicate_fallback.py
--rw-r--r--   0        0        0     3071 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/cli/impl/progress_bar.py
--rw-r--r--   0        0        0     1247 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/__init__.py
--rw-r--r--   0        0        0     5908 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_auth.py
--rw-r--r--   0        0        0    11591 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_cloud_provider.py
--rw-r--r--   0        0        0     4315 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_key_manager.py
--rw-r--r--   0        0        0    11509 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_network.py
--rw-r--r--   0        0        0     1606 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_pricing.py
--rw-r--r--   0        0        0     6294 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_server.py
--rw-r--r--   0        0        0     9526 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/azure/azure_auth.py
--rw-r--r--   0        0        0    20681 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/azure/azure_cloud_provider.py
--rw-r--r--   0        0        0     7503 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/azure/azure_server.py
--rw-r--r--   0        0        0     3564 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/cloud_provider.py
--rw-r--r--   0        0        0     2883 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/const_cmds.py
--rw-r--r--   0        0        0    12043 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_auth.py
--rw-r--r--   0        0        0     9355 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_cloud_provider.py
--rw-r--r--   0        0        0     2462 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_key_manager.py
--rw-r--r--   0        0        0     5365 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_network.py
--rw-r--r--   0        0        0     2786 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_pricing.py
--rw-r--r--   0        0        0     5151 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_server.py
--rw-r--r--   0        0        0      211 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_credentials.yaml.template
--rw-r--r--   0        0        0        0 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/__init__.py
--rw-r--r--   0        0        0     2242 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/config.py
--rw-r--r--   0        0        0      877 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/constants.py
--rw-r--r--   0        0        0     5353 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py
--rw-r--r--   0        0        0      710 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/utils.py
--rw-r--r--   0        0        0    40464 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py
--rw-r--r--   0        0        0     5320 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibmcloud_auth.py
--rw-r--r--   0        0        0     2851 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibmcloud_provider.py
--rw-r--r--   0        0        0     3522 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibmcloud_server.py
--rw-r--r--   0        0        0      937 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/key_utils.py
--rw-r--r--   0        0        0    17426 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/compute/server.py
--rw-r--r--   0        0        0    13589 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/config.py
--rw-r--r--   0        0        0     1229 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/config_paths.py
--rw-r--r--   0        0        0        0 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/data/__init__.py
--rw-r--r--   0        0        0    19636 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/data/aws_transfer_costs.csv
--rw-r--r--   0        0        0      617 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/data/vcpu_info.csv
--rw-r--r--   0        0        0     3078 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/exceptions.py
--rw-r--r--   0        0        0      811 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/cert.py
--rw-r--r--   0        0        0     4349 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/chunk_store.py
--rw-r--r--   0        0        0    15512 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/gateway_daemon.py
--rw-r--r--   0        0        0    16570 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/gateway_daemon_api.py
--rw-r--r--   0        0        0      718 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/gateway_onprem.py
--rw-r--r--   0        0        0     5149 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/gateway_program.py
--rw-r--r--   0        0        0     1732 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/gateway_queue.py
--rw-r--r--   0        0        0        0 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/operators/__init__.py
--rw-r--r--   0        0        0    25380 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/operators/gateway_operator.py
--rw-r--r--   0        0        0     9658 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/operators/gateway_receiver.py
--rw-r--r--   0        0        0       37 2023-07-10 23:45:14.586367 skyplane_nightly-0.3.2.dev20230710/skyplane/gateway_version.py
--rw-r--r--   0        0        0    13101 2023-07-10 23:44:26.017998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/azure_blob_interface.py
--rw-r--r--   0        0        0     2887 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/azure_storage_account_interface.py
--rw-r--r--   0        0        0    10871 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/cos_interface.py
--rw-r--r--   0        0        0     2010 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/file_system_interface.py
--rw-r--r--   0        0        0    12754 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/gcs_interface.py
--rw-r--r--   0        0        0     5963 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/hdfs_interface.py
--rw-r--r--   0        0        0     3287 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/object_store_interface.py
--rw-r--r--   0        0        0     5644 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/posix_file_interface.py
--rw-r--r--   0        0        0     3606 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/r2_interface.py
--rw-r--r--   0        0        0    11595 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/s3_interface.py
--rw-r--r--   0        0        0     2569 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/storage_interface.py
--rw-r--r--   0        0        0    23370 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/planner/planner.py
--rw-r--r--   0        0        0    18157 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/planner/solver.py
--rw-r--r--   0        0        0     6467 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/planner/solver_ilp.py
--rw-r--r--   0        0        0     1996 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/planner/solver_ron.py
--rw-r--r--   0        0        0     7920 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/planner/topology.py
--rw-r--r--   0        0        0      846 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/utils/cache.py
--rw-r--r--   0        0        0      617 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/utils/definitions.py
--rw-r--r--   0        0        0     2494 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/utils/fn.py
--rw-r--r--   0        0        0     1881 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/utils/generator.py
--rw-r--r--   0        0        0     1386 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/utils/imports.py
--rw-r--r--   0        0        0     2131 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/utils/logger.py
--rw-r--r--   0        0        0     1447 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/utils/networking_tools.py
--rw-r--r--   0        0        0     3162 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/utils/path.py
--rw-r--r--   0        0        0     1160 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/utils/retry.py
--rw-r--r--   0        0        0      612 2023-07-10 23:44:26.021998 skyplane_nightly-0.3.2.dev20230710/skyplane/utils/timer.py
--rw-r--r--   0        0        0    10493 1970-01-01 00:00:00.000000 skyplane_nightly-0.3.2.dev20230710/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 23:44:11.436443 skyplane_nightly-0.3.2.dev20230711/LICENSE
+-rw-r--r--   0        0        0     7221 2023-07-11 23:44:11.436443 skyplane_nightly-0.3.2.dev20230711/README.md
+-rw-r--r--   0        0        0     3669 2023-07-11 23:44:58.360827 skyplane_nightly-0.3.2.dev20230711/pyproject.toml
+-rw-r--r--   0        0        0      649 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/__init__.py
+-rw-r--r--   0        0        0     4331 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/client.py
+-rw-r--r--   0        0        0     3040 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/config.py
+-rw-r--r--   0        0        0    14841 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/dataplane.py
+-rw-r--r--   0        0        0     2081 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/obj_store.py
+-rw-r--r--   0        0        0     6750 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/pipeline.py
+-rw-r--r--   0        0        0    15091 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/provisioner.py
+-rw-r--r--   0        0        0    17597 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/tracker.py
+-rw-r--r--   0        0        0    39196 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/transfer_job.py
+-rw-r--r--   0        0        0    14790 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/api/usage.py
+-rw-r--r--   0        0        0     6120 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/chunk.py
+-rw-r--r--   0        0        0     3317 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli.py
+-rw-r--r--   0        0        0    18045 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_cloud.py
+-rw-r--r--   0        0        0     1678 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_config.py
+-rw-r--r--   0        0        0    27030 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_init.py
+-rw-r--r--   0        0        0    24587 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_transfer.py
+-rw-r--r--   0        0        0      461 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/__init__.py
+-rw-r--r--   0        0        0    23462 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/cli_profile.py
+-rw-r--r--   0        0        0     1757 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/cli_query.py
+-rw-r--r--   0        0        0     9215 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/provision.py
+-rw-r--r--   0        0        0     3100 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/common.py
+-rw-r--r--   0        0        0     4678 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/cp_replicate_fallback.py
+-rw-r--r--   0        0        0     3071 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/progress_bar.py
+-rw-r--r--   0        0        0     1247 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/__init__.py
+-rw-r--r--   0        0        0     5908 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_auth.py
+-rw-r--r--   0        0        0    11591 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_cloud_provider.py
+-rw-r--r--   0        0        0     4315 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_key_manager.py
+-rw-r--r--   0        0        0    11509 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_network.py
+-rw-r--r--   0        0        0     1606 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_pricing.py
+-rw-r--r--   0        0        0     6294 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_server.py
+-rw-r--r--   0        0        0     9526 2023-07-11 23:44:11.452443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_auth.py
+-rw-r--r--   0        0        0    20681 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_cloud_provider.py
+-rw-r--r--   0        0        0     7503 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_server.py
+-rw-r--r--   0        0        0     3564 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/cloud_provider.py
+-rw-r--r--   0        0        0     2883 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/const_cmds.py
+-rw-r--r--   0        0        0    12043 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_auth.py
+-rw-r--r--   0        0        0     9355 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_cloud_provider.py
+-rw-r--r--   0        0        0     2462 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_key_manager.py
+-rw-r--r--   0        0        0     5365 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_network.py
+-rw-r--r--   0        0        0     2786 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_pricing.py
+-rw-r--r--   0        0        0     5151 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_server.py
+-rw-r--r--   0        0        0      211 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_credentials.yaml.template
+-rw-r--r--   0        0        0        0 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/__init__.py
+-rw-r--r--   0        0        0     2242 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/config.py
+-rw-r--r--   0        0        0      877 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/constants.py
+-rw-r--r--   0        0        0     5353 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py
+-rw-r--r--   0        0        0      710 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/utils.py
+-rw-r--r--   0        0        0    40464 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py
+-rw-r--r--   0        0        0     5320 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_auth.py
+-rw-r--r--   0        0        0     2851 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_provider.py
+-rw-r--r--   0        0        0     3522 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_server.py
+-rw-r--r--   0        0        0      937 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/key_utils.py
+-rw-r--r--   0        0        0    17426 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/compute/server.py
+-rw-r--r--   0        0        0    13589 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/config.py
+-rw-r--r--   0        0        0     1229 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/config_paths.py
+-rw-r--r--   0        0        0        0 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/data/__init__.py
+-rw-r--r--   0        0        0    19636 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/data/aws_transfer_costs.csv
+-rw-r--r--   0        0        0      617 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/data/vcpu_info.csv
+-rw-r--r--   0        0        0     3078 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/exceptions.py
+-rw-r--r--   0        0        0      811 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/cert.py
+-rw-r--r--   0        0        0     4349 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/chunk_store.py
+-rw-r--r--   0        0        0    15655 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_daemon.py
+-rw-r--r--   0        0        0    16570 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_daemon_api.py
+-rw-r--r--   0        0        0      718 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_onprem.py
+-rw-r--r--   0        0        0     5149 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_program.py
+-rw-r--r--   0        0        0     1732 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_queue.py
+-rw-r--r--   0        0        0        0 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/operators/__init__.py
+-rw-r--r--   0        0        0    25487 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/operators/gateway_operator.py
+-rw-r--r--   0        0        0    10552 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/operators/gateway_receiver.py
+-rw-r--r--   0        0        0       37 2023-07-11 23:44:58.360827 skyplane_nightly-0.3.2.dev20230711/skyplane/gateway_version.py
+-rw-r--r--   0        0        0    13101 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/azure_blob_interface.py
+-rw-r--r--   0        0        0     2887 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/azure_storage_account_interface.py
+-rw-r--r--   0        0        0    10871 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/cos_interface.py
+-rw-r--r--   0        0        0     2010 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/file_system_interface.py
+-rw-r--r--   0        0        0    12754 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/gcs_interface.py
+-rw-r--r--   0        0        0     5963 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/hdfs_interface.py
+-rw-r--r--   0        0        0     3287 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/object_store_interface.py
+-rw-r--r--   0        0        0     5644 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/posix_file_interface.py
+-rw-r--r--   0        0        0     3606 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/r2_interface.py
+-rw-r--r--   0        0        0    11595 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/s3_interface.py
+-rw-r--r--   0        0        0     2569 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/storage_interface.py
+-rw-r--r--   0        0        0    23858 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/planner/planner.py
+-rw-r--r--   0        0        0    18157 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver.py
+-rw-r--r--   0        0        0     6467 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver_ilp.py
+-rw-r--r--   0        0        0     1996 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver_ron.py
+-rw-r--r--   0        0        0     7920 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/planner/topology.py
+-rw-r--r--   0        0        0      846 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/cache.py
+-rw-r--r--   0        0        0      617 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/definitions.py
+-rw-r--r--   0        0        0     2494 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/fn.py
+-rw-r--r--   0        0        0     1881 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/generator.py
+-rw-r--r--   0        0        0     1386 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/imports.py
+-rw-r--r--   0        0        0     2131 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/logger.py
+-rw-r--r--   0        0        0     1447 2023-07-11 23:44:11.456443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/networking_tools.py
+-rw-r--r--   0        0        0     3162 2023-07-11 23:44:11.460443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/path.py
+-rw-r--r--   0        0        0     1160 2023-07-11 23:44:11.460443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/retry.py
+-rw-r--r--   0        0        0      612 2023-07-11 23:44:11.460443 skyplane_nightly-0.3.2.dev20230711/skyplane/utils/timer.py
+-rw-r--r--   0        0        0    10493 1970-01-01 00:00:00.000000 skyplane_nightly-0.3.2.dev20230711/PKG-INFO
```

### Comparing `skyplane_nightly-0.3.2.dev20230710/LICENSE` & `skyplane_nightly-0.3.2.dev20230711/LICENSE`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/README.md` & `skyplane_nightly-0.3.2.dev20230711/README.md`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/pyproject.toml` & `skyplane_nightly-0.3.2.dev20230711/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "skyplane-nightly"
 packages = [{ include = "skyplane" }]
-version = "0.3.2.dev20230710"
+version = "0.3.2.dev20230711"
 description = "Skyplane efficiently transports data between cloud regions and providers."
 authors = ["Skyplane authors <skyplaneproject@gmail.com>"]
 license = "Apache-2.0"
 homepage = "https://skyplane.org/"
 repository = "https://github.com/skyplane-project/skyplane"
 documentation = "https://skyplane.org/"
 readme = "README.md"
```

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/__init__.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/__init__.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/api/client.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/api/client.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/api/config.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/api/config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/api/dataplane.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/api/dataplane.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
         # start gateway
         gateway_server.start_gateway(
             # setup_args,
             gateway_docker_image=gateway_docker_image,
             gateway_program_path=str(gateway_program_filename),
             gateway_info_path=f"{gateway_log_dir}/gateway_info.json",
-            e2ee_key_bytes=None,  # TODO: remove
+            e2ee_key_bytes=e2ee_key_bytes,  # TODO: remove
             use_bbr=self.transfer_config.use_bbr,  # TODO: remove
             use_compression=self.transfer_config.use_compression,
             use_socket_tls=self.transfer_config.use_socket_tls,
         )
 
     def provision(
         self,
```

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/api/obj_store.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/api/obj_store.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/api/pipeline.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/api/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     def __init__(
         self,
         clientid: str,
         provisioner: "Provisioner",
         transfer_config: TransferConfig,
         # cloud_regions: dict,
         max_instances: Optional[int] = 1,
+        n_connections: Optional[int] = 64,
         planning_algorithm: Optional[str] = "direct",
         debug: Optional[bool] = False,
     ):
         """
         :param clientid: the uuid of the local host to create the dataplane
         :type clientid: str
         :param provisioner: the provisioner to launch the VMs
@@ -50,33 +51,34 @@
         :param transfer_config: the configuration during the transfer
         :type transfer_config: TransferConfig
         """
         self.clientid = clientid
         # self.cloud_regions = cloud_regions
         # TODO: set max instances with VM CPU limits and/or config
         self.max_instances = max_instances
+        self.n_connections = n_connections
         self.provisioner = provisioner
         self.transfer_config = transfer_config
         self.http_pool = urllib3.PoolManager(retries=urllib3.Retry(total=3))
         self.provisioning_lock = threading.Lock()
         self.provisioned = False
         self.transfer_dir = tmp_log_dir / "transfer_logs" / datetime.now().strftime("%Y%m%d_%H%M%S")
         self.transfer_dir.mkdir(exist_ok=True, parents=True)
 
         # dataplane
         self.dataplane = None
 
         # planner
         self.planning_algorithm = planning_algorithm
         if self.planning_algorithm == "direct":
-            self.planner = MulticastDirectPlanner(self.max_instances, 64, self.transfer_config)
+            self.planner = MulticastDirectPlanner(self.max_instances, self.n_connections, self.transfer_config)
         elif self.planning_algorithm == "src_one_sided":
-            self.planner = DirectPlannerSourceOneSided(self.max_instances, 64, self.transfer_config)
+            self.planner = DirectPlannerSourceOneSided(self.max_instances, self.n_connections, self.transfer_config)
         elif self.planning_algorithm == "dst_one_sided":
-            self.planner = DirectPlannerDestOneSided(self.max_instances, 64, self.transfer_config)
+            self.planner = DirectPlannerDestOneSided(self.max_instances, self.n_connections, self.transfer_config)
         else:
             raise ValueError(f"No such planning algorithm {planning_algorithm}")
 
         # transfer logs
         self.transfer_dir = tmp_log_dir / "transfer_logs" / datetime.now().strftime("%Y%m%d_%H%M%S")
         self.transfer_dir.mkdir(exist_ok=True, parents=True)
         self.debug = debug
```

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/api/provisioner.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/api/provisioner.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/api/tracker.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/api/tracker.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/api/transfer_job.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/api/transfer_job.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/api/usage.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/api/usage.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/chunk.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/chunk.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,21 @@
 
     # multi-part upload/download info
     multi_part: Optional[bool] = False
     file_offset_bytes: Optional[int] = None
     part_number: Optional[int] = None
     upload_id: Optional[str] = None  # TODO: for broadcast, this is not used
 
-    def to_wire_header(self, n_chunks_left_on_socket: int, wire_length: int, is_compressed: bool = False):
+    def to_wire_header(self, n_chunks_left_on_socket: int, wire_length: int, raw_wire_length: int, is_compressed: bool = False):
         return WireProtocolHeader(
-            chunk_id=self.chunk_id, data_len=wire_length, is_compressed=is_compressed, n_chunks_left_on_socket=n_chunks_left_on_socket
+            chunk_id=self.chunk_id,
+            data_len=wire_length,
+            raw_data_len=raw_wire_length,
+            is_compressed=is_compressed,
+            n_chunks_left_on_socket=n_chunks_left_on_socket,
         )
 
     def as_dict(self):
         return asdict(self)
 
     @staticmethod
     def from_dict(d: Dict):
@@ -90,14 +94,15 @@
 
 @dataclass
 class WireProtocolHeader:
     """Lightweight wire protocol header for chunk transfers along socket."""
 
     chunk_id: str  # 128bit UUID
     data_len: int  # long
+    raw_data_len: int  # long (uncompressed, unecrypted)
     is_compressed: bool  # char
     n_chunks_left_on_socket: int  # long
 
     @staticmethod
     def magic_hex():
         return 0x534B595F4C41524B  # "SKY_LARK"
 
@@ -106,42 +111,48 @@
         # v1 = base protocol
         # v2 = compression
         # v3 = uuid chunk_id
         return 3
 
     @staticmethod
     def length_bytes():
-        # magic (8) + protocol_version (4) + chunk_id (16) + data_len (8) + is_compressed (1) + n_chunks_left_on_socket (8)
-        return 8 + 4 + 16 + 8 + 1 + 8
+        # magic (8) + protocol_version (4) + chunk_id (16) + data_len (8) + raw_data_len(8) + is_compressed (1) + n_chunks_left_on_socket (8)
+        return 8 + 4 + 16 + 8 + 8 + 1 + 8
 
     @staticmethod
     def from_bytes(data: bytes):
         assert len(data) == WireProtocolHeader.length_bytes(), f"{len(data)} != {WireProtocolHeader.length_bytes()}"
         magic = int.from_bytes(data[:8], byteorder="big")
         if magic != WireProtocolHeader.magic_hex():
             raise ValueError(f"Invalid magic number, got {magic:x} but expected {WireProtocolHeader.magic_hex():x}")
         version = int.from_bytes(data[8:12], byteorder="big")
         if version != WireProtocolHeader.protocol_version():
             raise ValueError(f"Invalid protocol version, got {version} but expected {WireProtocolHeader.protocol_version()}")
         chunk_id = data[12:28].hex()
         chunk_len = int.from_bytes(data[28:36], byteorder="big")
-        is_compressed = bool(int.from_bytes(data[36:37], byteorder="big"))
-        n_chunks_left_on_socket = int.from_bytes(data[37:45], byteorder="big")
+        raw_chunk_len = int.from_bytes(data[36:44], byteorder="big")
+        is_compressed = bool(int.from_bytes(data[44:45], byteorder="big"))
+        n_chunks_left_on_socket = int.from_bytes(data[45:53], byteorder="big")
         return WireProtocolHeader(
-            chunk_id=chunk_id, data_len=chunk_len, is_compressed=is_compressed, n_chunks_left_on_socket=n_chunks_left_on_socket
+            chunk_id=chunk_id,
+            data_len=chunk_len,
+            raw_data_len=raw_chunk_len,
+            is_compressed=is_compressed,
+            n_chunks_left_on_socket=n_chunks_left_on_socket,
         )
 
     def to_bytes(self):
         out_bytes = b""
         out_bytes += self.magic_hex().to_bytes(8, byteorder="big")
         out_bytes += self.protocol_version().to_bytes(4, byteorder="big")
         chunk_id_bytes = bytes.fromhex(self.chunk_id)
         assert len(chunk_id_bytes) == 16
         out_bytes += chunk_id_bytes
         out_bytes += self.data_len.to_bytes(8, byteorder="big")
+        out_bytes += self.raw_data_len.to_bytes(8, byteorder="big")
         out_bytes += self.is_compressed.to_bytes(1, byteorder="big")
         out_bytes += self.n_chunks_left_on_socket.to_bytes(8, byteorder="big")
         assert len(out_bytes) == WireProtocolHeader.length_bytes(), f"{len(out_bytes)} != {WireProtocolHeader.length_bytes()}"
         return out_bytes
 
     @staticmethod
     def from_socket(sock: socket.socket):
```

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/cli.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/cli_cloud.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_cloud.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/cli_config.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/cli_init.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_init.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/cli_transfer.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/cli_transfer.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/experiments/cli_profile.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/cli_profile.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/experiments/cli_query.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/cli_query.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/experiments/provision.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/experiments/provision.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/impl/common.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/common.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/impl/cp_replicate_fallback.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/cp_replicate_fallback.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/cli/impl/progress_bar.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/cli/impl/progress_bar.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/__init__.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_auth.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_key_manager.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_key_manager.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_network.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_network.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_pricing.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_pricing.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/aws/aws_server.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/aws/aws_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/azure/azure_auth.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/azure/azure_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/azure/azure_server.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/azure/azure_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/const_cmds.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/const_cmds.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_auth.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_key_manager.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_key_manager.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_network.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_network.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_pricing.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_pricing.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/gcp/gcp_server.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/gcp/gcp_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/config.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/constants.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/constants.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/utils.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/utils.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibmcloud_auth.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibmcloud_provider.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/ibmcloud/ibmcloud_server.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/ibmcloud/ibmcloud_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/key_utils.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/key_utils.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/compute/server.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/compute/server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/config.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/config_paths.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/config_paths.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/data/aws_transfer_costs.csv` & `skyplane_nightly-0.3.2.dev20230711/skyplane/data/aws_transfer_costs.csv`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/data/vcpu_info.csv` & `skyplane_nightly-0.3.2.dev20230711/skyplane/data/vcpu_info.csv`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/exceptions.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/exceptions.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/cert.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/cert.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/chunk_store.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/chunk_store.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/gateway_daemon.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from skyplane.gateway.gateway_daemon_api import GatewayDaemonAPI
 from skyplane.gateway.operators.gateway_operator import (
     GatewaySender,
     GatewayRandomDataGen,
     GatewayWriteLocal,
     GatewayObjStoreReadOperator,
     GatewayObjStoreWriteOperator,
-    GatewayWaitReciever,
+    GatewayWaitReceiver,
 )
 from skyplane.gateway.operators.gateway_receiver import GatewayReceiver
 from skyplane.utils import logger
 from collections import defaultdict
 
 
 # TODO: add default partition ID to main
@@ -34,15 +34,16 @@
 class GatewayDaemon:
     def __init__(
         self,
         region: str,
         chunk_dir: PathLike,
         max_incoming_ports=64,
         use_tls=True,
-        use_e2ee=False,
+        use_e2ee=True,  # TODO: read from operator field
+        use_compression=True,  # TODO: read from operator field
     ):
         # read gateway program
         gateway_program_path = Path(os.environ["GATEWAY_PROGRAM_FILE"]).expanduser()
         gateway_program = json.load(open(gateway_program_path, "r"))
 
         self.upload_id_map = Manager().dict()
 
@@ -67,32 +68,33 @@
 
         self.error_event = Event()
         self.error_queue = Queue()
         if use_e2ee:
             e2ee_key_path = Path(os.environ["E2EE_KEY_FILE"]).expanduser()
             with open(e2ee_key_path, "rb") as f:
                 self.e2ee_key_bytes = f.read()
+            print("Server side E2EE key loaded: ", self.e2ee_key_bytes)
         else:
             self.e2ee_key_bytes = None
 
         # create gateway operators
         self.terminal_operators = defaultdict(list)  # track terminal operators per partition
         self.num_required_terminal = {}
         self.operators = self.create_gateway_operators(gateway_program)
 
-        # single gateway reciever
+        # single gateway receiver
         self.gateway_receiver = GatewayReceiver(
             "reciever",
             region=region,
             chunk_store=self.chunk_store,
             error_event=self.error_event,
             error_queue=self.error_queue,
             max_pending_chunks=max_incoming_ports,
             use_tls=self.use_tls,
-            use_compression=False,  # use_compression,
+            use_compression=use_compression,
             e2ee_key_bytes=self.e2ee_key_bytes,
         )
 
         # API server
         self.api_server = GatewayDaemonAPI(
             self.chunk_store,
             self.gateway_receiver,
@@ -174,21 +176,21 @@
                 if output_queue is None:
                     # track what opeartors need to complete processing the chunk
                     for partition in partition_ids:
                         self.terminal_operators[str(partition)].append(handle)
 
                 # create operators
                 if op["op_type"] == "receive":
-                    # wait for chunks from reciever
-                    operators[handle] = GatewayWaitReciever(
+                    # wait for chunks from receiver
+                    operators[handle] = GatewayWaitReceiver(
                         handle=handle,
                         region=self.region,
                         input_queue=input_queue,
                         output_queue=output_queue,
-                        n_processes=1,  # dummy wait thread, not actual reciever
+                        n_processes=1,  # dummy wait thread, not actual receiver
                         chunk_store=self.chunk_store,
                         error_event=self.error_event,
                         error_queue=self.error_queue,
                     )
                     total_p += 1
                 elif op["op_type"] == "read_object_store":
                     operators[handle] = GatewayObjStoreReadOperator(
@@ -226,15 +228,15 @@
                         ip_addr=ip_addr,
                         input_queue=input_queue,
                         output_queue=output_queue,
                         error_event=self.error_event,
                         error_queue=self.error_queue,
                         chunk_store=self.chunk_store,
                         use_tls=self.use_tls,
-                        use_compression=False,  # operator["compress"],
+                        use_compression=op["compress"],
                         e2ee_key_bytes=self.e2ee_key_bytes,
                         n_processes=op["num_connections"],
                     )
                     total_p += op["num_connections"]
                 elif op["op_type"] == "write_object_store":
                     operators[handle] = GatewayObjStoreWriteOperator(
                         handle=handle,
```

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/gateway_daemon_api.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_daemon_api.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/gateway_onprem.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_onprem.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/gateway_program.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_program.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/gateway_queue.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/gateway_queue.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/operators/gateway_operator.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/operators/gateway_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 import os
 from typing import List
 import queue
 import socket
 import ssl
 import time
+import lz4.frame
 import traceback
 from functools import partial
 from multiprocessing import Event, Process, Queue
 from multiprocessing.managers import DictProxy
 from typing import Dict, List, Optional
 
 import urllib3
@@ -117,38 +118,38 @@
         pass
 
     @abstractmethod
     def process(self, chunk_req: ChunkRequest, **args):
         pass
 
 
-class GatewayWaitReciever(GatewayOperator):
+class GatewayWaitReceiver(GatewayOperator):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    # TODO: alternative (potentially better performnace) implementation: connect via queue with GatewayReciever to listen
+    # TODO: alternative (potentially better performnace) implementation: connect via queue with GatewayReceiver to listen
     # for download completition events - join with chunk request queue from ChunkStore
     def process(self, chunk_req: ChunkRequest):
         chunk_file_path = self.chunk_store.get_chunk_file_path(chunk_req.chunk.chunk_id)
         if not os.path.exists(chunk_file_path):  # chunk still not downloaded, re-queue
             # logger.debug(f"[{self.handle}:{self.worker_id}] Chunk {chunk_req.chunk.chunk_id} not downloaded yet, re-queueing")
             return False
 
         # check to see if file is completed downloading
-        # Successfully recieved chunk 38400a29812142a486eaefcdebedf371, 161867776    0, 67108864
+        # Successfully received chunk 38400a29812142a486eaefcdebedf371, 161867776    0, 67108864
         with open(chunk_file_path, "rb") as f:
             data = f.read()
             if len(data) < chunk_req.chunk.chunk_length_bytes:
                 # download not complete
                 return False
             assert (
                 len(data) == chunk_req.chunk.chunk_length_bytes
             ), f"Downloaded chunk length does not match expected length: {len(data)}, {chunk_req.chunk.chunk_length_bytes}"
         print(
-            f"[{self.handle}:{self.worker_id}] Successfully recieved chunk {chunk_req.chunk.chunk_id}, {len(data)}, {chunk_req.chunk.chunk_length_bytes}"
+            f"[{self.handle}:{self.worker_id}] Successfully received chunk {chunk_req.chunk.chunk_id}, {len(data)}, {chunk_req.chunk.chunk_length_bytes}"
         )
         return True
 
 
 class GatewaySender(GatewayOperator):
     def __init__(
         self,
@@ -324,25 +325,32 @@
 
             # read data from disk (and optionally compress if sending from source region)
             with open(chunk_file_path, "rb") as f:
                 data = f.read()
             assert len(data) == chunk.chunk_length_bytes, f"chunk {chunk_id} has size {len(data)} but should be {chunk.chunk_length_bytes}"
 
             wire_length = len(data)
-            # compressed_length = None
-            # if self.use_compression and self.region == chunk_req.src_region:
-            #    data = lz4.frame.compress(data)
-            #    wire_length = len(data)
-            #    compressed_length = wire_length
-            # if self.e2ee_secretbox is not None and self.region == chunk_req.src_region:
-            #    data = self.e2ee_secretbox.encrypt(data)
-            #    wire_length = len(data)
+            raw_wire_length = wire_length
+            compressed_length = None
+
+            if self.use_compression:
+                data = lz4.frame.compress(data)
+                wire_length = len(data)
+                compressed_length = wire_length
+            if self.e2ee_secretbox is not None:
+                data = self.e2ee_secretbox.encrypt(data)
+                wire_length = len(data)
 
             # send chunk header
-            header = chunk.to_wire_header(n_chunks_left_on_socket=len(chunk_ids) - idx - 1, wire_length=wire_length, is_compressed=False)
+            header = chunk.to_wire_header(
+                n_chunks_left_on_socket=len(chunk_ids) - idx - 1,
+                wire_length=wire_length,
+                raw_wire_length=raw_wire_length,
+                is_compressed=(compressed_length is not None),
+            )
             # print(f"[sender-{self.worker_id}]:{chunk_id} sending chunk header {header}")
             header.to_socket(sock)
             # print(f"[sender-{self.worker_id}]:{chunk_id} sent chunk header")
 
             # send chunk data
             assert chunk_file_path.exists(), f"chunk file {chunk_file_path} does not exist"
             # file_size = os.path.getsize(chunk_file_path)
@@ -524,18 +532,18 @@
         # update md5sum for chunk requests
         # TODO: create checksum operator
         # if not md5sum:
         #    logger.error(f"[obj_store:{self.worker_id}] Checksum was not generated for {chunk_req.chunk.src_key}")
         # else:
         #    self.chunk_store.update_chunk_checksum(chunk_req.chunk.chunk_id, md5sum)
 
-        recieved_chunk_size = self.chunk_store.get_chunk_file_path(chunk_req.chunk.chunk_id).stat().st_size
+        received_chunk_size = self.chunk_store.get_chunk_file_path(chunk_req.chunk.chunk_id).stat().st_size
         assert (
-            recieved_chunk_size == chunk_req.chunk.chunk_length_bytes
-        ), f"Downloaded chunk {chunk_req.chunk.chunk_id} to {fpath} has incorrect size (expected {chunk_req.chunk.chunk_length_bytes} but got {recieved_chunk_size}, {chunk_req.chunk.chunk_length_bytes})"
+            received_chunk_size == chunk_req.chunk.chunk_length_bytes
+        ), f"Downloaded chunk {chunk_req.chunk.chunk_id} to {fpath} has incorrect size (expected {chunk_req.chunk.chunk_length_bytes} but got {received_chunk_size}, {chunk_req.chunk.chunk_length_bytes})"
         logger.debug(f"[obj_store:{self.worker_id}] Downloaded {chunk_req.chunk.chunk_id} from {self.bucket_name}")
         return True
 
 
 class GatewayObjStoreWriteOperator(GatewayObjStoreOperator):
     def __init__(
         self,
```

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/gateway/operators/gateway_receiver.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/gateway/operators/gateway_receiver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import signal
 import socket
 import ssl
 import time
+import lz4.frame
 import traceback
 from contextlib import closing
 from multiprocessing import Event, Process, Value, Queue
 from typing import Optional, Tuple
 
 import nacl.secret
 
@@ -148,16 +149,16 @@
             logger.debug(f"[receiver:{server_port}] Blocking for next header")
             chunk_header = WireProtocolHeader.from_socket(conn)
             logger.debug(f"[receiver:{server_port}]:{chunk_header.chunk_id} Got chunk header {chunk_header}")
 
             # TODO: this wont work
             # chunk_request = self.chunk_store.get_chunk_request(chunk_header.chunk_id)
 
-            # should_decrypt = self.e2ee_secretbox is not None and chunk_request.dst_region == self.region
-            # should_decompress = chunk_header.is_compressed and chunk_request.dst_region == self.region
+            should_decrypt = self.e2ee_secretbox is not None  # and chunk_request.dst_region == self.region
+            should_decompress = chunk_header.is_compressed  # and chunk_request.dst_region == self.region
 
             # wait for space
             # while self.chunk_store.remaining_bytes() < chunk_header.data_len * self.max_pending_chunks:
             #    print(
             #        f"[receiver:{server_port}]: No remaining space with bytes {self.chunk_store.remaining_bytes()} data len {chunk_header.data_len} max pending {self.max_pending_chunks}, total space {init_space}"
             #    )
             #    time.sleep(0.1)
@@ -166,15 +167,15 @@
             # self.chunk_store.state_queue_download(chunk_header.chunk_id)
             # self.chunk_store.state_start_download(chunk_header.chunk_id, f"receiver:{self.worker_id}")
             logger.debug(f"[receiver:{server_port}]:{chunk_header.chunk_id} wire header length {chunk_header.data_len}")
             with Timer() as t:
                 fpath = self.chunk_store.get_chunk_file_path(chunk_header.chunk_id)
                 with fpath.open("wb") as f:
                     socket_data_len = chunk_header.data_len
-                    chunk_received_size = 0
+                    chunk_received_size, chunk_received_size_decompressed = 0, 0
                     to_write = bytearray(socket_data_len)
                     to_write_view = memoryview(to_write)
                     while socket_data_len > 0:
                         nbytes = conn.recv_into(to_write_view[chunk_received_size:], min(socket_data_len, self.recv_block_size))
                         socket_data_len -= nbytes
                         chunk_received_size += nbytes
                         self.socket_profiler_event_queue.put(
@@ -183,30 +184,44 @@
                                 chunk_id=chunk_header.chunk_id,
                                 time_ms=t.elapsed * 1000.0,
                                 bytes=chunk_received_size,
                             )
                         )
                     to_write = bytes(to_write)
 
+                    if should_decrypt:
+                        to_write = self.e2ee_secretbox.decrypt(to_write)
+                        print(f"[receiver:{server_port}]:{chunk_header.chunk_id} Decrypting {len(to_write)} bytes")
+
+                    if should_decompress:
+                        data_batch_decompressed = lz4.frame.decompress(to_write)
+                        chunk_received_size_decompressed += len(data_batch_decompressed)
+                        to_write = data_batch_decompressed
+                        print(
+                            f"[receiver:{server_port}]:{chunk_header.chunk_id} Decompressing {len(to_write)} bytes to {chunk_received_size_decompressed} bytes"
+                        )
+
                     # try to write data until successful
                     while True:
                         try:
                             f.seek(0, 0)
                             f.write(to_write)
                             f.flush()
 
+                            # check write succeeds
+                            assert os.path.exists(fpath)
+
                             # check size
                             file_size = os.path.getsize(fpath)
-                            if file_size == chunk_header.data_len:
+                            if file_size == chunk_header.raw_data_len:
                                 break
-                            elif file_size >= chunk_header.data_len:
-                                raise ValueError(f"[Gateway] File size {file_size} greater than chunk size {chunk_header.data_len}")
+                            elif file_size >= chunk_header.raw_data_len:
+                                raise ValueError(f"[Gateway] File size {file_size} greater than chunk size {chunk_header.raw_data_len}")
                         except Exception as e:
                             print(e)
-
                         print(
                             f"[receiver:{server_port}]: No remaining space with bytes {self.chunk_store.remaining_bytes()} data len {chunk_header.data_len} max pending {self.max_pending_chunks}, total space {init_space}"
                         )
                         time.sleep(1)
             assert (
                 socket_data_len == 0 and chunk_received_size == chunk_header.data_len
             ), f"Size mismatch: got {chunk_received_size} expected {chunk_header.data_len} and had {socket_data_len} bytes remaining"
```

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/azure_blob_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/azure_blob_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/azure_storage_account_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/azure_storage_account_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/cos_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/cos_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/file_system_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/file_system_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/gcs_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/gcs_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/hdfs_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/hdfs_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/object_store_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/object_store_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/posix_file_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/posix_file_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/r2_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/r2_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/s3_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/s3_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/obj_store/storage_interface.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/obj_store/storage_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/planner/planner.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/planner/planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,21 +236,27 @@
             # source region gateway program
             obj_store_read = src_program.add_operator(
                 GatewayReadObjectStore(src_bucket, src_region_tag, self.n_connections), partition_id=partition_id
             )
             mux_or = src_program.add_operator(GatewayMuxOr(), parent_handle=obj_store_read, partition_id=partition_id)
             for i in range(n_instances):
                 src_program.add_operator(
-                    GatewaySend(target_gateway_id=dst_gateways[i].gateway_id, region=src_region_tag, num_connections=self.n_connections),
+                    GatewaySend(
+                        target_gateway_id=dst_gateways[i].gateway_id,
+                        region=src_region_tag,
+                        num_connections=self.n_connections,
+                        compress=True,
+                        encrypt=True,
+                    ),
                     parent_handle=mux_or,
                     partition_id=partition_id,
                 )
 
             # dst region gateway program
-            recv_op = dst_program.add_operator(GatewayReceive(), partition_id=partition_id)
+            recv_op = dst_program.add_operator(GatewayReceive(decompress=True, decrypt=True), partition_id=partition_id)
             dst_program.add_operator(
                 GatewayWriteObjectStore(dst_bucket, dst_region_tag, self.n_connections), parent_handle=recv_op, partition_id=partition_id
             )
 
             # update cost per GB
             plan.cost_per_gb += compute.CloudProvider.get_transfer_cost(src_region_tag, dst_region_tag)
 
@@ -337,21 +343,26 @@
                         private_ip = True
                     src_program.add_operator(
                         GatewaySend(
                             target_gateway_id=dst_gateways[i].gateway_id,
                             region=dst_region_tag,
                             num_connections=int(self.n_connections / len(dst_gateways)),
                             private_ip=private_ip,
+                            compress=self.transfer_config.use_compression,
+                            encrypt=self.transfer_config.use_e2ee,
                         ),
                         parent_handle=mux_or,
                         partition_id=partition_id,
                     )
 
                 # each gateway also recieves data from source
-                recv_op = dst_program[dst_region_tag].add_operator(GatewayReceive(), partition_id=partition_id)
+                recv_op = dst_program[dst_region_tag].add_operator(
+                    GatewayReceive(decompress=self.transfer_config.use_compression, decrypt=self.transfer_config.use_e2ee),
+                    partition_id=partition_id,
+                )
                 dst_program[dst_region_tag].add_operator(
                     GatewayWriteObjectStore(dst_bucket, dst_region_tag, self.n_connections, key_prefix=dst_prefix),
                     parent_handle=recv_op,
                     partition_id=partition_id,
                 )
 
                 # update cost per GB
```

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/planner/solver.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/planner/solver_ilp.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver_ilp.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/planner/solver_ron.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/planner/solver_ron.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/planner/topology.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/planner/topology.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/utils/cache.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/cache.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/utils/definitions.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/utils/fn.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/fn.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/utils/generator.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/generator.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/utils/imports.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/imports.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/utils/logger.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/logger.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/utils/networking_tools.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/networking_tools.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/utils/path.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/path.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/utils/retry.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/retry.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/skyplane/utils/timer.py` & `skyplane_nightly-0.3.2.dev20230711/skyplane/utils/timer.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230710/PKG-INFO` & `skyplane_nightly-0.3.2.dev20230711/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyplane-nightly
-Version: 0.3.2.dev20230710
+Version: 0.3.2.dev20230711
 Summary: Skyplane efficiently transports data between cloud regions and providers.
 Home-page: https://skyplane.org/
 License: Apache-2.0
 Author: Skyplane authors
 Author-email: skyplaneproject@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

