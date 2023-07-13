# Comparing `tmp/kayobe-9.3.0.tar.gz` & `tmp/kayobe-9.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kayobe-9.3.0.tar", last modified: Tue Feb  1 17:14:26 2022, max compression
+gzip compressed data, was "kayobe-9.4.0.tar", last modified: Thu Apr 28 10:16:06 2022, max compression
```

## Comparing `kayobe-9.3.0.tar` & `kayobe-9.4.0.tar`

### file list

```diff
@@ -1,1090 +1,1104 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.288590 kayobe-9.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2022-02-01 17:13:48.000000 kayobe-9.3.0/.coveragerc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.136585 kayobe-9.3.0/.github/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-02-01 17:13:48.000000 kayobe-9.3.0/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-02-01 17:13:48.000000 kayobe-9.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2022-02-01 17:13:48.000000 kayobe-9.3.0/.yamllint
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2347 2022-02-01 17:14:25.000000 kayobe-9.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2022-02-01 17:13:48.000000 kayobe-9.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62039 2022-02-01 17:14:25.000000 kayobe-9.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-02-01 17:13:48.000000 kayobe-9.3.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-02-01 17:13:48.000000 kayobe-9.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3834 2022-02-01 17:14:26.288590 kayobe-9.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2404 2022-02-01 17:13:48.000000 kayobe-9.3.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1889 2022-02-01 17:13:48.000000 kayobe-9.3.0/Vagrantfile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.152586 kayobe-9.3.0/ansible/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.152586 kayobe-9.3.0/ansible/action_plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/action_plugins/kolla_ansible_host_vars.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1982 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/baremetal-compute-inspect.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/baremetal-compute-manage.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/baremetal-compute-provide.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2631 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/baremetal-compute-rename.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/baremetal-compute-serial-console-post-config.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5520 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/baremetal-compute-serial-console.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/bootstrap.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2392 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/compute-node-discovery.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/compute-node-provide.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/container-image-build.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/container-image-builders-check.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/dell-compute-node-boot-mode.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/dell-compute-node-discovery.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/dell-compute-node-inventory.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/dell-switch-bmp.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/dev-tools.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/disable-cloud-init.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/disable-glean.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/disable-selinux.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/dnf.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1633 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/docker-devicemapper.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/docker-registry.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/docker.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/drac-bios.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/drac-boot-order.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/drac-facts.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/dump-config.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/external-net.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.152586 kayobe-9.3.0/ansible/filter_plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/filter_plugins/bmc_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18980 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/filter_plugins/networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2533 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/filter_plugins/switches.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.108585 kayobe-9.3.0/ansible/group_vars/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.156586 kayobe-9.3.0/ansible/group_vars/all/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5150 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/bifrost
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/bmc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5083 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/compute
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6088 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/controllers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/dell-switch-bmp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/dnf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/dns
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/docker
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/docker-registry
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1624 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/globals
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/grafana
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/idrac
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13346 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/inspector
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6106 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/ipa
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4850 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/ironic
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22352 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/kolla
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/monasca
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3948 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/monitoring
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/network
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2536 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/neutron
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/nova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/opensm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2372 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/openstack
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/overcloud
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/pip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4154 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/seed
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5047 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/seed-hypervisor
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/seed-vm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/ssh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5531 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/storage
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2622 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/swift
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.160586 kayobe-9.3.0/ansible/group_vars/all/switches/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      646 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/switches/arista
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/switches/config
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/switches/dell
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/switches/dell-powerconnect
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/switches/junos
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/switches/mellanox
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/time
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/all/users
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.160586 kayobe-9.3.0/ansible/group_vars/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/compute/ansible-user
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/compute/bios
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/compute/luks
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/compute/lvm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/compute/mdadm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/compute/network
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/compute/raid
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/compute/sysctl
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/compute/users
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.160586 kayobe-9.3.0/ansible/group_vars/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/controllers/ansible-user
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/controllers/bios
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/controllers/luks
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/controllers/lvm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/controllers/mdadm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/controllers/network
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/controllers/raid
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/controllers/sysctl
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/controllers/users
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.164586 kayobe-9.3.0/ansible/group_vars/monitoring/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/monitoring/ansible-user
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/monitoring/bios
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/monitoring/luks
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/monitoring/lvm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/monitoring/mdadm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/monitoring/network
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/monitoring/raid
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/monitoring/sysctl
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/monitoring/users
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.164586 kayobe-9.3.0/ansible/group_vars/overcloud/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/overcloud/ansible-host
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.164586 kayobe-9.3.0/ansible/group_vars/seed/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed/ansible-host
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed/ansible-user
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed/luks
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed/lvm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed/mdadm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed/network
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed/sysctl
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed/users
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/group_vars/seed-hypervisor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed-hypervisor/ansible-host
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed-hypervisor/ansible-user
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed-hypervisor/luks
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed-hypervisor/lvm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed-hypervisor/mdadm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed-hypervisor/network
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed-hypervisor/sysctl
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/seed-hypervisor/users
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/group_vars/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/storage/ansible-user
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/storage/bios
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/storage/luks
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/storage/lvm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/storage/mdadm
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/storage/network
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/storage/raid
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/storage/sysctl
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/group_vars/storage/users
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/host-command-run.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/host-package-update.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7394 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/idrac-bootstrap-one.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10175 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/idrac-bootstrap.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      583 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/inspection-store.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/ip-allocation.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/ip-routing.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3611 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kayobe-ansible-user.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3500 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kayobe-target-venv.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kolla-ansible-user.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10678 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kolla-ansible.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kolla-bifrost-hostvars.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kolla-bifrost.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kolla-build.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kolla-host.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11658 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kolla-openstack.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kolla-pip.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2606 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/kolla-target-venv.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/luks.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/lvm.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/mdadm.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2869 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/network-connectivity.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4603 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/network.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/opensm.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4230 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-bios-raid.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5327 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-deprovision.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-docker-sdk-upgrade.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2588 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-etc-hosts-fixup.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-extras.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-facts-gather.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3393 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-grafana-configure.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5949 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-hardware-inspect.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2449 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-introspection-data-save.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-introspection-rules-dell-lldp-workaround.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3077 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-introspection-rules.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-inventory-discover.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1926 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-ipa-build.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4365 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-ipa-images.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8393 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-provision.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/overcloud-service-config-save.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6505 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/physical-network.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/pip.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6094 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/provision-net.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/public-openrc.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.124585 kayobe-9.3.0/ansible/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/arista-switch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2408 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/arista-switch/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/arista-switch/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/arista-switch/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/arista-switch/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/arista-switch/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/arista-switch/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/arista-switch/templates/arista-config.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.108585 kayobe-9.3.0/ansible/roles/bootstrap/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/bootstrap/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/bootstrap/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/bootstrap/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/bootstrap/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/bootstrap/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/bootstrap/vars/Debian.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/bootstrap/vars/RedHat.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.108585 kayobe-9.3.0/ansible/roles/console-allocation/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/console-allocation/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/console-allocation/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/console-allocation/library/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6361 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/console-allocation/library/console_allocation.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/console-allocation/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1696 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/console-allocation/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.168586 kayobe-9.3.0/ansible/roles/dell-switch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2447 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dell-switch/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dell-switch/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dell-switch/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dell-switch/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dell-switch/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dell-switch/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dell-switch/templates/dellos6-config.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dell-switch/templates/dellos9-config.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dell-switch-bmp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2234 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dell-switch-bmp/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dell-switch-bmp/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dell-switch-bmp/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dell-switch-bmp/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1066 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dell-switch-bmp/handlers/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dell-switch-bmp/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dell-switch-bmp/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dell-switch-bmp/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dell-switch-bmp/templates/dell-switch-bmp.conf.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.112585 kayobe-9.3.0/ansible/roles/deploy-containers/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/deploy-containers/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/deploy-containers/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/deploy-containers/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/deploy-containers/tasks/deploy.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/deploy-containers/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.112585 kayobe-9.3.0/ansible/roles/dev-tools/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dev-tools/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dev-tools/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dev-tools/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dev-tools/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.112585 kayobe-9.3.0/ansible/roles/disable-cloud-init/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/disable-cloud-init/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/disable-cloud-init/handlers/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/disable-cloud-init/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/disable-cloud-init/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/disable-glean/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/disable-glean/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/disable-glean/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/disable-glean/handlers/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/disable-glean/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/disable-glean/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.112585 kayobe-9.3.0/ansible/roles/disable-selinux/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/disable-selinux/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/disable-selinux/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/disable-selinux/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/disable-selinux/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.112585 kayobe-9.3.0/ansible/roles/dnf/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/dnf/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/dnf/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf/tasks/custom-repo.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf/tasks/local-mirror.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/dnf/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf/templates/CentOS-Linux-AppStream.repo.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf/templates/CentOS-Linux-BaseOS.repo.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf/templates/CentOS-Linux-Extras.repo.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf/templates/epel-modular.repo.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf/templates/epel.repo.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.112585 kayobe-9.3.0/ansible/roles/dnf-automatic/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.172586 kayobe-9.3.0/ansible/roles/dnf-automatic/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf-automatic/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/dnf-automatic/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/dnf-automatic/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.112585 kayobe-9.3.0/ansible/roles/docker/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/docker/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/docker/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker/handlers/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/docker/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.112585 kayobe-9.3.0/ansible/roles/docker-devicemapper/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/docker-devicemapper/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-devicemapper/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/docker-devicemapper/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-devicemapper/handlers/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/docker-devicemapper/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2055 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-devicemapper/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/docker-devicemapper/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-devicemapper/templates/docker-thinpool.profile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/docker-registry/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/docker-registry/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3580 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.176586 kayobe-9.3.0/ansible/roles/docker-registry/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/handlers/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/docker-registry/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/tasks/config.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/tasks/deploy.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/tasks/destroy.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/tasks/pull.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/tasks/reconfigure.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/tasks/stop.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/docker-registry/tasks/upgrade.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/drac-boot-mode/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/drac-boot-mode/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/drac-boot-mode/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/drac-boot-mode/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/drac-boot-mode/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2430 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/drac-boot-mode/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/drac-boot-mode/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/drac-boot-mode/vars/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.116585 kayobe-9.3.0/ansible/roles/drac-pxe/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/drac-pxe/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/drac-pxe/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/drac-pxe/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6758 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/drac-pxe/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/drac-pxe/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/drac-pxe/vars/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.116585 kayobe-9.3.0/ansible/roles/image-download/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/image-download/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/image-download/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/image-download/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/image-download/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/inspection-store/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/inspection-store/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.180587 kayobe-9.3.0/ansible/roles/inspection-store/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/handlers/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/inspection-store/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/tasks/config.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/tasks/deploy.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/tasks/destroy.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/tasks/pull.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/tasks/reconfigure.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/tasks/start.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/tasks/stop.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/tasks/upgrade.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/inspection-store/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/inspection-store/templates/nginx.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.116585 kayobe-9.3.0/ansible/roles/ip-allocation/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ip-allocation/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ip-allocation/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ip-allocation/library/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6663 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ip-allocation/library/ip_allocation.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ip-allocation/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ip-allocation/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.116585 kayobe-9.3.0/ansible/roles/ip-routing/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ip-routing/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ip-routing/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ip-routing/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ip-routing/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.116585 kayobe-9.3.0/ansible/roles/ipa-images/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ipa-images/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1920 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ipa-images/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ipa-images/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ipa-images/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ipa-images/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5629 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ipa-images/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2391 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ipa-images/tasks/set-driver-info.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ironic-inspector-rules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ironic-inspector-rules/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ironic-inspector-rules/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ironic-inspector-rules/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ironic-inspector-rules/library/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6538 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ironic-inspector-rules/library/os_ironic_inspector_rule.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ironic-inspector-rules/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ironic-inspector-rules/meta/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/ironic-inspector-rules/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ironic-inspector-rules/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/junos-switch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/junos-switch/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.184587 kayobe-9.3.0/ansible/roles/junos-switch/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/junos-switch/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.188587 kayobe-9.3.0/ansible/roles/junos-switch/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/junos-switch/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.188587 kayobe-9.3.0/ansible/roles/junos-switch/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/junos-switch/templates/junos-config-set.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/junos-switch/templates/junos-config.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/junos-switch/templates/junos-config.json.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.120585 kayobe-9.3.0/ansible/roles/kolla/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/kolla/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/kolla/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla/tasks/config.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2350 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla/tasks/install.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.120585 kayobe-9.3.0/ansible/roles/kolla-ansible/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.188587 kayobe-9.3.0/ansible/roles/kolla-ansible/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9001 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.188587 kayobe-9.3.0/ansible/roles/kolla-ansible/library/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7054 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/library/kolla_passwords.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.188587 kayobe-9.3.0/ansible/roles/kolla-ansible/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5145 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/tasks/config.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2468 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/tasks/install.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.188587 kayobe-9.3.0/ansible/roles/kolla-ansible/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/templates/daemon.json.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21450 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/templates/globals.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2738 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/templates/overcloud-components.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8054 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/templates/overcloud-services.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/templates/overcloud-top-level.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/templates/seed.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-ansible/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/tests/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.120585 kayobe-9.3.0/ansible/roles/kolla-ansible/tests/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-ansible/tests/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/tests/releasenotes/notes/add-support-for-nova-cells-8e18425b52ba06ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7247 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/tests/test-defaults.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21758 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/tests/test-extras.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2423 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/tests/test-requirements.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-ansible/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/vars/Debian.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/vars/RedHat.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6056 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible/vars/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.116585 kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.188587 kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.188587 kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.188587 kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/templates/host-vars.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.188587 kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/tests/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5792 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/tests/test.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.120585 kayobe-9.3.0/ansible/roles/kolla-bifrost/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-bifrost/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2324 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-bifrost/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-bifrost/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-bifrost/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-bifrost/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3271 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-bifrost/templates/bifrost.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-bifrost/templates/dib.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-bifrost/templates/servers.yml.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.120585 kayobe-9.3.0/ansible/roles/kolla-build/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-build/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1243 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-build/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-build/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-build/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-build/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-build/templates/kolla-build.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-build/templates/template-override.j2.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/.ansible-lint
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/.yamllint
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.192587 kayobe-9.3.0/ansible/roles/kolla-openstack/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14939 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.120585 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.196587 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/INSTALL.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2394 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/create.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/destroy.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/molecule.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/playbook.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/prepare.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.196587 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1631 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/tests/test_default.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.196587 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/INSTALL.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/create.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/destroy.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3927 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/molecule.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/playbook.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/prepare.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.196587 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2639 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/tests/test_default.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.196587 kayobe-9.3.0/ansible/roles/kolla-openstack/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6896 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/tasks/config.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.200587 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/aodh.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/backup.my.cnf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/barbican.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/blazar.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/ceilometer.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/cinder.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/cloudkitty.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/designate.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/galera.cnf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/glance.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/global.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/gnocchi.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/grafana.ini.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/heat.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/ironic-inspector.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/ironic.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/kafka.server.properties.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/keystone.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/magnum.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/manila.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/masakari.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1276 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/ml2_conf.ini.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/murano.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/neutron.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/nova.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/octavia.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/sahara.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/templates/zookeeper.cfg.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/kolla-openstack/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7615 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/kolla-openstack/vars/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/nclu-switch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/nclu-switch/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/nclu-switch/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/nclu-switch/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/nclu-switch/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/nclu-switch/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/nclu-switch/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/nclu-switch/templates/nclu-config.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/opensm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/opensm/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/opensm/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/opensm/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/opensm/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/opensm/tasks/deploy.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/opensm/tasks/destroy.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/opensm/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/opensm/tasks/pull.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/opensm/tasks/reconfigure.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/opensm/tasks/stop.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/opensm/tasks/upgrade.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.120585 kayobe-9.3.0/ansible/roles/pip/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/pip/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/pip/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/pip/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/pip/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/pip/tasks/pip_conf.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.124585 kayobe-9.3.0/ansible/roles/public-openrc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.204587 kayobe-9.3.0/ansible/roles/public-openrc/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/public-openrc/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/public-openrc/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/public-openrc/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/public-openrc/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/public-openrc/templates/public-openrc.sh.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.124585 kayobe-9.3.0/ansible/roles/snat/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/snat/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/snat/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.124585 kayobe-9.3.0/ansible/roles/ssh-known-host/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/ssh-known-host/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/ssh-known-host/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.124585 kayobe-9.3.0/ansible/roles/swift-block-devices/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/swift-block-devices/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-block-devices/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/swift-block-devices/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2114 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-block-devices/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/swift-block-devices/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-block-devices/tests/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1835 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-block-devices/tests/test-bootstrapped.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-block-devices/tests/test-invalid-format.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1688 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-block-devices/tests/test-mount.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.124585 kayobe-9.3.0/ansible/roles/swift-rings/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/swift-rings/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1786 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-rings/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/swift-rings/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3590 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-rings/files/swift-ring-builder.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/swift-rings/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2309 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-rings/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/swift-rings/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-rings/templates/swift-ring.yml.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/swift-rings/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/swift-rings/vars/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/sysctl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/sysctl/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/sysctl/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/sysctl/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/sysctl/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/sysctl/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.124585 kayobe-9.3.0/ansible/roles/veth/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/veth/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/veth/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/veth/files/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      295 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/veth/files/ifdown-veth
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      562 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/veth/files/ifup-veth
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.208587 kayobe-9.3.0/ansible/roles/veth/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/veth/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.212587 kayobe-9.3.0/ansible/roles/veth/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/veth/templates/ifcfg-peer.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/veth/templates/ifcfg-veth.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.212587 kayobe-9.3.0/ansible/roles/veth/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/veth/vars/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.124585 kayobe-9.3.0/ansible/roles/wipe-disks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.212587 kayobe-9.3.0/ansible/roles/wipe-disks/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2084 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/roles/wipe-disks/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/seed-deploy-containers.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/seed-hypervisor-libvirt-host.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/seed-introspection-rules.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2379 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/seed-ipa-build.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1798 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/seed-service-upgrade-prep.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/seed-vm-deprovision.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4249 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/seed-vm-provision.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/snat.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/ssh-known-host.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/swift-block-devices.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/swift-rings.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/sysctl.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.212587 kayobe-9.3.0/ansible/test_plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/test_plugins/functional.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/timezone.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/users.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2022-02-01 17:13:48.000000 kayobe-9.3.0/ansible/wipe-disks.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-02-01 17:13:48.000000 kayobe-9.3.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.216588 kayobe-9.3.0/dev/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/config.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      283 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/configure-firewall.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/dev-hosts
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/dev-vagrant-network-allocation.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/dev-vagrant.yml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      570 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/environment-setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26391 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/functions
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      450 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/install-dev.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      446 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/install.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      348 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/overcloud-deploy.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      210 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/overcloud-test-baremetal.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      205 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/overcloud-test-vm.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      348 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/overcloud-upgrade.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       75 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/ovs-vsctl
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      312 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/seed-deploy.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      331 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/seed-hypervisor-deploy.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      312 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/seed-upgrade.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      473 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/tenks-deploy-compute.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1698 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/tenks-deploy-config-compute.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/tenks-deploy-config-overcloud.yml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      475 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/tenks-deploy-overcloud.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      465 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/tenks-deploy.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      463 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/tenks-teardown-compute.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      465 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/tenks-teardown-overcloud.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      455 2022-02-01 17:13:48.000000 kayobe-9.3.0/dev/tenks-teardown.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.216588 kayobe-9.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.220588 kayobe-9.3.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.220588 kayobe-9.3.0/doc/source/_extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/_extra/.htaccess
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.220588 kayobe-9.3.0/doc/source/administration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5181 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/administration/bare-metal.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2649 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/administration/general.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/administration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9537 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/administration/overcloud.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4837 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/administration/seed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2838 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4079 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.220588 kayobe-9.3.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.220588 kayobe-9.3.0/doc/source/configuration/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5181 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/ansible.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12038 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/bifrost.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/docker-registry.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22777 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/hosts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12324 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/ironic-python-agent.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6170 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/kayobe.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27443 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/kolla-ansible.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10129 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/kolla.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34602 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/network.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6651 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/nova-cells.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8034 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/physical-network.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/reference/seed-custom-containers.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.224588 kayobe-9.3.0/doc/source/configuration/scenarios/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.224588 kayobe-9.3.0/doc/source/configuration/scenarios/all-in-one/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3649 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/scenarios/all-in-one/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12439 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/scenarios/all-in-one/overcloud.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/configuration/scenarios/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.224588 kayobe-9.3.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8281 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/contributor/automated.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/contributor/development.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1912 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/contributor/manual.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1680 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/contributor/release-notes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5873 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/contributor/releases.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3718 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/contributor/testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1549 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/contributor/vagrant.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10097 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/control-plane-service-placement.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7424 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/custom-ansible-playbooks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17266 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/deployment.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/getting-started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1138 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4694 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/resources.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/support-matrix.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15124 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/upgrading.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2471 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.224588 kayobe-9.3.0/doc/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1948 2022-02-01 17:13:48.000000 kayobe-9.3.0/doc/test/redirect-tests.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.128585 kayobe-9.3.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/etc/kayobe/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4765 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/bifrost.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/bmc.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4126 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/compute.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4627 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/controllers.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/dell-switch-bmp.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1713 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/dnf.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/dns.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/docker-registry.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/docker.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/globals.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/grafana.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/etc/kayobe/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/hooks/.gitkeep
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/idrac.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5125 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/inspector.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/etc/kayobe/inventory/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.128585 kayobe-9.3.0/etc/kayobe/inventory/group_vars/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/etc/kayobe/inventory/group_vars/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/inventory/group_vars/compute/network-interfaces
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/etc/kayobe/inventory/group_vars/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/inventory/group_vars/controllers/network-interfaces
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/etc/kayobe/inventory/group_vars/overcloud/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/inventory/group_vars/overcloud/ansible-python-interpreter
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/etc/kayobe/inventory/group_vars/seed/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/inventory/group_vars/seed/ansible-python-interpreter
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/inventory/group_vars/seed/network-interfaces
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/etc/kayobe/inventory/group_vars/seed-hypervisor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/inventory/group_vars/seed-hypervisor/ansible-python-interpreter
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/etc/kayobe/inventory/group_vars/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/inventory/group_vars/storage/network-interfaces
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/inventory/groups
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/inventory/hosts.example
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4503 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/ipa.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4338 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/ironic.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/etc/kayobe/kolla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/kolla/globals.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13905 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/kolla.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/monasca.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/monitoring.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6149 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/networks.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2249 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/neutron.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/nova.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/ntp.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/opensm.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/openstack.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/overcloud.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/pip.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3992 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/seed-hypervisor.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/seed-vm.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3482 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/seed.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/ssh.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4255 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/storage.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/swift.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/time.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2022-02-01 17:13:48.000000 kayobe-9.3.0/etc/kayobe/users.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.232588 kayobe-9.3.0/kayobe/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12153 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/ansible.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.236588 kayobe-9.3.0/kayobe/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    72389 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/cli/commands.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.236588 kayobe-9.3.0/kayobe/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/cmd/kayobe.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/cmd/kayobe_vault_password_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8228 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/kolla_ansible.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.236588 kayobe-9.3.0/kayobe/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.236588 kayobe-9.3.0/kayobe/plugins/action/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/plugins/action/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6984 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/plugins/action/kolla_ansible_host_vars.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.236588 kayobe-9.3.0/kayobe/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.236588 kayobe-9.3.0/kayobe/tests/molecule/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/molecule/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2139 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/molecule/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.240588 kayobe-9.3.0/kayobe/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.240588 kayobe-9.3.0/kayobe/tests/unit/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/unit/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    76378 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/unit/cli/test_commands.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.240588 kayobe-9.3.0/kayobe/tests/unit/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/unit/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.240588 kayobe-9.3.0/kayobe/tests/unit/plugins/action/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/unit/plugins/action/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14895 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/unit/plugins/action/test_kolla_ansible_host_vars.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23916 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/unit/test_ansible.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12831 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/unit/test_kolla_ansible.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7275 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4478 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/tests/unit/test_vault.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7613 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4950 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/vault.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2022-02-01 17:13:48.000000 kayobe-9.3.0/kayobe/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.236588 kayobe-9.3.0/kayobe.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3834 2022-02-01 17:14:25.000000 kayobe-9.3.0/kayobe.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37636 2022-02-01 17:14:26.000000 kayobe-9.3.0/kayobe.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-02-01 17:14:25.000000 kayobe-9.3.0/kayobe.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8656 2022-02-01 17:14:25.000000 kayobe-9.3.0/kayobe.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-02-01 17:14:25.000000 kayobe-9.3.0/kayobe.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-02-01 17:14:25.000000 kayobe-9.3.0/kayobe.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2022-02-01 17:14:25.000000 kayobe-9.3.0/kayobe.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.240588 kayobe-9.3.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.240588 kayobe-9.3.0/playbooks/kayobe-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-base/post.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2086 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-base/pre.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.240588 kayobe-9.3.0/playbooks/kayobe-overcloud-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-base/globals.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1703 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-base/overrides.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1706 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-base/pre.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1141 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-base/run.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.240588 kayobe-9.3.0/playbooks/kayobe-overcloud-host-configure-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3200 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-host-configure-base/overrides.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1371 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-host-configure-base/pre.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1521 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-host-configure-base/run.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.240588 kayobe-9.3.0/playbooks/kayobe-overcloud-host-configure-base/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4936 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-host-configure-base/tests/test_overcloud_host_configure.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.240588 kayobe-9.3.0/playbooks/kayobe-overcloud-upgrade-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-upgrade-base/globals.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-upgrade-base/overrides.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-upgrade-base/pre.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4049 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-overcloud-upgrade-base/run.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.244588 kayobe-9.3.0/playbooks/kayobe-seed-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-base/bifrost-overrides.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-base/globals.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1817 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-base/overrides.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-base/pre.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-base/run.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.244588 kayobe-9.3.0/playbooks/kayobe-seed-upgrade-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-upgrade-base/bifrost-overrides.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-upgrade-base/globals.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-upgrade-base/overrides.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-upgrade-base/pre.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-upgrade-base/run.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.244588 kayobe-9.3.0/playbooks/kayobe-seed-vm-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-vm-base/overrides.yml.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2236 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-vm-base/pre.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-vm-base/run.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-seed-vm-base/seed-group-vars.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.244588 kayobe-9.3.0/playbooks/kayobe-tox-molecule/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2022-02-01 17:13:48.000000 kayobe-9.3.0/playbooks/kayobe-tox-molecule/pre.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.132585 kayobe-9.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.280589 kayobe-9.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-admin-network.yml-cf4b5e6387d0eb3f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-command-hooks-827aa0732b7399de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-custom-config-for-elasticsearch-a762134e51b50f91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-ironic-node-serial-console-commands-75f1255d62e05c87.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-kolla_ansible_venv_extra_requirements-4d4f70b024207ffb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-monasca-3e6da709b3b4c269.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-monasca-defaults-8486abe37ed3a13b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-serial-console-enable-to-post-configure-c61704185c57783d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-stop-command-8f66235870720f31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-storm-5d29163b61ef01ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-barbican-conf-c15f0ab4294281cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-configuring-mariadb-646badcc9dd07019.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-custom-aodh-conf-81a5a623f771d1c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-custom-blazar-conf-c82ee78f2a92d693.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-custom-ceilometer-conf-66d907cf3c7ec29b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-custom-cloudkitty-conf-af224caad9cd1ad4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-custom-gnocchi-conf-51b110196f966c32.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-custom-group-vars-3760547c3505487d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-custom-masakari-conf-af224cead3cd1ad4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-global-conf-411316a7250611b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-support-for-haproxy-config-b7b8f331e8adb2e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add-variable-docker-registry-datadir-volume-a5ec931a5eb2c59d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add_support_for_custom_barbican_conf-b94272d73d53aa87.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/add_support_for_custom_keepalived_conf-b26a242761c1f5b3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ansible-2.5-2.7-c06a682f4f07755d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ansible-2.5-785e3c764f450d09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ansible-2.6-2.8-ce141db0edb87e1c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ansible-2.8-2.9-2df006b066704417.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      562 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ansible-facts-2b3389a2534d47a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/arista-switch-aedc46148506c56e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ask-vault-pass-b6ced0220384dde1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/avoid-unconditional-fact-gathering-4dfbf96e2111ad51.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bifrost-dib-extra-c4eac903986ec700.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bifrost-firewalld-zone-09a29651a058531a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bifrost-ironic-extra-kernel-params-e3e56a9dcdf24bb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bifrost-use-firewalld-90b69e2ac6eead67.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bifrost-victoria-fixes-eed49b088afdac5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/blacklist-ansible-2.9.8-f83ad748b01a575b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bootproto-52316b6dbc30e98c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bootstrap-openrc-9aec3d53d0d62c81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bootstrap-servers-user-8cb5114de1dd10ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bugfix-dnf-proxy-cd934867c3d64388.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bugfix-monasca-grafana-dashboard-config-b81781cf10c2a236.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/bugfix-update-idrac-role-71ede6900dc000a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/build-neutron-sriov-836acf378bae0b48.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/cacert-514b8645d6912bf9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/centos-8-12073e91a157d0a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/centos-8-chrony-bec9d7bc8b346363.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/centos-8.3-89d07c8f8db5b17b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/centos-ipa-images-60dde12f2b4f4f8c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/concurrent-known-hosts-update-8dc94557e9a48021.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/config-galaxy-roles-6bd129824436a983.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/cumulus-switch-baf554118ef23afe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/custom-ansible-config-d0f1bcdf2607e521.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/custom-certificates-5f2c1fff6503b77a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/custom-route-options-2ed446961262a34a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/db-backup-recovery-d4f1ced2ebd7dac4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/default-disable-ironic-2c20b8a7e69f19c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/default-lvm-data-vg-f2848066975beeda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/default-overlay2-970bdb5b7b62b60a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/default-target-virtualenv-3a68472f66b7aaf3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/defroute-9bbcff8b2f8abc94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/dell-powerconnect-switch-860fbcbf7e4323ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/deploy_containers-4199127a91f29be0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/disable-bifrost-cleaning-ff10995a0bf11079.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/disable-chrony-5f1e4f9db509c42d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/disable-ironic-networks-86ba35f58f317ab6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/dnf-2071fc40b0d783b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/dnf-proxy-22a6eb457c06a223.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/docker-custom-config-5103260d5ddb7223.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/docker-registry-basic-auth-b94b4a66e1ce9095.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/docker-registry-env-e954a0642555864f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/docker-registry-on-seed-2eb4fb643d6fda9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/docker-registry-tls-a823fc5717ef2b52.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/docker-storage-driver-7d560e7d350b14ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/drop-kolla-ceph-deployment-47095b032085e8f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/drop-py-2-7-3d0a7f3eb8f11d6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ethtool-options-e90ace0555e3fba3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/external-api-no-ip-f04951ffc9659949.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/extra-kernel-options-strings-bec7d851e334fec5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/feature-automatic-node-rename-fc5fbe0f7c38151c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/feature-update-ironic-driver-info-02371a593ca0f734.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/filter-out-ruckus-lldp-port-description-ad2b0774609aedbf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/first-official-release-6dff5747d34d161c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-baremetal-compute-commands-b72862a53f88c5ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-baremetal-serial-autoenable-0ccfec017cf2ddbc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-bifrost-ironic-extra-kernel-params-9ebdec1212ac9827.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-coreutils-single-conflict-208036c66b9f7e59.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-data-files-path-detection-on-ubuntu-dfa8e4e7a1d3ea27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-default-docker-storage-driver-e05832be7a4c2ab8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-default-public-net-name-067338275460b50d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-dell-physical-network-config-b4eaf752e62eeadb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-disable-selinux-not-installed-eff17c715efc1fdb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-image-build-regex-964c8c6359841662.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-inspection-when-using-ipxe-9bf6ed9e6456840b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-inspector-ipxe-uefi-86f435ebaf4eee08.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-inspector-rule-idempotency-f6e5a61f7dca580f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-introspection-data-save-51001baa37d97084.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-introspection-data-save-cfc83714f66fd63c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-ipa-build-b31fb20ddcbe3ece.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-ipa-image-download-3f90f0f40d0feafd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-limit-with-commas-04a357b0b7ef0371.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-network-hosts-interfaces-f0206aa91b218a25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-no-ip-addr-on-nic-38d6f8e8078f534d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-persistent-sysctls-1aef170599a49608.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-post-config-public-eb72f3a692a2be6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-python-setup-5e7ff929a6cab092.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-remote-seed-vm-provisioning-faa8de569ca6bc89.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-seed-multiple-networks-458915b085a9478c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-seed-vm-provision-c432ebfae8bfee8b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fix-selinux-disable-reboot-65c32f5dc895211c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/fluentd-custom-inputs-1b911bd229e8a9e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/hardware-inspection-timeouts-777f3bb569929f0f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/host-package-update-c5bddba791754646.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/host-run-command-eb98cb077d546551.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ignore-unconfigured-nets-93beaf96f43af1ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/improve-ssh-known-host-error-15fbc6ae4fa3dbd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/initial-f71c8e25375afa25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/inspector-25gbe-port-9bdc3bb354e3dfb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/inspector-dhcp-range-netmask-bb46eb7df77587a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/install-prefix-multiple-lib-9288e8c11da3c0bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/internal-api-tls-4e7383e6a0262f5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ipa-build-dib-packages-5e85baba3294eb65.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ipa-build-upper-constraints-5686abaa161b0d94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1345 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ipa-builder-ea6308b6691ae71e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/kolla-ansible-become-false-95aa88edd3c8c259.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/kolla-docker-registry-e1adce280fc17db7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/kolla-enable-openstack-core-ce4866dd388f262e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/kolla-external-fqdn-cacert-048aa1299050cfd7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/kolla-inventory-host-vars-7f9dc14c82e3ea20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/kolla-tag-and-suffix-a223b0c7173a245e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/kolla-user-group-85bbe8038c3f719c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/luks-ed1d301ad0168e91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/manage-lvm-0.1.4-d33b398060232874.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/mariabackup-9370d55279c1aa78.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/mdadm-ed1d301ad0168e91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/mellanox-switch-cb82a8c278f5e652.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/neutron-mlnx-agent-19631a3936da47df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/non-shared-ironic-nets-06a43c9b6dea2a77.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/openrc-upgrade-9e14888d600f6839.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/openstack-branch-87df0c2f647037c0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/optional-epel-release-92eaf3dc4aa1021b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/package-runtime-files-in-python-package-c3dda2bd32844fdf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/passwords-in-tmp-18e55d5e9b894b4d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/per-host-interfaces-6e548331fa3a4244.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/physical-network-disable-discovery-15916760e0a4d0bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/pip-index-url-conditional-3f9c5b3c5c808500.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/pip-local-mirror-d9a80257c8441970.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/pip_proxy-6c6022b6566dae69.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/plug-ovs-phy-f180d9bb9dd25dab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/prevent-resolv.conf-4a09d50f60f3fe28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/prevent-wrong-oscacert-variable-9ede7f60c1562a77.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/public-os-endpoint-type-a678a8ddc51ce3b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/quote-escape-vars-3d42c7de8dc39d15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/quote-kolla-limit-042422e69c008109.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-congress-support-0f6a327de69e2173.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-ifcfg-eth0-c179ea98fc34e164.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-inspector-manage-firewall-b1117b04a0f6904d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-ironic-drivers-939a9c6afad33e2a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-libvirt-pool-capacity-e428b893ca5bdb88.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-mongodb-fcdfba997e1abb51.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-neutron-fwaas-0g6a327ae69e2117.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-opendaylight-ac316f8ada083cc9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-overcloud-cadvisor-deployment-3866f823cd1dc0b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-overcloud-cloud-init-workaround-4f4643f15c20b2e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-overcloud-prometheus-deployment-75792bba2fc39385.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-resolv-conf-workaround-4cb484d3a66c4e58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-stop-chrony-1944c6cba72730c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-storage-mgmt-net-from-controllers-8f9c1d252d9f318b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/remove-yum-variables-0a1ab4e958c27171.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/restrict-ip-allocation-8e20022110c2283e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/rocky-355875d3f38b0d02.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/save-include-exclude-df8cca17da0aa3de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/seed-hypervisor-bootstrap-58bafc1ea0d125bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/seed-hypervisor-host-package-update-2ad745a2d9fec134.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/seed-hypervisor-host-package-update-fix-9411205aadc92b8f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/seed-hypervisor-lvm-80864721ff42f6a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/seed-service-upgrade-71b847e3658a1948.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/seed-vm-centos-8.2-36b7a480a7725da1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/seed-vm-centos-8.3-7726c9d0603508eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/seperate-storage-networks-a659bcd30dd70665.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/setup-module-args-2c36e56bf78ab5f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ssh-batchmode-cda7a4ed63006378.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/stale-virtualenvs-125c513af3de9396.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/story-2007297-73f498ef6bc89fe9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/story-2008354-0c34e2ad7aeb7d3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/story-2008430-6a50101d05219aad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/support-deploy-containers-7acf4c647fb5c3fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/support_configuring_tunnel_network-1646eef887d72abf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/support_ironic_neutron_agent-a41e44ef41f5a96d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/swift-improvements-07a2b75967f642e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/tftp-listen-on-internal-interface-09aeec7ad99fc13d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/timezone-config-298cff76834f5fb4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/use-public-fqdn-in-openrc-f7990958ceec817d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/ussuri-prelude-25dc5d922eff1104.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/workaround-bifrost-ipa-kernel-rename-59bf75ac8285f103.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/workaround-cloud-init-vlan-0efa97b866d46783.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/yum-config-58274185a00004e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/notes/yum-repository-metalink-26afa7c9f7026539.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.284590 kayobe-9.3.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.284590 kayobe-9.3.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.284590 kayobe-9.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8144 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5142 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6307 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-02-01 17:13:48.000000 kayobe-9.3.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-02-01 17:13:48.000000 kayobe-9.3.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2022-02-01 17:13:48.000000 kayobe-9.3.0/requirements.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.284590 kayobe-9.3.0/roles/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-02-01 17:13:48.000000 kayobe-9.3.0/roles/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.132585 kayobe-9.3.0/roles/kayobe-ci-prep/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.284590 kayobe-9.3.0/roles/kayobe-ci-prep/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2022-02-01 17:13:48.000000 kayobe-9.3.0/roles/kayobe-ci-prep/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.284590 kayobe-9.3.0/roles/kayobe-diagnostics/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-02-01 17:13:48.000000 kayobe-9.3.0/roles/kayobe-diagnostics/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.284590 kayobe-9.3.0/roles/kayobe-diagnostics/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2022-02-01 17:13:48.000000 kayobe-9.3.0/roles/kayobe-diagnostics/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.284590 kayobe-9.3.0/roles/kayobe-diagnostics/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4832 2022-02-01 17:13:48.000000 kayobe-9.3.0/roles/kayobe-diagnostics/files/get_logs.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.284590 kayobe-9.3.0/roles/kayobe-diagnostics/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-02-01 17:13:48.000000 kayobe-9.3.0/roles/kayobe-diagnostics/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2022-02-01 17:13:48.000000 kayobe-9.3.0/roles/kayobe-diagnostics/tasks/post.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2022-02-01 17:13:48.000000 kayobe-9.3.0/roles/kayobe-diagnostics/tasks/pre.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9854 2022-02-01 17:14:26.288590 kayobe-9.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2022-02-01 17:13:48.000000 kayobe-9.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-02-01 17:13:48.000000 kayobe-9.3.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.288590 kayobe-9.3.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      367 2022-02-01 17:13:48.000000 kayobe-9.3.0/tools/ansible-galaxy-retried.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      404 2022-02-01 17:13:48.000000 kayobe-9.3.0/tools/feature-flags.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      624 2022-02-01 17:13:48.000000 kayobe-9.3.0/tools/loc
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1895 2022-02-01 17:13:48.000000 kayobe-9.3.0/tools/release.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      363 2022-02-01 17:13:48.000000 kayobe-9.3.0/tools/run-bashate.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1154 2022-02-01 17:13:48.000000 kayobe-9.3.0/tools/sphinx8
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      703 2022-02-01 17:13:48.000000 kayobe-9.3.0/tools/test-ansible.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      696 2022-02-01 17:13:48.000000 kayobe-9.3.0/tools/test-molecule.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4260 2022-02-01 17:13:48.000000 kayobe-9.3.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-02-01 17:14:26.288590 kayobe-9.3.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6206 2022-02-01 17:13:48.000000 kayobe-9.3.0/zuul.d/jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2022-02-01 17:13:48.000000 kayobe-9.3.0/zuul.d/nodesets.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      974 2022-02-01 17:13:48.000000 kayobe-9.3.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2022-04-28 10:15:35.000000 kayobe-9.4.0/.coveragerc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.353728 kayobe-9.4.0/.github/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-04-28 10:15:35.000000 kayobe-9.4.0/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-04-28 10:15:35.000000 kayobe-9.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2022-04-28 10:15:35.000000 kayobe-9.4.0/.yamllint
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2383 2022-04-28 10:16:06.000000 kayobe-9.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2022-04-28 10:15:35.000000 kayobe-9.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62947 2022-04-28 10:16:06.000000 kayobe-9.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-04-28 10:15:35.000000 kayobe-9.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-04-28 10:15:35.000000 kayobe-9.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3834 2022-04-28 10:16:06.437739 kayobe-9.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2404 2022-04-28 10:15:35.000000 kayobe-9.4.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1889 2022-04-28 10:15:35.000000 kayobe-9.4.0/Vagrantfile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.365730 kayobe-9.4.0/ansible/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.365730 kayobe-9.4.0/ansible/action_plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/action_plugins/kolla_ansible_host_vars.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1982 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/baremetal-compute-inspect.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/baremetal-compute-manage.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/baremetal-compute-provide.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2631 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/baremetal-compute-rename.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/baremetal-compute-serial-console-post-config.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5520 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/baremetal-compute-serial-console.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/bootstrap.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2392 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/compute-node-discovery.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/compute-node-provide.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/container-image-build.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/container-image-builders-check.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/dell-compute-node-boot-mode.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/dell-compute-node-discovery.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/dell-compute-node-inventory.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/dell-switch-bmp.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/dev-tools.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/disable-cloud-init.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/disable-glean.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/disable-selinux.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/dnf.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1633 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/docker-devicemapper.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/docker-registry.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/docker.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/drac-bios.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/drac-boot-order.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/drac-facts.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/dump-config.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/external-net.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.365730 kayobe-9.4.0/ansible/filter_plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/filter_plugins/bmc_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19219 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/filter_plugins/networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2533 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/filter_plugins/switches.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.341727 kayobe-9.4.0/ansible/group_vars/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.365730 kayobe-9.4.0/ansible/group_vars/all/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5157 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/bifrost
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/bmc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5083 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/compute
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6088 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/controllers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/dell-switch-bmp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/dnf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/dns
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/docker
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/docker-registry
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1624 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/globals
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/grafana
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/idrac
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13346 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/inspector
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6302 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/ipa
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4850 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/ironic
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22366 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/kolla
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/monasca
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3948 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/monitoring
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/network
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2536 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/neutron
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/nova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/opensm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2372 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/openstack
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/overcloud
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/pip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4154 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/seed
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5047 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/seed-hypervisor
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/seed-vm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/ssh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5531 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/storage
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2622 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/swift
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.369730 kayobe-9.4.0/ansible/group_vars/all/switches/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      646 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/switches/arista
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/switches/config
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/switches/dell
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/switches/dell-powerconnect
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/switches/junos
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/switches/mellanox
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/time
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/all/users
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.369730 kayobe-9.4.0/ansible/group_vars/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/compute/ansible-user
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/compute/bios
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/compute/luks
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/compute/lvm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/compute/mdadm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/compute/network
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/compute/raid
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/compute/sysctl
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/compute/users
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.369730 kayobe-9.4.0/ansible/group_vars/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/controllers/ansible-user
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/controllers/bios
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/controllers/luks
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/controllers/lvm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/controllers/mdadm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/controllers/network
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/controllers/raid
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/controllers/sysctl
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/controllers/users
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.369730 kayobe-9.4.0/ansible/group_vars/monitoring/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/monitoring/ansible-user
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/monitoring/bios
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/monitoring/luks
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/monitoring/lvm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/monitoring/mdadm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/monitoring/network
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/monitoring/raid
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/monitoring/sysctl
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/monitoring/users
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.369730 kayobe-9.4.0/ansible/group_vars/overcloud/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/overcloud/ansible-host
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.369730 kayobe-9.4.0/ansible/group_vars/seed/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed/ansible-host
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed/ansible-user
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed/luks
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed/lvm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed/mdadm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed/network
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed/sysctl
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed/users
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/group_vars/seed-hypervisor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed-hypervisor/ansible-host
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed-hypervisor/ansible-user
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed-hypervisor/luks
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed-hypervisor/lvm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed-hypervisor/mdadm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed-hypervisor/network
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed-hypervisor/sysctl
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/seed-hypervisor/users
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/group_vars/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/storage/ansible-user
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/storage/bios
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/storage/luks
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/storage/lvm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/storage/mdadm
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/storage/network
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/storage/raid
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/storage/sysctl
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/group_vars/storage/users
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/host-command-run.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/host-package-update.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7394 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/idrac-bootstrap-one.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10175 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/idrac-bootstrap.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      583 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/inspection-store.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/ip-allocation.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/ip-routing.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3611 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kayobe-ansible-user.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3500 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kayobe-target-venv.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kolla-ansible-user.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10678 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kolla-ansible.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kolla-bifrost-hostvars.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1318 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kolla-bifrost.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kolla-build.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kolla-host.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11658 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kolla-openstack.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kolla-pip.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2606 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/kolla-target-venv.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/luks.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/lvm.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/mdadm.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2869 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/network-connectivity.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4644 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/network.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/opensm.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4230 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-bios-raid.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5327 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-deprovision.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-docker-sdk-upgrade.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2588 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-etc-hosts-fixup.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-extras.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-facts-gather.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3393 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-grafana-configure.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5949 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-hardware-inspect.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2449 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-introspection-data-save.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-introspection-rules-dell-lldp-workaround.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3077 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-introspection-rules.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-inventory-discover.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1926 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-ipa-build.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4365 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-ipa-images.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8393 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-provision.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/overcloud-service-config-save.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6505 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/physical-network.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/pip.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6090 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/provision-net.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/public-openrc.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/ansible/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/arista-switch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2408 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/arista-switch/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/arista-switch/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/arista-switch/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/arista-switch/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/arista-switch/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/arista-switch/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/arista-switch/templates/arista-config.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.341727 kayobe-9.4.0/ansible/roles/bootstrap/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/bootstrap/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/bootstrap/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/bootstrap/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/bootstrap/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/bootstrap/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/bootstrap/vars/Debian.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/bootstrap/vars/RedHat.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.341727 kayobe-9.4.0/ansible/roles/console-allocation/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/console-allocation/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/console-allocation/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/console-allocation/library/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6361 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/console-allocation/library/console_allocation.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/console-allocation/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1696 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/console-allocation/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/dell-switch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2447 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dell-switch/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/dell-switch/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dell-switch/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/dell-switch/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dell-switch/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/dell-switch/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dell-switch/templates/dellos6-config.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dell-switch/templates/dellos9-config.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/dell-switch-bmp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2234 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dell-switch-bmp/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/dell-switch-bmp/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dell-switch-bmp/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/dell-switch-bmp/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1066 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dell-switch-bmp/handlers/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/dell-switch-bmp/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dell-switch-bmp/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/dell-switch-bmp/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dell-switch-bmp/templates/dell-switch-bmp.conf.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.341727 kayobe-9.4.0/ansible/roles/deploy-containers/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/deploy-containers/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/deploy-containers/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/deploy-containers/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/deploy-containers/tasks/deploy.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/deploy-containers/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.341727 kayobe-9.4.0/ansible/roles/dev-tools/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.373731 kayobe-9.4.0/ansible/roles/dev-tools/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dev-tools/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/dev-tools/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dev-tools/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.341727 kayobe-9.4.0/ansible/roles/disable-cloud-init/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/disable-cloud-init/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/disable-cloud-init/handlers/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/disable-cloud-init/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/disable-cloud-init/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/disable-glean/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/disable-glean/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/disable-glean/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/disable-glean/handlers/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/disable-glean/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/disable-glean/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.341727 kayobe-9.4.0/ansible/roles/disable-selinux/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/disable-selinux/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/disable-selinux/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/disable-selinux/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/disable-selinux/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.341727 kayobe-9.4.0/ansible/roles/dnf/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/dnf/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/dnf/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/tasks/custom-repo.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/tasks/local-mirror.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/dnf/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/templates/CentOS-Linux-AppStream.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/templates/CentOS-Linux-BaseOS.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/templates/CentOS-Linux-Extras.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/templates/CentOS-Stream-AppStream.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/templates/CentOS-Stream-BaseOS.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/templates/CentOS-Stream-Extras.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/templates/epel-modular.repo.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf/templates/epel.repo.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.341727 kayobe-9.4.0/ansible/roles/dnf-automatic/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/dnf-automatic/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf-automatic/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/dnf-automatic/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/dnf-automatic/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/docker/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker/handlers/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.341727 kayobe-9.4.0/ansible/roles/docker-devicemapper/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker-devicemapper/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-devicemapper/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker-devicemapper/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-devicemapper/handlers/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker-devicemapper/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2055 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-devicemapper/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker-devicemapper/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-devicemapper/templates/docker-thinpool.profile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker-registry/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker-registry/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3580 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker-registry/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/handlers/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/docker-registry/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/tasks/config.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/tasks/deploy.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/tasks/destroy.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/tasks/pull.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/tasks/reconfigure.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/tasks/stop.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/docker-registry/tasks/upgrade.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/drac-boot-mode/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/drac-boot-mode/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.377731 kayobe-9.4.0/ansible/roles/drac-boot-mode/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/drac-boot-mode/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/drac-boot-mode/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2430 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/drac-boot-mode/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/drac-boot-mode/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/drac-boot-mode/vars/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/drac-pxe/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/drac-pxe/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/drac-pxe/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/drac-pxe/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6758 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/drac-pxe/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/drac-pxe/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/drac-pxe/vars/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/image-download/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/image-download/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/image-download/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/image-download/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/image-download/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/inspection-store/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/inspection-store/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/inspection-store/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/handlers/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/inspection-store/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/tasks/config.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/tasks/deploy.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/tasks/destroy.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/tasks/pull.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/tasks/reconfigure.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/tasks/start.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/tasks/stop.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/tasks/upgrade.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/inspection-store/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/inspection-store/templates/nginx.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/ip-allocation/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ip-allocation/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ip-allocation/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ip-allocation/library/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6663 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ip-allocation/library/ip_allocation.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ip-allocation/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ip-allocation/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/ip-routing/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ip-routing/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ip-routing/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ip-routing/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ip-routing/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/ipa-images/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ipa-images/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1920 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ipa-images/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ipa-images/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ipa-images/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ipa-images/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5629 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ipa-images/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2391 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ipa-images/tasks/set-driver-info.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ironic-inspector-rules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ironic-inspector-rules/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ironic-inspector-rules/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ironic-inspector-rules/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ironic-inspector-rules/library/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6538 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ironic-inspector-rules/library/os_ironic_inspector_rule.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ironic-inspector-rules/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ironic-inspector-rules/meta/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/ironic-inspector-rules/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ironic-inspector-rules/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/junos-switch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/junos-switch/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/junos-switch/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/junos-switch/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/junos-switch/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/junos-switch/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/junos-switch/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/junos-switch/templates/junos-config-set.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/junos-switch/templates/junos-config.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/junos-switch/templates/junos-config.json.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/ansible/roles/kolla/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/kolla/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/kolla/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla/tasks/config.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2350 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla/tasks/install.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/kolla-ansible/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-ansible/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9001 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-ansible/library/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7054 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/library/kolla_passwords.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-ansible/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5145 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/tasks/config.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2468 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/tasks/install.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-ansible/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/templates/daemon.json.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21450 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/templates/globals.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2738 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/templates/overcloud-components.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8054 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/templates/overcloud-services.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1934 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/templates/overcloud-top-level.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/templates/seed.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-ansible/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/tests/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/kolla-ansible/tests/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-ansible/tests/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/tests/releasenotes/notes/add-support-for-nova-cells-8e18425b52ba06ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7247 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/tests/test-defaults.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21758 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/tests/test-extras.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2423 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/tests/test-requirements.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-ansible/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/vars/Debian.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/vars/RedHat.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6056 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible/vars/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.381732 kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/templates/host-vars.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/tests/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5792 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/tests/test.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/kolla-bifrost/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-bifrost/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2324 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-bifrost/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-bifrost/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-bifrost/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-bifrost/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3271 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-bifrost/templates/bifrost.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-bifrost/templates/dib.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-bifrost/templates/servers.yml.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/kolla-build/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-build/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1243 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-build/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-build/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-build/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-build/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-build/templates/kolla-build.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-build/templates/template-override.j2.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/.ansible-lint
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/.yamllint
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.385733 kayobe-9.4.0/ansible/roles/kolla-openstack/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14939 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.345727 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.389733 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/INSTALL.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2394 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/create.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/destroy.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/molecule.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/playbook.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/prepare.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.389733 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1631 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/tests/test_default.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.389733 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/INSTALL.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/create.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/destroy.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3954 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/molecule.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/playbook.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/prepare.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.389733 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2639 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/tests/test_default.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.389733 kayobe-9.4.0/ansible/roles/kolla-openstack/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6878 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/tasks/config.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/aodh.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/backup.my.cnf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/barbican.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/blazar.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/ceilometer.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/cinder.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/cloudkitty.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/designate.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/galera.cnf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/glance.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/global.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/gnocchi.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/grafana.ini.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/heat.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/ironic-inspector.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/ironic.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/kafka.server.properties.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/keystone.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/magnum.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/manila.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/masakari.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1276 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/ml2_conf.ini.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/murano.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/neutron.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/nova.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/octavia.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/sahara.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/templates/zookeeper.cfg.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/kolla-openstack/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7615 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/kolla-openstack/vars/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/nclu-switch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/nclu-switch/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/nclu-switch/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/nclu-switch/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/nclu-switch/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/nclu-switch/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/nclu-switch/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/nclu-switch/templates/nclu-config.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/opensm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/opensm/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/opensm/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/opensm/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/opensm/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/opensm/tasks/deploy.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/opensm/tasks/destroy.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/opensm/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/opensm/tasks/pull.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/opensm/tasks/reconfigure.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/opensm/tasks/stop.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/opensm/tasks/upgrade.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/ansible/roles/pip/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/pip/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/pip/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/pip/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/pip/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/pip/tasks/pip_conf.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/ansible/roles/public-openrc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/public-openrc/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/public-openrc/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/public-openrc/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/public-openrc/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/public-openrc/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/public-openrc/templates/public-openrc.sh.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/ansible/roles/snat/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/snat/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/snat/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/ansible/roles/ssh-known-host/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/ssh-known-host/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/ssh-known-host/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/ansible/roles/swift-block-devices/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/swift-block-devices/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-block-devices/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/swift-block-devices/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2114 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-block-devices/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/swift-block-devices/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-block-devices/tests/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1835 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-block-devices/tests/test-bootstrapped.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-block-devices/tests/test-invalid-format.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1688 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-block-devices/tests/test-mount.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/ansible/roles/swift-rings/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/swift-rings/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1786 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-rings/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/swift-rings/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3590 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-rings/files/swift-ring-builder.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/swift-rings/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2309 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-rings/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.393733 kayobe-9.4.0/ansible/roles/swift-rings/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-rings/templates/swift-ring.yml.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/roles/swift-rings/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/swift-rings/vars/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/roles/sysctl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/sysctl/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/roles/sysctl/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/sysctl/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/roles/sysctl/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/sysctl/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/ansible/roles/veth/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/roles/veth/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/veth/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/roles/veth/files/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      295 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/veth/files/ifdown-veth
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      562 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/veth/files/ifup-veth
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/roles/veth/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/veth/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/roles/veth/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/veth/templates/ifcfg-peer.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/veth/templates/ifcfg-veth.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/roles/veth/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/veth/vars/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/ansible/roles/wipe-disks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/roles/wipe-disks/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2084 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/roles/wipe-disks/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/seed-deploy-containers.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/seed-hypervisor-libvirt-host.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/seed-introspection-rules.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2379 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/seed-ipa-build.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1798 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/seed-service-upgrade-prep.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/seed-vm-deprovision.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4249 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/seed-vm-provision.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/snat.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/ssh-known-host.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/swift-block-devices.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/swift-rings.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/sysctl.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/ansible/test_plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/test_plugins/functional.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/timezone.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/users.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2022-04-28 10:15:35.000000 kayobe-9.4.0/ansible/wipe-disks.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-04-28 10:15:35.000000 kayobe-9.4.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/dev/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/config.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      283 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/configure-firewall.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/dev-hosts
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/dev-vagrant-network-allocation.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/dev-vagrant.yml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      570 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/environment-setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26886 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/functions
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      450 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/install-dev.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      446 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/install.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      348 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/overcloud-deploy.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      210 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/overcloud-test-baremetal.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      205 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/overcloud-test-vm.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      348 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/overcloud-upgrade.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       75 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/ovs-vsctl
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      312 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/seed-deploy.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      331 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/seed-hypervisor-deploy.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      312 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/seed-upgrade.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      473 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/tenks-deploy-compute.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1698 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/tenks-deploy-config-compute.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/tenks-deploy-config-overcloud.yml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      475 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/tenks-deploy-overcloud.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      465 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/tenks-deploy.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      463 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/tenks-teardown-compute.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      465 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/tenks-teardown-overcloud.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      455 2022-04-28 10:15:35.000000 kayobe-9.4.0/dev/tenks-teardown.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.397734 kayobe-9.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.401734 kayobe-9.4.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.401734 kayobe-9.4.0/doc/source/_extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/_extra/.htaccess
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.401734 kayobe-9.4.0/doc/source/administration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5181 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/administration/bare-metal.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2649 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/administration/general.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/administration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9537 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/administration/overcloud.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4837 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/administration/seed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2838 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4079 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.401734 kayobe-9.4.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.401734 kayobe-9.4.0/doc/source/configuration/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5181 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/ansible.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12045 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/bifrost.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/docker-registry.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22792 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/hosts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12484 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/ironic-python-agent.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6170 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/kayobe.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27443 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/kolla-ansible.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10129 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/kolla.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34602 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/network.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6651 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/nova-cells.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8034 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/physical-network.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/reference/seed-custom-containers.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.401734 kayobe-9.4.0/doc/source/configuration/scenarios/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.401734 kayobe-9.4.0/doc/source/configuration/scenarios/all-in-one/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3649 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/scenarios/all-in-one/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12439 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/scenarios/all-in-one/overcloud.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/configuration/scenarios/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.405735 kayobe-9.4.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8281 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/contributor/automated.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/contributor/development.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1912 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/contributor/manual.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1680 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/contributor/release-notes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5873 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/contributor/releases.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3718 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/contributor/testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1549 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/contributor/vagrant.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10097 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/control-plane-service-placement.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7424 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/custom-ansible-playbooks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17266 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/deployment.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/getting-started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1138 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4694 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/resources.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/support-matrix.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15124 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/upgrading.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2471 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.405735 kayobe-9.4.0/doc/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1948 2022-04-28 10:15:35.000000 kayobe-9.4.0/doc/test/redirect-tests.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.405735 kayobe-9.4.0/etc/kayobe/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4765 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/bifrost.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/bmc.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4126 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/compute.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4627 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/controllers.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/dell-switch-bmp.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1713 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/dnf.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/dns.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/docker-registry.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/docker.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/globals.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/grafana.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.405735 kayobe-9.4.0/etc/kayobe/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/hooks/.gitkeep
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/idrac.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5125 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/inspector.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.405735 kayobe-9.4.0/etc/kayobe/inventory/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.349728 kayobe-9.4.0/etc/kayobe/inventory/group_vars/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/etc/kayobe/inventory/group_vars/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/inventory/group_vars/compute/network-interfaces
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/etc/kayobe/inventory/group_vars/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/inventory/group_vars/controllers/network-interfaces
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/etc/kayobe/inventory/group_vars/overcloud/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/inventory/group_vars/overcloud/ansible-python-interpreter
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/etc/kayobe/inventory/group_vars/seed/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/inventory/group_vars/seed/ansible-python-interpreter
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/inventory/group_vars/seed/network-interfaces
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/etc/kayobe/inventory/group_vars/seed-hypervisor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/inventory/group_vars/seed-hypervisor/ansible-python-interpreter
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/etc/kayobe/inventory/group_vars/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/inventory/group_vars/storage/network-interfaces
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/inventory/groups
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/inventory/hosts.example
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4572 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/ipa.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4338 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/ironic.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/etc/kayobe/kolla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/kolla/globals.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13905 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/kolla.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/monasca.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/monitoring.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6149 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/networks.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2249 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/neutron.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/nova.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/ntp.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/opensm.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/openstack.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/overcloud.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/pip.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3992 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/seed-hypervisor.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/seed-vm.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3482 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/seed.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/ssh.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4255 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/storage.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/swift.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/time.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2022-04-28 10:15:35.000000 kayobe-9.4.0/etc/kayobe/users.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/kayobe/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12153 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/ansible.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/kayobe/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    72626 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/cli/commands.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/kayobe/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/cmd/kayobe.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/cmd/kayobe_vault_password_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8228 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/kolla_ansible.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/kayobe/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/kayobe/plugins/action/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/plugins/action/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6984 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/plugins/action/kolla_ansible_host_vars.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/kayobe/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/kayobe/tests/molecule/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/molecule/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2139 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/molecule/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/kayobe/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/kayobe/tests/unit/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/unit/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    78738 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/unit/cli/test_commands.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/kayobe/tests/unit/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/unit/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/kayobe/tests/unit/plugins/action/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/unit/plugins/action/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14895 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/unit/plugins/action/test_kolla_ansible_host_vars.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23916 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/unit/test_ansible.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12831 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/unit/test_kolla_ansible.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7275 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4478 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/tests/unit/test_vault.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7613 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4950 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/vault.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2022-04-28 10:15:35.000000 kayobe-9.4.0/kayobe/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.409736 kayobe-9.4.0/kayobe.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3834 2022-04-28 10:16:06.000000 kayobe-9.4.0/kayobe.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38517 2022-04-28 10:16:06.000000 kayobe-9.4.0/kayobe.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-04-28 10:16:06.000000 kayobe-9.4.0/kayobe.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8656 2022-04-28 10:16:06.000000 kayobe-9.4.0/kayobe.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-04-28 10:16:06.000000 kayobe-9.4.0/kayobe.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-04-28 10:16:06.000000 kayobe-9.4.0/kayobe.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-04-28 10:16:06.000000 kayobe-9.4.0/kayobe.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2022-04-28 10:16:06.000000 kayobe-9.4.0/kayobe.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/playbooks/kayobe-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-base/post.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2086 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-base/pre.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/playbooks/kayobe-overcloud-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-base/globals.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1613 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-base/overrides.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1706 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-base/pre.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1141 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-base/run.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/playbooks/kayobe-overcloud-host-configure-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3200 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-host-configure-base/overrides.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1371 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-host-configure-base/pre.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1521 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-host-configure-base/run.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/playbooks/kayobe-overcloud-host-configure-base/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4936 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-host-configure-base/tests/test_overcloud_host_configure.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/playbooks/kayobe-overcloud-upgrade-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-upgrade-base/globals.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-upgrade-base/overrides.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-upgrade-base/pre.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4049 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-overcloud-upgrade-base/run.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/playbooks/kayobe-seed-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-base/bifrost-overrides.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-base/globals.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-base/overrides.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-base/pre.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-base/run.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/playbooks/kayobe-seed-upgrade-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-upgrade-base/bifrost-overrides.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-upgrade-base/globals.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-upgrade-base/overrides.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-upgrade-base/pre.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-upgrade-base/run.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/playbooks/kayobe-seed-vm-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-vm-base/overrides.yml.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2236 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-vm-base/pre.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-vm-base/run.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-seed-vm-base/seed-group-vars.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.413736 kayobe-9.4.0/playbooks/kayobe-tox-molecule/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2022-04-28 10:15:35.000000 kayobe-9.4.0/playbooks/kayobe-tox-molecule/pre.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.353728 kayobe-9.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.433739 kayobe-9.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-admin-network.yml-cf4b5e6387d0eb3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-command-hooks-827aa0732b7399de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-custom-config-for-elasticsearch-a762134e51b50f91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-ironic-node-serial-console-commands-75f1255d62e05c87.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-kolla_ansible_venv_extra_requirements-4d4f70b024207ffb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-monasca-3e6da709b3b4c269.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-monasca-defaults-8486abe37ed3a13b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-serial-console-enable-to-post-configure-c61704185c57783d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-stop-command-8f66235870720f31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-storm-5d29163b61ef01ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-barbican-conf-c15f0ab4294281cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-configuring-mariadb-646badcc9dd07019.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-custom-aodh-conf-81a5a623f771d1c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-custom-blazar-conf-c82ee78f2a92d693.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-custom-ceilometer-conf-66d907cf3c7ec29b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-custom-cloudkitty-conf-af224caad9cd1ad4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-custom-gnocchi-conf-51b110196f966c32.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-custom-group-vars-3760547c3505487d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-custom-masakari-conf-af224cead3cd1ad4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-global-conf-411316a7250611b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-support-for-haproxy-config-b7b8f331e8adb2e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add-variable-docker-registry-datadir-volume-a5ec931a5eb2c59d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add_support_for_custom_barbican_conf-b94272d73d53aa87.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/add_support_for_custom_keepalived_conf-b26a242761c1f5b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ansible-2.5-2.7-c06a682f4f07755d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ansible-2.5-785e3c764f450d09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ansible-2.6-2.8-ce141db0edb87e1c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ansible-2.8-2.9-2df006b066704417.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      562 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ansible-facts-2b3389a2534d47a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/arista-switch-aedc46148506c56e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ask-vault-pass-b6ced0220384dde1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/avoid-unconditional-fact-gathering-4dfbf96e2111ad51.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bifrost-dib-extra-c4eac903986ec700.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bifrost-firewalld-zone-09a29651a058531a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bifrost-inspection-gateway-316ab384430ef8df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bifrost-ironic-extra-kernel-params-e3e56a9dcdf24bb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bifrost-use-firewalld-90b69e2ac6eead67.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bifrost-victoria-fixes-eed49b088afdac5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/blacklist-ansible-2.9.8-f83ad748b01a575b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bootproto-52316b6dbc30e98c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bootstrap-openrc-9aec3d53d0d62c81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bootstrap-servers-user-8cb5114de1dd10ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bugfix-dnf-proxy-cd934867c3d64388.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bugfix-monasca-grafana-dashboard-config-b81781cf10c2a236.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/bugfix-update-idrac-role-71ede6900dc000a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/build-centos8s-images-509f04d8d68cb357.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/build-neutron-sriov-836acf378bae0b48.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/cacert-514b8645d6912bf9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/centos-8-12073e91a157d0a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/centos-8-chrony-bec9d7bc8b346363.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/centos-8.3-89d07c8f8db5b17b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/centos-ipa-images-60dde12f2b4f4f8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/concurrent-known-hosts-update-8dc94557e9a48021.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/config-galaxy-roles-6bd129824436a983.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/config-idemoptence-37846db82ecd9f43.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/configdrive-vlans-4e8b6ed07b229233.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/cumulus-switch-baf554118ef23afe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/custom-ansible-config-d0f1bcdf2607e521.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/custom-certificates-5f2c1fff6503b77a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/custom-route-options-2ed446961262a34a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/db-backup-recovery-d4f1ced2ebd7dac4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/default-disable-ironic-2c20b8a7e69f19c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/default-lvm-data-vg-f2848066975beeda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/default-overlay2-970bdb5b7b62b60a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/default-target-virtualenv-3a68472f66b7aaf3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/defroute-9bbcff8b2f8abc94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/dell-powerconnect-switch-860fbcbf7e4323ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/deploy_containers-4199127a91f29be0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/disable-bifrost-cleaning-ff10995a0bf11079.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/disable-chrony-5f1e4f9db509c42d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/disable-ironic-networks-86ba35f58f317ab6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/dnf-2071fc40b0d783b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/dnf-proxy-22a6eb457c06a223.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/docker-custom-config-5103260d5ddb7223.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/docker-registry-basic-auth-b94b4a66e1ce9095.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/docker-registry-env-e954a0642555864f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/docker-registry-on-seed-2eb4fb643d6fda9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/docker-registry-tls-a823fc5717ef2b52.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/docker-storage-driver-7d560e7d350b14ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/drop-kolla-ceph-deployment-47095b032085e8f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/drop-py-2-7-3d0a7f3eb8f11d6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ethtool-options-e90ace0555e3fba3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/external-api-no-ip-f04951ffc9659949.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/extra-kernel-options-strings-bec7d851e334fec5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/feature-automatic-node-rename-fc5fbe0f7c38151c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/feature-update-ironic-driver-info-02371a593ca0f734.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/filter-out-ruckus-lldp-port-description-ad2b0774609aedbf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/first-official-release-6dff5747d34d161c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-baremetal-compute-commands-b72862a53f88c5ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-baremetal-serial-autoenable-0ccfec017cf2ddbc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-bifrost-ironic-extra-kernel-params-9ebdec1212ac9827.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-coreutils-single-conflict-208036c66b9f7e59.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-data-files-path-detection-on-ubuntu-dfa8e4e7a1d3ea27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-default-docker-storage-driver-e05832be7a4c2ab8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-default-public-net-name-067338275460b50d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-dell-physical-network-config-b4eaf752e62eeadb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-disable-selinux-not-installed-eff17c715efc1fdb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-image-build-regex-964c8c6359841662.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-inspection-when-using-ipxe-9bf6ed9e6456840b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-inspector-ipxe-uefi-86f435ebaf4eee08.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-inspector-rule-idempotency-f6e5a61f7dca580f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-introspection-data-save-51001baa37d97084.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-introspection-data-save-cfc83714f66fd63c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-ipa-build-b31fb20ddcbe3ece.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-ipa-image-download-3f90f0f40d0feafd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-kolla-ansible-group-mapping-8fcd6cbb1e744e18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-limit-with-commas-04a357b0b7ef0371.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-network-hosts-interfaces-f0206aa91b218a25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-no-ip-addr-on-nic-38d6f8e8078f534d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-overcloud-database-backup-with-no-kolla-config-4f857915adabad41.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-persistent-sysctls-1aef170599a49608.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-post-config-public-eb72f3a692a2be6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-python-setup-5e7ff929a6cab092.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-remote-seed-vm-provisioning-faa8de569ca6bc89.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-seed-multiple-networks-458915b085a9478c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-seed-vm-provision-c432ebfae8bfee8b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fix-selinux-disable-reboot-65c32f5dc895211c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fixes-keyerror-vlan-link-c177cf719e070df6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/fluentd-custom-inputs-1b911bd229e8a9e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/hardware-inspection-timeouts-777f3bb569929f0f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/host-package-update-c5bddba791754646.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/host-run-command-eb98cb077d546551.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ignore-unconfigured-nets-93beaf96f43af1ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/improve-ssh-known-host-error-15fbc6ae4fa3dbd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/initial-f71c8e25375afa25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/inspector-25gbe-port-9bdc3bb354e3dfb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/inspector-dhcp-range-netmask-bb46eb7df77587a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/install-prefix-multiple-lib-9288e8c11da3c0bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/internal-api-tls-4e7383e6a0262f5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ipa-branch-b29c377c531013a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ipa-build-dib-packages-5e85baba3294eb65.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ipa-build-upper-constraints-5686abaa161b0d94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1345 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ipa-builder-ea6308b6691ae71e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/kolla-ansible-become-false-95aa88edd3c8c259.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/kolla-docker-registry-e1adce280fc17db7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/kolla-enable-openstack-core-ce4866dd388f262e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/kolla-external-fqdn-cacert-048aa1299050cfd7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/kolla-inventory-host-vars-7f9dc14c82e3ea20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/kolla-tag-and-suffix-a223b0c7173a245e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/kolla-user-group-85bbe8038c3f719c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/luks-ed1d301ad0168e91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/manage-lvm-0.1.4-d33b398060232874.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/mariabackup-9370d55279c1aa78.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/mdadm-ed1d301ad0168e91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/mellanox-switch-cb82a8c278f5e652.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/neutron-mlnx-agent-19631a3936da47df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/non-shared-ironic-nets-06a43c9b6dea2a77.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/openrc-upgrade-9e14888d600f6839.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/openstack-branch-87df0c2f647037c0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/optional-epel-release-92eaf3dc4aa1021b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/package-runtime-files-in-python-package-c3dda2bd32844fdf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/passwords-in-tmp-18e55d5e9b894b4d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/patch-links-on-overcloud-e24dbc858d3399cc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/per-host-interfaces-6e548331fa3a4244.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/physical-network-disable-discovery-15916760e0a4d0bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/pip-index-url-conditional-3f9c5b3c5c808500.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/pip-local-mirror-d9a80257c8441970.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/pip_proxy-6c6022b6566dae69.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/plug-ovs-phy-f180d9bb9dd25dab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/prevent-resolv.conf-4a09d50f60f3fe28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/prevent-wrong-oscacert-variable-9ede7f60c1562a77.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/public-os-endpoint-type-a678a8ddc51ce3b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/quote-escape-vars-3d42c7de8dc39d15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/quote-kolla-limit-042422e69c008109.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-congress-support-0f6a327de69e2173.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-ifcfg-eth0-c179ea98fc34e164.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-inspector-manage-firewall-b1117b04a0f6904d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-ironic-drivers-939a9c6afad33e2a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-libvirt-pool-capacity-e428b893ca5bdb88.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-mongodb-fcdfba997e1abb51.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-neutron-fwaas-0g6a327ae69e2117.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-opendaylight-ac316f8ada083cc9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-overcloud-cadvisor-deployment-3866f823cd1dc0b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-overcloud-cloud-init-workaround-4f4643f15c20b2e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-overcloud-prometheus-deployment-75792bba2fc39385.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-resolv-conf-workaround-4cb484d3a66c4e58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-stop-chrony-1944c6cba72730c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-storage-mgmt-net-from-controllers-8f9c1d252d9f318b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/remove-yum-variables-0a1ab4e958c27171.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/restrict-ip-allocation-8e20022110c2283e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/rocky-355875d3f38b0d02.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/save-include-exclude-df8cca17da0aa3de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/seed-hypervisor-bootstrap-58bafc1ea0d125bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/seed-hypervisor-host-package-update-2ad745a2d9fec134.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/seed-hypervisor-host-package-update-fix-9411205aadc92b8f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/seed-hypervisor-lvm-80864721ff42f6a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/seed-service-upgrade-71b847e3658a1948.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/seed-vm-centos-8.2-36b7a480a7725da1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/seed-vm-centos-8.3-7726c9d0603508eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/seperate-storage-networks-a659bcd30dd70665.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/setup-module-args-2c36e56bf78ab5f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/specify-requirements-branch-for-ipa-build-c3ca977ec21b58f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ssh-batchmode-cda7a4ed63006378.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/stale-virtualenvs-125c513af3de9396.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/story-2007297-73f498ef6bc89fe9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/story-2008354-0c34e2ad7aeb7d3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/story-2008430-6a50101d05219aad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/support-deploy-containers-7acf4c647fb5c3fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/support_configuring_tunnel_network-1646eef887d72abf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/support_ironic_neutron_agent-a41e44ef41f5a96d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/swift-improvements-07a2b75967f642e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/tftp-listen-on-internal-interface-09aeec7ad99fc13d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/timezone-config-298cff76834f5fb4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/use-public-fqdn-in-openrc-f7990958ceec817d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/ussuri-prelude-25dc5d922eff1104.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/workaround-bifrost-ipa-kernel-rename-59bf75ac8285f103.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/workaround-cloud-init-vlan-0efa97b866d46783.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/yum-config-58274185a00004e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/notes/yum-repository-metalink-26afa7c9f7026539.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8144 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5142 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6307 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-04-28 10:15:35.000000 kayobe-9.4.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-04-28 10:15:35.000000 kayobe-9.4.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2022-04-28 10:15:35.000000 kayobe-9.4.0/requirements.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/roles/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-04-28 10:15:35.000000 kayobe-9.4.0/roles/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.353728 kayobe-9.4.0/roles/kayobe-ci-prep/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/roles/kayobe-ci-prep/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2022-04-28 10:15:35.000000 kayobe-9.4.0/roles/kayobe-ci-prep/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/roles/kayobe-diagnostics/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-04-28 10:15:35.000000 kayobe-9.4.0/roles/kayobe-diagnostics/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/roles/kayobe-diagnostics/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2022-04-28 10:15:35.000000 kayobe-9.4.0/roles/kayobe-diagnostics/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/roles/kayobe-diagnostics/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4832 2022-04-28 10:15:35.000000 kayobe-9.4.0/roles/kayobe-diagnostics/files/get_logs.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/roles/kayobe-diagnostics/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-04-28 10:15:35.000000 kayobe-9.4.0/roles/kayobe-diagnostics/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2022-04-28 10:15:35.000000 kayobe-9.4.0/roles/kayobe-diagnostics/tasks/post.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2022-04-28 10:15:35.000000 kayobe-9.4.0/roles/kayobe-diagnostics/tasks/pre.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9854 2022-04-28 10:16:06.441740 kayobe-9.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2022-04-28 10:15:35.000000 kayobe-9.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-04-28 10:15:35.000000 kayobe-9.4.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      367 2022-04-28 10:15:35.000000 kayobe-9.4.0/tools/ansible-galaxy-retried.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      404 2022-04-28 10:15:35.000000 kayobe-9.4.0/tools/feature-flags.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      624 2022-04-28 10:15:35.000000 kayobe-9.4.0/tools/loc
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1895 2022-04-28 10:15:35.000000 kayobe-9.4.0/tools/release.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      363 2022-04-28 10:15:35.000000 kayobe-9.4.0/tools/run-bashate.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1154 2022-04-28 10:15:35.000000 kayobe-9.4.0/tools/sphinx8
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      703 2022-04-28 10:15:35.000000 kayobe-9.4.0/tools/test-ansible.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      696 2022-04-28 10:15:35.000000 kayobe-9.4.0/tools/test-molecule.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4260 2022-04-28 10:15:35.000000 kayobe-9.4.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-04-28 10:16:06.437739 kayobe-9.4.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6203 2022-04-28 10:15:35.000000 kayobe-9.4.0/zuul.d/jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2022-04-28 10:15:35.000000 kayobe-9.4.0/zuul.d/nodesets.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2022-04-28 10:15:35.000000 kayobe-9.4.0/zuul.d/project.yaml
```

### Comparing `kayobe-9.3.0/AUTHORS` & `kayobe-9.4.0/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 Radoslaw Smigielski <radoslaw.smigielski@nokia.com>
 Radosław Piliszek <radoslaw.piliszek@gmail.com>
 Raimund Hook <openstack@sting-ray.za.net>
 Ross Martyn <ross.martyn@gresearch.co.uk>
 Ross Martyn <rossmartyn04@gmail.com>
 Scott Solkhon <scott.solkhon@gresearch.co.uk>
 Scott Solkhon <scottsolkhon@gmail.com>
