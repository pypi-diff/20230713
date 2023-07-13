# Comparing `tmp/metalsmith-1.9.1.tar.gz` & `tmp/metalsmith-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalsmith-1.9.1.tar", last modified: Fri Feb 10 16:30:35 2023, max compression
+gzip compressed data, was "metalsmith-2.0.0.tar", last modified: Thu Jul 13 15:46:53 2023, max compression
```

## Comparing `metalsmith-1.9.1.tar` & `metalsmith-2.0.0.tar`

### file list

```diff
@@ -1,134 +1,136 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.097597 metalsmith-1.9.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-02-10 16:30:05.000000 metalsmith-1.9.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5722 2023-02-10 16:30:05.000000 metalsmith-1.9.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2023-02-10 16:30:34.000000 metalsmith-1.9.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10899 2023-02-10 16:30:34.000000 metalsmith-1.9.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-02-10 16:30:05.000000 metalsmith-1.9.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2023-02-10 16:30:35.097597 metalsmith-1.9.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1383 2023-02-10 16:30:05.000000 metalsmith-1.9.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.077597 metalsmith-1.9.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-02-10 16:30:05.000000 metalsmith-1.9.1/doc/joined-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-02-10 16:30:05.000000 metalsmith-1.9.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.077597 metalsmith-1.9.1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.077597 metalsmith-1.9.1/doc/source/_exts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9068 2023-02-10 16:30:05.000000 metalsmith-1.9.1/doc/source/_exts/ansible-autodoc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.077597 metalsmith-1.9.1/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-02-10 16:30:05.000000 metalsmith-1.9.1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2889 2023-02-10 16:30:05.000000 metalsmith-1.9.1/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-02-10 16:30:05.000000 metalsmith-1.9.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.077597 metalsmith-1.9.1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-02-10 16:30:05.000000 metalsmith-1.9.1/doc/source/user/ansible.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.085597 metalsmith-1.9.1/metalsmith/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11066 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/_cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5498 2023-02-10 16:30:06.000000 metalsmith-1.9.1/metalsmith/_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3506 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/_network_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9141 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/_nics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31075 2023-02-10 16:30:06.000000 metalsmith-1.9.1/metalsmith/_provisioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6097 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5717 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/instance_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13422 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/sources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.089597 metalsmith-1.9.1/metalsmith/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/test/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33972 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/test/test_cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7228 2023-02-10 16:30:06.000000 metalsmith-1.9.1/metalsmith/test/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5820 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/test/test_instance_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10415 2023-02-10 16:30:06.000000 metalsmith-1.9.1/metalsmith/test/test_metalsmith_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5206 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/test/test_network_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/test/test_nics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   100851 2023-02-10 16:30:06.000000 metalsmith-1.9.1/metalsmith/test/test_provisioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/test/test_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9678 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/test/test_sources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/test/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.085597 metalsmith-1.9.1/metalsmith.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2023-02-10 16:30:34.000000 metalsmith-1.9.1/metalsmith.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4108 2023-02-10 16:30:35.000000 metalsmith-1.9.1/metalsmith.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:30:34.000000 metalsmith-1.9.1/metalsmith.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-02-10 16:30:34.000000 metalsmith-1.9.1/metalsmith.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:30:34.000000 metalsmith-1.9.1/metalsmith.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-10 16:30:34.000000 metalsmith-1.9.1/metalsmith.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-02-10 16:30:34.000000 metalsmith-1.9.1/metalsmith.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-02-10 16:30:34.000000 metalsmith-1.9.1/metalsmith.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.077597 metalsmith-1.9.1/metalsmith_ansible/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.077597 metalsmith-1.9.1/metalsmith_ansible/ansible_plugins/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.089597 metalsmith-1.9.1/metalsmith_ansible/ansible_plugins/modules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4457 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15881 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.077597 metalsmith-1.9.1/metalsmith_ansible/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.089597 metalsmith-1.9.1/metalsmith_ansible/roles/metalsmith_deployment/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7254 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith_ansible/roles/metalsmith_deployment/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.089597 metalsmith-1.9.1/metalsmith_ansible/roles/metalsmith_deployment/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith_ansible/roles/metalsmith_deployment/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.089597 metalsmith-1.9.1/metalsmith_ansible/roles/metalsmith_deployment/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith_ansible/roles/metalsmith_deployment/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.089597 metalsmith-1.9.1/metalsmith_ansible/roles/metalsmith_deployment/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2023-02-10 16:30:05.000000 metalsmith-1.9.1/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.077597 metalsmith-1.9.1/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.089597 metalsmith-1.9.1/playbooks/integration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4541 2023-02-10 16:30:05.000000 metalsmith-1.9.1/playbooks/integration/centos-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2023-02-10 16:30:05.000000 metalsmith-1.9.1/playbooks/integration/centos8-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2023-02-10 16:30:05.000000 metalsmith-1.9.1/playbooks/integration/centos8-integration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3778 2023-02-10 16:30:05.000000 metalsmith-1.9.1/playbooks/integration/cirros-image.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3686 2023-02-10 16:30:05.000000 metalsmith-1.9.1/playbooks/integration/exercise.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2023-02-10 16:30:05.000000 metalsmith-1.9.1/playbooks/integration/initial-setup.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-02-10 16:30:05.000000 metalsmith-1.9.1/playbooks/integration/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2023-02-10 16:30:05.000000 metalsmith-1.9.1/playbooks/integration/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-02-10 16:30:05.000000 metalsmith-1.9.1/playbooks/integration/ssh-key.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.077597 metalsmith-1.9.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.093598 metalsmith-1.9.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/0.9-deprecations-f403ce4961b77fe1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/allocation-hostname-f148e8adf0aee89a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/allow-both-network-and-subnet-in-nic-info-af8b40a26d55828e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/api-stein-8e5d165aa6d115cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/associated-993c26ac5dc0cfc0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/config_drive-f59bb5d8e684b2ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/deprecations-14-4292eaa456564782.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/drop-py-2-7-3cd57c85e8eb8d2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/exceptions-395ae4f1ad4de6da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/file-checksum-d19370a8fde00a81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/fix-ip-allocation-deferred-causing-broken-network-metadata-9c3ccfab2c563466.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/format-hostname-634a412ea933a966.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/iinfo-2014b1de4dbeca2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/initial-5afe4a5f6a13fa8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/instance-config-c4ea6a169f782138.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/keep-instance-info-3e7bb09244d5aaa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/no-clean-up-03bfaee6bbb112fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/prettytable-1db78a96c1d921d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/raw_http_images-41007351896ff642.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/reserve-hostname-85d02321156bde3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/resource-class-1957e83fa8235641.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/source-detect-673ad8c3e98c3df1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/states-79b593683c0783d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/stein-deprecation-6a4c9217a6ac4f13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/subnet-1c177e4b40cc607c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/notes/whole-disk-root-gb-bd8ee3600de9ec8d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.097597 metalsmith-1.9.1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.097597 metalsmith-1.9.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.097597 metalsmith-1.9.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6627 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-10 16:30:05.000000 metalsmith-1.9.1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-02-10 16:30:05.000000 metalsmith-1.9.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-02-10 16:30:35.097597 metalsmith-1.9.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-10 16:30:05.000000 metalsmith-1.9.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-02-10 16:30:05.000000 metalsmith-1.9.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:30:35.097597 metalsmith-1.9.1/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-02-10 16:30:05.000000 metalsmith-1.9.1/tools/ansible-lint.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3312 2023-02-10 16:30:05.000000 metalsmith-1.9.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.729181 metalsmith-2.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-07-13 15:46:24.000000 metalsmith-2.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5765 2023-07-13 15:46:24.000000 metalsmith-2.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2023-07-13 15:46:53.000000 metalsmith-2.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11238 2023-07-13 15:46:53.000000 metalsmith-2.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-07-13 15:46:24.000000 metalsmith-2.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2023-07-13 15:46:53.729181 metalsmith-2.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1383 2023-07-13 15:46:24.000000 metalsmith-2.0.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.709178 metalsmith-2.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-07-13 15:46:24.000000 metalsmith-2.0.0/doc/joined-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-07-13 15:46:24.000000 metalsmith-2.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.709178 metalsmith-2.0.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.709178 metalsmith-2.0.0/doc/source/_exts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9068 2023-07-13 15:46:24.000000 metalsmith-2.0.0/doc/source/_exts/ansible-autodoc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.709178 metalsmith-2.0.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-07-13 15:46:24.000000 metalsmith-2.0.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2889 2023-07-13 15:46:24.000000 metalsmith-2.0.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-07-13 15:46:24.000000 metalsmith-2.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.709178 metalsmith-2.0.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-07-13 15:46:24.000000 metalsmith-2.0.0/doc/source/user/ansible.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.713179 metalsmith-2.0.0/metalsmith/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11069 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/_cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5504 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3506 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/_network_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9141 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/_nics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31736 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/_provisioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6097 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5717 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/instance_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13443 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/sources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.717179 metalsmith-2.0.0/metalsmith/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33972 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/test_cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7069 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5820 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/test_instance_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10431 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/test_metalsmith_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5206 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/test_network_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/test_nics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   101043 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/test_provisioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/test_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9678 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/test_sources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/test/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.713179 metalsmith-2.0.0/metalsmith.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2023-07-13 15:46:53.000000 metalsmith-2.0.0/metalsmith.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4212 2023-07-13 15:46:53.000000 metalsmith-2.0.0/metalsmith.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-13 15:46:53.000000 metalsmith-2.0.0/metalsmith.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-07-13 15:46:53.000000 metalsmith-2.0.0/metalsmith.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-13 15:46:53.000000 metalsmith-2.0.0/metalsmith.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-13 15:46:53.000000 metalsmith-2.0.0/metalsmith.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-07-13 15:46:53.000000 metalsmith-2.0.0/metalsmith.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-07-13 15:46:53.000000 metalsmith-2.0.0/metalsmith.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.705177 metalsmith-2.0.0/metalsmith_ansible/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.705177 metalsmith-2.0.0/metalsmith_ansible/ansible_plugins/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.717179 metalsmith-2.0.0/metalsmith_ansible/ansible_plugins/modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4457 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15915 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.705177 metalsmith-2.0.0/metalsmith_ansible/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.717179 metalsmith-2.0.0/metalsmith_ansible/roles/metalsmith_deployment/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7263 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith_ansible/roles/metalsmith_deployment/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.717179 metalsmith-2.0.0/metalsmith_ansible/roles/metalsmith_deployment/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith_ansible/roles/metalsmith_deployment/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.717179 metalsmith-2.0.0/metalsmith_ansible/roles/metalsmith_deployment/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith_ansible/roles/metalsmith_deployment/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.717179 metalsmith-2.0.0/metalsmith_ansible/roles/metalsmith_deployment/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2023-07-13 15:46:24.000000 metalsmith-2.0.0/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.705177 metalsmith-2.0.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.721180 metalsmith-2.0.0/playbooks/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4541 2023-07-13 15:46:24.000000 metalsmith-2.0.0/playbooks/integration/centos-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2023-07-13 15:46:24.000000 metalsmith-2.0.0/playbooks/integration/centos8-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2023-07-13 15:46:24.000000 metalsmith-2.0.0/playbooks/integration/centos8-integration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3790 2023-07-13 15:46:24.000000 metalsmith-2.0.0/playbooks/integration/cirros-image.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3686 2023-07-13 15:46:24.000000 metalsmith-2.0.0/playbooks/integration/exercise.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2023-07-13 15:46:24.000000 metalsmith-2.0.0/playbooks/integration/initial-setup.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-07-13 15:46:24.000000 metalsmith-2.0.0/playbooks/integration/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2023-07-13 15:46:24.000000 metalsmith-2.0.0/playbooks/integration/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-07-13 15:46:24.000000 metalsmith-2.0.0/playbooks/integration/ssh-key.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.705177 metalsmith-2.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.725180 metalsmith-2.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/0.9-deprecations-f403ce4961b77fe1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/allocation-hostname-f148e8adf0aee89a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/allow-both-network-and-subnet-in-nic-info-af8b40a26d55828e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/api-stein-8e5d165aa6d115cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/associated-993c26ac5dc0cfc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/config_drive-f59bb5d8e684b2ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/deprecations-14-4292eaa456564782.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/drop-py-2-7-3cd57c85e8eb8d2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/exceptions-395ae4f1ad4de6da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/file-checksum-d19370a8fde00a81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/fix-ip-allocation-deferred-causing-broken-network-metadata-9c3ccfab2c563466.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/format-hostname-634a412ea933a966.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/iinfo-2014b1de4dbeca2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/initial-5afe4a5f6a13fa8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/instance-config-c4ea6a169f782138.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/keep-instance-info-3e7bb09244d5aaa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/no-clean-up-03bfaee6bbb112fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/prettytable-1db78a96c1d921d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/raw_http_images-41007351896ff642.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/reserve-hostname-85d02321156bde3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/resource-class-1957e83fa8235641.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/source-detect-673ad8c3e98c3df1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/states-79b593683c0783d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/stein-deprecation-6a4c9217a6ac4f13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/subnet-1c177e4b40cc607c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/update-references-for-checksums-44206e710b0506fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/notes/whole-disk-root-gb-bd8ee3600de9ec8d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.729181 metalsmith-2.0.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.729181 metalsmith-2.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.729181 metalsmith-2.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6627 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-13 15:46:24.000000 metalsmith-2.0.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-07-13 15:46:24.000000 metalsmith-2.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-07-13 15:46:53.729181 metalsmith-2.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-07-13 15:46:24.000000 metalsmith-2.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-07-13 15:46:24.000000 metalsmith-2.0.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:53.729181 metalsmith-2.0.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-07-13 15:46:24.000000 metalsmith-2.0.0/tools/ansible-lint.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3305 2023-07-13 15:46:24.000000 metalsmith-2.0.0/tox.ini
```

### Comparing `metalsmith-1.9.1/.zuul.yaml` & `metalsmith-2.0.0/.zuul.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
         IRONIC_VM_SPECS_DISK: 10
         IRONIC_VM_SPECS_RAM: 1024
         LIBVIRT_STORAGE_POOL_PATH: /opt/libvirt/images
         SWIFT_ENABLE_TEMPURLS: true
         SWIFT_HASH: 54bd5642300c4b45-846f8636a70a07d2
         SWIFT_START_ALL_SERVICES: false
         SWIFT_TEMPURL_KEY: 54bd5642300c4b45846f8636a70a07d2