+Sorin Sbarnea <ssbarnea@redhat.com>
 Stig Telfer <stig.github@telfer.org>
 Stig Telfer <stig.openstack@telfer.org>
 Stig Telfer <stig@stackhpc.com>
 Vieri <15050873171@163.com>
 Will Miller <willm@stackhpc.com>
 Will Szumski <will@stackhpc.com>
 chenxing <chason.chan@foxmail.com>
```

### Comparing `kayobe-9.3.0/CONTRIBUTING.rst` & `kayobe-9.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ChangeLog` & `kayobe-9.4.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,37 @@
 CHANGES
 =======
 
+9.4.0
+-----
+
+* docs: Fix custom LVM example
+* Fix variable name for stackhpc.os-networks upper constraints
+* Restore forgotten linuxbridge-agent container
+* Fix Ansible inventory generation when reusing group names
+* CI: Avoid image downloads and builds in seed jobs
+* Fix custom config idempotence
+* Only create patch links on overcloud hosts
+* Use naming convention to infer VLAN tagging
+* Build CentOS stream images
+* CI: stop using zuul as kayobe\_ansible\_user in TLS jobs
+* Set correct gateway for the bifrost provision network
+* Set requirements branch for IPA build
+* Revert "CI: temporary disable voting of some jobs"
+* Use stream8 images with molecule
+* CentOS Stream: update DNF repo file names
+* CI: temporary disable voting of some jobs
+
 9.3.0
 -----
 
 * Pin rich to <11 due to breaking ansible-lint in kayobe-tox-molecule
+* ipa: Use openstack\_branch instead of master
+* Fix seed VM configdrive when admin network is a VLAN
+* Generate kolla config when running database commands
 * Build neutron-sriov-agent image when enabled
 * [CI] Stop testing non-stream CentOS
 
 9.2.0
 -----
 
 * docs: Improve all-in-one scenario
```

### Comparing `kayobe-9.3.0/LICENSE` & `kayobe-9.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/PKG-INFO` & `kayobe-9.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kayobe
-Version: 9.3.0
+Version: 9.4.0
 Summary: Deployment of OpenStack to bare metal using OpenStack kolla and bifrost
 Home-page: https://docs.openstack.org/kayobe/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: Kayobe
         ======
```

### Comparing `kayobe-9.3.0/README.rst` & `kayobe-9.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/Vagrantfile` & `kayobe-9.4.0/Vagrantfile`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/action_plugins/kolla_ansible_host_vars.py` & `kayobe-9.4.0/ansible/action_plugins/kolla_ansible_host_vars.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/baremetal-compute-inspect.yml` & `kayobe-9.4.0/ansible/baremetal-compute-inspect.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/baremetal-compute-manage.yml` & `kayobe-9.4.0/ansible/baremetal-compute-manage.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/baremetal-compute-provide.yml` & `kayobe-9.4.0/ansible/baremetal-compute-provide.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/baremetal-compute-rename.yml` & `kayobe-9.4.0/ansible/baremetal-compute-rename.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/baremetal-compute-serial-console.yml` & `kayobe-9.4.0/ansible/baremetal-compute-serial-console.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/compute-node-discovery.yml` & `kayobe-9.4.0/ansible/compute-node-discovery.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/compute-node-provide.yml` & `kayobe-9.4.0/ansible/compute-node-provide.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/container-image-build.yml` & `kayobe-9.4.0/ansible/container-image-build.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/dell-compute-node-discovery.yml` & `kayobe-9.4.0/ansible/dell-compute-node-discovery.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/dell-compute-node-inventory.yml` & `kayobe-9.4.0/ansible/dell-compute-node-inventory.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/dell-switch-bmp.yml` & `kayobe-9.4.0/ansible/dell-switch-bmp.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/docker-devicemapper.yml` & `kayobe-9.4.0/ansible/docker-devicemapper.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/drac-bios.yml` & `kayobe-9.4.0/ansible/drac-bios.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/drac-boot-order.yml` & `kayobe-9.4.0/ansible/drac-boot-order.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/drac-facts.yml` & `kayobe-9.4.0/ansible/drac-facts.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/dump-config.yml` & `kayobe-9.4.0/ansible/dump-config.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/external-net.yml` & `kayobe-9.4.0/ansible/external-net.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/filter_plugins/bmc_type.py` & `kayobe-9.4.0/ansible/filter_plugins/bmc_type.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/filter_plugins/networks.py` & `kayobe-9.4.0/ansible/filter_plugins/networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,22 +428,30 @@
             (name, inventory_hostname))
     ip = net_ip(context, name, inventory_hostname)
     cidr = net_cidr(context, name, inventory_hostname)
     netmask = net_mask(context, name, inventory_hostname)
     gateway = net_gateway(context, name, inventory_hostname)
     bootproto = net_bootproto(context, name, inventory_hostname)
     mtu = net_mtu(context, name, inventory_hostname)
+    vlan = net_vlan(context, name, inventory_hostname)
+    if vlan and '.' in device:
+        backend = [device.split('.')[0]]
+    else:
+        backend = None
     interface = {
         'device': device,
         'address': ip,
         'netmask': netmask,
         'gateway': gateway,
         'bootproto': bootproto or 'static',
         'mtu': mtu,
+        'backend': backend,
     }
+    if backend:
+        interface['type'] = 'vlan'
     interface = {k: v for k, v in interface.items() if v is not None}
     return interface
 
 
 @jinja2.contextfilter
 def net_libvirt_network(context, name, inventory_hostname=None):
     """Return a dict which describes the Libvirt network for a network.
```