+        IRONIC_PXE_BOOT_RETRY_TIMEOUT: 600
       centos_glance_initramds_image: test-centos-initramfs
       centos_glance_kernel_image: test-centos-kernel
       centos_glance_root_image: test-centos-partition
       centos_glance_whole_disk_image: test-centos-wholedisk
       metalsmith_netboot: false
       metalsmith_root_size: 9
       metalsmith_python: python3
```

### Comparing `metalsmith-1.9.1/AUTHORS` & `metalsmith-2.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/ChangeLog` & `metalsmith-2.0.0/ChangeLog`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 CHANGES
 =======
 
+2.0.0
+-----
+
+* Reduce retry timeout for Metalsmith CI
+* Update MD5 checksum references
+* Update to hacking v6
+* Update master for stable/2023.1
+
+1.10.0
+------
+
+* test\_provision: don't assert provision\_node call order
+* list\_instances - cache allocations
+* Get ports by 'binding:host\_id' query filter
+* Use a network cache in Instance
+
 1.9.1
 -----
 
 * Remove not used old job
 * Fixes for tox 4.0
 
 1.9.0
```

### Comparing `metalsmith-1.9.1/LICENSE` & `metalsmith-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/PKG-INFO` & `metalsmith-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: metalsmith
-Version: 1.9.1
+Version: 2.0.0
 Summary: Deployment and Scheduling tool for Bare Metal
 Home-page: https://opendev.org/openstack/metalsmith
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Deployment and Scheduling tool for Bare Metal
         =============================================