### Comparing `kayobe-9.3.0/ansible/filter_plugins/switches.py` & `kayobe-9.4.0/ansible/filter_plugins/switches.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/bifrost` & `kayobe-9.4.0/ansible/group_vars/all/bifrost`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ###############################################################################
 # Diskimage-builder configuration.
 
 # DIB base OS element.
 kolla_bifrost_dib_os_element: "centos"
 
 # DIB image OS release.
-kolla_bifrost_dib_os_release: "8"
+kolla_bifrost_dib_os_release: "8-stream"
 
 # List of default DIB elements.
 kolla_bifrost_dib_elements_default:
   - "disable-selinux"
   - "enable-serial-console"
   - "vm"
```

### Comparing `kayobe-9.3.0/ansible/group_vars/all/compute` & `kayobe-9.4.0/ansible/group_vars/all/compute`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/controllers` & `kayobe-9.4.0/ansible/group_vars/all/controllers`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/dnf` & `kayobe-9.4.0/ansible/group_vars/all/dnf`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/docker` & `kayobe-9.4.0/ansible/group_vars/all/docker`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/docker-registry` & `kayobe-9.4.0/ansible/group_vars/all/docker-registry`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/globals` & `kayobe-9.4.0/ansible/group_vars/all/globals`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/grafana` & `kayobe-9.4.0/ansible/group_vars/all/grafana`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/idrac` & `kayobe-9.4.0/ansible/group_vars/all/idrac`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/inspector` & `kayobe-9.4.0/ansible/group_vars/all/inspector`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/ipa` & `kayobe-9.4.0/ansible/group_vars/all/ipa`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 # Version of IPA source repository. Default is {{ openstack_branch }}.
 ipa_build_source_version: "{{ openstack_branch }}"
 
 # URL of IPA builder source repository.
 ipa_builder_source_url: "https://opendev.org/openstack/ironic-python-agent-builder"
 
-# Version of IPA builder source repository. Default is master.
-ipa_builder_source_version: master
+# Version of IPA builder source repository. Default is stable/wallaby.
+ipa_builder_source_version: "stable/wallaby"
 
 # List of default Diskimage Builder (DIB) elements to use when building IPA
 # images. Default is ["centos", "enable-serial-console",
 # "ironic-python-agent-ramdisk"].
 ipa_build_dib_elements_default:
   - centos
   - enable-serial-console
@@ -37,16 +37,18 @@
 ipa_build_dib_elements: >
   {{ ipa_build_dib_elements_default +
      ipa_build_dib_elements_extra }}
 
 # Dictionary of default environment variables to provide to Diskimage Builder
 # (DIB) during IPA image build.
 ipa_build_dib_env_default:
-  DIB_REPOLOCATION_ironic_agent: "{{ ipa_build_source_url }}"
-  DIB_REPOREF_ironic_agent: "{{ ipa_build_source_version }}"
+  DIB_RELEASE: "8-stream"
+  DIB_REPOLOCATION_ironic_python_agent: "{{ ipa_build_source_url }}"
+  DIB_REPOREF_ironic_python_agent: "{{ ipa_build_source_version }}"
+  DIB_REPOREF_requirements: "{{ openstack_branch }}"
 
 # Dictionary of additional environment variables to provide to Diskimage
 # Builder (DIB) during IPA image build.
 ipa_build_dib_env_extra: {}
 
 # Dictionary of environment variables to provide to Diskimage Builder (DIB)
 # during IPA image build.
@@ -72,16 +74,17 @@
 ipa_build_dib_git_elements: >-
   {{ ipa_build_dib_git_elements_default + ipa_build_dib_git_elements_extra }}
 
 # List of DIB packages to install. Default is none.
 ipa_build_dib_packages: []
 
 # Upper constraints file for installing packages in the virtual environment
-# used for building IPA images. Default is {{ pip_upper_constraints_file }}.
-ipa_build_upper_constraints_file: "{{ pip_upper_constraints_file }}"
+# used for building IPA images. To build CentOS Stream 8 images, default is
+# "https://releases.openstack.org/constraints/upper/wallaby".
+ipa_build_upper_constraints_file: "https://releases.openstack.org/constraints/upper/wallaby"
 
 ###############################################################################
 # Ironic Python Agent (IPA) images configuration.
 
 # Suffix of upstream Ironic deployment image files. Default is based on
 # {{ openstack_branch }}.
 ipa_images_upstream_url_suffix: "-{{ openstack_branch | replace('/', '-') }}"
```

### Comparing `kayobe-9.3.0/ansible/group_vars/all/ironic` & `kayobe-9.4.0/ansible/group_vars/all/ironic`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/kolla` & `kayobe-9.4.0/ansible/group_vars/all/kolla`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
   - regex: ^multipathd
     enabled: "{{ kolla_enable_multipathd | bool }}"
   - regex: ^murano
     enabled: "{{ kolla_enable_murano | bool }}"
   - regex: neutron-server
     enabled: "{{ kolla_enable_neutron | bool }}"
   # Neutron SFC agent not currently supported on CentOS binary builds.
-  - regex: "neutron-\\(dhcp\\|l3\\|metadata\\|openvswitch\\)-agent"
+  - regex: "neutron-\\(dhcp\\|l3\\|metadata\\|linuxbridge\\|openvswitch\\)-agent"
     enabled: "{{ kolla_enable_neutron | bool }}"
   - regex: neutron-mlnx-agent
     enabled: "{{ kolla_enable_neutron_mlnx | bool }}"
   - regex: neutron-sriov-agent
     enabled: "{{ kolla_enable_neutron_sriov | bool }}"
   - regex: ^nova
     enabled: "{{ kolla_enable_nova | bool }}"
```

### Comparing `kayobe-9.3.0/ansible/group_vars/all/monitoring` & `kayobe-9.4.0/ansible/group_vars/all/monitoring`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/network` & `kayobe-9.4.0/ansible/group_vars/all/network`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/neutron` & `kayobe-9.4.0/ansible/group_vars/all/neutron`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/openstack` & `kayobe-9.4.0/ansible/group_vars/all/openstack`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/overcloud` & `kayobe-9.4.0/ansible/group_vars/all/overcloud`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/seed` & `kayobe-9.4.0/ansible/group_vars/all/seed`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/seed-hypervisor` & `kayobe-9.4.0/ansible/group_vars/all/seed-hypervisor`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/seed-vm` & `kayobe-9.4.0/ansible/group_vars/all/seed-vm`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/ssh` & `kayobe-9.4.0/ansible/group_vars/all/ssh`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/storage` & `kayobe-9.4.0/ansible/group_vars/all/storage`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/swift` & `kayobe-9.4.0/ansible/group_vars/all/swift`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/switches/arista` & `kayobe-9.4.0/ansible/group_vars/all/switches/arista`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/switches/config` & `kayobe-9.4.0/ansible/group_vars/all/switches/config`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/group_vars/all/switches/junos` & `kayobe-9.4.0/ansible/group_vars/all/switches/junos`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/host-package-update.yml` & `kayobe-9.4.0/ansible/host-package-update.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/idrac-bootstrap-one.yml` & `kayobe-9.4.0/ansible/idrac-bootstrap-one.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/idrac-bootstrap.yml` & `kayobe-9.4.0/ansible/idrac-bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/inspection-store.yml` & `kayobe-9.4.0/ansible/inspection-store.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/ip-allocation.yml` & `kayobe-9.4.0/ansible/ip-allocation.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/kayobe-ansible-user.yml` & `kayobe-9.4.0/ansible/kayobe-ansible-user.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/kayobe-target-venv.yml` & `kayobe-9.4.0/ansible/kayobe-target-venv.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/kolla-ansible-user.yml` & `kayobe-9.4.0/ansible/kolla-ansible-user.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/kolla-ansible.yml` & `kayobe-9.4.0/ansible/kolla-ansible.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/kolla-bifrost-hostvars.yml` & `kayobe-9.4.0/ansible/kolla-bifrost-hostvars.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/kolla-bifrost.yml` & `kayobe-9.4.0/ansible/kolla-bifrost.yml`

 * *Files 4% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 
   roles:
     - role: kolla-bifrost
 
       # Network configuration.
       kolla_bifrost_dhcp_pool_start: "{{ provision_oc_net_name | net_inspection_allocation_pool_start }}"
       kolla_bifrost_dhcp_pool_end: "{{ provision_oc_net_name | net_inspection_allocation_pool_end }}"
-      kolla_bifrost_dnsmasq_router: "{{ provision_oc_net_name | net_gateway }}"
+      kolla_bifrost_dnsmasq_router: "{{ provision_oc_net_name | net_inspection_gateway or provision_oc_net_name | net_gateway }}"
       kolla_bifrost_dnsmasq_dns_servers: "{{ resolv_nameservers | default([]) }}"
       kolla_bifrost_domain: "{{ resolv_domain | default }}"
       kolla_bifrost_download_ipa: "{{ not ipa_build_images | bool }}"
```

### Comparing `kayobe-9.3.0/ansible/kolla-host.yml` & `kayobe-9.4.0/ansible/kolla-host.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/kolla-openstack.yml` & `kayobe-9.4.0/ansible/kolla-openstack.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/kolla-pip.yml` & `kayobe-9.4.0/ansible/kolla-pip.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/kolla-target-venv.yml` & `kayobe-9.4.0/ansible/kolla-target-venv.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/lvm.yml` & `kayobe-9.4.0/ansible/lvm.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/network-connectivity.yml` & `kayobe-9.4.0/ansible/network-connectivity.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/network.yml` & `kayobe-9.4.0/ansible/network.yml`

 * *Files 2% similar despite different names*

```diff
@@ -113,7 +113,8 @@
                'peer_device': network_patch_prefix ~ item.key ~ network_patch_suffix_ovs,
                'peer_bootproto': 'static',
                'peer_mtu': item.value,
                'onboot': 'yes'}] }}
       with_dict: "{{ veth_mtu_map }}"
   roles:
     - role: veth
+      when: "'overcloud' in group_names"
```

### Comparing `kayobe-9.3.0/ansible/overcloud-bios-raid.yml` & `kayobe-9.4.0/ansible/overcloud-bios-raid.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-deprovision.yml` & `kayobe-9.4.0/ansible/overcloud-deprovision.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-docker-sdk-upgrade.yml` & `kayobe-9.4.0/ansible/overcloud-docker-sdk-upgrade.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-etc-hosts-fixup.yml` & `kayobe-9.4.0/ansible/overcloud-etc-hosts-fixup.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-grafana-configure.yml` & `kayobe-9.4.0/ansible/overcloud-grafana-configure.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-hardware-inspect.yml` & `kayobe-9.4.0/ansible/overcloud-hardware-inspect.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-introspection-data-save.yml` & `kayobe-9.4.0/ansible/overcloud-introspection-data-save.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-introspection-rules-dell-lldp-workaround.yml` & `kayobe-9.4.0/ansible/overcloud-introspection-rules-dell-lldp-workaround.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-introspection-rules.yml` & `kayobe-9.4.0/ansible/overcloud-introspection-rules.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-inventory-discover.yml` & `kayobe-9.4.0/ansible/overcloud-inventory-discover.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-ipa-build.yml` & `kayobe-9.4.0/ansible/overcloud-ipa-build.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-ipa-images.yml` & `kayobe-9.4.0/ansible/overcloud-ipa-images.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-provision.yml` & `kayobe-9.4.0/ansible/overcloud-provision.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/overcloud-service-config-save.yml` & `kayobe-9.4.0/ansible/overcloud-service-config-save.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/physical-network.yml` & `kayobe-9.4.0/ansible/physical-network.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/provision-net.yml` & `kayobe-9.4.0/ansible/provision-net.yml`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
       tags:
         - config-validation
 
   roles:
     - role: stackhpc.os-networks
       os_openstacksdk_install_epel: "{{ dnf_install_epel }}"
       os_openstacksdk_state: latest
-      os_openstacksdk_upper_constraints_file: "{{ pip_upper_constraints_file }}"
+      os_networks_upper_constraints_file: "{{ pip_upper_constraints_file }}"
       os_networks_venv: "{{ venv }}"
       os_networks_auth_type: "{{ openstack_auth_type }}"
       os_networks_auth: "{{ openstack_auth }}"
       os_networks_cacert: "{{ openstack_cacert | default(omit, true) }}"
       os_networks_interface: "{{ openstack_interface | default(omit, true) }}"
       # Network configuration.
       os_networks: "{{ network_registrations }}"
```

### Comparing `kayobe-9.3.0/ansible/public-openrc.yml` & `kayobe-9.4.0/ansible/public-openrc.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/arista-switch/README.md` & `kayobe-9.4.0/ansible/roles/arista-switch/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/bootstrap/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/bootstrap/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/console-allocation/library/console_allocation.py` & `kayobe-9.4.0/ansible/roles/console-allocation/library/console_allocation.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/console-allocation/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/console-allocation/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dell-switch/README.md` & `kayobe-9.4.0/ansible/roles/dell-switch/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dell-switch/templates/dellos9-config.j2` & `kayobe-9.4.0/ansible/roles/dell-switch/templates/dellos9-config.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dell-switch-bmp/README.md` & `kayobe-9.4.0/ansible/roles/dell-switch-bmp/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dell-switch-bmp/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/dell-switch-bmp/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dell-switch-bmp/handlers/main.yml` & `kayobe-9.4.0/ansible/roles/dell-switch-bmp/handlers/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dell-switch-bmp/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/dell-switch-bmp/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/deploy-containers/tasks/deploy.yml` & `kayobe-9.4.0/ansible/roles/deploy-containers/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/disable-glean/README.md` & `kayobe-9.4.0/ansible/roles/disable-glean/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/disable-glean/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/disable-glean/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/disable-selinux/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/disable-selinux/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dnf/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/dnf/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dnf/tasks/custom-repo.yml` & `kayobe-9.4.0/ansible/roles/dnf/tasks/custom-repo.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dnf/tasks/local-mirror.yml` & `kayobe-9.4.0/ansible/roles/dnf/tasks/local-mirror.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 ---
+- name: Slurp /etc/centos-release
+  slurp:
+    src: /etc/centos-release
+  register: centos_release
+
 - name: Copy CentOS repo templates
   template:
     src: "{{ item }}.j2"
     dest: /etc/yum.repos.d/{{ item }}
     owner: root
     group: root
     mode: 0664
   become: True
   loop:
-    - CentOS-Linux-AppStream.repo
-    - CentOS-Linux-BaseOS.repo
-    - CentOS-Linux-Extras.repo
+    - "CentOS-{{ linux_or_stream }}-AppStream.repo"
+    - "CentOS-{{ linux_or_stream }}-BaseOS.repo"
+    - "CentOS-{{ linux_or_stream }}-Extras.repo"
+  vars:
+    linux_or_stream: "{{ 'Stream' if 'Stream' in centos_release['content'] | b64decode else 'Linux' }}"
 
 - name: Remove old (pre CentOS 8.3) repo files
   file:
     path: /etc/yum.repos.d/{{ item }}
     state: absent
   become: True
   loop:
```

### Comparing `kayobe-9.3.0/ansible/roles/dnf/templates/CentOS-Linux-AppStream.repo.j2` & `kayobe-9.4.0/ansible/roles/dnf/templates/CentOS-Linux-AppStream.repo.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dnf/templates/CentOS-Linux-BaseOS.repo.j2` & `kayobe-9.4.0/ansible/roles/dnf/templates/CentOS-Linux-BaseOS.repo.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dnf/templates/CentOS-Linux-Extras.repo.j2` & `kayobe-9.4.0/ansible/roles/dnf/templates/CentOS-Linux-Extras.repo.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dnf/templates/epel-modular.repo.j2` & `kayobe-9.4.0/ansible/roles/dnf/templates/epel-modular.repo.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dnf/templates/epel.repo.j2` & `kayobe-9.4.0/ansible/roles/dnf/templates/epel.repo.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/dnf-automatic/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/dnf-automatic/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/docker/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/docker/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/docker-devicemapper/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/docker-devicemapper/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/docker-devicemapper/handlers/main.yml` & `kayobe-9.4.0/ansible/roles/docker-devicemapper/handlers/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/docker-devicemapper/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/docker-devicemapper/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/docker-registry/README.md` & `kayobe-9.4.0/ansible/roles/docker-registry/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/docker-registry/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/docker-registry/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/docker-registry/tasks/config.yml` & `kayobe-9.4.0/ansible/roles/docker-registry/tasks/config.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/docker-registry/tasks/deploy.yml` & `kayobe-9.4.0/ansible/roles/docker-registry/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/docker-registry/tasks/destroy.yml` & `kayobe-9.4.0/ansible/roles/docker-registry/tasks/destroy.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/docker-registry/tasks/reconfigure.yml` & `kayobe-9.4.0/ansible/roles/docker-registry/tasks/reconfigure.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/drac-boot-mode/README.md` & `kayobe-9.4.0/ansible/roles/drac-boot-mode/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/drac-boot-mode/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/drac-boot-mode/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/drac-pxe/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/drac-pxe/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/drac-pxe/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/drac-pxe/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/image-download/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/image-download/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/inspection-store/README.md` & `kayobe-9.4.0/ansible/roles/inspection-store/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/inspection-store/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/inspection-store/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/inspection-store/handlers/main.yml` & `kayobe-9.4.0/ansible/roles/inspection-store/handlers/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/inspection-store/tasks/config.yml` & `kayobe-9.4.0/ansible/roles/inspection-store/tasks/config.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/inspection-store/tasks/destroy.yml` & `kayobe-9.4.0/ansible/roles/inspection-store/tasks/destroy.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/inspection-store/tasks/start.yml` & `kayobe-9.4.0/ansible/roles/inspection-store/tasks/start.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/inspection-store/templates/nginx.conf` & `kayobe-9.4.0/ansible/roles/inspection-store/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/ip-allocation/library/ip_allocation.py` & `kayobe-9.4.0/ansible/roles/ip-allocation/library/ip_allocation.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/ip-allocation/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/ip-allocation/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/ipa-images/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/ipa-images/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/ipa-images/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/ipa-images/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/ipa-images/tasks/set-driver-info.yml` & `kayobe-9.4.0/ansible/roles/ipa-images/tasks/set-driver-info.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/ironic-inspector-rules/README.md` & `kayobe-9.4.0/ansible/roles/ironic-inspector-rules/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/ironic-inspector-rules/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/ironic-inspector-rules/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/ironic-inspector-rules/library/os_ironic_inspector_rule.py` & `kayobe-9.4.0/ansible/roles/ironic-inspector-rules/library/os_ironic_inspector_rule.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/ironic-inspector-rules/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/ironic-inspector-rules/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/junos-switch/README.md` & `kayobe-9.4.0/ansible/roles/junos-switch/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/junos-switch/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/junos-switch/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/junos-switch/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/junos-switch/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/junos-switch/templates/junos-config-set.j2` & `kayobe-9.4.0/ansible/roles/junos-switch/templates/junos-config-set.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/kolla/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla/tasks/install.yml` & `kayobe-9.4.0/ansible/roles/kolla/tasks/install.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/kolla-ansible/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/library/kolla_passwords.py` & `kayobe-9.4.0/ansible/roles/kolla-ansible/library/kolla_passwords.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/tasks/config.yml` & `kayobe-9.4.0/ansible/roles/kolla-ansible/tasks/config.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/tasks/install.yml` & `kayobe-9.4.0/ansible/roles/kolla-ansible/tasks/install.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/templates/daemon.json.j2` & `kayobe-9.4.0/ansible/roles/kolla-ansible/templates/daemon.json.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/templates/globals.yml.j2` & `kayobe-9.4.0/ansible/roles/kolla-ansible/templates/globals.yml.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/templates/overcloud-components.j2` & `kayobe-9.4.0/ansible/roles/kolla-ansible/templates/overcloud-components.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/templates/overcloud-services.j2` & `kayobe-9.4.0/ansible/roles/kolla-ansible/templates/overcloud-services.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/templates/overcloud-top-level.j2` & `kayobe-9.4.0/ansible/roles/kolla-ansible/templates/overcloud-top-level.j2`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 {% for kolla_group, kolla_group_config in kolla_overcloud_inventory_top_level_group_map.items() %}
 {% if 'groups' in kolla_group_config %}
 {% set renamed_groups = kolla_group_config.groups | difference([kolla_group]) | list %}
 {% if renamed_groups | length > 0 %}
 # Mapping from kolla-ansible group {{ kolla_group }} to top level kayobe
 # groups.
 [{{ kolla_group }}:children]
-{% for group in kolla_group_config.groups %}
+{% for group in renamed_groups %}
 {{ group }}
 {% endfor %}
 
 {% endif %}
 {% endif %}
 {% if 'vars' in kolla_group_config %}
 # Mapping from kolla-ansible group {{ kolla_group }} to top level kayobe
```

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/tests/test-defaults.yml` & `kayobe-9.4.0/ansible/roles/kolla-ansible/tests/test-defaults.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/tests/test-extras.yml` & `kayobe-9.4.0/ansible/roles/kolla-ansible/tests/test-extras.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/tests/test-requirements.yml` & `kayobe-9.4.0/ansible/roles/kolla-ansible/tests/test-requirements.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible/vars/main.yml` & `kayobe-9.4.0/ansible/roles/kolla-ansible/vars/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-ansible-host-vars/tests/test.yml` & `kayobe-9.4.0/ansible/roles/kolla-ansible-host-vars/tests/test.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-bifrost/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/kolla-bifrost/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-bifrost/templates/bifrost.yml.j2` & `kayobe-9.4.0/ansible/roles/kolla-bifrost/templates/bifrost.yml.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-build/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/kolla-build/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-build/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/kolla-build/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-build/templates/kolla-build.conf.j2` & `kayobe-9.4.0/ansible/roles/kolla-build/templates/kolla-build.conf.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/kolla-openstack/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/Dockerfile.j2` & `kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/create.yml` & `kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/create.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/destroy.yml` & `kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/destroy.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/default/tests/test_default.py` & `kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/default/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/Dockerfile.j2` & `kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/create.yml` & `kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/create.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/destroy.yml` & `kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/destroy.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/molecule.yml` & `kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/molecule.yml`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 dependency:
   name: galaxy
 driver:
   name: docker
 lint:
   name: yamllint
 platforms:
-  - name: centos-8
-    image: centos:8
+  - name: centos-stream8
+    image: quay.io/centos/centos:stream8
 provisioner:
   name: ansible
   inventory:
     group_vars:
       all:
         kolla_extra_config_path:
         kolla_enable_aodh: true
```

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/prepare.yml` & `kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/prepare.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/molecule/enable-everything/tests/test_default.py` & `kayobe-9.4.0/ansible/roles/kolla-openstack/molecule/enable-everything/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/tasks/config.yml` & `kayobe-9.4.0/ansible/roles/kolla-openstack/tasks/config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
     patterns: "{{ item.patterns }}"
   with_items: "{{ kolla_openstack_custom_config }}"
   register: find_dest_result
 
 - name: Ensure extra configuration parent directories are present
   file:
     path: "{{ item.0.item.dest }}/{{ item.1.path | relpath(item.0.item.src) | dirname }}"
-    recurse: true
     state: directory
     mode: 0750
   with_subelements:
     - "{{ find_src_result.results }}"
     - files
     - skip_missing: true
   when:
```

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/templates/glance.conf.j2` & `kayobe-9.4.0/ansible/roles/kolla-openstack/templates/glance.conf.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/templates/ironic-inspector.conf.j2` & `kayobe-9.4.0/ansible/roles/kolla-openstack/templates/ironic-inspector.conf.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/templates/ironic.conf.j2` & `kayobe-9.4.0/ansible/roles/kolla-openstack/templates/ironic.conf.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/templates/ml2_conf.ini.j2` & `kayobe-9.4.0/ansible/roles/kolla-openstack/templates/ml2_conf.ini.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/kolla-openstack/vars/main.yml` & `kayobe-9.4.0/ansible/roles/kolla-openstack/vars/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/nclu-switch/README.md` & `kayobe-9.4.0/ansible/roles/nclu-switch/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/opensm/README.md` & `kayobe-9.4.0/ansible/roles/opensm/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/opensm/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/opensm/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/opensm/tasks/deploy.yml` & `kayobe-9.4.0/ansible/roles/opensm/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/opensm/tasks/destroy.yml` & `kayobe-9.4.0/ansible/roles/opensm/tasks/destroy.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/opensm/tasks/reconfigure.yml` & `kayobe-9.4.0/ansible/roles/opensm/tasks/reconfigure.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/pip/tasks/pip_conf.yml` & `kayobe-9.4.0/ansible/roles/pip/tasks/pip_conf.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/public-openrc/templates/public-openrc.sh.j2` & `kayobe-9.4.0/ansible/roles/public-openrc/templates/public-openrc.sh.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/ssh-known-host/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/ssh-known-host/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/swift-block-devices/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/swift-block-devices/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/swift-block-devices/tests/test-bootstrapped.yml` & `kayobe-9.4.0/ansible/roles/swift-block-devices/tests/test-bootstrapped.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/swift-block-devices/tests/test-invalid-format.yml` & `kayobe-9.4.0/ansible/roles/swift-block-devices/tests/test-invalid-format.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/swift-block-devices/tests/test-mount.yml` & `kayobe-9.4.0/ansible/roles/swift-block-devices/tests/test-mount.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/swift-rings/defaults/main.yml` & `kayobe-9.4.0/ansible/roles/swift-rings/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/swift-rings/files/swift-ring-builder.py` & `kayobe-9.4.0/ansible/roles/swift-rings/files/swift-ring-builder.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/swift-rings/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/swift-rings/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/swift-rings/templates/swift-ring.yml.j2` & `kayobe-9.4.0/ansible/roles/swift-rings/templates/swift-ring.yml.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/sysctl/README.md` & `kayobe-9.4.0/ansible/roles/sysctl/README.md`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/veth/files/ifup-veth` & `kayobe-9.4.0/ansible/roles/veth/files/ifup-veth`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/veth/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/veth/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/veth/templates/ifcfg-peer.j2` & `kayobe-9.4.0/ansible/roles/veth/templates/ifcfg-peer.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/veth/templates/ifcfg-veth.j2` & `kayobe-9.4.0/ansible/roles/veth/templates/ifcfg-veth.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/roles/wipe-disks/tasks/main.yml` & `kayobe-9.4.0/ansible/roles/wipe-disks/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/seed-introspection-rules.yml` & `kayobe-9.4.0/ansible/seed-introspection-rules.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/seed-ipa-build.yml` & `kayobe-9.4.0/ansible/seed-ipa-build.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/seed-service-upgrade-prep.yml` & `kayobe-9.4.0/ansible/seed-service-upgrade-prep.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/seed-vm-deprovision.yml` & `kayobe-9.4.0/ansible/seed-vm-deprovision.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/seed-vm-provision.yml` & `kayobe-9.4.0/ansible/seed-vm-provision.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/swift-rings.yml` & `kayobe-9.4.0/ansible/swift-rings.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/test_plugins/functional.py` & `kayobe-9.4.0/ansible/test_plugins/functional.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/ansible/wipe-disks.yml` & `kayobe-9.4.0/ansible/wipe-disks.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/dev/config.sh` & `kayobe-9.4.0/dev/config.sh`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/dev/dev-vagrant.yml` & `kayobe-9.4.0/dev/dev-vagrant.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/dev/environment-setup.sh` & `kayobe-9.4.0/dev/environment-setup.sh`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/dev/functions` & `kayobe-9.4.0/dev/functions`

 * *Files 2% similar despite different names*

```diff
@@ -357,14 +357,25 @@
     # required since https://review.openstack.org/#/c/584427 was merged.
     echo "Workaround: upgrading the controller host"
     run_kayobe overcloud host upgrade
 
     if [[ ${KAYOBE_OVERCLOUD_GENERATE_CERTIFICATES} = 1 ]]; then
         echo "Generate TLS certificates"
         run_kayobe kolla ansible run certificates --kolla-extra kolla_certificates_dir=${KAYOBE_CONFIG_PATH}/kolla/certificates
+        # Add CA cert to trust store.
+        ca_cert=${KAYOBE_CONFIG_PATH}/kolla/certificates/ca/root.crt
+        if [[ -e /etc/debian_version ]]; then
+            # Ubuntu
+            sudo cp $ca_cert "/usr/local/share/ca-certificates/kayobe-customca.crt"
+            sudo update-ca-certificates
+        elif [[ -e /etc/redhat-release ]]; then
+            # CentOS
+            sudo cp $ca_cert "/etc/pki/ca-trust/source/anchors/kayobe-customca.crt"
+            sudo update-ca-trust
+        fi
     fi
 
     # Note: This must currently be before host configure, because host
     # configure runs kolla-ansible.yml, which validates the presence of the
     # built deploy images.
     if is_deploy_image_built_locally; then
         echo "Building overcloud deployment images"
```

### Comparing `kayobe-9.3.0/dev/tenks-deploy-config-compute.yml` & `kayobe-9.4.0/dev/tenks-deploy-config-compute.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/dev/tenks-deploy-config-overcloud.yml` & `kayobe-9.4.0/dev/tenks-deploy-config-overcloud.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/_extra/.htaccess` & `kayobe-9.4.0/doc/source/_extra/.htaccess`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/administration/bare-metal.rst` & `kayobe-9.4.0/doc/source/administration/bare-metal.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/administration/general.rst` & `kayobe-9.4.0/doc/source/administration/general.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/administration/overcloud.rst` & `kayobe-9.4.0/doc/source/administration/overcloud.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/administration/seed.rst` & `kayobe-9.4.0/doc/source/administration/seed.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/architecture.rst` & `kayobe-9.4.0/doc/source/architecture.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/conf.py` & `kayobe-9.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/ansible.rst` & `kayobe-9.4.0/doc/source/configuration/reference/ansible.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/bifrost.rst` & `kayobe-9.4.0/doc/source/configuration/reference/bifrost.rst`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 <https://cloudinit.readthedocs.io/en/latest/>`__ is used to process the
 configuration drive built by Bifrost, rather than the Bifrost default of
 :diskimage-builder-doc:`simple-init <elements/simple-init/README>`.
 
 ``kolla_bifrost_dib_os_element``
     DIB base OS element. Default is ``centos``.
 ``kolla_bifrost_dib_os_release``
-    DIB image OS release. Default is ``8``.
+    DIB image OS release. Default is ``8-stream``.
 ``kolla_bifrost_dib_elements_default``
     *Added in the Train release. Use kolla_bifrost_dib_elements in earlier
     releases.*
 
     List of default DIB elements. Default is ``["disable-selinux",
     "enable-serial-console", "vm"]``. The ``vm`` element is poorly named, and
     causes DIB to build a whole disk image rather than a single partition.
```

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/docker-registry.rst` & `kayobe-9.4.0/doc/source/configuration/reference/docker-registry.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/hosts.rst` & `kayobe-9.4.0/doc/source/configuration/reference/hosts.rst`

 * *Files 0% similar despite different names*

```diff
@@ -625,19 +625,20 @@
 For example:
 
 .. code-block:: yaml
    :caption: ``compute.yml``
 
    compute_lvm_groups_extra:
      - vgname: other-vg
-       disks: /dev/sdb
+       disks:
+         - /dev/sdb
        create: true
        lvnames:
          - lvname: other-vol
-           size: 100%
+           size: 100%FREE
            create: true
            mount: false
 
 Alternatively, replace the entire volume group list via one of the
 ``<host>_lvm_groups`` variables to replace the default configuration with a
 custom one.
```

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/ironic-python-agent.rst` & `kayobe-9.4.0/doc/source/configuration/reference/ironic-python-agent.rst`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,18 @@
 ``ipa_build_dib_elements``
     List of Diskimage Builder (DIB) elements to use when building IPA images.
     Default is combination of ``ipa_build_dib_elements_default`` and
     ``ipa_build_dib_elements_extra``.
 ``ipa_build_dib_env_default``
     Dictionary of default environment variables to provide to Diskimage Builder
     (DIB) during IPA image build. Default is
-    ``{"DIB_REPOLOCATION_ironic_agent": "{{ ipa_build_source_url }}",
-    "DIB_REPOREF_ironic_agent": "{{ ipa_build_source_version }}"}``.
+    ``{"DIB_RELEASE": "8-stream", "DIB_REPOLOCATION_ironic_python_agent": "{{
+    ipa_build_source_url }}", "DIB_REPOREF_ironic_python_agent": "{{
+    ipa_build_source_version }}", "DIB_REPOREF_requirements": "{{
+    openstack_branch }}"}``.
 ``ipa_build_dib_env_extra``
     Dictionary of additional environment variables to provide to Diskimage
     Builder (DIB) during IPA image build. Default is empty.
 ``ipa_build_dib_env``
     Dictionary of environment variables to provide to Diskimage Builder (DIB)
     during IPA image build. Default is a combination of
     ``ipa_build_dib_env_default`` and ``ipa_build_dib_env_extra``.
@@ -82,16 +84,16 @@
     `stackhpc.os-images <https://galaxy.ansible.com/stackhpc/os-images>`__ role
     for usage. Default is combination of ``ipa_build_dib_git_elements_default``
     and ``ipa_build_dib_git_elements_extra``.
 ``ipa_build_dib_packages``
     List of DIB packages to install. Default is none.
 ``ipa_build_upper_constraints_file``
     Upper constraints file for installing packages in the virtual environment
-    used for building IPA images. Default is ``{{ pip_upper_constraints_file
-    }}``.
+    used for building IPA images. To build CentOS Stream 8 images, default is
+    ``https://releases.openstack.org/constraints/upper/wallaby``.
 
 Example: Building IPA images locally
 ------------------------------------
 
 To build IPA images locally:
 
 .. code-block:: yaml
```

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/kayobe.rst` & `kayobe-9.4.0/doc/source/configuration/reference/kayobe.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/kolla-ansible.rst` & `kayobe-9.4.0/doc/source/configuration/reference/kolla-ansible.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/kolla.rst` & `kayobe-9.4.0/doc/source/configuration/reference/kolla.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/network.rst` & `kayobe-9.4.0/doc/source/configuration/reference/network.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/nova-cells.rst` & `kayobe-9.4.0/doc/source/configuration/reference/nova-cells.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/physical-network.rst` & `kayobe-9.4.0/doc/source/configuration/reference/physical-network.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/reference/seed-custom-containers.rst` & `kayobe-9.4.0/doc/source/configuration/reference/seed-custom-containers.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/scenarios/all-in-one/index.rst` & `kayobe-9.4.0/doc/source/configuration/scenarios/all-in-one/index.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/configuration/scenarios/all-in-one/overcloud.rst` & `kayobe-9.4.0/doc/source/configuration/scenarios/all-in-one/overcloud.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/contributor/automated.rst` & `kayobe-9.4.0/doc/source/contributor/automated.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/contributor/contributing.rst` & `kayobe-9.4.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/contributor/development.rst` & `kayobe-9.4.0/doc/source/contributor/development.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/contributor/manual.rst` & `kayobe-9.4.0/doc/source/contributor/manual.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/contributor/release-notes.rst` & `kayobe-9.4.0/doc/source/contributor/release-notes.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/contributor/releases.rst` & `kayobe-9.4.0/doc/source/contributor/releases.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/contributor/testing.rst` & `kayobe-9.4.0/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/contributor/vagrant.rst` & `kayobe-9.4.0/doc/source/contributor/vagrant.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/control-plane-service-placement.rst` & `kayobe-9.4.0/doc/source/control-plane-service-placement.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/custom-ansible-playbooks.rst` & `kayobe-9.4.0/doc/source/custom-ansible-playbooks.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/deployment.rst` & `kayobe-9.4.0/doc/source/deployment.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/getting-started.rst` & `kayobe-9.4.0/doc/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/index.rst` & `kayobe-9.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/installation.rst` & `kayobe-9.4.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/resources.rst` & `kayobe-9.4.0/doc/source/resources.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/support-matrix.rst` & `kayobe-9.4.0/doc/source/support-matrix.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/upgrading.rst` & `kayobe-9.4.0/doc/source/upgrading.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/source/usage.rst` & `kayobe-9.4.0/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/doc/test/redirect-tests.txt` & `kayobe-9.4.0/doc/test/redirect-tests.txt`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/bifrost.yml` & `kayobe-9.4.0/etc/kayobe/bifrost.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/bmc.yml` & `kayobe-9.4.0/etc/kayobe/bmc.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/compute.yml` & `kayobe-9.4.0/etc/kayobe/compute.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/controllers.yml` & `kayobe-9.4.0/etc/kayobe/controllers.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/dell-switch-bmp.yml` & `kayobe-9.4.0/etc/kayobe/dell-switch-bmp.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/dnf.yml` & `kayobe-9.4.0/etc/kayobe/dnf.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/dns.yml` & `kayobe-9.4.0/etc/kayobe/dns.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/docker-registry.yml` & `kayobe-9.4.0/etc/kayobe/docker-registry.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/docker.yml` & `kayobe-9.4.0/etc/kayobe/docker.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/globals.yml` & `kayobe-9.4.0/etc/kayobe/globals.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/grafana.yml` & `kayobe-9.4.0/etc/kayobe/grafana.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/idrac.yml` & `kayobe-9.4.0/etc/kayobe/idrac.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/inspector.yml` & `kayobe-9.4.0/etc/kayobe/inspector.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/inventory/group_vars/compute/network-interfaces` & `kayobe-9.4.0/etc/kayobe/inventory/group_vars/compute/network-interfaces`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/inventory/group_vars/controllers/network-interfaces` & `kayobe-9.4.0/etc/kayobe/inventory/group_vars/controllers/network-interfaces`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/inventory/group_vars/seed/network-interfaces` & `kayobe-9.4.0/etc/kayobe/inventory/group_vars/seed/network-interfaces`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/inventory/group_vars/storage/network-interfaces` & `kayobe-9.4.0/etc/kayobe/inventory/group_vars/storage/network-interfaces`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/inventory/groups` & `kayobe-9.4.0/etc/kayobe/inventory/groups`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/inventory/hosts.example` & `kayobe-9.4.0/etc/kayobe/inventory/hosts.example`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/ipa.yml` & `kayobe-9.4.0/etc/kayobe/ipa.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Version of IPA source repository. Default is {{ openstack_branch }}.
 #ipa_build_source_version:
 
 # URL of IPA builder source repository.
 #ipa_builder_source_url:
 