```

### Comparing `metalsmith-1.9.1/README.rst` & `metalsmith-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/doc/source/_exts/ansible-autodoc.py` & `metalsmith-2.0.0/doc/source/_exts/ansible-autodoc.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/doc/source/cli/index.rst` & `metalsmith-2.0.0/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/doc/source/conf.py` & `metalsmith-2.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/__init__.py` & `metalsmith-2.0.0/metalsmith/__init__.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/_cmd.py` & `metalsmith-2.0.0/metalsmith/_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                           help='time (in seconds) to wait for node to become '
                           'active')
     wait_grp.add_argument('--no-wait', action='store_true',
                           help='disable waiting for deploy to finish')
     deploy.add_argument('--image', help='image to use (name, UUID or URL)',
                         required=True)
     deploy.add_argument('--image-checksum',
-                        help='image MD5 checksum or URL with checksums')
+                        help='image SHA256 checksum or URL with checksums')
     deploy.add_argument('--image-kernel', help='URL of the image\'s kernel')
     deploy.add_argument('--image-ramdisk', help='URL of the image\'s ramdisk')
     deploy.add_argument('--network', help='network to create a port on '
                         '(name or UUID)', dest='nics', action=NICAction)
     deploy.add_argument('--subnet', help='subnet to create a port on '
                         '(name or UUID)', dest='nics', action=NICAction)
     deploy.add_argument('--port', help='port to attach (name or UUID)',
```

### Comparing `metalsmith-1.9.1/metalsmith/_format.py` & `metalsmith-2.0.0/metalsmith/_format.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/_instance.py` & `metalsmith-2.0.0/metalsmith/_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import enum
 import logging
 
-from openstack import exceptions as os_exc
-
 from metalsmith import _utils
 
 
 LOG = logging.getLogger(__name__)
 
 _PROGRESS_STATES = frozenset(['deploying', 'wait call-back',
                               'deploy complete'])
@@ -69,14 +67,16 @@
 _HEALTHY_STATES = frozenset([InstanceState.ACTIVE, InstanceState.DEPLOYING])
 _DEPLOYED_STATES = frozenset([InstanceState.ACTIVE, InstanceState.MAINTENANCE])
 
 
 class Instance(object):
     """Instance status in metalsmith."""
 
+    network_cache = dict()
+
     def __init__(self, connection, node, allocation=None):
         self._connection = connection
         self._uuid = node.id
         self._node = node
         self._allocation = allocation
 
     @property
@@ -116,23 +116,22 @@
     def nics(self):
         """List NICs for this instance.
 
         :return: List of `Port` objects with additional ``network`` fields
             with full representations of their networks.
         """
         result = []
-        vifs = self._connection.baremetal.list_node_vifs(self.node)
-        for vif in vifs:
-            try:
-                port = self._connection.network.get_port(vif)
-                port.network = self._connection.network.get_network(
-                    port.network_id)
-                result.append(port)
-            except os_exc.ResourceNotFound:
-                LOG.warning('vif has missing port: %s', vif)
+        ports_query = {'binding:host_id': self.node.id}
+        ports = self._connection.network.ports(**ports_query)
+        for port in ports:
+            if port.network_id not in Instance.network_cache:
+                Instance.network_cache[port.network_id] = (
+                    self._connection.network.get_network(port.network_id))
+            port.network = Instance.network_cache[port.network_id]
+            result.append(port)
         return result
 
     @property
     def node(self):
         """Underlying `Node` object."""
         return self._node
```

### Comparing `metalsmith-1.9.1/metalsmith/_network_metadata.py` & `metalsmith-2.0.0/metalsmith/_network_metadata.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/_nics.py` & `metalsmith-2.0.0/metalsmith/_nics.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/_provisioner.py` & `metalsmith-2.0.0/metalsmith/_provisioner.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     :param dry_run: boolean value, set to ``True`` to prevent any API calls
         from being actually made.
 
     :ivar connection: `openstacksdk` `Connection` object used for accessing
         OpenStack API during provisioning.
     """
 
+    allocations_cache = dict()
+
     def __init__(self, session=None, cloud_region=None, dry_run=False):
         if cloud_region is None:
             if session is None:
                 raise TypeError('Either session or cloud_region must '
                                 'be provided')
             self.connection = connection.Connection(session=session)
         elif session is not None:
@@ -626,14 +628,16 @@
 
     def list_instances(self):
         """List instances deployed by metalsmith.
 
         :return: list of :py:class:`metalsmith.Instance` objects.
         """
         nodes = self.connection.baremetal.nodes(associated=True, details=True)
+        Provisioner.allocations_cache = {
+            a.id: a for a in self.connection.baremetal.allocations()}
         instances = [i for i in map(self._get_instance, nodes)
                      if i.state != _instance.InstanceState.UNKNOWN]
         return instances
 
     def _get_node(self, node, refresh=False):
         """A helper to find and return a node."""
         if isinstance(node, str):
@@ -674,17 +678,28 @@
                      'alloc': allocation.id})
         else:
             raise exceptions.InstanceNotFound(
                 'Allocation %s exists but is not associated '
                 'with a node' % node)
 
     def _get_instance(self, ident):
-        node, allocation = self._find_node_and_allocation(ident)
-        if allocation is None and node.allocation_id:
+        if hasattr(ident, 'allocation_id'):
+            node = ident
             try:
-                allocation = self.connection.baremetal.get_allocation(
-                    node.allocation_id)
+                try:
+                    allocation = Provisioner.allocations_cache[
+                        node.instance_id]
+                except KeyError:
+                    allocation = self.connection.baremetal.get_allocation(
+                        node.allocation_id)
             except os_exc.ResourceNotFound as exc:
                 raise exceptions.InstanceNotFound(str(exc))
-
+        else:
+            node, allocation = self._find_node_and_allocation(ident)
+            if allocation is None and node.allocation_id:
+                try:
+                    allocation = self.connection.baremetal.get_allocation(
+                        node.allocation_id)
+                except os_exc.ResourceNotFound as exc:
+                    raise exceptions.InstanceNotFound(str(exc))
         return _instance.Instance(self.connection, node,
                                   allocation=allocation)
```

### Comparing `metalsmith-1.9.1/metalsmith/_scheduler.py` & `metalsmith-2.0.0/metalsmith/_scheduler.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/_utils.py` & `metalsmith-2.0.0/metalsmith/_utils.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/exceptions.py` & `metalsmith-2.0.0/metalsmith/exceptions.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/instance_config.py` & `metalsmith-2.0.0/metalsmith/instance_config.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/sources.py` & `metalsmith-2.0.0/metalsmith/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,18 @@
     """
 
     def __init__(self, url, checksum=None, checksum_url=None,
                  disk_format=None):
         """Create an HTTP source.
 
         :param url: URL of the image.
-        :param checksum: MD5 checksum of the image. Mutually exclusive with
+        :param checksum: SHA256 checksum of the image. Mutually exclusive with
             ``checksum_url``.
         :param checksum_url: URL of the checksum file for the image. Has to
-            be in the standard format of the ``md5sum`` tool. Mutually
+            be in the standard format of the ``sha256sum`` tool. Mutually
             exclusive with ``checksum``.
         :param disk_format: Optional value to set for ``instance_info``
             ``image_disk_format``.
         """
         if (checksum and checksum_url) or (not checksum and not checksum_url):
             raise TypeError('Exactly one of checksum and checksum_url has '
                             'to be specified')
@@ -166,19 +166,19 @@
     def __init__(self, url, kernel_url, ramdisk_url, checksum=None,
                  checksum_url=None, disk_format=None):
         """Create an HTTP source.
 
         :param url: URL of the root disk image.
         :param kernel_url: URL of the kernel image.
         :param ramdisk_url: URL of the initramfs image.
-        :param checksum: MD5 checksum of the root disk image. Mutually
+        :param checksum: SHA256 checksum of the root disk image. Mutually
             exclusive with ``checksum_url``.
         :param checksum_url: URL of the checksum file for the root disk image.
-            Has to be in the standard format of the ``md5sum`` tool. Mutually
-            exclusive with ``checksum``.
+            Has to be in the standard format of the ``sha256sum`` tool.
+            Mutually exclusive with ``checksum``.
         :param disk_format: Optional value to set for ``instance_info``
             ``image_disk_format``.
         """
         super(HttpPartitionImage, self).__init__(url, checksum=checksum,
                                                  checksum_url=checksum_url,
                                                  disk_format=disk_format)
         self.kernel_url = kernel_url
@@ -208,15 +208,15 @@
     """
 
     def __init__(self, location, checksum=None):
         """Create a local file source.
 
         :param location: Location of the image, optionally starting with
             ``file://``.
-        :param checksum: MD5 checksum of the image. DEPRECATED: checksums do
+        :param checksum: SHA256 checksum of the image. DEPRECATED: checksums do
             not actually work with file images.
         """
         if not location.startswith('file://'):
             location = 'file://' + location
         self.location = location
         self.checksum = checksum
         if self.checksum:
@@ -246,15 +246,15 @@
 
         :param location: Location of the image, optionally starting with
             ``file://``.
         :param kernel_location: Location of the kernel of the image,
             optionally starting with ``file://``.
         :param ramdisk_location: Location of the ramdisk of the image,
             optionally starting with ``file://``.
-        :param checksum: MD5 checksum of the image. DEPRECATED: checksums do
+        :param checksum: SHA256 checksum of the image. DEPRECATED: checksums do
             not actually work with file images.
         """
         super(FilePartitionImage, self).__init__(location, checksum)
         if not kernel_location.startswith('file://'):
             kernel_location = 'file://' + kernel_location
         if not ramdisk_location.startswith('file://'):
             ramdisk_location = 'file://' + ramdisk_location
@@ -282,15 +282,15 @@
 
     :param image: Location of the image: ``file://``, ``http://``, ``https://``
         link or a Glance image name or UUID.
     :param kernel: Location of the kernel (if present): ``file://``,
         ``http://``, ``https://`` link or a Glance image name or UUID.
     :param ramdisk: Location of the ramdisk (if present): ``file://``,
         ``http://``, ``https://`` link or a Glance image name or UUID.
-    :param checksum: MD5 checksum of the image: ``http://`` or ``https://``
+    :param checksum: SHA256 checksum of the image: ``http://`` or ``https://``
         link or a string.
     :return: A valid source object.
     :raises: ValueError if the given parameters do not correspond to any
         valid source.
     """
     image_type = _link_type(image)
     checksum_type = _link_type(checksum)
```

### Comparing `metalsmith-1.9.1/metalsmith/test/test_cmd.py` & `metalsmith-2.0.0/metalsmith/test/test_cmd.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/test/test_instance.py` & `metalsmith-2.0.0/metalsmith/test/test_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,31 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from unittest import mock
 
-from openstack import exceptions as os_exc
-
 from metalsmith import _instance
 from metalsmith.test import test_provisioner
 
 
 class TestInstanceIPAddresses(test_provisioner.Base):
     def setUp(self):
         super(TestInstanceIPAddresses, self).setUp()
         self.instance = _instance.Instance(self.api, self.node)
-        self.api.baremetal.list_node_vifs.return_value = ['111', '222']
         self.ports = [
             mock.Mock(spec=['network_id', 'fixed_ips', 'network'],
                       network_id=n, fixed_ips=[{'ip_address': ip}])
             for n, ip in [('0', '192.168.0.1'), ('1', '10.0.0.2')]
         ]
-        self.api.network.get_port.side_effect = self.ports
+        self.api.network.ports.return_value = self.ports
         self.nets = [
             mock.Mock(spec=['id', 'name'], id=str(i)) for i in range(2)
         ]
         for n in self.nets:
             n.name = 'name-%s' % n.id
         self.api.network.get_network.side_effect = self.nets
 
@@ -52,17 +49,16 @@
                           'name-1': ['10.0.0.2']}, ips)
 
     def test_missing_port(self):
         self.ports = [
             mock.Mock(spec=['network_id', 'fixed_ips', 'network'],
                       network_id='0',
                       fixed_ips=[{'ip_address': '192.168.0.1'}]),
-            os_exc.ResourceNotFound(),
         ]
-        self.api.network.get_port.side_effect = self.ports
+        self.api.network.ports.return_value = self.ports
         ips = self.instance.ip_addresses()
         self.assertEqual({'name-0': ['192.168.0.1']}, ips)
 
 
 class TestInstanceStates(test_provisioner.Base):
     def setUp(self):
         super(TestInstanceStates, self).setUp()
```

### Comparing `metalsmith-1.9.1/metalsmith/test/test_instance_config.py` & `metalsmith-2.0.0/metalsmith/test/test_instance_config.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/test/test_metalsmith_instances.py` & `metalsmith-2.0.0/metalsmith/test/test_metalsmith_instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
                 hostname='overcloud-compute-0',
                 image=image,
                 netboot=False,
                 nics=None,
                 root_size_gb=None,
                 swap_size_mb=None
             ),
-        ])
+        ], any_order=True)
         mock_config.assert_has_calls([
             mock.call(ssh_keys=None, user_data=None, meta_data=None),
             mock.call(ssh_keys='abcd',
                       user_data={'bootcmd': ['echo henlo world']},
                       meta_data={'foo': 'bar'})
         ])
         config.add_user.assert_called_once_with(
```

### Comparing `metalsmith-1.9.1/metalsmith/test/test_network_metadata.py` & `metalsmith-2.0.0/metalsmith/test/test_network_metadata.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/test/test_nics.py` & `metalsmith-2.0.0/metalsmith/test/test_nics.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/test/test_provisioner.py` & `metalsmith-2.0.0/metalsmith/test/test_provisioner.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from metalsmith import sources
 
 
 NODE_FIELDS = ['name', 'id', 'instance_info', 'instance_id', 'is_maintenance',
                'maintenance_reason', 'properties', 'provision_state', 'extra',
                'last_error', 'traits', 'resource_class', 'conductor_group',
                'allocation_id']
+ALLOCATION_FIELDS = ['id', 'name', 'node_id']
 
 
 class TestInit(unittest.TestCase):
     def test_missing_auth(self):
         self.assertRaisesRegex(TypeError, 'must be provided',
                                _provisioner.Provisioner)
 
@@ -2069,18 +2070,20 @@
                       instance_id='1234', allocation_id=None)
             for state in ('active', 'active', 'deploying', 'wait call-back',
                           'deploy failed', 'available', 'available', 'enroll')
         ]
         self.nodes[0].allocation_id = 'id2'
         self.nodes[6].instance_id = None
         self.api.baremetal.nodes.return_value = self.nodes
+        self.allocations = [mock.Mock(id='id2')]
+        self.api.baremetal.allocations.return_value = self.allocations
 
     def test_list(self):
         instances = self.pr.list_instances()
         self.assertTrue(all(isinstance(i, _instance.Instance)
                             for i in instances))
         self.assertEqual(self.nodes[:6], [i.node for i in instances])
-        self.assertEqual([self.api.baremetal.get_allocation.return_value]
-                         + [None] * 5,
+        self.assertEqual([self.api.baremetal.get_allocation.return_value] * 6,
                          [i.allocation for i in instances])
         self.api.baremetal.nodes.assert_called_once_with(associated=True,
                                                          details=True)
+        self.api.baremetal.allocations.assert_called_once()
```

### Comparing `metalsmith-1.9.1/metalsmith/test/test_scheduler.py` & `metalsmith-2.0.0/metalsmith/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/test/test_sources.py` & `metalsmith-2.0.0/metalsmith/test/test_sources.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/test/test_utils.py` & `metalsmith-2.0.0/metalsmith/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith/version.py` & `metalsmith-2.0.0/metalsmith/version.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith.egg-info/PKG-INFO` & `metalsmith-2.0.0/metalsmith.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: metalsmith
-Version: 1.9.1
+Version: 2.0.0
 Summary: Deployment and Scheduling tool for Bare Metal
 Home-page: https://opendev.org/openstack/metalsmith
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Deployment and Scheduling tool for Bare Metal
         =============================================
```

### Comparing `metalsmith-1.9.1/metalsmith.egg-info/SOURCES.txt` & `metalsmith-2.0.0/metalsmith.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,17 @@
 releasenotes/notes/raw_http_images-41007351896ff642.yaml
 releasenotes/notes/reserve-hostname-85d02321156bde3b.yaml
 releasenotes/notes/resource-class-1957e83fa8235641.yaml
 releasenotes/notes/source-detect-673ad8c3e98c3df1.yaml
 releasenotes/notes/states-79b593683c0783d5.yaml
 releasenotes/notes/stein-deprecation-6a4c9217a6ac4f13.yaml
 releasenotes/notes/subnet-1c177e4b40cc607c.yaml
+releasenotes/notes/update-references-for-checksums-44206e710b0506fe.yaml
 releasenotes/notes/whole-disk-root-gb-bd8ee3600de9ec8d.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/ussuri.rst
 releasenotes/source/victoria.rst
```

### Comparing `metalsmith-1.9.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py` & `metalsmith-2.0.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_deployment_defaults.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py` & `metalsmith-2.0.0/metalsmith_ansible/ansible_plugins/modules/metalsmith_instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
           href:
             description:
               - Image to use (name, UUID or URL)
             type: str
             required: True
           checksum :
             description:
-              - Image MD5 checksum or URL with checksums
+              - Image SHA256, or SHA512 checksum or URL with checksums. MD5 is deprecated.
             type: str
           kernel:
             description:
               - URL of the image's kernel
             type: str
           ramdisk:
             description:
```

### Comparing `metalsmith-1.9.1/metalsmith_ansible/roles/metalsmith_deployment/README.rst` & `metalsmith-2.0.0/metalsmith_ansible/roles/metalsmith_deployment/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 ``extra_args`` (defaults to ``metalsmith_extra_args``)
     additional arguments to pass to the ``metalsmith`` CLI on all calls.
     (No longer supported, will raise an error if used)
 ``image`` (defaults to ``metalsmith_image``)
     UUID, name or HTTP(s) URL of the image to use for deployment. Mandatory.
 ``image_checksum`` (defaults to ``metalsmith_image_checksum``)
-    MD5 checksum or checksum file URL for an HTTP(s) image.
+    SHA256 checksum or checksum file URL for an HTTP(s) image.
 ``image_kernel`` (defaults to ``metalsmith_image_kernel``)
     URL of the kernel image if and only if the ``image`` is a URL of
     a partition image.
 ``image_ramdisk`` (defaults to ``metalsmith_image_ramdisk``)
     URL of the ramdisk image if and only if the ``image`` is a URL of
     a partition image.
 ``netboot``
@@ -199,12 +199,12 @@
                   - network: ctlplane
                   - port: 1899af15-149d-47dc-b0dc-a68614eeb5c4
               - hostname: custom-partition-image
                 resource_class: custom
                 image: https://example.com/images/custom-1.0.root.img
                 image_kernel: https://example.com/images/custom-1.0.vmlinuz
                 image_ramdisk: https://example.com/images/custom-1.0.initrd
-                image_checksum: https://example.com/images/MD5SUMS
+                image_checksum: https://example.com/images/SHA256SUMS
               - hostname: custom-whole-disk-image
                 resource_class: custom
                 image: https://example.com/images/custom-1.0.qcow2
-                image_checksum: https://example.com/images/MD5SUMS
+                image_checksum: https://example.com/images/SHA256SUMS
```

### Comparing `metalsmith-1.9.1/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml` & `metalsmith-2.0.0/metalsmith_ansible/roles/metalsmith_deployment/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/playbooks/integration/centos-image.yaml` & `metalsmith-2.0.0/playbooks/integration/centos-image.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/playbooks/integration/centos8-image.yaml` & `metalsmith-2.0.0/playbooks/integration/centos8-image.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/playbooks/integration/centos8-integration.yaml` & `metalsmith-2.0.0/playbooks/integration/centos8-integration.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/playbooks/integration/cirros-image.yaml` & `metalsmith-2.0.0/playbooks/integration/cirros-image.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -50,32 +50,32 @@
       command: >
         cp /opt/stack/data/ironic/{{ cirros_partition_image_result.stdout }}.img
             /opt/stack/data/ironic/httpboot/metalsmith
       args:
         creates: /opt/stack/data/ironic/httpboot/metalsmith/{{ cirros_partition_image_result.stdout }}.img
       become: yes
 
-    - name: Create MD5 checksums file for images
-      shell: md5sum cirros-* > CHECKSUMS
+    - name: Create SHA256 checksums file for images
+      shell: sha256sum cirros-* > CHECKSUMS
       args:
         chdir: /opt/stack/data/ironic/httpboot/metalsmith
       become: yes
 
     - name: Change ownership of image files
       file:
         path: /opt/stack/data/ironic/httpboot/metalsmith
         state: directory
         owner: "{{ ansible_user }}"
         recurse: yes
         mode: a+r
       become: yes
 
-    - name: Calculate MD5 checksum for HTTP disk image
+    - name: Calculate SHA256 checksum for HTTP disk image
       shell: |
-          md5sum /opt/stack/devstack/files/{{ cirros_disk_image_result.stdout }}.img \
+          sha256sum /opt/stack/devstack/files/{{ cirros_disk_image_result.stdout }}.img \
               | awk '{ print $1; }'
       register: cirros_disk_image_checksum_result
       failed_when: cirros_disk_image_checksum_result.stdout == ""
 
     - name: Set facts for HTTP image
       set_fact:
         metalsmith_partition_image: "{{ baremetal_endpoint_result.stdout}}/metalsmith/{{ cirros_partition_image_result.stdout }}.img"
```

### Comparing `metalsmith-1.9.1/playbooks/integration/exercise.yaml` & `metalsmith-2.0.0/playbooks/integration/exercise.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/playbooks/integration/initial-setup.yaml` & `metalsmith-2.0.0/playbooks/integration/initial-setup.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/playbooks/integration/run.yaml` & `metalsmith-2.0.0/playbooks/integration/run.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml` & `metalsmith-2.0.0/releasenotes/notes/network-metadata-ff0c3e80e5e0f53c.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml` & `metalsmith-2.0.0/releasenotes/notes/openstacksdk-9ad2298b84e34a5f.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/releasenotes/notes/states-79b593683c0783d5.yaml` & `metalsmith-2.0.0/releasenotes/notes/states-79b593683c0783d5.yaml`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/releasenotes/source/conf.py` & `metalsmith-2.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/setup.cfg` & `metalsmith-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/setup.py` & `metalsmith-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `metalsmith-1.9.1/tox.ini` & `metalsmith-2.0.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     OS_CACERT
 
 [testenv:pep8]
 deps =
     Pygments>=2.2.0 # BSD
     doc8>=0.8.1 # Apache-2.0
     flake8-import-order>=0.17.1 # LGPLv3
-    hacking>=4.1.0,<5.0.0 # Apache-2.0
+    hacking~=6.0.0 # Apache-2.0
     pycodestyle>=2.0.0,<3.0.0 # MIT
 commands =
     flake8 metalsmith
     doc8 README.rst doc/source metalsmith_ansible/roles
 
 [testenv:docs]
 deps =
```