-# Version of IPA builder source repository. Default is master.
+# Version of IPA builder source repository. Default is stable/wallaby.
 #ipa_builder_source_version:
 
 # List of default Diskimage Builder (DIB) elements to use when building IPA
 # images. Default is ["centos", "enable-serial-console",
 # "ironic-python-agent-ramdisk"].
 #ipa_build_dib_elements_default:
 
@@ -58,15 +58,16 @@
 # ipa_build_dib_git_elements_default and ipa_build_dib_git_elements_extra.
 #ipa_build_dib_git_elements:
 
 # List of DIB packages to install. Default is none.
 #ipa_build_dib_packages:
 
 # Upper constraints file for installing packages in the virtual environment
-# used for building IPA images. Default is {{ pip_upper_constraints_file }}.
+# used for building IPA images. To build CentOS Stream 8 images, default is
+# "https://releases.openstack.org/constraints/upper/wallaby".
 #ipa_build_upper_constraints_file:
 
 ###############################################################################
 # Ironic Python Agent (IPA) images configuration.
 
 # Suffix of upstream Ironic deployment image files. Default is based on
 # {{ openstack_branch }}.
```

### Comparing `kayobe-9.3.0/etc/kayobe/ironic.yml` & `kayobe-9.4.0/etc/kayobe/ironic.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/kolla.yml` & `kayobe-9.4.0/etc/kayobe/kolla.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/monasca.yml` & `kayobe-9.4.0/etc/kayobe/monasca.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/monitoring.yml` & `kayobe-9.4.0/etc/kayobe/monitoring.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/networks.yml` & `kayobe-9.4.0/etc/kayobe/networks.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/neutron.yml` & `kayobe-9.4.0/etc/kayobe/neutron.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/ntp.yml` & `kayobe-9.4.0/etc/kayobe/ntp.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/overcloud.yml` & `kayobe-9.4.0/etc/kayobe/overcloud.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/pip.yml` & `kayobe-9.4.0/etc/kayobe/pip.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/seed-hypervisor.yml` & `kayobe-9.4.0/etc/kayobe/seed-hypervisor.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/seed-vm.yml` & `kayobe-9.4.0/etc/kayobe/seed-vm.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/seed.yml` & `kayobe-9.4.0/etc/kayobe/seed.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/storage.yml` & `kayobe-9.4.0/etc/kayobe/storage.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/etc/kayobe/swift.yml` & `kayobe-9.4.0/etc/kayobe/swift.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/ansible.py` & `kayobe-9.4.0/kayobe/ansible.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/cli/commands.py` & `kayobe-9.4.0/kayobe/cli/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1060,14 +1060,18 @@
         group.add_argument("--incremental", action='store_true',
                            help="Whether to perform an incremental database "
                                 "backup. Default is false.")
         return parser
 
     def take_action(self, parsed_args):
         self.app.LOG.debug("Performing overcloud database backup")
+
+        # First prepare configuration.
+        self.generate_kolla_ansible_config(parsed_args, service_config=False)
+
         extra_args = []
         if parsed_args.incremental:
             extra_args.append('--incremental')
         self.run_kolla_ansible_overcloud(parsed_args, "mariadb_backup",
                                          extra_args=extra_args)
 
 
@@ -1084,14 +1088,18 @@
                                 "automatically determine which host to use, "
                                 "and this option should not be used.")
         return parser
 
     def take_action(self, parsed_args):
         self.app.LOG.debug("Performing overcloud database recovery")
         extra_vars = {}
+
+        # First prepare configuration.
+        self.generate_kolla_ansible_config(parsed_args, service_config=True)
+
         if parsed_args.force_recovery_host:
             extra_vars['mariadb_recover_inventory_name'] = (
                 parsed_args.force_recovery_host)
         self.run_kolla_ansible_overcloud(parsed_args, "mariadb_recovery",
                                          extra_vars=extra_vars)
```

### Comparing `kayobe-9.3.0/kayobe/cmd/kayobe.py` & `kayobe-9.4.0/kayobe/cmd/kayobe.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/cmd/kayobe_vault_password_helper.py` & `kayobe-9.4.0/kayobe/cmd/kayobe_vault_password_helper.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/exception.py` & `kayobe-9.4.0/kayobe/exception.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/kolla_ansible.py` & `kayobe-9.4.0/kayobe/kolla_ansible.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/plugins/action/kolla_ansible_host_vars.py` & `kayobe-9.4.0/kayobe/plugins/action/kolla_ansible_host_vars.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/tests/molecule/utils.py` & `kayobe-9.4.0/kayobe/tests/molecule/utils.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/tests/unit/cli/test_commands.py` & `kayobe-9.4.0/kayobe/tests/unit/cli/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1206,83 +1206,153 @@
                         "ansible", "overcloud-etc-hosts-fixup.yml"),
                 ],
                 limit="overcloud",
             ),
         ]
         self.assertEqual(expected_calls, mock_run.call_args_list)
 
+    @mock.patch.object(commands.KayobeAnsibleMixin,
+                       "run_kayobe_playbooks")
     @mock.patch.object(commands.KollaAnsibleMixin,
                        "run_kolla_ansible_overcloud")
-    def test_overcloud_database_backup(self, mock_run):
+    def test_overcloud_database_backup(self, mock_kolla_run, mock_run):
         command = commands.OvercloudDatabaseBackup(TestApp(), [])
         parser = command.get_parser("test")
         parsed_args = parser.parse_args([])
         result = command.run(parsed_args)
         self.assertEqual(0, result)
+
+        expected_calls = [
+            mock.call(
+                mock.ANY,
+                [utils.get_data_files_path("ansible", "kolla-ansible.yml")],
+                tags="config",
+                ignore_limit=True,
+            ),
+        ]
+        self.assertEqual(expected_calls, mock_run.call_args_list)
+
         expected_calls = [
             mock.call(
                 mock.ANY,
                 "mariadb_backup",
                 extra_args=[]
             ),
         ]
-        self.assertEqual(expected_calls, mock_run.call_args_list)
+        self.assertEqual(expected_calls, mock_kolla_run.call_args_list)
 
+    @mock.patch.object(commands.KayobeAnsibleMixin,
+                       "run_kayobe_playbooks")
     @mock.patch.object(commands.KollaAnsibleMixin,
                        "run_kolla_ansible_overcloud")
-    def test_overcloud_database_backup_incremental(self, mock_run):
+    def test_overcloud_database_backup_incremental(self, mock_kolla_run,
+                                                   mock_run):
         command = commands.OvercloudDatabaseBackup(TestApp(), [])
         parser = command.get_parser("test")
         parsed_args = parser.parse_args(["--incremental"])
         result = command.run(parsed_args)
         self.assertEqual(0, result)
+
+        expected_calls = [
+            mock.call(
+                mock.ANY,
+                [utils.get_data_files_path("ansible", "kolla-ansible.yml")],
+                tags="config",
+                ignore_limit=True,
+            ),
+        ]
+        self.assertEqual(expected_calls, mock_run.call_args_list)
+
         expected_calls = [
             mock.call(
                 mock.ANY,
                 "mariadb_backup",
                 extra_args=["--incremental"]
             ),
         ]
-        self.assertEqual(expected_calls, mock_run.call_args_list)
+        self.assertEqual(expected_calls, mock_kolla_run.call_args_list)
 
+    @mock.patch.object(commands.KayobeAnsibleMixin,
+                       "run_kayobe_playbooks")
     @mock.patch.object(commands.KollaAnsibleMixin,
                        "run_kolla_ansible_overcloud")
-    def test_overcloud_database_recover(self, mock_run):
+    def test_overcloud_database_recover(self, mock_kolla_run, mock_run):
         command = commands.OvercloudDatabaseRecover(TestApp(), [])
         parser = command.get_parser("test")
         parsed_args = parser.parse_args([])
         result = command.run(parsed_args)
         self.assertEqual(0, result)
+
+        expected_calls = [
+            mock.call(
+                mock.ANY,
+                [utils.get_data_files_path("ansible", "kolla-ansible.yml")],
+                tags="config",
+                ignore_limit=True,
+            ),
+            mock.call(
+                mock.ANY,
+                [
+                    utils.get_data_files_path("ansible",
+                                              "kolla-openstack.yml"),
+                ],
+                ignore_limit=True,
+            ),
+        ]
+        self.assertEqual(expected_calls, mock_run.call_args_list)
+
         expected_calls = [
             mock.call(
                 mock.ANY,
                 "mariadb_recovery",
                 extra_vars={}
             ),
         ]
-        self.assertEqual(expected_calls, mock_run.call_args_list)
+        self.assertEqual(expected_calls, mock_kolla_run.call_args_list)
 
+    @mock.patch.object(commands.KayobeAnsibleMixin,
+                       "run_kayobe_playbooks")
     @mock.patch.object(commands.KollaAnsibleMixin,
                        "run_kolla_ansible_overcloud")
-    def test_overcloud_database_recover_force_host(self, mock_run):
+    def test_overcloud_database_recover_force_host(self, mock_kolla_run,
+                                                   mock_run):
         command = commands.OvercloudDatabaseRecover(TestApp(), [])
         parser = command.get_parser("test")
         parsed_args = parser.parse_args(["--force-recovery-host", "foo"])
         result = command.run(parsed_args)
         self.assertEqual(0, result)
+
+        expected_calls = [
+            mock.call(
+                mock.ANY,
+                [utils.get_data_files_path("ansible", "kolla-ansible.yml")],
+                tags="config",
+                ignore_limit=True,
+            ),
+            mock.call(
+                mock.ANY,
+                [
+                    utils.get_data_files_path("ansible",
+                                              "kolla-openstack.yml"),
+                ],
+                ignore_limit=True,
+            ),
+        ]
+        self.assertEqual(expected_calls, mock_run.call_args_list)
+
         expected_calls = [
             mock.call(
                 mock.ANY,
                 "mariadb_recovery",
                 extra_vars={
                     "mariadb_recover_inventory_name": "foo"
                 }
             ),
         ]
-        self.assertEqual(expected_calls, mock_run.call_args_list)
+        self.assertEqual(expected_calls, mock_kolla_run.call_args_list)
 
     @mock.patch.object(commands.KayobeAnsibleMixin,
                        "run_kayobe_playbooks")
     def test_overcloud_service_configuration_save(self, mock_run):
         command = commands.OvercloudServiceConfigurationSave(TestApp(), [])
         parser = command.get_parser("test")
         parsed_args = parser.parse_args([])
```

### Comparing `kayobe-9.3.0/kayobe/tests/unit/plugins/action/test_kolla_ansible_host_vars.py` & `kayobe-9.4.0/kayobe/tests/unit/plugins/action/test_kolla_ansible_host_vars.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/tests/unit/test_ansible.py` & `kayobe-9.4.0/kayobe/tests/unit/test_ansible.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/tests/unit/test_kolla_ansible.py` & `kayobe-9.4.0/kayobe/tests/unit/test_kolla_ansible.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/tests/unit/test_utils.py` & `kayobe-9.4.0/kayobe/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/tests/unit/test_vault.py` & `kayobe-9.4.0/kayobe/tests/unit/test_vault.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/utils.py` & `kayobe-9.4.0/kayobe/utils.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/vault.py` & `kayobe-9.4.0/kayobe/vault.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe/version.py` & `kayobe-9.4.0/kayobe/version.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/kayobe.egg-info/PKG-INFO` & `kayobe-9.4.0/kayobe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kayobe
-Version: 9.3.0
+Version: 9.4.0
 Summary: Deployment of OpenStack to bare metal using OpenStack kolla and bifrost
 Home-page: https://docs.openstack.org/kayobe/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: Kayobe
         ======
```

### Comparing `kayobe-9.3.0/kayobe.egg-info/SOURCES.txt` & `kayobe-9.4.0/kayobe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,17 @@
 ansible/roles/dnf/defaults/main.yml
 ansible/roles/dnf/tasks/custom-repo.yml
 ansible/roles/dnf/tasks/local-mirror.yml
 ansible/roles/dnf/tasks/main.yml
 ansible/roles/dnf/templates/CentOS-Linux-AppStream.repo.j2
 ansible/roles/dnf/templates/CentOS-Linux-BaseOS.repo.j2
 ansible/roles/dnf/templates/CentOS-Linux-Extras.repo.j2
+ansible/roles/dnf/templates/CentOS-Stream-AppStream.repo.j2
+ansible/roles/dnf/templates/CentOS-Stream-BaseOS.repo.j2
+ansible/roles/dnf/templates/CentOS-Stream-Extras.repo.j2
 ansible/roles/dnf/templates/epel-modular.repo.j2
 ansible/roles/dnf/templates/epel.repo.j2
 ansible/roles/docker-devicemapper/defaults/main.yml
 ansible/roles/docker-devicemapper/handlers/main.yml
 ansible/roles/docker-devicemapper/tasks/main.yml
 ansible/roles/docker-devicemapper/templates/docker-thinpool.profile.j2
 ansible/roles/docker-registry/README.md
@@ -558,14 +561,15 @@
 kayobe/vault.py
 kayobe/version.py
 kayobe.egg-info/PKG-INFO
 kayobe.egg-info/SOURCES.txt
 kayobe.egg-info/dependency_links.txt
 kayobe.egg-info/entry_points.txt
 kayobe.egg-info/not-zip-safe
+kayobe.egg-info/pbr.json
 kayobe.egg-info/requires.txt
 kayobe.egg-info/top_level.txt
 kayobe/cli/__init__.py
 kayobe/cli/commands.py
 kayobe/cmd/__init__.py
 kayobe/cmd/kayobe.py
 kayobe/cmd/kayobe_vault_password_helper.py
@@ -645,32 +649,36 @@
 releasenotes/notes/ansible-2.8-2.9-2df006b066704417.yaml
 releasenotes/notes/ansible-facts-2b3389a2534d47a2.yaml
 releasenotes/notes/arista-switch-aedc46148506c56e.yaml
 releasenotes/notes/ask-vault-pass-b6ced0220384dde1.yaml
 releasenotes/notes/avoid-unconditional-fact-gathering-4dfbf96e2111ad51.yaml
 releasenotes/notes/bifrost-dib-extra-c4eac903986ec700.yaml
 releasenotes/notes/bifrost-firewalld-zone-09a29651a058531a.yaml
+releasenotes/notes/bifrost-inspection-gateway-316ab384430ef8df.yaml
 releasenotes/notes/bifrost-ironic-extra-kernel-params-e3e56a9dcdf24bb6.yaml
 releasenotes/notes/bifrost-use-firewalld-90b69e2ac6eead67.yaml
 releasenotes/notes/bifrost-victoria-fixes-eed49b088afdac5b.yaml
 releasenotes/notes/blacklist-ansible-2.9.8-f83ad748b01a575b.yaml
 releasenotes/notes/bootproto-52316b6dbc30e98c.yaml
 releasenotes/notes/bootstrap-openrc-9aec3d53d0d62c81.yaml
 releasenotes/notes/bootstrap-servers-user-8cb5114de1dd10ec.yaml
 releasenotes/notes/bugfix-dnf-proxy-cd934867c3d64388.yaml
 releasenotes/notes/bugfix-monasca-grafana-dashboard-config-b81781cf10c2a236.yaml
 releasenotes/notes/bugfix-update-idrac-role-71ede6900dc000a7.yaml
+releasenotes/notes/build-centos8s-images-509f04d8d68cb357.yaml
 releasenotes/notes/build-neutron-sriov-836acf378bae0b48.yaml
 releasenotes/notes/cacert-514b8645d6912bf9.yaml
 releasenotes/notes/centos-8-12073e91a157d0a2.yaml
 releasenotes/notes/centos-8-chrony-bec9d7bc8b346363.yaml
 releasenotes/notes/centos-8.3-89d07c8f8db5b17b.yaml
 releasenotes/notes/centos-ipa-images-60dde12f2b4f4f8c.yaml
 releasenotes/notes/concurrent-known-hosts-update-8dc94557e9a48021.yaml
 releasenotes/notes/config-galaxy-roles-6bd129824436a983.yaml
+releasenotes/notes/config-idemoptence-37846db82ecd9f43.yaml
+releasenotes/notes/configdrive-vlans-4e8b6ed07b229233.yaml
 releasenotes/notes/cumulus-switch-baf554118ef23afe.yaml
 releasenotes/notes/custom-ansible-config-d0f1bcdf2607e521.yaml
 releasenotes/notes/custom-certificates-5f2c1fff6503b77a.yaml
 releasenotes/notes/custom-route-options-2ed446961262a34a.yaml
 releasenotes/notes/db-backup-recovery-d4f1ced2ebd7dac4.yaml
 releasenotes/notes/default-disable-ironic-2c20b8a7e69f19c5.yaml
 releasenotes/notes/default-lvm-data-vg-f2848066975beeda.yaml
@@ -712,35 +720,39 @@
 releasenotes/notes/fix-inspection-when-using-ipxe-9bf6ed9e6456840b.yaml
 releasenotes/notes/fix-inspector-ipxe-uefi-86f435ebaf4eee08.yaml
 releasenotes/notes/fix-inspector-rule-idempotency-f6e5a61f7dca580f.yaml
 releasenotes/notes/fix-introspection-data-save-51001baa37d97084.yaml
 releasenotes/notes/fix-introspection-data-save-cfc83714f66fd63c.yaml
 releasenotes/notes/fix-ipa-build-b31fb20ddcbe3ece.yaml
 releasenotes/notes/fix-ipa-image-download-3f90f0f40d0feafd.yaml
+releasenotes/notes/fix-kolla-ansible-group-mapping-8fcd6cbb1e744e18.yaml
 releasenotes/notes/fix-limit-with-commas-04a357b0b7ef0371.yaml
 releasenotes/notes/fix-network-hosts-interfaces-f0206aa91b218a25.yaml
 releasenotes/notes/fix-no-ip-addr-on-nic-38d6f8e8078f534d.yaml
+releasenotes/notes/fix-overcloud-database-backup-with-no-kolla-config-4f857915adabad41.yaml
 releasenotes/notes/fix-persistent-sysctls-1aef170599a49608.yaml
 releasenotes/notes/fix-post-config-public-eb72f3a692a2be6b.yaml
 releasenotes/notes/fix-python-setup-5e7ff929a6cab092.yaml
 releasenotes/notes/fix-remote-seed-vm-provisioning-faa8de569ca6bc89.yaml
 releasenotes/notes/fix-seed-multiple-networks-458915b085a9478c.yaml
 releasenotes/notes/fix-seed-vm-provision-c432ebfae8bfee8b.yaml
 releasenotes/notes/fix-selinux-disable-reboot-65c32f5dc895211c.yaml
+releasenotes/notes/fixes-keyerror-vlan-link-c177cf719e070df6.yaml
 releasenotes/notes/fluentd-custom-inputs-1b911bd229e8a9e4.yaml
 releasenotes/notes/hardware-inspection-timeouts-777f3bb569929f0f.yaml
 releasenotes/notes/host-package-update-c5bddba791754646.yaml
 releasenotes/notes/host-run-command-eb98cb077d546551.yaml
 releasenotes/notes/ignore-unconfigured-nets-93beaf96f43af1ed.yaml
 releasenotes/notes/improve-ssh-known-host-error-15fbc6ae4fa3dbd6.yaml
 releasenotes/notes/initial-f71c8e25375afa25.yaml
 releasenotes/notes/inspector-25gbe-port-9bdc3bb354e3dfb6.yaml
 releasenotes/notes/inspector-dhcp-range-netmask-bb46eb7df77587a4.yaml
 releasenotes/notes/install-prefix-multiple-lib-9288e8c11da3c0bc.yaml
 releasenotes/notes/internal-api-tls-4e7383e6a0262f5f.yaml
+releasenotes/notes/ipa-branch-b29c377c531013a8.yaml
 releasenotes/notes/ipa-build-dib-packages-5e85baba3294eb65.yaml
 releasenotes/notes/ipa-build-upper-constraints-5686abaa161b0d94.yaml
 releasenotes/notes/ipa-builder-ea6308b6691ae71e.yaml
 releasenotes/notes/kolla-ansible-become-false-95aa88edd3c8c259.yaml
 releasenotes/notes/kolla-docker-registry-e1adce280fc17db7.yaml
 releasenotes/notes/kolla-enable-openstack-core-ce4866dd388f262e.yaml
 releasenotes/notes/kolla-external-fqdn-cacert-048aa1299050cfd7.yaml
@@ -755,14 +767,15 @@
 releasenotes/notes/neutron-mlnx-agent-19631a3936da47df.yaml
 releasenotes/notes/non-shared-ironic-nets-06a43c9b6dea2a77.yaml
 releasenotes/notes/openrc-upgrade-9e14888d600f6839.yaml
 releasenotes/notes/openstack-branch-87df0c2f647037c0.yaml
 releasenotes/notes/optional-epel-release-92eaf3dc4aa1021b.yaml
 releasenotes/notes/package-runtime-files-in-python-package-c3dda2bd32844fdf.yaml
 releasenotes/notes/passwords-in-tmp-18e55d5e9b894b4d.yaml
+releasenotes/notes/patch-links-on-overcloud-e24dbc858d3399cc.yaml
 releasenotes/notes/per-host-interfaces-6e548331fa3a4244.yaml
 releasenotes/notes/physical-network-disable-discovery-15916760e0a4d0bc.yaml
 releasenotes/notes/pip-index-url-conditional-3f9c5b3c5c808500.yaml
 releasenotes/notes/pip-local-mirror-d9a80257c8441970.yaml
 releasenotes/notes/pip_proxy-6c6022b6566dae69.yaml
 releasenotes/notes/plug-ovs-phy-f180d9bb9dd25dab.yaml
 releasenotes/notes/prevent-resolv.conf-4a09d50f60f3fe28.yaml
@@ -793,14 +806,15 @@
 releasenotes/notes/seed-hypervisor-host-package-update-fix-9411205aadc92b8f.yaml
 releasenotes/notes/seed-hypervisor-lvm-80864721ff42f6a5.yaml
 releasenotes/notes/seed-service-upgrade-71b847e3658a1948.yaml
 releasenotes/notes/seed-vm-centos-8.2-36b7a480a7725da1.yaml
 releasenotes/notes/seed-vm-centos-8.3-7726c9d0603508eb.yaml
 releasenotes/notes/seperate-storage-networks-a659bcd30dd70665.yaml
 releasenotes/notes/setup-module-args-2c36e56bf78ab5f0.yaml
+releasenotes/notes/specify-requirements-branch-for-ipa-build-c3ca977ec21b58f4.yaml
 releasenotes/notes/ssh-batchmode-cda7a4ed63006378.yaml
 releasenotes/notes/stale-virtualenvs-125c513af3de9396.yaml
 releasenotes/notes/story-2007297-73f498ef6bc89fe9.yaml
 releasenotes/notes/story-2008354-0c34e2ad7aeb7d3d.yaml
 releasenotes/notes/story-2008430-6a50101d05219aad.yaml
 releasenotes/notes/support-deploy-containers-7acf4c647fb5c3fa.yaml
 releasenotes/notes/support_configuring_tunnel_network-1646eef887d72abf.yaml
```

### Comparing `kayobe-9.3.0/kayobe.egg-info/entry_points.txt` & `kayobe-9.4.0/kayobe.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-base/pre.yml` & `kayobe-9.4.0/playbooks/kayobe-base/pre.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-base/overrides.yml.j2` & `kayobe-9.4.0/playbooks/kayobe-overcloud-base/overrides.yml.j2`

 * *Files 4% similar despite different names*

```diff
@@ -31,13 +31,10 @@
 # Enable ironic for testing baremetal compute.
 kolla_enable_ironic: true
 
 {% if tls_enabled %}
 kolla_enable_tls_external: "yes"
 kolla_enable_tls_internal: "yes"
 
-# FIXME: ipa-images fails to access OS_CACERT from /home/zuul.
-kayobe_ansible_user: zuul
-
 kolla_ironic_pxe_append_params_extra:
   - ipa-insecure=1
 {% endif %}
```

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-base/pre.yml` & `kayobe-9.4.0/playbooks/kayobe-overcloud-base/pre.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-base/run.yml` & `kayobe-9.4.0/playbooks/kayobe-overcloud-base/run.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-host-configure-base/overrides.yml.j2` & `kayobe-9.4.0/playbooks/kayobe-overcloud-host-configure-base/overrides.yml.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-host-configure-base/pre.yml` & `kayobe-9.4.0/playbooks/kayobe-overcloud-host-configure-base/pre.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-host-configure-base/run.yml` & `kayobe-9.4.0/playbooks/kayobe-overcloud-host-configure-base/run.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-host-configure-base/tests/test_overcloud_host_configure.py` & `kayobe-9.4.0/playbooks/kayobe-overcloud-host-configure-base/tests/test_overcloud_host_configure.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-upgrade-base/globals.yml.j2` & `kayobe-9.4.0/playbooks/kayobe-overcloud-upgrade-base/globals.yml.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-upgrade-base/overrides.yml.j2` & `kayobe-9.4.0/playbooks/kayobe-overcloud-upgrade-base/overrides.yml.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-upgrade-base/pre.yml` & `kayobe-9.4.0/playbooks/kayobe-overcloud-upgrade-base/pre.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-overcloud-upgrade-base/run.yml` & `kayobe-9.4.0/playbooks/kayobe-overcloud-upgrade-base/run.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-seed-base/overrides.yml.j2` & `kayobe-9.4.0/playbooks/kayobe-seed-upgrade-base/overrides.yml.j2`

 * *Files 14% similar despite different names*

```diff
@@ -6,36 +6,31 @@
 # Use the OpenStack infra's Dockerhub mirror.
 docker_registry_mirrors:
   - "http://{{ zuul_site_mirror_fqdn }}:8082/"
 
 kolla_docker_namespace: "openstack.kolla"
 # use the published images from a site mirror of quay.io
 kolla_docker_registry: "{{ zuul_site_mirror_fqdn }}:4447"
+{% if not is_previous_release | default(false) %}
 kolla_source_url: "{{ ansible_env.PWD ~ '/' ~ zuul.projects['opendev.org/openstack/kolla'].src_dir }}"
 kolla_source_version: "{{ zuul.projects['opendev.org/openstack/kolla'].checkout }}"
 kolla_ansible_source_url: "{{ ansible_env.PWD ~ '/' ~ zuul.projects['opendev.org/openstack/kolla-ansible'].src_dir }}"
 kolla_ansible_source_version: "{{ zuul.projects['opendev.org/openstack/kolla-ansible'].checkout }}"
-kolla_openstack_logging_debug: True
 pip_upper_constraints_file: "/tmp/upper-constraints.txt"
+{% endif %}
+kolla_openstack_logging_debug: True
+
+# NOTE(mgoddard): We're using a cirros image, which doesn't require the
+# resolv.conf work around used for CentOS.
+# NOTE(piotrp): to be removed after Wallaby is released
+overcloud_host_image_workaround_resolv_enabled: false
 
 # Use the CI infra's PyPI mirror.
 pip_local_mirror: true
 pip_index_url: "http://{{ zuul_site_mirror_fqdn }}/pypi/simple"
 
 # NOTE(mgoddard): CentOS 8 removes interfaces from their bridge during ifdown,
 # and removes the bridge if there are no interfaces left. When Kayobe bounces
 # veth links plugged into the bridge, it causes the bridge which has the IP we
 # are using for SSH to be removed. Use a dummy interface.
 aio_bridge_ports:
   - dummy1
-
-# Build seed deployment images (IPA) with extra-hardware element
-ipa_build_images: true
-ipa_build_dib_elements_extra:
-  - "extra-hardware"
-{% if is_centos_stream | default(false) %}
-ipa_build_dib_env_extra:
-  DIB_RELEASE: "8-stream"
-# diskimage-builder 3.2.1 only includes CentOS Stream 8 support in the
-# centos-minimal element.
-ipa_build_upper_constraints_file: "https://releases.openstack.org/constraints/upper/wallaby"
-{% endif %}
```

### Comparing `kayobe-9.3.0/playbooks/kayobe-seed-base/pre.yml` & `kayobe-9.4.0/playbooks/kayobe-seed-base/pre.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-seed-upgrade-base/overrides.yml.j2` & `kayobe-9.4.0/playbooks/kayobe-seed-base/overrides.yml.j2`

 * *Files 26% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 # Use the OpenStack infra's Dockerhub mirror.
 docker_registry_mirrors:
   - "http://{{ zuul_site_mirror_fqdn }}:8082/"
 
 kolla_docker_namespace: "openstack.kolla"
 # use the published images from a site mirror of quay.io
 kolla_docker_registry: "{{ zuul_site_mirror_fqdn }}:4447"
-{% if not is_previous_release | default(false) %}
 kolla_source_url: "{{ ansible_env.PWD ~ '/' ~ zuul.projects['opendev.org/openstack/kolla'].src_dir }}"
 kolla_source_version: "{{ zuul.projects['opendev.org/openstack/kolla'].checkout }}"
 kolla_ansible_source_url: "{{ ansible_env.PWD ~ '/' ~ zuul.projects['opendev.org/openstack/kolla-ansible'].src_dir }}"
 kolla_ansible_source_version: "{{ zuul.projects['opendev.org/openstack/kolla-ansible'].checkout }}"
-pip_upper_constraints_file: "/tmp/upper-constraints.txt"
-{% endif %}
 kolla_openstack_logging_debug: True
-
-# NOTE(mgoddard): We're using a cirros image, which doesn't require the
-# resolv.conf work around used for CentOS.
-# NOTE(piotrp): to be removed after Wallaby is released
-overcloud_host_image_workaround_resolv_enabled: false
+pip_upper_constraints_file: "/tmp/upper-constraints.txt"
 
 # Use the CI infra's PyPI mirror.
 pip_local_mirror: true
 pip_index_url: "http://{{ zuul_site_mirror_fqdn }}/pypi/simple"
 
 # NOTE(mgoddard): CentOS 8 removes interfaces from their bridge during ifdown,
 # and removes the bridge if there are no interfaces left. When Kayobe bounces
```

### Comparing `kayobe-9.3.0/playbooks/kayobe-seed-upgrade-base/pre.yml` & `kayobe-9.4.0/playbooks/kayobe-seed-upgrade-base/pre.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-seed-upgrade-base/run.yml` & `kayobe-9.4.0/playbooks/kayobe-seed-upgrade-base/run.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-seed-vm-base/overrides.yml.j2` & `kayobe-9.4.0/playbooks/kayobe-seed-vm-base/overrides.yml.j2`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-seed-vm-base/pre.yml` & `kayobe-9.4.0/playbooks/kayobe-seed-vm-base/pre.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/playbooks/kayobe-seed-vm-base/run.yml` & `kayobe-9.4.0/playbooks/kayobe-seed-vm-base/run.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/ansible-facts-2b3389a2534d47a2.yaml` & `kayobe-9.4.0/releasenotes/notes/ansible-facts-2b3389a2534d47a2.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/bifrost-dib-extra-c4eac903986ec700.yaml` & `kayobe-9.4.0/releasenotes/notes/bifrost-dib-extra-c4eac903986ec700.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/bifrost-firewalld-zone-09a29651a058531a.yaml` & `kayobe-9.4.0/releasenotes/notes/bifrost-firewalld-zone-09a29651a058531a.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/bifrost-use-firewalld-90b69e2ac6eead67.yaml` & `kayobe-9.4.0/releasenotes/notes/bifrost-use-firewalld-90b69e2ac6eead67.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/bifrost-victoria-fixes-eed49b088afdac5b.yaml` & `kayobe-9.4.0/releasenotes/notes/bifrost-victoria-fixes-eed49b088afdac5b.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/bootstrap-servers-user-8cb5114de1dd10ec.yaml` & `kayobe-9.4.0/releasenotes/notes/bootstrap-servers-user-8cb5114de1dd10ec.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/centos-8-12073e91a157d0a2.yaml` & `kayobe-9.4.0/releasenotes/notes/centos-8-12073e91a157d0a2.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/custom-certificates-5f2c1fff6503b77a.yaml` & `kayobe-9.4.0/releasenotes/notes/custom-certificates-5f2c1fff6503b77a.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/default-lvm-data-vg-f2848066975beeda.yaml` & `kayobe-9.4.0/releasenotes/notes/default-lvm-data-vg-f2848066975beeda.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/default-target-virtualenv-3a68472f66b7aaf3.yaml` & `kayobe-9.4.0/releasenotes/notes/default-target-virtualenv-3a68472f66b7aaf3.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/disable-chrony-5f1e4f9db509c42d.yaml` & `kayobe-9.4.0/releasenotes/notes/disable-chrony-5f1e4f9db509c42d.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/dnf-2071fc40b0d783b6.yaml` & `kayobe-9.4.0/releasenotes/notes/dnf-2071fc40b0d783b6.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/docker-registry-env-e954a0642555864f.yaml` & `kayobe-9.4.0/releasenotes/notes/docker-registry-env-e954a0642555864f.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/docker-registry-on-seed-2eb4fb643d6fda9a.yaml` & `kayobe-9.4.0/releasenotes/notes/docker-registry-on-seed-2eb4fb643d6fda9a.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/fix-ipa-image-download-3f90f0f40d0feafd.yaml` & `kayobe-9.4.0/releasenotes/notes/fix-ipa-image-download-3f90f0f40d0feafd.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/fix-network-hosts-interfaces-f0206aa91b218a25.yaml` & `kayobe-9.4.0/releasenotes/notes/fix-network-hosts-interfaces-f0206aa91b218a25.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/fix-seed-multiple-networks-458915b085a9478c.yaml` & `kayobe-9.4.0/releasenotes/notes/fix-seed-multiple-networks-458915b085a9478c.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/hardware-inspection-timeouts-777f3bb569929f0f.yaml` & `kayobe-9.4.0/releasenotes/notes/hardware-inspection-timeouts-777f3bb569929f0f.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/initial-f71c8e25375afa25.yaml` & `kayobe-9.4.0/releasenotes/notes/initial-f71c8e25375afa25.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/ipa-builder-ea6308b6691ae71e.yaml` & `kayobe-9.4.0/releasenotes/notes/ipa-builder-ea6308b6691ae71e.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/package-runtime-files-in-python-package-c3dda2bd32844fdf.yaml` & `kayobe-9.4.0/releasenotes/notes/package-runtime-files-in-python-package-c3dda2bd32844fdf.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/passwords-in-tmp-18e55d5e9b894b4d.yaml` & `kayobe-9.4.0/releasenotes/notes/passwords-in-tmp-18e55d5e9b894b4d.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/physical-network-disable-discovery-15916760e0a4d0bc.yaml` & `kayobe-9.4.0/releasenotes/notes/physical-network-disable-discovery-15916760e0a4d0bc.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/seperate-storage-networks-a659bcd30dd70665.yaml` & `kayobe-9.4.0/releasenotes/notes/seperate-storage-networks-a659bcd30dd70665.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/stale-virtualenvs-125c513af3de9396.yaml` & `kayobe-9.4.0/releasenotes/notes/stale-virtualenvs-125c513af3de9396.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/notes/swift-improvements-07a2b75967f642e8.yaml` & `kayobe-9.4.0/releasenotes/notes/swift-improvements-07a2b75967f642e8.yaml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/source/conf.py` & `kayobe-9.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/source/ocata.rst` & `kayobe-9.4.0/releasenotes/source/ocata.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/releasenotes/source/pike.rst` & `kayobe-9.4.0/releasenotes/source/pike.rst`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/requirements.yml` & `kayobe-9.4.0/requirements.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ---
 - src: ahuffman.resolv
   version: 1.3.1
 - src: jriguera.configdrive
   # There are no versioned releases of this role.
-  version: e12d38378ae127c9c61d170fa4ba4729f2c5f2ad
+  version: 29871bf3279ef95fc8f7339b9abd13f869980750
 - src: MichaelRigart.interfaces
   version: v1.12.0
 - src: mrlesmithjr.manage-lvm
   version: v0.2.2
 - src: mrlesmithjr.mdadm
   version: v0.1.1
 - src: singleplatform-eng.users
```

### Comparing `kayobe-9.3.0/roles/kayobe-ci-prep/tasks/main.yml` & `kayobe-9.4.0/roles/kayobe-ci-prep/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/roles/kayobe-diagnostics/files/get_logs.sh` & `kayobe-9.4.0/roles/kayobe-diagnostics/files/get_logs.sh`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/roles/kayobe-diagnostics/tasks/post.yml` & `kayobe-9.4.0/roles/kayobe-diagnostics/tasks/post.yml`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/setup.cfg` & `kayobe-9.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/setup.py` & `kayobe-9.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/test-requirements.txt` & `kayobe-9.4.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/tools/loc` & `kayobe-9.4.0/tools/loc`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/tools/release.sh` & `kayobe-9.4.0/tools/release.sh`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/tools/sphinx8` & `kayobe-9.4.0/tools/sphinx8`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/tools/test-ansible.sh` & `kayobe-9.4.0/tools/test-ansible.sh`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/tools/test-molecule.sh` & `kayobe-9.4.0/tools/test-molecule.sh`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/tox.ini` & `kayobe-9.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `kayobe-9.3.0/zuul.d/jobs.yaml` & `kayobe-9.4.0/zuul.d/jobs.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,15 @@
     # previous release which takes a considerable amount of time.
     attempts: 3
 
 - job:
     name: kayobe-overcloud-upgrade-centos8s
     parent: kayobe-overcloud-upgrade-base
     nodeset: kayobe-centos8s
+    voting: false
 
 - job:
     name: kayobe-seed-base
     parent: kayobe-base
     description: |
       Base job for testing seed deployment.
 
@@ -145,16 +146,14 @@
     run: playbooks/kayobe-seed-base/run.yml
     timeout: 5400
 
 - job:
     name: kayobe-seed-centos8s
     parent: kayobe-seed-base
     nodeset: kayobe-centos8s
-    vars:
-      is_centos_stream: true
 
 - job:
     name: kayobe-overcloud-host-configure-base
     parent: kayobe-overcloud-base
     description: |
       Base job for testing overcloud host configure.
 
@@ -183,14 +182,15 @@
     # previous release which takes a considerable amount of time.
     attempts: 3
 
 - job:
     name: kayobe-seed-upgrade-centos8s
     parent: kayobe-seed-upgrade-base
     nodeset: kayobe-centos8s
+    voting: false
 
 - job:
     name: kayobe-seed-vm-base
     parent: kayobe-base
     description: |
       Base job for testing seed VM provisioning.
```

### Comparing `kayobe-9.3.0/zuul.d/project.yaml` & `kayobe-9.4.0/zuul.d/project.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -22,11 +22,9 @@
       jobs:
         - kayobe-tox-ansible-syntax
         - kayobe-tox-ansible
         - kayobe-tox-molecule
         - kayobe-overcloud-centos8s
         - kayobe-overcloud-tls-centos8s
         - kayobe-overcloud-host-configure-centos8s
-        - kayobe-overcloud-upgrade-centos8s
         - kayobe-seed-centos8s
-        - kayobe-seed-upgrade-centos8s
         - kayobe-seed-vm-centos8s
```

