# Comparing `tmp/kolla-9.3.1.tar.gz` & `tmp/kolla-9.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kolla-9.3.1.tar", last modified: Mon Feb  1 17:17:07 2021, max compression
+gzip compressed data, was "dist/kolla-9.4.0.tar", last modified: Sat Jun 19 09:38:10 2021, max compression
```

## Comparing `kolla-9.3.1.tar` & `kolla-9.4.0.tar`

### file list

```diff
@@ -1,1326 +1,1330 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.734882 kolla-9.3.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-02-01 17:16:32.000000 kolla-9.3.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2021-02-01 17:16:32.000000 kolla-9.3.1/.yamllint
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.566877 kolla-9.3.1/.zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2663 2021-02-01 17:16:32.000000 kolla-9.3.1/.zuul.d/base.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4085 2021-02-01 17:16:32.000000 kolla-9.3.1/.zuul.d/centos.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2021-02-01 17:16:32.000000 kolla-9.3.1/.zuul.d/debian.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2021-02-01 17:16:32.000000 kolla-9.3.1/.zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2020 2021-02-01 17:16:32.000000 kolla-9.3.1/.zuul.d/ubuntu.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20427 2021-02-01 17:17:07.000000 kolla-9.3.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   204609 2021-02-01 17:17:06.000000 kolla-9.3.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-02-01 17:16:32.000000 kolla-9.3.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-02-01 17:16:32.000000 kolla-9.3.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12764 2021-02-01 17:17:07.734882 kolla-9.3.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10172 2021-02-01 17:16:32.000000 kolla-9.3.1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2021-02-01 17:16:32.000000 kolla-9.3.1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.518876 kolla-9.3.1/contrib/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.566877 kolla-9.3.1/contrib/template-override/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2021-02-01 17:16:32.000000 kolla-9.3.1/contrib/template-override/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2021-02-01 17:16:32.000000 kolla-9.3.1/contrib/template-override/opendaylight-template-overrides.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2021-02-01 17:16:32.000000 kolla-9.3.1/contrib/template-override/ovs-dpdk.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2021-02-01 17:16:32.000000 kolla-9.3.1/deliverables.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.566877 kolla-9.3.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.566877 kolla-9.3.1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.566877 kolla-9.3.1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17082 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/admin/image-building.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7231 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/admin/kolla_api.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.566877 kolla-9.3.1/doc/source/admin/template-override/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/admin/template-override/opendaylight-source.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/admin/template-override/ovs-dpdk.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/ceph_versions.csv
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3158 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4118 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/contributor/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/contributor/bug-triage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3320 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/contributor/ptl-guide.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6452 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/contributor/release-management.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2834 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/contributor/running-tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1886 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/matrix_aarch64.csv
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/matrix_x86.csv
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2192 2021-02-01 17:16:32.000000 kolla-9.3.1/doc/source/support_matrix.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.522876 kolla-9.3.1/docker/almanach/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/almanach/almanach-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/almanach/almanach-api/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/almanach/almanach-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/almanach/almanach-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/almanach/almanach-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/almanach/almanach-collector/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/almanach/almanach-collector/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.522876 kolla-9.3.1/docker/aodh/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/aodh/aodh-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/aodh/aodh-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/aodh/aodh-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/aodh/aodh-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/aodh/aodh-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/aodh/aodh-base/aodh_sudoers
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      382 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/aodh/aodh-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/aodh/aodh-evaluator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/aodh/aodh-evaluator/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/aodh/aodh-expirer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/aodh/aodh-expirer/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/aodh/aodh-listener/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/aodh/aodh-listener/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/aodh/aodh-notifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/aodh/aodh-notifier/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.522876 kolla-9.3.1/docker/barbican/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.570877 kolla-9.3.1/docker/barbican/barbican-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1671 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/barbican/barbican-api/Dockerfile.j2
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      276 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/barbican/barbican-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.574877 kolla-9.3.1/docker/barbican/barbican-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/barbican/barbican-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/barbican/barbican-base/barbican_sudoers
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      367 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/barbican/barbican-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.574877 kolla-9.3.1/docker/barbican/barbican-keystone-listener/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/barbican/barbican-keystone-listener/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.574877 kolla-9.3.1/docker/barbican/barbican-worker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/barbican/barbican-worker/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.578877 kolla-9.3.1/docker/base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21561 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/apt_preferences
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      984 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/apt_preferences.debian
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/apt_preferences.ubuntu
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/ceph_master.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      991 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/copy_cacerts.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/crmsh.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/curlrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/dnf.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/dpkg_reducing_disk_footprint
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/elasticsearch.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/grafana.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/httpd_setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/influxdb.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/kolla_bashrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/opendaylight.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/rabbitmq_rabbitmq-erlang.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/rabbitmq_rabbitmq-server.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14631 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/set_configs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/sources.list
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/sources.list.debian
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1366 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/sources.list.ubuntu
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/sources.list.ubuntu.aarch64
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/sources.list.ubuntu.ppc64le
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/sudoers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/td.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/base/yum.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.522876 kolla-9.3.1/docker/bifrost/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.578877 kolla-9.3.1/docker/bifrost/bifrost-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2228 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/bifrost/bifrost-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/bifrost/bifrost-base/bifrost_sudoers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/bifrost/bifrost-base/build_arg.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.578877 kolla-9.3.1/docker/bifrost/bifrost-deploy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/bifrost/bifrost-deploy/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.522876 kolla-9.3.1/docker/blazar/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.578877 kolla-9.3.1/docker/blazar/blazar-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/blazar/blazar-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/blazar/blazar-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.578877 kolla-9.3.1/docker/blazar/blazar-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/blazar/blazar-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/blazar/blazar-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.578877 kolla-9.3.1/docker/blazar/blazar-manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/blazar/blazar-manager/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.522876 kolla-9.3.1/docker/ceilometer/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceilometer/ceilometer-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2717 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceilometer/ceilometer-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceilometer/ceilometer-base/ceilometer_sudoers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceilometer/ceilometer-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceilometer/ceilometer-central/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceilometer/ceilometer-central/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceilometer/ceilometer-compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1804 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceilometer/ceilometer-compute/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceilometer/ceilometer-ipmi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceilometer/ceilometer-ipmi/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceilometer/ceilometer-notification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceilometer/ceilometer-notification/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceilometer/ceilometer-notification/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.522876 kolla-9.3.1/docker/ceph/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceph/ceph-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1355 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceph/ceph-mds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-mds/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceph/ceph-mgr/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-mgr/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceph/ceph-mon/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-mon/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2257 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-mon/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2344 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-mon/fetch_ceph_keys.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceph/ceph-nfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-nfs/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceph/ceph-osd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-osd/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9140 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-osd/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceph/ceph-rgw/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/ceph-rgw/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/ceph/cephfs-fuse/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ceph/cephfs-fuse/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/certmonger/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/certmonger/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.582877 kolla-9.3.1/docker/chrony/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/chrony/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/chrony/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.526876 kolla-9.3.1/docker/cinder/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/cinder/cinder-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2939 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cinder/cinder-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cinder/cinder-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/cinder/cinder-backup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cinder/cinder-backup/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/cinder/cinder-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3253 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cinder/cinder-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cinder/cinder-base/cinder_sudoers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cinder/cinder-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/cinder/cinder-scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cinder/cinder-scheduler/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/cinder/cinder-volume/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cinder/cinder-volume/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cinder/cinder-volume/cinder_sudoers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cinder/cinder-volume/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.526876 kolla-9.3.1/docker/cloudkitty/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/cloudkitty/cloudkitty-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2304 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cloudkitty/cloudkitty-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cloudkitty/cloudkitty-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/cloudkitty/cloudkitty-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cloudkitty/cloudkitty-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cloudkitty/cloudkitty-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/cloudkitty/cloudkitty-processor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cloudkitty/cloudkitty-processor/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/collectd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/collectd/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/collectd/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.526876 kolla-9.3.1/docker/congress/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/congress/congress-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/congress/congress-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/congress/congress-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/congress/congress-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1382 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/congress/congress-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/congress/congress-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/congress/congress-datasource/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/congress/congress-datasource/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.586877 kolla-9.3.1/docker/congress/congress-policy-engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/congress/congress-policy-engine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/cron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cron/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.526876 kolla-9.3.1/docker/cyborg/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/cyborg/cyborg-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1823 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cyborg/cyborg-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/cyborg/cyborg-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cyborg/cyborg-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cyborg/cyborg-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/cyborg/cyborg-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cyborg/cyborg-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cyborg/cyborg-base/cyborg_sudoers
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      406 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cyborg/cyborg-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/cyborg/cyborg-conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/cyborg/cyborg-conductor/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.526876 kolla-9.3.1/docker/designate/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/designate/designate-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-api/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/designate/designate-backend-bind9/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-backend-bind9/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/designate/designate-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2330 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-base/designate_sudoers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/designate/designate-central/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-central/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-central/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/designate/designate-mdns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-mdns/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/designate/designate-producer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-producer/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/designate/designate-sink/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-sink/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/designate/designate-worker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1158 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/designate/designate-worker/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.590878 kolla-9.3.1/docker/dind/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/dind/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/dind/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/dnsmasq/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/dnsmasq/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.526876 kolla-9.3.1/docker/dragonflow/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/dragonflow/dragonflow-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1439 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/dragonflow/dragonflow-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/dragonflow/dragonflow-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/dragonflow/dragonflow-controller/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/dragonflow/dragonflow-controller/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/dragonflow/dragonflow-metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/dragonflow/dragonflow-metadata/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/dragonflow/dragonflow-publisher-service/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/dragonflow/dragonflow-publisher-service/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/ec2-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1246 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ec2-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ec2-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.530876 kolla-9.3.1/docker/elasticsearch/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/elasticsearch/elasticsearch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/elasticsearch/elasticsearch/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/elasticsearch/elasticsearch/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/elasticsearch/elasticsearch-curator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/elasticsearch/elasticsearch-curator/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/elasticsearch/elasticsearch-curator/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/elasticsearch6/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/elasticsearch6/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/elasticsearch6/elasticsearch.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/elasticsearch6/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/etcd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/etcd/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/etcd/etcd_sudoers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/etcd/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.594878 kolla-9.3.1/docker/fluentd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3875 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/fluentd/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/fluentd/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/fluentd/fluentd_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.530876 kolla-9.3.1/docker/freezer/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/freezer/freezer-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/freezer/freezer-api/Dockerfile.j2
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      274 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/freezer/freezer-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/freezer/freezer-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1439 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/freezer/freezer-base/Dockerfile.j2
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      362 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/freezer/freezer-base/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/freezer/freezer-base/freezer_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/freezer/freezer-scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/freezer/freezer-scheduler/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.530876 kolla-9.3.1/docker/glance/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/glance/glance-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/glance/glance-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/glance/glance-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/glance/glance-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2540 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/glance/glance-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/glance/glance-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/glance/glance-registry/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/glance/glance-registry/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.530876 kolla-9.3.1/docker/gnocchi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/gnocchi/gnocchi-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/gnocchi/gnocchi-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/gnocchi/gnocchi-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/gnocchi/gnocchi-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4535 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/gnocchi/gnocchi-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/gnocchi/gnocchi-base/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/gnocchi/gnocchi-base/gnocchi_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/gnocchi/gnocchi-metricd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/gnocchi/gnocchi-metricd/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/gnocchi/gnocchi-statsd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/gnocchi/gnocchi-statsd/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.598878 kolla-9.3.1/docker/grafana/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/grafana/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/grafana/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/grafana/grafana_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.530876 kolla-9.3.1/docker/hacluster/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/hacluster/hacluster-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/hacluster/hacluster-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/hacluster/hacluster-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/hacluster/hacluster-corosync/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/hacluster/hacluster-corosync/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/hacluster/hacluster-pacemaker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/hacluster/hacluster-pacemaker/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/hacluster/hacluster-pacemaker-remote/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/hacluster/hacluster-pacemaker-remote/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/hacluster/hacluster-pcs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/hacluster/hacluster-pcs/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/haproxy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/haproxy/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/haproxy/ensure_latest_config.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.530876 kolla-9.3.1/docker/heat/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/heat/heat-all/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/heat/heat-all/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/heat/heat-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/heat/heat-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      701 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/heat/heat-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/heat/heat-api-cfn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/heat/heat-api-cfn/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/heat/heat-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/heat/heat-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/heat/heat-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/heat/heat-engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/heat/heat-engine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/helm-repository/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1830 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/helm-repository/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/horizon/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7559 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/horizon/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14691 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/horizon/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.602878 kolla-9.3.1/docker/influxdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/influxdb/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/influxdb/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/influxdb/influxdb_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.534876 kolla-9.3.1/docker/ironic/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/ironic/ironic-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2053 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic/ironic-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic/ironic-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/ironic/ironic-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1614 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic/ironic-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic/ironic-base/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic/ironic-base/ironic_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/ironic/ironic-conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4972 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic/ironic-conductor/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/ironic/ironic-pxe/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic/ironic-pxe/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic/ironic-pxe/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic/ironic-pxe/tftp-map-file
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/ironic-inspector/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2304 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic-inspector/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic-inspector/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ironic-inspector/ironic_inspector_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/iscsid/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/iscsid/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/iscsid/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/kafka/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kafka/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kafka/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.534876 kolla-9.3.1/docker/karbor/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/karbor/karbor-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/karbor/karbor-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/karbor/karbor-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/karbor/karbor-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/karbor/karbor-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/karbor/karbor-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/karbor/karbor-operationengine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/karbor/karbor-operationengine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.606878 kolla-9.3.1/docker/karbor/karbor-protection/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/karbor/karbor-protection/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.610878 kolla-9.3.1/docker/keepalived/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keepalived/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keepalived/check_alive.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keepalived/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.534876 kolla-9.3.1/docker/keystone/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.610878 kolla-9.3.1/docker/keystone/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1887 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keystone/keystone/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1845 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keystone/keystone/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keystone/keystone/keystone_bootstrap.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.610878 kolla-9.3.1/docker/keystone/keystone-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4338 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keystone/keystone-base/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.610878 kolla-9.3.1/docker/keystone/keystone-fernet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keystone/keystone-fernet/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keystone/keystone-fernet/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2648 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keystone/keystone-fernet/fetch_fernet_tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1210 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keystone/keystone-fernet/keystone_bootstrap.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.610878 kolla-9.3.1/docker/keystone/keystone-ssh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keystone/keystone-ssh/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/keystone/keystone-ssh/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.610878 kolla-9.3.1/docker/kibana/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kibana/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kibana/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.610878 kolla-9.3.1/docker/kibana6/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kibana6/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kibana6/elasticsearch.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kibana6/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kolla-toolbox/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4045 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kolla-toolbox/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kolla-toolbox/ansible.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kolla-toolbox/ansible_sudoers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13335 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kolla-toolbox/find_disks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3851 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kolla-toolbox/kolla_keystone_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2935 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kolla-toolbox/kolla_keystone_user.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2161 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kolla-toolbox/kolla_sanity.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.534876 kolla-9.3.1/docker/kube/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kube/kube-apiserver/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kube/kube-apiserver/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kube/kube-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kube/kube-base/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kube/kube-controller-manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kube/kube-controller-manager/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kube/kube-discovery/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kube/kube-discovery/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kube/kube-proxy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kube/kube-proxy/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kube/kube-scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kube/kube-scheduler/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kubernetes-entrypoint/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      601 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kubernetes-entrypoint/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kubetoolbox/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kubetoolbox/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.534876 kolla-9.3.1/docker/kuryr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kuryr/kuryr-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kuryr/kuryr-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kuryr/kuryr-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/kuryr/kuryr-libnetwork/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1358 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/kuryr/kuryr-libnetwork/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/logstash/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/logstash/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/logstash/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/logstash6/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1649 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/logstash6/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/logstash6/elasticsearch.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/logstash6/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4783 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/macros.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.534876 kolla-9.3.1/docker/magnum/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.614878 kolla-9.3.1/docker/magnum/magnum-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/magnum/magnum-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/magnum/magnum-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/magnum/magnum-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/magnum/magnum-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/magnum/magnum-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/magnum/magnum-conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/magnum/magnum-conductor/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.538876 kolla-9.3.1/docker/manila/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/manila/manila-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2832 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/manila/manila-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/manila/manila-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/manila/manila-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2038 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/manila/manila-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/manila/manila-base/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/manila/manila-base/manila_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/manila/manila-data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/manila/manila-data/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/manila/manila-scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/manila/manila-scheduler/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/manila/manila-share/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1496 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/manila/manila-share/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/mariadb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mariadb/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mariadb/backup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2308 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mariadb/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mariadb/mariadb_sudoers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2010 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mariadb/security_reset.expect
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.538876 kolla-9.3.1/docker/masakari/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/masakari/masakari-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/masakari/masakari-api/Dockerfile.j2
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      273 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/masakari/masakari-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/masakari/masakari-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/masakari/masakari-base/Dockerfile.j2
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      248 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/masakari/masakari-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.618878 kolla-9.3.1/docker/masakari/masakari-engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/masakari/masakari-engine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/masakari/masakari-monitors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1754 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/masakari/masakari-monitors/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/masakari/masakari-monitors/masakari_monitors_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/memcached/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/memcached/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.538876 kolla-9.3.1/docker/mistral/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/mistral/mistral-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2390 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mistral/mistral-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mistral/mistral-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/mistral/mistral-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1724 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mistral/mistral-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mistral/mistral-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/mistral/mistral-engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mistral/mistral-engine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/mistral/mistral-event-engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mistral/mistral-event-engine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/mistral/mistral-executor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mistral/mistral-executor/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.538876 kolla-9.3.1/docker/monasca/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/monasca/monasca-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/monasca/monasca-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1217 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/monasca/monasca-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/monasca/monasca-grafana/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3178 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-grafana/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-grafana/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-grafana/grafana_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/monasca/monasca-log-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-log-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-log-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/monasca/monasca-notification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-notification/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.622879 kolla-9.3.1/docker/monasca/monasca-persister/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      874 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-persister/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/monasca/monasca-thresh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2135 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-thresh/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1485 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/monasca/monasca-thresh/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/mongodb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1094 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mongodb/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mongodb/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/mongodb/mongodb_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/multipathd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/multipathd/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.538876 kolla-9.3.1/docker/murano/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/murano/murano-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/murano/murano-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/murano/murano-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/murano/murano-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1442 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/murano/murano-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/murano/murano-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/murano/murano-engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      701 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/murano/murano-engine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.538876 kolla-9.3.1/docker/networking-baremetal/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/networking-baremetal/ironic-neutron-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1087 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/networking-baremetal/ironic-neutron-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.542876 kolla-9.3.1/docker/neutron/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/neutron/neutron-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5423 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-base/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-base/neutron_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/neutron/neutron-bgp-dragent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1147 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-bgp-dragent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/neutron/neutron-dhcp-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-dhcp-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/neutron/neutron-infoblox-ipam-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-infoblox-ipam-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/neutron/neutron-l3-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1380 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-l3-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/neutron/neutron-linuxbridge-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-linuxbridge-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/neutron/neutron-metadata-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-metadata-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/neutron/neutron-metadata-agent-ovn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1333 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-metadata-agent-ovn/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.626879 kolla-9.3.1/docker/neutron/neutron-metering-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-metering-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/neutron/neutron-openvswitch-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-openvswitch-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/neutron/neutron-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-server/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-server/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/neutron/neutron-server-opendaylight/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-server-opendaylight/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/neutron/neutron-server-ovn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-server-ovn/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/neutron/neutron-sriov-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/neutron/neutron-sriov-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.542876 kolla-9.3.1/docker/nova/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/nova/nova-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2360 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/nova/nova-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5290 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-base/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-base/nova_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/nova/nova-compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6318 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-compute/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-compute/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/nova/nova-compute-ironic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-compute-ironic/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/nova/nova-conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-conductor/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-conductor/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/nova/nova-libvirt/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-libvirt/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-libvirt/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/nova/nova-mksproxy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-mksproxy/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.630879 kolla-9.3.1/docker/nova/nova-novncproxy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-novncproxy/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/nova/nova-scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-scheduler/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/nova/nova-serialproxy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-serialproxy/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/nova/nova-spicehtml5proxy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-spicehtml5proxy/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/nova/nova-ssh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-ssh/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/nova/nova-ssh/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.542876 kolla-9.3.1/docker/novajoin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/novajoin/novajoin-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1871 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/novajoin/novajoin-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/novajoin/novajoin-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/novajoin/novajoin-notifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/novajoin/novajoin-notifier/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/novajoin/novajoin-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/novajoin/novajoin-server/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.542876 kolla-9.3.1/docker/octavia/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/octavia/octavia-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2169 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/octavia/octavia-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/octavia/octavia-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/octavia/octavia-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/octavia/octavia-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/octavia/octavia-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/octavia/octavia-health-manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/octavia/octavia-health-manager/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/octavia/octavia-housekeeping/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/octavia/octavia-housekeeping/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/octavia/octavia-worker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/octavia/octavia-worker/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/opendaylight/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1408 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/opendaylight/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/opendaylight/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/openstack-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12355 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/openstack-base/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.546876 kolla-9.3.1/docker/openvswitch/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.634879 kolla-9.3.1/docker/openvswitch/openvswitch-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/openvswitch/openvswitch-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/openvswitch/openvswitch-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/openvswitch/openvswitch-db-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/openvswitch/openvswitch-db-server/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/openvswitch/openvswitch-db-server/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/openvswitch/openvswitch-db-server/ovs_ensure_configured.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1984 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/openvswitch/openvswitch-db-server/start_ovsdb_server.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/openvswitch/openvswitch-vswitchd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/openvswitch/openvswitch-vswitchd/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/openvswitch/openvswitch-vswitchd/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.546876 kolla-9.3.1/docker/ovn/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/ovn/ovn-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovn/ovn-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovn/ovn-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/ovn/ovn-controller/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      645 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovn/ovn-controller/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/ovn/ovn-nb-db-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovn/ovn-nb-db-server/Dockerfile.j2
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      971 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovn/ovn-nb-db-server/start_nb_db_server.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/ovn/ovn-northd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovn/ovn-northd/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/ovn/ovn-sb-db-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovn/ovn-sb-db-server/Dockerfile.j2
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      972 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovn/ovn-sb-db-server/start_sb_db_server.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.546876 kolla-9.3.1/docker/ovsdpdk/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/ovsdpdk/ovsdpdk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovsdpdk/ovsdpdk/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovsdpdk/ovsdpdk/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/ovsdpdk/ovsdpdk-db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovsdpdk/ovsdpdk-db/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovsdpdk/ovsdpdk-db/extend_start.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1936 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovsdpdk/ovsdpdk-db/start_ovsdb_server.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/ovsdpdk/ovsdpdk-vswitchd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovsdpdk/ovsdpdk-vswitchd/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ovsdpdk/ovsdpdk-vswitchd/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.546876 kolla-9.3.1/docker/panko/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.638879 kolla-9.3.1/docker/panko/panko-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1148 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/panko/panko-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/panko/panko-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/panko/panko-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3037 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/panko/panko-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/panko/panko-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.546876 kolla-9.3.1/docker/placement/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/placement/placement-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2446 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/placement/placement-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      632 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/placement/placement-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/placement/placement-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2357 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/placement/placement-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/placement/placement-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.546876 kolla-9.3.1/docker/prometheus/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-alertmanager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-alertmanager/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-blackbox-exporter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-blackbox-exporter/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-cadvisor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-cadvisor/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-elasticsearch-exporter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-elasticsearch-exporter/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-haproxy-exporter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-haproxy-exporter/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-memcached-exporter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-memcached-exporter/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-mtail/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1060 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-mtail/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-mysqld-exporter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-mysqld-exporter/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-node-exporter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-node-exporter/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-openstack-exporter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-openstack-exporter/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/prometheus/prometheus-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/prometheus/prometheus-server/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.642879 kolla-9.3.1/docker/ptp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ptp/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/ptp/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/qdrouterd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/qdrouterd/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/qdrouterd/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/qdrouterd/qdrouterd_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.546876 kolla-9.3.1/docker/qinling/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/qinling/qinling-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/qinling/qinling-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/qinling/qinling-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/qinling/qinling-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/qinling/qinling-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/qinling/qinling-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/qinling/qinling-engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/qinling/qinling-engine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/rabbitmq/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2519 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rabbitmq/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rabbitmq/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1930 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rabbitmq/rabbitmq_get_gospel_node.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/rabbitmq-3.7.24/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rabbitmq-3.7.24/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rabbitmq-3.7.24/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rabbitmq-3.7.24/rabbitmq_rabbitmq-erlang.repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rabbitmq-3.7.24/rabbitmq_rabbitmq-server.repo
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/radvd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/radvd/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/rally/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rally/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rally/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.550876 kolla-9.3.1/docker/redis/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/redis/redis/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/redis/redis/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/redis/redis-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/redis/redis-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/redis/redis-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.646879 kolla-9.3.1/docker/redis/redis-sentinel/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/redis/redis-sentinel/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.550876 kolla-9.3.1/docker/rsyslog/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/rsyslog/rsyslog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rsyslog/rsyslog/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/rsyslog/rsyslog-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/rsyslog/rsyslog-base/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.550876 kolla-9.3.1/docker/sahara/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/sahara/sahara-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sahara/sahara-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sahara/sahara-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/sahara/sahara-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2737 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sahara/sahara-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sahara/sahara-base/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sahara/sahara-base/sahara_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/sahara/sahara-engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sahara/sahara-engine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.550876 kolla-9.3.1/docker/searchlight/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/searchlight/searchlight-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/searchlight/searchlight-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/searchlight/searchlight-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/searchlight/searchlight-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/searchlight/searchlight-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/searchlight/searchlight-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/searchlight/searchlight-listener/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/searchlight/searchlight-listener/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.550876 kolla-9.3.1/docker/senlin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/senlin/senlin-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/senlin/senlin-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/senlin/senlin-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/senlin/senlin-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/senlin/senlin-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/senlin/senlin-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/senlin/senlin-engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/senlin/senlin-engine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.550876 kolla-9.3.1/docker/sensu/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/sensu/sensu-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sensu/sensu-api/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/sensu/sensu-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sensu/sensu-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sensu/sensu-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.650879 kolla-9.3.1/docker/sensu/sensu-client/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2911 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sensu/sensu-client/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/sensu/sensu-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/sensu/sensu-server/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.550876 kolla-9.3.1/docker/skydive/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/skydive/skydive-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/skydive/skydive-agent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/skydive/skydive-analyzer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/skydive/skydive-analyzer/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/skydive/skydive-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/skydive/skydive-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/skydive/skydive-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.550876 kolla-9.3.1/docker/solum/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/solum/solum-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/solum/solum-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/solum/solum-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/solum/solum-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/solum/solum-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/solum/solum-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/solum/solum-conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/solum/solum-conductor/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/solum/solum-deployer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/solum/solum-deployer/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/solum/solum-worker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/solum/solum-worker/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.554877 kolla-9.3.1/docker/storm/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/storm/storm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/storm/storm/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/storm/storm-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1774 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/storm/storm-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/storm/storm-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.554877 kolla-9.3.1/docker/swift/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/swift/swift-account/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-account/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/swift/swift-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1158 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-base/rootwrap.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-base/swift-rootwrap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-base/swift_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/swift/swift-container/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-container/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.654879 kolla-9.3.1/docker/swift/swift-object/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-object/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/swift/swift-object-expirer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-object-expirer/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/swift/swift-proxy-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1616 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-proxy-server/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/swift/swift-rsyncd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-rsyncd/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/swift/swift-rsyncd/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.554877 kolla-9.3.1/docker/tacker/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/tacker/tacker-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/tacker/tacker-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/tacker/tacker-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/tacker/tacker-conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/tacker/tacker-conductor/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/tacker/tacker-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/tacker/tacker-server/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/tacker/tacker-server/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/telegraf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/telegraf/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/telegraf/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/telegraf/telegraf_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/tempest/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/tempest/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/tempest/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/tgtd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/tgtd/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/tripleoclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1554 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/tripleoclient/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/tripleoclient/create_super_user.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.554877 kolla-9.3.1/docker/trove/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/trove/trove-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      787 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/trove/trove-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/trove/trove-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.658880 kolla-9.3.1/docker/trove/trove-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/trove/trove-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/trove/trove-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/trove/trove-conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/trove/trove-conductor/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/trove/trove-guestagent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/trove/trove-guestagent/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/trove/trove-taskmanager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/trove/trove-taskmanager/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.554877 kolla-9.3.1/docker/vitrage/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/vitrage/vitrage-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/vitrage/vitrage-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/vitrage/vitrage-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/vitrage/vitrage-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2978 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/vitrage/vitrage-base/Dockerfile.j2
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      384 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/vitrage/vitrage-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/vitrage/vitrage-graph/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/vitrage/vitrage-graph/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/vitrage/vitrage-ml/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/vitrage/vitrage-ml/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/vitrage/vitrage-notifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/vitrage/vitrage-notifier/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/vitrage/vitrage-persistor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/vitrage/vitrage-persistor/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/vmtp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/vmtp/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/vmtp/vmtp_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.554877 kolla-9.3.1/docker/watcher/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/watcher/watcher-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/watcher/watcher-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/watcher/watcher-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/watcher/watcher-applier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/watcher/watcher-applier/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/watcher/watcher-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/watcher/watcher-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/watcher/watcher-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/watcher/watcher-engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/watcher/watcher-engine/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.558877 kolla-9.3.1/docker/zaqar/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/zaqar/zaqar-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3698 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zaqar/zaqar-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zaqar/zaqar-base/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.662880 kolla-9.3.1/docker/zaqar/zaqar-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zaqar/zaqar-server/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.666880 kolla-9.3.1/docker/zaqar/zaqar-wsgi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zaqar/zaqar-wsgi/Dockerfile.j2
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       48 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zaqar/zaqar-wsgi/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.666880 kolla-9.3.1/docker/zookeeper/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zookeeper/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zookeeper/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.558877 kolla-9.3.1/docker/zun/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.666880 kolla-9.3.1/docker/zun/zun-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zun/zun-api/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zun/zun-api/extend_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.666880 kolla-9.3.1/docker/zun/zun-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zun/zun-base/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zun/zun-base/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zun/zun-base/zun_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.666880 kolla-9.3.1/docker/zun/zun-compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zun/zun-compute/Dockerfile.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zun/zun-compute/extend_start.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zun/zun-compute/zun_sudoers
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.666880 kolla-9.3.1/docker/zun/zun-wsproxy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2021-02-01 17:16:32.000000 kolla-9.3.1/docker/zun/zun-wsproxy/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.558877 kolla-9.3.1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.666880 kolla-9.3.1/etc/kolla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/etc/kolla/.keep
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.666880 kolla-9.3.1/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-02-01 17:16:32.000000 kolla-9.3.1/etc/oslo-config-generator/kolla-build.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.666880 kolla-9.3.1/kolla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.670880 kolla-9.3.1/kolla/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/cmd/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1513 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/cmd/build.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.670880 kolla-9.3.1/kolla/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/common/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    43181 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/common/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2372 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.670880 kolla-9.3.1/kolla/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2565 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.670880 kolla-9.3.1/kolla/image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/image/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    59815 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/image/build.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.670880 kolla-9.3.1/kolla/template/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/template/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/template/filters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/template/methods.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.674880 kolla-9.3.1/kolla/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1583 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.674880 kolla-9.3.1/kolla/tests/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/tests/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/tests/common/test_config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.558877 kolla-9.3.1/kolla/tests/docker/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.674880 kolla-9.3.1/kolla/tests/docker/base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/tests/docker/base/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.674880 kolla-9.3.1/kolla/tests/docker/neutron-server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/tests/docker/neutron-server/Dockerfile.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.674880 kolla-9.3.1/kolla/tests/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/tests/etc/default.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29902 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/tests/test_build.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1714 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/tests/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/tests/test_methods.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2021-02-01 17:16:32.000000 kolla-9.3.1/kolla/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.670880 kolla-9.3.1/kolla.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12764 2021-02-01 17:17:07.000000 kolla-9.3.1/kolla.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41023 2021-02-01 17:17:07.000000 kolla-9.3.1/kolla.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-01 17:17:07.000000 kolla-9.3.1/kolla.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-02-01 17:17:07.000000 kolla-9.3.1/kolla.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-01 17:17:07.000000 kolla-9.3.1/kolla.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-02-01 17:17:07.000000 kolla-9.3.1/kolla.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-02-01 17:17:07.000000 kolla-9.3.1/kolla.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-02-01 17:17:07.000000 kolla-9.3.1/kolla.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1780 2021-02-01 17:16:32.000000 kolla-9.3.1/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.558877 kolla-9.3.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/Add-distro_python_version-variable-3688288558f4e586.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/Add-mod_ssl-to-images-2d2972c3cf794f65.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/Add-work-dir-command-line-option-dd83aa934d5c9e3e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/MAINTAINER-to-LABEL-344044f33ccfa161.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-aodh-a5de8a339f25c1a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-apache-storm-927c5318d91b5db3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-barbican-8f0636668001de73.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-blazar-dashboard-e201d1aeeccc0eaa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-ceilometer-a4759f21564de7eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-ceilometer-agent-ipmi-container-aa498b90c3d2f326.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-ceph-disk-init-protection-5b38ce8f1502ff69.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-ceph-nfs-b64cfba4775589a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-certmonger-0bf3a37089c5c267.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-cinder-vg-check-c70d9f79d8cfd09b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-cloudkitty-10eb09a96de60144.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-collectd-6e3387dfff75040a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-congress-877644b4b0e2ed0a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-congress-dashboard-e302d9aeecdc0eaa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-cyborg-images-cab2b3a24a071c38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-debian_arch-variable-9559ac31809afaca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-designate-c789e47f8ced394d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-designate-producer-1420e7c4744e9b09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-dragonflow-da8ff734139c9de5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-dumb-init-manage-root-process-e25a529b322d4fac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-ec2-api-e7d3e60173e8a3d8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-elasticsearch-curator-88089d04f7ccd549.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-etcd3gw-to-ubuntu-binary-1aaf4b5e1ee670ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-fernet-support-54ccb88b901d8d8b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-freezer-74c9b538348cd62a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-freezer-sceduler-b64cfba4666889a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-gnocchi-94296c3ed6e979a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-grafana-in-heka-6397498442c00670.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-hacluster-role-d10bc3918395ccdf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-header-blocks-9ac76254e5f5ab20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-heat-all-efdefb3189ec8403.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-heat-api-cloudwatch-95259c920ba7d19e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-kafka-26c9e54c934b1119.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-karbor-e6cfd97f965a4a9f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-kubernetes-images-76f5a60e98d09eb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-logstash-27da5de156efb943.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-logstash6-7418a88dc5cb88eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-manila-api-httpd-packages-and-conf-1bea1364037cd64e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-mistral-event-engine-053ebdfbd50e2e65.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-monasca-3c60b3e44d3c4267.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-monasca-grafana-868f1dd95725a030.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-monasca-thresh-f3df34dee9eee562.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-mtail-b806e87da3ae950d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-multipath-9ee29be1fcea6d94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-mysql-ceilometer-backend-9ffdc4c0495fb801.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-network-interface-checks-0e789f3f93cbdb09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-networking-ansible-b27128f544f300e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-networking-baremtal-ed44e0fc04371eb8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-networking-sfc-62ae433ed7aa4e33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-neutron-bgp-dragent-c831d5ec9a130937.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-neutron-dvr-f1b3541e22c0fbc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-neutron-ipam-driver-infoblox-0cee3c06f359c5e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-neutron-lbaas-dbb92dada9d34ceb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-neutron-server-opendaylight-bf8407e0b91059c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-neutron-server-ovn-5728bbd35b08083e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-neutron-vpnaas-88e0780326100e36.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-novajoin-9e8ae602b29335b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-octavia-dashboard-e2b1d1aeebcc0eba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-opendaylight-fee2807442ce3c6d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-openssh-clients-to-ironic-conductor-7275bd65dfe238a6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-openvswitch-ovn-2855384c9720161e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-panko-dockerfile-ff69a745aca3ec15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-ptp-service-image-3fb4eadeeeda3aa0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-py35-f0ddb519029f5ee3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-python3-systemd-for-ironic-source-9a6883496e101da9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-qdrouterd-4676f6cad921a3f8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-qinling-618886c3375eea4a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-radvd-dockerfile-64668525dae7ead8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-rally-c6d1468accfb1da6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-reno-f5e9ff4d9ccfa785.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-sahara-f2be7bf79935792e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-sensu-a763a155649e068d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-skydive-52c3fb964fe6cc1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-solum-aa448921b2b58989.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-tacker-dockerfile-3388429491d80239.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-tarballs-base-parameter-c1ddfa6de5dfd622.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-tripleo-ui-image-6a17f9a31894d908.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-tripleoclient-image-0341fb72fe27ba14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-use-dumb-init-config-option-26b47f6d97d7585c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-vmtp-7d6aef3125a38dbe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-watcher-a97995ace827cf71.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-zookeeper-2454cdfbfa7047b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add-zun-dockerfile-fb604877dc9c15fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/add_dpdk_telemetry_and_logparser-bcf9b13bcefc99c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/additional-docker-dir-7121c33da7eec160.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/allow_setting_group_in_config_files-cef8580912854741.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/almanach-images-f0a9a424ac3fe7cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/ansible-tempest-44edbca4436f3c19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/apache-image-serve-89942346ff89f767.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/base-package-type-bf53d8d63611b5ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bifrost-f080de99005ad38e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/blazar-images-c54435b3bd5b0425.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bp-support-network-ha-1a771d735a268219.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1814552-a037354969dcf7e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1859047-d41762357da8ae0b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1866017-9e31ddbfca9fd0f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1866827-5351ec43486d7f33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1868574.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1869319-aa032c1330b540dc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1884034-328afb8831779e02.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1884484-d26488c9c1f3977f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1886975-454ac12be3d8e1d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1897948-a0eb6d890eea8061.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/bug-1907213-e0cee8498d19a170.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/build-skip-parents-102a82736935f027.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/cadf-notifications-6c102c16090688d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/centos-8-950d979507939643.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/centos8-aarch64-not-part-of-release-330893c1f7d5f394.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/ceph-jewel-33caab815946cb4c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/clean_package_cache-fa08d1808a2f2b49.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/cloudkitty-docker-fb6b3d7e006a0697.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/config_files_new_options-0267e1ab804335ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/configurable-horizon-sessions-1dd22eae714a7001.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/congress-broken-cbf8ca59d90a85cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/custom-policies-5a9bb2b59d19b484.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/customise-toolbox-pip-e574c422afae0d93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/debian-buster-7bd8be7ec4ce0d13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/debian-stretch-38cadd54fc895f20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/deprecate-almanach-0ca0c9bb8522119a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/deprecate-ceilometer-api-71e5c7b01a3aad6c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/deprecate-dind-9ed17229d2c3137b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/deprecate-dragonflow-0404a4a1aa5a6644.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/deprecate-fedora-97f8f963a410eb44.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/deprecate-kubernetes-dbabf9f86c15a0ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/deprecate-neutron-sfc-agent-94445b4e140236a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/deprecate-nova-network-76e5c7b61a3add5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/deprecate-tgtd-scsi-target-utils-3ee002b832382f14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/deprecated-include-header-and-footer-71f16045920b0100.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/disable-systemd-nss-on-rhel-based-distros-5d586fcdb9a82da7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/distro-package-manager-49634f537be63036.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/do-not-load-modules-9b651e40d3479c39.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/docker-build-nopull-base-a860d046b9059cfc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/dockerfile-customizations-26981ebefe3b710b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/dpkg-reducing-disk-footprint-2a6b0056d57bd1de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/drop-xtrabackup-e58a97b617ff708c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/elasticsearch-upgrade-5.X-df217e3742b8b94a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/elk-6-573a9f2b4af4444a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/enable-nova-microversion-b445f22548b41c2a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/etcd-docker-ansible-51baaa1322a0c5a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/etcd-dockerfile-69b8bfc1df4bb2ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/fix-cinder-endpoints-urls-22746b1524accbbf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/fix-config-check-c973c462761a4fa9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/fix-keystone-bootstrap-unprintable-e01b088ef821fd18.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/fix-kolla-toolbox-venv-customisation-dc66f7bc621908a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/fix-loading-of-storm-in-centos8-containers-86b38c9166ceb0dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/fix-masakari-dashboard-policy-bb8c6c2364666401.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/fix-masakari-monitors-centos8-6b030ab9531505be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/fix-monasca-agent-stats-cc728000b6b05362.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/fix-monasca-cyborg-ubuntu-source-832a978a3ac5cd3e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/fix-skips-d5cb9546110300ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/freezer-drop-trickle-9b3eaaa7d1e4ea5a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/get_pip-macro-906a78462b216049.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/heka-deprecation-d53e757470b3f7b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/implement-glance-zero-downtime-upgrade-2825a2c76315d23d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/implement-keystone-zero-downtime-upgrade-2a082ad24b26751d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/implement-mongo-replicate-set-cluster-0d3f140f7116c3ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/import-murano-core-library-86f00abaa21cfb94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/install_sensu_from_centos_opstools-99d64edb91526fc7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/integrate-gnocchi-cloudkitty-4b2fcfe8ce9d520e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/integrate-gnocchi-with-ceph-a6d5f81f4d8b0391.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/ironic_syslinux-70eac225d227dc2e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/kibana-4-6-7765f556efba2724.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/kolla-ceph-bluestore-a30ce85948d28427.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1229 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/kolla-host-584270e3aee6dfd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/kolla_build_skip_existing-92aebdd858a0bfa5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/kubernetes-for-arm64-b149983c7e11ab60.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/kuryr-libnetwork-1e6ab1916a8a0d10.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/make_init_system_configurable-0ee16808b6e90954.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/mariadb-dumb-init-b23949398fd44021.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/masakari-a047b0387a474186.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/mistral-fix-wrong-service-type-72ff772fc7cf0b82.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/monitoring-ad566513454614db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/more-flexible-image-skipping-8e1320ed78976026.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/move-manila-share-to-network-node-57c61e757c5b96b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/multiple-physical-networks-f2de7444f7e2d145.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/network_mode-build-configuration-5e7c15b84dae9199.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/neutron-sriov-agent-4dae576ca279ef87.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/new_networking_ovn_metadata_agent_kolla_image-6f87ef59cf62cb8f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/non-x86-support-bce168d78db50202.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/nova-compute-add-ndctl-811f923d81bbd6ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/nova-plugins-f3ceab61b19d008a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/nova_compute_daxio-b8655d31df15139a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/performance-monitoring-experimental-f9ceaacd4d5cb71a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/pin-distro-version-4d835846a1ab5283.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/ppc64le_delorean_deps-cde2e1a5dc03699e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/prefer_headless_jre-005b5a6f17673e33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/prometheus-alertmanager-3dbe1b8ee3b312ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/prometheus-cadvisor-05906b0894651a29.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/prometheus-containers-1599a6417cc6a264.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/prometheus-memcached-exporter-3ca7f701a5069509.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/rabbit-3.6.2-accdb2d3ecd493cc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/rabbitmq-3.7.24-ba6f071b59000731.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/rally-manage-fix-8c98a0beb6dae50e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/redis-container-810eec9915d426d8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/redis-sentinel-container-defa09d0ac420f64.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-ceilometer-collector-image-c5d1c4b6463b2ecd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-crane-ad12c12b633d4d73.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-fedora-44af79f3e061e8d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-heat-cloudwatch-api-c71e9deafffdb3e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-include-header-footer-parameters-68a6374635a8c9b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-neutron-sfc-agent-181ec5dbc52ac1da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-neutron-vpnaas-agent-216810affb495ad0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-nova-consoleauth-caf1c027b6403dc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-nova-network-container-69f8c0b61b3aed5a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-nova-placement-75124fd8290a2634.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-oraclelinux-support-109ce54b1952ec3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-sensu-plugins-48b206bb0d278423.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-tripleo-ui-855da0b4f4c73385.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/remove-vitrage-collector-ed76366b9bb6e8e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/retire-neutron-lbaas-4441ce36928fc375.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/rhel-python3-support-1078f829dc42c4d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/rsyslog-13d5798163953322.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/sahara-split-plugins-66e31717b7c24472.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/senlin-container-e1ae6aa932097e51.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/sensu-client-image-45cb9c4573cd22fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/skip_rpm_doc_install-887dc22312c787a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/split-placement-from-nova-27b7ea2359c2d3ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/static-uid-gid-b90800f2947e656d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/stein-prelude-92e47ccd60c76325.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/support-ceilometer-in-cinder-4386a3e5d134d84f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/support-disk-size-as-weight-in-ceph-9d6353f1d3f03199.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/support-docker-image-squash-8396c0de63085f5d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/support-ipxe-chainload-273d55741a83a2a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/support-ldap-e678ce5b0a7eaedb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/support-posting-to-monasca-api-from-fluentd-1b653db78a8644e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/swift-object-expirer-fix-b837de80cea4fb8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/tacker-conductor-246d23f8c4a97de0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/tacker-networking-sfc-138b9fedd09b8728.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/tacker-rpm-binary-137dc2771bdfc5d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/templete-override-files-c7489543d92d1811.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/train-prelude-2420ae1363bd92bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/ubuntu-sources.list-change-65bb0f936b0ec95b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/ubuntu-upstream-mariadb-34ce8106811a1f75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/unbuildable-helm-repository-5e361266659b29d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/unicode-locale-018fe01eaccc556d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/unmount-ceph-osds-43b7b59685bff5b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/update-zaqar-images-95a5909b48893698.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/update_rpm_security_fixes-f99a3fa509cb5b3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/upgade-to-ubuntu-xenial-93e68d2330e9bd84.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/upgrade-ceph-luminous-415581032d25699e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/upgrade-fluentd-monasca-output-plugin-739caf0af953d533.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/upgrade-influxdb-for-monasca-202f3cf22ff8597e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/upgrade-ubuntu-base-image-to-bionic-eb0d421014ed48ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/upgrage-to-mariadb-10.3.10-for-redhat-family-93df8bf63da25659.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/use-barbican-with-httpd-d6d7599c07315e32.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/vagrant-dev-env-moved-8328674713020dda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/vitrage-containers-3bfb360357aa628b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/notes/yum_conf-36fef802e8c003f1.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8221 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/liberty.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-02-01 17:16:32.000000 kolla-9.3.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2021-02-01 17:16:32.000000 kolla-9.3.1/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.558877 kolla-9.3.1/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.558877 kolla-9.3.1/roles/collect-collectd/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/roles/collect-collectd/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4363 2021-02-01 17:16:32.000000 kolla-9.3.1/roles/collect-collectd/files/rrdtool_graph.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/roles/collect-collectd/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2021-02-01 17:16:32.000000 kolla-9.3.1/roles/collect-collectd/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/roles/collect-collectd/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2021-02-01 17:16:32.000000 kolla-9.3.1/roles/collect-collectd/templates/graph.html.j2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.562877 kolla-9.3.1/roles/collectd/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/roles/collectd/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2021-02-01 17:16:32.000000 kolla-9.3.1/roles/collectd/defaults/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/roles/collectd/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-02-01 17:16:32.000000 kolla-9.3.1/roles/collectd/handlers/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/roles/collectd/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      919 2021-02-01 17:16:32.000000 kolla-9.3.1/roles/collectd/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.722881 kolla-9.3.1/roles/collectd/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2021-02-01 17:16:32.000000 kolla-9.3.1/roles/collectd/templates/collectd.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2021-02-01 17:17:07.734882 kolla-9.3.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-02-01 17:16:32.000000 kolla-9.3.1/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.726882 kolla-9.3.1/specs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13160 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/ansible-multi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9219 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/containerize-openstack.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   274611 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/ha.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13679 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/high-availability.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3570 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/kolla-ceph-bluestore.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14263 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/kubernetes-deployment.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13601 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/logging-with-heka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    93939 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/logging-with-heka.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8063 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/mariadb-backup-recovery.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2021-02-01 17:16:32.000000 kolla-9.3.1/specs/template.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2021-02-01 17:16:32.000000 kolla-9.3.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.726882 kolla-9.3.1/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2228 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/clients.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.726882 kolla-9.3.1/tests/files/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2780 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/files/process_build_logs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.730882 kolla-9.3.1/tests/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/playbooks/post.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2200 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/playbooks/pre.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/playbooks/publish.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/playbooks/run.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.730882 kolla-9.3.1/tests/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/templates/kolla-build.conf.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4581 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/templates/template_overrides.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5102 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/test_build.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/test_keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14012 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/test_set_config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.730882 kolla-9.3.1/tests/vars/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2021-02-01 17:16:32.000000 kolla-9.3.1/tests/vars/zuul.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:17:07.734882 kolla-9.3.1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1513 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/build.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      562 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/cleanup-images
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      551 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/diag
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      423 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/dump_info.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      825 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/loc
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      855 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/pre-commit-hook
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      239 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/run-bashate.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      580 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/setup_Debian.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      497 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/setup_RedHat.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      144 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/start-registry
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      461 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/validate-all-dockerfiles.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3734 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/validate-all-file.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      216 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/validate-all-yaml.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1501 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/validate-binary-build.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      384 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/validate-docker-execute.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      502 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/validate-indentation.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      278 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/validate-install-command.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      247 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/validate-maintainer.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1170 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/validate-yaml.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7624 2021-02-01 17:16:32.000000 kolla-9.3.1/tools/version-check.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5936 2021-02-01 17:16:32.000000 kolla-9.3.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.306338 kolla-9.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-06-19 09:37:41.000000 kolla-9.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2021-06-19 09:37:41.000000 kolla-9.4.0/.yamllint
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.134338 kolla-9.4.0/.zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2631 2021-06-19 09:37:41.000000 kolla-9.4.0/.zuul.d/base.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4085 2021-06-19 09:37:41.000000 kolla-9.4.0/.zuul.d/centos.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2021-06-19 09:37:41.000000 kolla-9.4.0/.zuul.d/debian.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2021-06-19 09:37:41.000000 kolla-9.4.0/.zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2020 2021-06-19 09:37:41.000000 kolla-9.4.0/.zuul.d/ubuntu.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20457 2021-06-19 09:38:09.000000 kolla-9.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   205104 2021-06-19 09:38:09.000000 kolla-9.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-06-19 09:37:41.000000 kolla-9.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-06-19 09:37:41.000000 kolla-9.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12764 2021-06-19 09:38:10.306338 kolla-9.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10172 2021-06-19 09:37:41.000000 kolla-9.4.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2021-06-19 09:37:41.000000 kolla-9.4.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.086338 kolla-9.4.0/contrib/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.134338 kolla-9.4.0/contrib/template-override/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2021-06-19 09:37:41.000000 kolla-9.4.0/contrib/template-override/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2021-06-19 09:37:41.000000 kolla-9.4.0/contrib/template-override/opendaylight-template-overrides.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2021-06-19 09:37:41.000000 kolla-9.4.0/contrib/template-override/ovs-dpdk.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2021-06-19 09:37:41.000000 kolla-9.4.0/deliverables.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.134338 kolla-9.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.134338 kolla-9.4.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.134338 kolla-9.4.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17082 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/admin/image-building.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7231 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/admin/kolla_api.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.134338 kolla-9.4.0/doc/source/admin/template-override/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/admin/template-override/opendaylight-source.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/admin/template-override/ovs-dpdk.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/ceph_versions.csv
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3158 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4118 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/contributor/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/contributor/bug-triage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3320 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/contributor/ptl-guide.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6452 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/contributor/release-management.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2834 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/contributor/running-tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1886 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/matrix_aarch64.csv
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/matrix_x86.csv
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2192 2021-06-19 09:37:41.000000 kolla-9.4.0/doc/source/support_matrix.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.086338 kolla-9.4.0/docker/almanach/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/almanach/almanach-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/almanach/almanach-api/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/almanach/almanach-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/almanach/almanach-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/almanach/almanach-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/almanach/almanach-collector/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/almanach/almanach-collector/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.090338 kolla-9.4.0/docker/aodh/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/aodh/aodh-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/aodh/aodh-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/aodh/aodh-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/aodh/aodh-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/aodh/aodh-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/aodh/aodh-base/aodh_sudoers
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      382 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/aodh/aodh-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/aodh/aodh-evaluator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/aodh/aodh-evaluator/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/aodh/aodh-expirer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/aodh/aodh-expirer/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/aodh/aodh-listener/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/aodh/aodh-listener/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/aodh/aodh-notifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/aodh/aodh-notifier/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.090338 kolla-9.4.0/docker/barbican/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/barbican/barbican-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1671 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/barbican/barbican-api/Dockerfile.j2
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      276 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/barbican/barbican-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/barbican/barbican-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/barbican/barbican-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/barbican/barbican-base/barbican_sudoers
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      367 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/barbican/barbican-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.138338 kolla-9.4.0/docker/barbican/barbican-keystone-listener/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/barbican/barbican-keystone-listener/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.142338 kolla-9.4.0/docker/barbican/barbican-worker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/barbican/barbican-worker/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.146338 kolla-9.4.0/docker/base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21904 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/apt_preferences
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      984 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/apt_preferences.debian
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/apt_preferences.ubuntu
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/ceph_master.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      991 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/copy_cacerts.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/crmsh.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/curlrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/dnf.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/dpkg_reducing_disk_footprint
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/elasticsearch.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/grafana.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/httpd_setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/influxdb.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/kolla_bashrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/opendaylight.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/rabbitmq_rabbitmq-erlang.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/rabbitmq_rabbitmq-server.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14631 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/set_configs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/sources.list
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/sources.list.debian
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/sources.list.ubuntu
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/sources.list.ubuntu.aarch64
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/sources.list.ubuntu.ppc64le
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/sudoers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/td.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/base/yum.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.090338 kolla-9.4.0/docker/bifrost/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.146338 kolla-9.4.0/docker/bifrost/bifrost-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2228 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/bifrost/bifrost-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/bifrost/bifrost-base/bifrost_sudoers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/bifrost/bifrost-base/build_arg.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.146338 kolla-9.4.0/docker/bifrost/bifrost-deploy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/bifrost/bifrost-deploy/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.090338 kolla-9.4.0/docker/blazar/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.146338 kolla-9.4.0/docker/blazar/blazar-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/blazar/blazar-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/blazar/blazar-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.146338 kolla-9.4.0/docker/blazar/blazar-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/blazar/blazar-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/blazar/blazar-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.146338 kolla-9.4.0/docker/blazar/blazar-manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/blazar/blazar-manager/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.090338 kolla-9.4.0/docker/ceilometer/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.146338 kolla-9.4.0/docker/ceilometer/ceilometer-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2717 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceilometer/ceilometer-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceilometer/ceilometer-base/ceilometer_sudoers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceilometer/ceilometer-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.146338 kolla-9.4.0/docker/ceilometer/ceilometer-central/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceilometer/ceilometer-central/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.146338 kolla-9.4.0/docker/ceilometer/ceilometer-compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1804 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceilometer/ceilometer-compute/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.146338 kolla-9.4.0/docker/ceilometer/ceilometer-ipmi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceilometer/ceilometer-ipmi/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/ceilometer/ceilometer-notification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceilometer/ceilometer-notification/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceilometer/ceilometer-notification/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.090338 kolla-9.4.0/docker/ceph/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/ceph/ceph-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1355 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/ceph/ceph-mds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-mds/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/ceph/ceph-mgr/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-mgr/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/ceph/ceph-mon/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-mon/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2257 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-mon/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2344 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-mon/fetch_ceph_keys.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/ceph/ceph-nfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-nfs/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/ceph/ceph-osd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-osd/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9140 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-osd/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/ceph/ceph-rgw/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/ceph-rgw/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/ceph/cephfs-fuse/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ceph/cephfs-fuse/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/certmonger/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/certmonger/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/chrony/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/chrony/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/chrony/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.094338 kolla-9.4.0/docker/cinder/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/cinder/cinder-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2939 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cinder/cinder-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cinder/cinder-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.150338 kolla-9.4.0/docker/cinder/cinder-backup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cinder/cinder-backup/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/cinder/cinder-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3253 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cinder/cinder-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cinder/cinder-base/cinder_sudoers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cinder/cinder-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/cinder/cinder-scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cinder/cinder-scheduler/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/cinder/cinder-volume/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cinder/cinder-volume/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cinder/cinder-volume/cinder_sudoers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cinder/cinder-volume/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.094338 kolla-9.4.0/docker/cloudkitty/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/cloudkitty/cloudkitty-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2304 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cloudkitty/cloudkitty-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cloudkitty/cloudkitty-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/cloudkitty/cloudkitty-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cloudkitty/cloudkitty-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cloudkitty/cloudkitty-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/cloudkitty/cloudkitty-processor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cloudkitty/cloudkitty-processor/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/collectd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/collectd/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/collectd/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.094338 kolla-9.4.0/docker/congress/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/congress/congress-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/congress/congress-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/congress/congress-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/congress/congress-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1382 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/congress/congress-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/congress/congress-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/congress/congress-datasource/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/congress/congress-datasource/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/congress/congress-policy-engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/congress/congress-policy-engine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/cron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cron/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.094338 kolla-9.4.0/docker/cyborg/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/cyborg/cyborg-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1823 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cyborg/cyborg-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.154338 kolla-9.4.0/docker/cyborg/cyborg-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cyborg/cyborg-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cyborg/cyborg-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/cyborg/cyborg-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cyborg/cyborg-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cyborg/cyborg-base/cyborg_sudoers
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      406 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cyborg/cyborg-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/cyborg/cyborg-conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/cyborg/cyborg-conductor/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.094338 kolla-9.4.0/docker/designate/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/designate/designate-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-api/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/designate/designate-backend-bind9/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-backend-bind9/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/designate/designate-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2330 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-base/designate_sudoers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/designate/designate-central/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-central/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-central/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/designate/designate-mdns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-mdns/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/designate/designate-producer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-producer/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/designate/designate-sink/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-sink/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/designate/designate-worker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1158 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/designate/designate-worker/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/dind/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/dind/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/dind/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/dnsmasq/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/dnsmasq/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.094338 kolla-9.4.0/docker/dragonflow/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/dragonflow/dragonflow-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1439 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/dragonflow/dragonflow-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/dragonflow/dragonflow-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/dragonflow/dragonflow-controller/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/dragonflow/dragonflow-controller/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/dragonflow/dragonflow-metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/dragonflow/dragonflow-metadata/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.158338 kolla-9.4.0/docker/dragonflow/dragonflow-publisher-service/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/dragonflow/dragonflow-publisher-service/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.162338 kolla-9.4.0/docker/ec2-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1246 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ec2-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ec2-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.098338 kolla-9.4.0/docker/elasticsearch/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.162338 kolla-9.4.0/docker/elasticsearch/elasticsearch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/elasticsearch/elasticsearch/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/elasticsearch/elasticsearch/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.162338 kolla-9.4.0/docker/elasticsearch/elasticsearch-curator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/elasticsearch/elasticsearch-curator/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/elasticsearch/elasticsearch-curator/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.162338 kolla-9.4.0/docker/elasticsearch6/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/elasticsearch6/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/elasticsearch6/elasticsearch.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/elasticsearch6/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.162338 kolla-9.4.0/docker/etcd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/etcd/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/etcd/etcd_sudoers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/etcd/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.162338 kolla-9.4.0/docker/fluentd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3875 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/fluentd/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/fluentd/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/fluentd/fluentd_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.098338 kolla-9.4.0/docker/freezer/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.162338 kolla-9.4.0/docker/freezer/freezer-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/freezer/freezer-api/Dockerfile.j2
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      274 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/freezer/freezer-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.162338 kolla-9.4.0/docker/freezer/freezer-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1439 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/freezer/freezer-base/Dockerfile.j2
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      362 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/freezer/freezer-base/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/freezer/freezer-base/freezer_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.162338 kolla-9.4.0/docker/freezer/freezer-scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/freezer/freezer-scheduler/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.098338 kolla-9.4.0/docker/glance/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/glance/glance-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/glance/glance-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/glance/glance-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/glance/glance-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2540 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/glance/glance-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/glance/glance-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/glance/glance-registry/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/glance/glance-registry/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.098338 kolla-9.4.0/docker/gnocchi/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/gnocchi/gnocchi-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/gnocchi/gnocchi-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/gnocchi/gnocchi-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/gnocchi/gnocchi-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4535 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/gnocchi/gnocchi-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/gnocchi/gnocchi-base/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/gnocchi/gnocchi-base/gnocchi_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/gnocchi/gnocchi-metricd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/gnocchi/gnocchi-metricd/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/gnocchi/gnocchi-statsd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/gnocchi/gnocchi-statsd/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/grafana/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/grafana/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/grafana/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/grafana/grafana_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.098338 kolla-9.4.0/docker/hacluster/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/hacluster/hacluster-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/hacluster/hacluster-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/hacluster/hacluster-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/hacluster/hacluster-corosync/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/hacluster/hacluster-corosync/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/hacluster/hacluster-pacemaker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/hacluster/hacluster-pacemaker/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/hacluster/hacluster-pacemaker-remote/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/hacluster/hacluster-pacemaker-remote/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/hacluster/hacluster-pcs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/hacluster/hacluster-pcs/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.166338 kolla-9.4.0/docker/haproxy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/haproxy/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/haproxy/ensure_latest_config.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.098338 kolla-9.4.0/docker/heat/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/heat/heat-all/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/heat/heat-all/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/heat/heat-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/heat/heat-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      701 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/heat/heat-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/heat/heat-api-cfn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/heat/heat-api-cfn/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/heat/heat-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/heat/heat-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/heat/heat-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/heat/heat-engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/heat/heat-engine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/helm-repository/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1830 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/helm-repository/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/horizon/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7559 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/horizon/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14691 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/horizon/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/influxdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/influxdb/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/influxdb/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/influxdb/influxdb_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.102338 kolla-9.4.0/docker/ironic/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/ironic/ironic-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2053 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic/ironic-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic/ironic-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/ironic/ironic-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1614 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic/ironic-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic/ironic-base/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic/ironic-base/ironic_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/ironic/ironic-conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4972 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic/ironic-conductor/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.174338 kolla-9.4.0/docker/ironic/ironic-pxe/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic/ironic-pxe/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic/ironic-pxe/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic/ironic-pxe/tftp-map-file
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.170338 kolla-9.4.0/docker/ironic-inspector/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2304 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic-inspector/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic-inspector/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ironic-inspector/ironic_inspector_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.174338 kolla-9.4.0/docker/iscsid/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/iscsid/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/iscsid/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.174338 kolla-9.4.0/docker/kafka/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kafka/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kafka/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.102338 kolla-9.4.0/docker/karbor/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.174338 kolla-9.4.0/docker/karbor/karbor-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/karbor/karbor-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/karbor/karbor-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.174338 kolla-9.4.0/docker/karbor/karbor-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/karbor/karbor-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/karbor/karbor-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.174338 kolla-9.4.0/docker/karbor/karbor-operationengine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/karbor/karbor-operationengine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.174338 kolla-9.4.0/docker/karbor/karbor-protection/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/karbor/karbor-protection/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.174338 kolla-9.4.0/docker/keepalived/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keepalived/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keepalived/check_alive.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keepalived/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.102338 kolla-9.4.0/docker/keystone/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.174338 kolla-9.4.0/docker/keystone/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1887 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keystone/keystone/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1845 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keystone/keystone/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keystone/keystone/keystone_bootstrap.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.174338 kolla-9.4.0/docker/keystone/keystone-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4338 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keystone/keystone-base/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/keystone/keystone-fernet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keystone/keystone-fernet/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keystone/keystone-fernet/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2648 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keystone/keystone-fernet/fetch_fernet_tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1210 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keystone/keystone-fernet/keystone_bootstrap.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/keystone/keystone-ssh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keystone/keystone-ssh/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/keystone/keystone-ssh/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/kibana/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kibana/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kibana/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/kibana6/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kibana6/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kibana6/elasticsearch.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kibana6/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/kolla-toolbox/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4072 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kolla-toolbox/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kolla-toolbox/ansible.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kolla-toolbox/ansible_sudoers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13335 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kolla-toolbox/find_disks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3851 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kolla-toolbox/kolla_keystone_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2935 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kolla-toolbox/kolla_keystone_user.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2161 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kolla-toolbox/kolla_sanity.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.102338 kolla-9.4.0/docker/kube/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/kube/kube-apiserver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kube/kube-apiserver/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/kube/kube-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kube/kube-base/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/kube/kube-controller-manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kube/kube-controller-manager/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/kube/kube-discovery/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kube/kube-discovery/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/kube/kube-proxy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kube/kube-proxy/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.178338 kolla-9.4.0/docker/kube/kube-scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kube/kube-scheduler/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/kubernetes-entrypoint/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      601 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kubernetes-entrypoint/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/kubetoolbox/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kubetoolbox/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.102338 kolla-9.4.0/docker/kuryr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/kuryr/kuryr-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kuryr/kuryr-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kuryr/kuryr-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/kuryr/kuryr-libnetwork/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1358 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/kuryr/kuryr-libnetwork/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/logstash/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/logstash/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/logstash/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/logstash6/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1649 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/logstash6/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/logstash6/elasticsearch.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/logstash6/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4783 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/macros.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.102338 kolla-9.4.0/docker/magnum/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/magnum/magnum-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/magnum/magnum-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/magnum/magnum-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/magnum/magnum-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/magnum/magnum-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/magnum/magnum-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/magnum/magnum-conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/magnum/magnum-conductor/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.106338 kolla-9.4.0/docker/manila/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/manila/manila-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2832 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/manila/manila-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/manila/manila-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/manila/manila-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2038 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/manila/manila-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/manila/manila-base/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/manila/manila-base/manila_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.182338 kolla-9.4.0/docker/manila/manila-data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/manila/manila-data/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/manila/manila-scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/manila/manila-scheduler/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/manila/manila-share/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1496 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/manila/manila-share/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/mariadb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mariadb/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mariadb/backup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2308 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mariadb/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mariadb/mariadb_sudoers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2010 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mariadb/security_reset.expect
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.106338 kolla-9.4.0/docker/masakari/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/masakari/masakari-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/masakari/masakari-api/Dockerfile.j2
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      273 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/masakari/masakari-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/masakari/masakari-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/masakari/masakari-base/Dockerfile.j2
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      248 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/masakari/masakari-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/masakari/masakari-engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/masakari/masakari-engine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/masakari/masakari-monitors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1754 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/masakari/masakari-monitors/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/masakari/masakari-monitors/masakari_monitors_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/memcached/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/memcached/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.106338 kolla-9.4.0/docker/mistral/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/mistral/mistral-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2390 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mistral/mistral-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mistral/mistral-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/mistral/mistral-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1703 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mistral/mistral-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mistral/mistral-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/mistral/mistral-engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mistral/mistral-engine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/mistral/mistral-event-engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mistral/mistral-event-engine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/mistral/mistral-executor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mistral/mistral-executor/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.106338 kolla-9.4.0/docker/monasca/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.186338 kolla-9.4.0/docker/monasca/monasca-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/monasca/monasca-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1217 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/monasca/monasca-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/monasca/monasca-grafana/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3178 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-grafana/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-grafana/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-grafana/grafana_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/monasca/monasca-log-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-log-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-log-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/monasca/monasca-notification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-notification/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/monasca/monasca-persister/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      874 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-persister/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/monasca/monasca-thresh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2135 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-thresh/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1485 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/monasca/monasca-thresh/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/mongodb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1094 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mongodb/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mongodb/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/mongodb/mongodb_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/multipathd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/multipathd/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.106338 kolla-9.4.0/docker/murano/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/murano/murano-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/murano/murano-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/murano/murano-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/murano/murano-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1442 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/murano/murano-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/murano/murano-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.190338 kolla-9.4.0/docker/murano/murano-engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      701 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/murano/murano-engine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.106338 kolla-9.4.0/docker/networking-baremetal/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/networking-baremetal/ironic-neutron-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1087 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/networking-baremetal/ironic-neutron-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.110338 kolla-9.4.0/docker/neutron/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5423 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-base/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-base/neutron_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-bgp-dragent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1147 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-bgp-dragent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-dhcp-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-dhcp-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-infoblox-ipam-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-infoblox-ipam-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-l3-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1380 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-l3-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-linuxbridge-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-linuxbridge-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-metadata-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-metadata-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-metadata-agent-ovn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1333 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-metadata-agent-ovn/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-metering-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-metering-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-openvswitch-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-openvswitch-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-server/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-server/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-server-opendaylight/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-server-opendaylight/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-server-ovn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-server-ovn/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/neutron/neutron-sriov-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/neutron/neutron-sriov-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.110338 kolla-9.4.0/docker/nova/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.194338 kolla-9.4.0/docker/nova/nova-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2360 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5290 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-base/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-base/nova_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6318 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-compute/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-compute/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-compute-ironic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-compute-ironic/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-conductor/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-conductor/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-libvirt/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-libvirt/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-libvirt/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-mksproxy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-mksproxy/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-novncproxy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-novncproxy/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-scheduler/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-serialproxy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-serialproxy/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-spicehtml5proxy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-spicehtml5proxy/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/nova/nova-ssh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-ssh/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/nova/nova-ssh/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.110338 kolla-9.4.0/docker/novajoin/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/novajoin/novajoin-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1871 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/novajoin/novajoin-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/novajoin/novajoin-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/novajoin/novajoin-notifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/novajoin/novajoin-notifier/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.198338 kolla-9.4.0/docker/novajoin/novajoin-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/novajoin/novajoin-server/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.110338 kolla-9.4.0/docker/octavia/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/octavia/octavia-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2169 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/octavia/octavia-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/octavia/octavia-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/octavia/octavia-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/octavia/octavia-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/octavia/octavia-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/octavia/octavia-health-manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/octavia/octavia-health-manager/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/octavia/octavia-housekeeping/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/octavia/octavia-housekeeping/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/octavia/octavia-worker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/octavia/octavia-worker/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/opendaylight/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1408 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/opendaylight/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/opendaylight/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/openstack-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12355 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/openstack-base/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.114338 kolla-9.4.0/docker/openvswitch/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/openvswitch/openvswitch-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/openvswitch/openvswitch-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/openvswitch/openvswitch-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/openvswitch/openvswitch-db-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/openvswitch/openvswitch-db-server/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/openvswitch/openvswitch-db-server/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/openvswitch/openvswitch-db-server/ovs_ensure_configured.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1984 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/openvswitch/openvswitch-db-server/start_ovsdb_server.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/openvswitch/openvswitch-vswitchd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/openvswitch/openvswitch-vswitchd/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/openvswitch/openvswitch-vswitchd/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.114338 kolla-9.4.0/docker/ovn/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/ovn/ovn-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovn/ovn-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovn/ovn-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.202338 kolla-9.4.0/docker/ovn/ovn-controller/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      645 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovn/ovn-controller/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.206338 kolla-9.4.0/docker/ovn/ovn-nb-db-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovn/ovn-nb-db-server/Dockerfile.j2
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      971 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovn/ovn-nb-db-server/start_nb_db_server.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.206338 kolla-9.4.0/docker/ovn/ovn-northd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovn/ovn-northd/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.206338 kolla-9.4.0/docker/ovn/ovn-sb-db-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovn/ovn-sb-db-server/Dockerfile.j2
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      972 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovn/ovn-sb-db-server/start_sb_db_server.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.114338 kolla-9.4.0/docker/ovsdpdk/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.206338 kolla-9.4.0/docker/ovsdpdk/ovsdpdk/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovsdpdk/ovsdpdk/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovsdpdk/ovsdpdk/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.206338 kolla-9.4.0/docker/ovsdpdk/ovsdpdk-db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovsdpdk/ovsdpdk-db/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovsdpdk/ovsdpdk-db/extend_start.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1936 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovsdpdk/ovsdpdk-db/start_ovsdb_server.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.206338 kolla-9.4.0/docker/ovsdpdk/ovsdpdk-vswitchd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovsdpdk/ovsdpdk-vswitchd/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ovsdpdk/ovsdpdk-vswitchd/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.114338 kolla-9.4.0/docker/panko/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.206338 kolla-9.4.0/docker/panko/panko-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1148 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/panko/panko-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/panko/panko-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.206338 kolla-9.4.0/docker/panko/panko-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3037 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/panko/panko-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/panko/panko-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.114338 kolla-9.4.0/docker/placement/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.206338 kolla-9.4.0/docker/placement/placement-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2446 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/placement/placement-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      632 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/placement/placement-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.206338 kolla-9.4.0/docker/placement/placement-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2357 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/placement/placement-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/placement/placement-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.114338 kolla-9.4.0/docker/prometheus/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-alertmanager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-alertmanager/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-blackbox-exporter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-blackbox-exporter/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-cadvisor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-cadvisor/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-elasticsearch-exporter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-elasticsearch-exporter/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-haproxy-exporter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-haproxy-exporter/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-memcached-exporter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-memcached-exporter/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-mtail/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1060 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-mtail/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-mysqld-exporter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-mysqld-exporter/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-node-exporter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-node-exporter/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-openstack-exporter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-openstack-exporter/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/prometheus/prometheus-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/prometheus/prometheus-server/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/ptp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ptp/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/ptp/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/qdrouterd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/qdrouterd/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/qdrouterd/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/qdrouterd/qdrouterd_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.114338 kolla-9.4.0/docker/qinling/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/qinling/qinling-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/qinling/qinling-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/qinling/qinling-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.210338 kolla-9.4.0/docker/qinling/qinling-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/qinling/qinling-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/qinling/qinling-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/qinling/qinling-engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/qinling/qinling-engine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/rabbitmq/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rabbitmq/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rabbitmq/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1930 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rabbitmq/rabbitmq_get_gospel_node.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/rabbitmq-3.7.24/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rabbitmq-3.7.24/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rabbitmq-3.7.24/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rabbitmq-3.7.24/rabbitmq_rabbitmq-erlang.repo
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rabbitmq-3.7.24/rabbitmq_rabbitmq-server.repo
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/radvd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/radvd/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/rally/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rally/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rally/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.118338 kolla-9.4.0/docker/redis/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/redis/redis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/redis/redis/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/redis/redis-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/redis/redis-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/redis/redis-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/redis/redis-sentinel/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/redis/redis-sentinel/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.118338 kolla-9.4.0/docker/rsyslog/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/rsyslog/rsyslog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rsyslog/rsyslog/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/rsyslog/rsyslog-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/rsyslog/rsyslog-base/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.118338 kolla-9.4.0/docker/sahara/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.214338 kolla-9.4.0/docker/sahara/sahara-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sahara/sahara-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sahara/sahara-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/sahara/sahara-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2737 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sahara/sahara-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sahara/sahara-base/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sahara/sahara-base/sahara_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/sahara/sahara-engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sahara/sahara-engine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.118338 kolla-9.4.0/docker/searchlight/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/searchlight/searchlight-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/searchlight/searchlight-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/searchlight/searchlight-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/searchlight/searchlight-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/searchlight/searchlight-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/searchlight/searchlight-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/searchlight/searchlight-listener/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/searchlight/searchlight-listener/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.118338 kolla-9.4.0/docker/senlin/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/senlin/senlin-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/senlin/senlin-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/senlin/senlin-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/senlin/senlin-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/senlin/senlin-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/senlin/senlin-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/senlin/senlin-engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/senlin/senlin-engine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.118338 kolla-9.4.0/docker/sensu/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/sensu/sensu-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sensu/sensu-api/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/sensu/sensu-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sensu/sensu-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sensu/sensu-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/sensu/sensu-client/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2911 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sensu/sensu-client/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/sensu/sensu-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/sensu/sensu-server/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.118338 kolla-9.4.0/docker/skydive/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/skydive/skydive-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/skydive/skydive-agent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/skydive/skydive-analyzer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/skydive/skydive-analyzer/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.218338 kolla-9.4.0/docker/skydive/skydive-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/skydive/skydive-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/skydive/skydive-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.118338 kolla-9.4.0/docker/solum/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/solum/solum-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/solum/solum-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/solum/solum-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/solum/solum-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/solum/solum-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/solum/solum-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/solum/solum-conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/solum/solum-conductor/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/solum/solum-deployer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/solum/solum-deployer/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/solum/solum-worker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/solum/solum-worker/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.118338 kolla-9.4.0/docker/storm/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/storm/storm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/storm/storm/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/storm/storm-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1774 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/storm/storm-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/storm/storm-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.122338 kolla-9.4.0/docker/swift/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/swift/swift-account/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-account/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/swift/swift-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1158 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-base/rootwrap.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-base/swift-rootwrap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-base/swift_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/swift/swift-container/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-container/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/swift/swift-object/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-object/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/swift/swift-object-expirer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-object-expirer/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/swift/swift-proxy-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1616 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-proxy-server/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.222338 kolla-9.4.0/docker/swift/swift-rsyncd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-rsyncd/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/swift/swift-rsyncd/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.122338 kolla-9.4.0/docker/tacker/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/tacker/tacker-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/tacker/tacker-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/tacker/tacker-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/tacker/tacker-conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/tacker/tacker-conductor/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/tacker/tacker-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/tacker/tacker-server/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/tacker/tacker-server/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/telegraf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/telegraf/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/telegraf/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/telegraf/telegraf_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/tempest/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/tempest/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/tempest/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/tgtd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/tgtd/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/tripleoclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1554 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/tripleoclient/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/tripleoclient/create_super_user.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.122338 kolla-9.4.0/docker/trove/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/trove/trove-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      787 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/trove/trove-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/trove/trove-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/trove/trove-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/trove/trove-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/trove/trove-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/trove/trove-conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/trove/trove-conductor/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/trove/trove-guestagent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/trove/trove-guestagent/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/trove/trove-taskmanager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/trove/trove-taskmanager/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.122338 kolla-9.4.0/docker/vitrage/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.226338 kolla-9.4.0/docker/vitrage/vitrage-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/vitrage/vitrage-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/vitrage/vitrage-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/vitrage/vitrage-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2978 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/vitrage/vitrage-base/Dockerfile.j2
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      384 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/vitrage/vitrage-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/vitrage/vitrage-graph/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/vitrage/vitrage-graph/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/vitrage/vitrage-ml/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/vitrage/vitrage-ml/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/vitrage/vitrage-notifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/vitrage/vitrage-notifier/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/vitrage/vitrage-persistor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/vitrage/vitrage-persistor/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/vmtp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/vmtp/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/vmtp/vmtp_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.122338 kolla-9.4.0/docker/watcher/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/watcher/watcher-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/watcher/watcher-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/watcher/watcher-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/watcher/watcher-applier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/watcher/watcher-applier/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/watcher/watcher-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/watcher/watcher-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/watcher/watcher-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/watcher/watcher-engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/watcher/watcher-engine/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.122338 kolla-9.4.0/docker/zaqar/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/zaqar/zaqar-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3698 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zaqar/zaqar-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zaqar/zaqar-base/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/zaqar/zaqar-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zaqar/zaqar-server/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/zaqar/zaqar-wsgi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zaqar/zaqar-wsgi/Dockerfile.j2
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       48 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zaqar/zaqar-wsgi/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/zookeeper/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zookeeper/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zookeeper/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.126338 kolla-9.4.0/docker/zun/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.230338 kolla-9.4.0/docker/zun/zun-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zun/zun-api/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zun/zun-api/extend_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.234338 kolla-9.4.0/docker/zun/zun-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zun/zun-base/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zun/zun-base/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zun/zun-base/zun_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.234338 kolla-9.4.0/docker/zun/zun-compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zun/zun-compute/Dockerfile.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zun/zun-compute/extend_start.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zun/zun-compute/zun_sudoers
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.234338 kolla-9.4.0/docker/zun/zun-wsproxy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2021-06-19 09:37:41.000000 kolla-9.4.0/docker/zun/zun-wsproxy/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.126338 kolla-9.4.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.234338 kolla-9.4.0/etc/kolla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/etc/kolla/.keep
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.234338 kolla-9.4.0/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-06-19 09:37:41.000000 kolla-9.4.0/etc/oslo-config-generator/kolla-build.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.234338 kolla-9.4.0/kolla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.238338 kolla-9.4.0/kolla/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/cmd/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1513 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/cmd/build.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.238338 kolla-9.4.0/kolla/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/common/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    43181 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/common/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2372 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.238338 kolla-9.4.0/kolla/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2565 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/hacking/checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.238338 kolla-9.4.0/kolla/image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/image/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    59863 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/image/build.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.238338 kolla-9.4.0/kolla/template/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/template/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/template/filters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/template/methods.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.238338 kolla-9.4.0/kolla/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1583 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.238338 kolla-9.4.0/kolla/tests/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/tests/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/tests/common/test_config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.126338 kolla-9.4.0/kolla/tests/docker/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.238338 kolla-9.4.0/kolla/tests/docker/base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/tests/docker/base/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.242338 kolla-9.4.0/kolla/tests/docker/neutron-server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/tests/docker/neutron-server/Dockerfile.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.242338 kolla-9.4.0/kolla/tests/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/tests/etc/default.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29902 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/tests/test_build.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1714 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/tests/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/tests/test_methods.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2021-06-19 09:37:41.000000 kolla-9.4.0/kolla/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.238338 kolla-9.4.0/kolla.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12764 2021-06-19 09:38:09.000000 kolla-9.4.0/kolla.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41295 2021-06-19 09:38:10.000000 kolla-9.4.0/kolla.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-06-19 09:38:09.000000 kolla-9.4.0/kolla.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-06-19 09:38:09.000000 kolla-9.4.0/kolla.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-06-19 09:38:09.000000 kolla-9.4.0/kolla.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-06-19 09:38:09.000000 kolla-9.4.0/kolla.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-06-19 09:38:09.000000 kolla-9.4.0/kolla.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-06-19 09:38:09.000000 kolla-9.4.0/kolla.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.126338 kolla-9.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.294339 kolla-9.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/Add-distro_python_version-variable-3688288558f4e586.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/Add-mod_ssl-to-images-2d2972c3cf794f65.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/Add-work-dir-command-line-option-dd83aa934d5c9e3e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/MAINTAINER-to-LABEL-344044f33ccfa161.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-aodh-a5de8a339f25c1a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-apache-storm-927c5318d91b5db3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-barbican-8f0636668001de73.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-blazar-dashboard-e201d1aeeccc0eaa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-ceilometer-a4759f21564de7eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-ceilometer-agent-ipmi-container-aa498b90c3d2f326.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-ceph-disk-init-protection-5b38ce8f1502ff69.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-ceph-nfs-b64cfba4775589a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-certmonger-0bf3a37089c5c267.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-cinder-vg-check-c70d9f79d8cfd09b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-cloudkitty-10eb09a96de60144.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-collectd-6e3387dfff75040a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-congress-877644b4b0e2ed0a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-congress-dashboard-e302d9aeecdc0eaa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-cyborg-images-cab2b3a24a071c38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-debian_arch-variable-9559ac31809afaca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-designate-c789e47f8ced394d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-designate-producer-1420e7c4744e9b09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-dragonflow-da8ff734139c9de5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-dumb-init-manage-root-process-e25a529b322d4fac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-ec2-api-e7d3e60173e8a3d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-elasticsearch-curator-88089d04f7ccd549.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-etcd3gw-to-ubuntu-binary-1aaf4b5e1ee670ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-fernet-support-54ccb88b901d8d8b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-freezer-74c9b538348cd62a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-freezer-sceduler-b64cfba4666889a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-gnocchi-94296c3ed6e979a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-grafana-in-heka-6397498442c00670.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-hacluster-role-d10bc3918395ccdf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-header-blocks-9ac76254e5f5ab20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-heat-all-efdefb3189ec8403.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-heat-api-cloudwatch-95259c920ba7d19e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-kafka-26c9e54c934b1119.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-karbor-e6cfd97f965a4a9f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-kubernetes-images-76f5a60e98d09eb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-logstash-27da5de156efb943.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-logstash6-7418a88dc5cb88eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-manila-api-httpd-packages-and-conf-1bea1364037cd64e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-mistral-event-engine-053ebdfbd50e2e65.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-monasca-3c60b3e44d3c4267.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-monasca-grafana-868f1dd95725a030.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-monasca-thresh-f3df34dee9eee562.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-mtail-b806e87da3ae950d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-multipath-9ee29be1fcea6d94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-mysql-ceilometer-backend-9ffdc4c0495fb801.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-network-interface-checks-0e789f3f93cbdb09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-networking-ansible-b27128f544f300e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-networking-baremtal-ed44e0fc04371eb8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-networking-sfc-62ae433ed7aa4e33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-neutron-bgp-dragent-c831d5ec9a130937.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-neutron-dvr-f1b3541e22c0fbc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-neutron-ipam-driver-infoblox-0cee3c06f359c5e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-neutron-lbaas-dbb92dada9d34ceb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-neutron-server-opendaylight-bf8407e0b91059c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-neutron-server-ovn-5728bbd35b08083e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-neutron-vpnaas-88e0780326100e36.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-novajoin-9e8ae602b29335b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-octavia-dashboard-e2b1d1aeebcc0eba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-opendaylight-fee2807442ce3c6d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-openssh-clients-to-ironic-conductor-7275bd65dfe238a6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-openvswitch-ovn-2855384c9720161e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-panko-dockerfile-ff69a745aca3ec15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-ptp-service-image-3fb4eadeeeda3aa0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-py35-f0ddb519029f5ee3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-python3-systemd-for-ironic-source-9a6883496e101da9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-qdrouterd-4676f6cad921a3f8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-qinling-618886c3375eea4a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-radvd-dockerfile-64668525dae7ead8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-rally-c6d1468accfb1da6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-reno-f5e9ff4d9ccfa785.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-sahara-f2be7bf79935792e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-sensu-a763a155649e068d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-skydive-52c3fb964fe6cc1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-solum-aa448921b2b58989.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-tacker-dockerfile-3388429491d80239.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-tarballs-base-parameter-c1ddfa6de5dfd622.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-tripleo-ui-image-6a17f9a31894d908.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-tripleoclient-image-0341fb72fe27ba14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-use-dumb-init-config-option-26b47f6d97d7585c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-vmtp-7d6aef3125a38dbe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-watcher-a97995ace827cf71.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-zookeeper-2454cdfbfa7047b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add-zun-dockerfile-fb604877dc9c15fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/add_dpdk_telemetry_and_logparser-bcf9b13bcefc99c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/additional-docker-dir-7121c33da7eec160.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/allow_setting_group_in_config_files-cef8580912854741.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/almanach-images-f0a9a424ac3fe7cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/ansible-tempest-44edbca4436f3c19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/apache-image-serve-89942346ff89f767.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/base-package-type-bf53d8d63611b5ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bifrost-f080de99005ad38e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/blazar-images-c54435b3bd5b0425.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bp-support-network-ha-1a771d735a268219.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1814552-a037354969dcf7e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1859047-d41762357da8ae0b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1866017-9e31ddbfca9fd0f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1866827-5351ec43486d7f33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1868574.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1869319-aa032c1330b540dc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1884034-328afb8831779e02.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1884484-d26488c9c1f3977f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1886975-454ac12be3d8e1d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1897948-a0eb6d890eea8061.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1907213-e0cee8498d19a170.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1930544-a8926990f3a578a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/bug-1931544-5a091735efb6d6dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/build-skip-parents-102a82736935f027.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/cadf-notifications-6c102c16090688d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/centos-8-950d979507939643.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/centos8-aarch64-not-part-of-release-330893c1f7d5f394.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/ceph-jewel-33caab815946cb4c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/clean_package_cache-fa08d1808a2f2b49.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/cloudkitty-docker-fb6b3d7e006a0697.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/config_files_new_options-0267e1ab804335ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/configurable-horizon-sessions-1dd22eae714a7001.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/congress-broken-cbf8ca59d90a85cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/custom-policies-5a9bb2b59d19b484.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/customise-toolbox-pip-e574c422afae0d93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/debian-buster-7bd8be7ec4ce0d13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/debian-stretch-38cadd54fc895f20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/deprecate-almanach-0ca0c9bb8522119a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/deprecate-ceilometer-api-71e5c7b01a3aad6c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/deprecate-dind-9ed17229d2c3137b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/deprecate-dragonflow-0404a4a1aa5a6644.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/deprecate-fedora-97f8f963a410eb44.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/deprecate-kubernetes-dbabf9f86c15a0ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/deprecate-neutron-sfc-agent-94445b4e140236a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/deprecate-nova-network-76e5c7b61a3add5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/deprecate-tgtd-scsi-target-utils-3ee002b832382f14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/deprecated-include-header-and-footer-71f16045920b0100.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/disable-systemd-nss-on-rhel-based-distros-5d586fcdb9a82da7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/distro-package-manager-49634f537be63036.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/do-not-load-modules-9b651e40d3479c39.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/docker-build-nopull-base-a860d046b9059cfc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/dockerfile-customizations-26981ebefe3b710b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/dpkg-reducing-disk-footprint-2a6b0056d57bd1de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/drop-xtrabackup-e58a97b617ff708c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/elasticsearch-upgrade-5.X-df217e3742b8b94a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/elk-6-573a9f2b4af4444a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/enable-nova-microversion-b445f22548b41c2a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/etcd-docker-ansible-51baaa1322a0c5a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/etcd-dockerfile-69b8bfc1df4bb2ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/fix-cinder-endpoints-urls-22746b1524accbbf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/fix-config-check-c973c462761a4fa9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/fix-keystone-bootstrap-unprintable-e01b088ef821fd18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/fix-kolla-toolbox-venv-customisation-dc66f7bc621908a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/fix-loading-of-storm-in-centos8-containers-86b38c9166ceb0dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/fix-masakari-dashboard-policy-bb8c6c2364666401.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/fix-masakari-monitors-centos8-6b030ab9531505be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/fix-monasca-agent-stats-cc728000b6b05362.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/fix-monasca-cyborg-ubuntu-source-832a978a3ac5cd3e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/fix-skips-d5cb9546110300ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/freezer-drop-trickle-9b3eaaa7d1e4ea5a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/get_pip-macro-906a78462b216049.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/heka-deprecation-d53e757470b3f7b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/implement-glance-zero-downtime-upgrade-2825a2c76315d23d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/implement-keystone-zero-downtime-upgrade-2a082ad24b26751d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/implement-mongo-replicate-set-cluster-0d3f140f7116c3ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/import-murano-core-library-86f00abaa21cfb94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/install_sensu_from_centos_opstools-99d64edb91526fc7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/integrate-gnocchi-cloudkitty-4b2fcfe8ce9d520e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/integrate-gnocchi-with-ceph-a6d5f81f4d8b0391.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/ironic_syslinux-70eac225d227dc2e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/kibana-4-6-7765f556efba2724.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/kolla-ceph-bluestore-a30ce85948d28427.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1229 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/kolla-host-584270e3aee6dfd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/kolla_build_skip_existing-92aebdd858a0bfa5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/kubernetes-for-arm64-b149983c7e11ab60.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/kuryr-libnetwork-1e6ab1916a8a0d10.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/make_init_system_configurable-0ee16808b6e90954.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/mariadb-dumb-init-b23949398fd44021.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/masakari-a047b0387a474186.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/mistral-fix-wrong-service-type-72ff772fc7cf0b82.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/mistral-respect-uc-77aea99b5c6506ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/monitoring-ad566513454614db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/more-flexible-image-skipping-8e1320ed78976026.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/move-manila-share-to-network-node-57c61e757c5b96b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/multiple-physical-networks-f2de7444f7e2d145.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/network_mode-build-configuration-5e7c15b84dae9199.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/neutron-sriov-agent-4dae576ca279ef87.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/new_networking_ovn_metadata_agent_kolla_image-6f87ef59cf62cb8f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/non-x86-support-bce168d78db50202.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/nova-compute-add-ndctl-811f923d81bbd6ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/nova-plugins-f3ceab61b19d008a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/nova_compute_daxio-b8655d31df15139a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/performance-monitoring-experimental-f9ceaacd4d5cb71a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/pin-distro-version-4d835846a1ab5283.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/ppc64le_delorean_deps-cde2e1a5dc03699e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/prefer_headless_jre-005b5a6f17673e33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/prometheus-alertmanager-3dbe1b8ee3b312ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/prometheus-cadvisor-05906b0894651a29.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/prometheus-containers-1599a6417cc6a264.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/prometheus-memcached-exporter-3ca7f701a5069509.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/rabbit-3.6.2-accdb2d3ecd493cc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/rabbitmq-3.7.24-ba6f071b59000731.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/rabbitmq-packagecloud-c009ff6d0d2bd02d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/rally-manage-fix-8c98a0beb6dae50e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/redis-container-810eec9915d426d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/redis-sentinel-container-defa09d0ac420f64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-ceilometer-collector-image-c5d1c4b6463b2ecd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-crane-ad12c12b633d4d73.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-fedora-44af79f3e061e8d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-heat-cloudwatch-api-c71e9deafffdb3e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-include-header-footer-parameters-68a6374635a8c9b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-neutron-sfc-agent-181ec5dbc52ac1da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-neutron-vpnaas-agent-216810affb495ad0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-nova-consoleauth-caf1c027b6403dc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-nova-network-container-69f8c0b61b3aed5a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-nova-placement-75124fd8290a2634.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-oraclelinux-support-109ce54b1952ec3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-sensu-plugins-48b206bb0d278423.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-tripleo-ui-855da0b4f4c73385.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/remove-vitrage-collector-ed76366b9bb6e8e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/retire-neutron-lbaas-4441ce36928fc375.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/rhel-python3-support-1078f829dc42c4d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       43 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/rsyslog-13d5798163953322.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/sahara-split-plugins-66e31717b7c24472.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/senlin-container-e1ae6aa932097e51.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/sensu-client-image-45cb9c4573cd22fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/skip_rpm_doc_install-887dc22312c787a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/split-placement-from-nova-27b7ea2359c2d3ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/static-uid-gid-b90800f2947e656d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/stein-prelude-92e47ccd60c76325.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/support-ceilometer-in-cinder-4386a3e5d134d84f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/support-disk-size-as-weight-in-ceph-9d6353f1d3f03199.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/support-docker-image-squash-8396c0de63085f5d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/support-ipxe-chainload-273d55741a83a2a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/support-ldap-e678ce5b0a7eaedb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/support-posting-to-monasca-api-from-fluentd-1b653db78a8644e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/swift-object-expirer-fix-b837de80cea4fb8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/tacker-conductor-246d23f8c4a97de0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/tacker-networking-sfc-138b9fedd09b8728.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/tacker-rpm-binary-137dc2771bdfc5d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/templete-override-files-c7489543d92d1811.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/train-prelude-2420ae1363bd92bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/ubuntu-sources.list-change-65bb0f936b0ec95b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/ubuntu-upstream-mariadb-34ce8106811a1f75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/ubuntu-uses-mirrors-now-0858d579944eea48.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/unbuildable-helm-repository-5e361266659b29d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/unicode-locale-018fe01eaccc556d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/unmount-ceph-osds-43b7b59685bff5b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/update-zaqar-images-95a5909b48893698.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/update_rpm_security_fixes-f99a3fa509cb5b3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/upgade-to-ubuntu-xenial-93e68d2330e9bd84.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/upgrade-ceph-luminous-415581032d25699e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/upgrade-fluentd-monasca-output-plugin-739caf0af953d533.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/upgrade-influxdb-for-monasca-202f3cf22ff8597e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/upgrade-ubuntu-base-image-to-bionic-eb0d421014ed48ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/upgrage-to-mariadb-10.3.10-for-redhat-family-93df8bf63da25659.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/use-barbican-with-httpd-d6d7599c07315e32.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/vagrant-dev-env-moved-8328674713020dda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/vitrage-containers-3bfb360357aa628b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/notes/yum_conf-36fef802e8c003f1.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.294339 kolla-9.4.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.294339 kolla-9.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.294339 kolla-9.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8221 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/liberty.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-06-19 09:37:41.000000 kolla-9.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2021-06-19 09:37:41.000000 kolla-9.4.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.126338 kolla-9.4.0/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.126338 kolla-9.4.0/roles/collect-collectd/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.294339 kolla-9.4.0/roles/collect-collectd/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4363 2021-06-19 09:37:41.000000 kolla-9.4.0/roles/collect-collectd/files/rrdtool_graph.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.294339 kolla-9.4.0/roles/collect-collectd/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2021-06-19 09:37:41.000000 kolla-9.4.0/roles/collect-collectd/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.294339 kolla-9.4.0/roles/collect-collectd/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2021-06-19 09:37:41.000000 kolla-9.4.0/roles/collect-collectd/templates/graph.html.j2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.126338 kolla-9.4.0/roles/collectd/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.294339 kolla-9.4.0/roles/collectd/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2021-06-19 09:37:41.000000 kolla-9.4.0/roles/collectd/defaults/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.298339 kolla-9.4.0/roles/collectd/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-06-19 09:37:41.000000 kolla-9.4.0/roles/collectd/handlers/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.298339 kolla-9.4.0/roles/collectd/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      919 2021-06-19 09:37:41.000000 kolla-9.4.0/roles/collectd/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.298339 kolla-9.4.0/roles/collectd/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2021-06-19 09:37:41.000000 kolla-9.4.0/roles/collectd/templates/collectd.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2021-06-19 09:38:10.306338 kolla-9.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-06-19 09:37:41.000000 kolla-9.4.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.298339 kolla-9.4.0/specs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13160 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/ansible-multi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9219 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/containerize-openstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   274611 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/ha.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13679 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/high-availability.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3570 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/kolla-ceph-bluestore.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14263 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/kubernetes-deployment.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13601 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/logging-with-heka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    93939 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/logging-with-heka.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8063 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/mariadb-backup-recovery.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2021-06-19 09:37:41.000000 kolla-9.4.0/specs/template.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2021-06-19 09:37:41.000000 kolla-9.4.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.298339 kolla-9.4.0/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2228 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/clients.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.302338 kolla-9.4.0/tests/files/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2780 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/files/process_build_logs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.302338 kolla-9.4.0/tests/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/playbooks/post.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2200 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/playbooks/pre.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/playbooks/publish.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/playbooks/run.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.302338 kolla-9.4.0/tests/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/templates/kolla-build.conf.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4898 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/templates/template_overrides.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5102 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/test_build.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/test_keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14012 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/test_set_config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.302338 kolla-9.4.0/tests/vars/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2021-06-19 09:37:41.000000 kolla-9.4.0/tests/vars/zuul.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-06-19 09:38:10.306338 kolla-9.4.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1513 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/build.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      562 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/cleanup-images
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      551 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/diag
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      423 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/dump_info.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      825 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/loc
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      855 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/pre-commit-hook
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      239 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/run-bashate.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      580 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/setup_Debian.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      497 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/setup_RedHat.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      144 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/start-registry
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      461 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/validate-all-dockerfiles.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3734 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/validate-all-file.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      216 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/validate-all-yaml.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1501 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/validate-binary-build.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      384 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/validate-docker-execute.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      502 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/validate-indentation.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      278 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/validate-install-command.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      247 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/validate-maintainer.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1170 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/validate-yaml.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7624 2021-06-19 09:37:41.000000 kolla-9.4.0/tools/version-check.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5770 2021-06-19 09:37:41.000000 kolla-9.4.0/tox.ini
```

### Comparing `kolla-9.3.1/.zuul.d/base.yaml` & `kolla-9.4.0/.zuul.d/base.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     run: tests/playbooks/run.yml
     post-run: tests/playbooks/post.yml
     attempts: 5
     irrelevant-files:
       - ^.*\.rst$
       - ^doc/.*
       - ^etc/.*
-      - ^lower-constraints.txt$
       - ^releasenotes/.*$
       - ^specs/.*$
       - ^test-requirements.txt$
       - ^\.zuul\.d/
       - ^\..+
       - ^contrib/
       - ^LICENSE$
```

### Comparing `kolla-9.3.1/.zuul.d/centos.yaml` & `kolla-9.4.0/.zuul.d/centos.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/.zuul.d/debian.yaml` & `kolla-9.4.0/.zuul.d/debian.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/.zuul.d/ubuntu.yaml` & `kolla-9.4.0/.zuul.d/ubuntu.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/AUTHORS` & `kolla-9.4.0/AUTHORS`

 * *Files 0% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 Isaac Prior <isaac@stackhpc.com>
 Jack Heskett <Jack.Heskett@gresearch.co.uk>
 James Benson <James.o.benson@gmail.com>
 James E. Blair <jeblair@redhat.com>
 James Labocki <jameslabocki@gmail.com>
 James Labocki <jlabocki@redhat.com>
 James McCarthy <james.m.mccarthy@oracle.com>
+James Pic <jpic@yourlabs.org>
 Jan Horstmann <j.horstmann@mittwald.de>
 Jan Vondra <jan.vondra@ultimum.io>
 Jason <jasonanderson@uchicago.edu>
 Jason Brooks <jbrooks@redhat.com>
 Jason Myers <jason@jasonamyers.com>
 Javier Castillo Alcíbar <javier.castillo.alcibar@gmail.com>
 Javier Pena <jpena@redhat.com>
```

### Comparing `kolla-9.3.1/ChangeLog` & `kolla-9.4.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 CHANGES
 =======
 
+9.4.0
+-----
+
+* Fix \_get\_images\_dir when pip-installed with --user
+* Bump final OpenStack versions for Train
+* Enable Debian updates repo
+* Fix build of masakari-monitors image
+* CI: drop bashism from template overrides
+* [CI] Trust only infra mirrors and fix APT mirrors
+* rabbitmq: Move to packagecloud
+* base: configure curl before first use
+* Bump OpenStack versions for Train
+* Fix several issues (Train)
+* Drop lower-constraints
+* Fix Mistral source images to respect upper-constraints
+
 9.3.1
 -----
 
 * nova-compute: 'pmdk-tools' is x86-64 only in Ubuntu 'bionic'
 * nova-compute: provide needed deps for debian/aarch64
 * CI: revert to public package mirrors after build
 * Improve pip install process for offline deployment
```

### Comparing `kolla-9.3.1/LICENSE` & `kolla-9.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/PKG-INFO` & `kolla-9.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kolla
-Version: 9.3.1
+Version: 9.4.0
 Summary: Kolla OpenStack Deployment
 Home-page: https://docs.openstack.org/kolla/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `kolla-9.3.1/README.rst` & `kolla-9.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/contrib/template-override/ovs-dpdk.j2` & `kolla-9.4.0/contrib/template-override/ovs-dpdk.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/deliverables.yaml` & `kolla-9.4.0/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/admin/image-building.rst` & `kolla-9.4.0/doc/source/admin/image-building.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/admin/index.rst` & `kolla-9.4.0/doc/source/admin/index.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/admin/kolla_api.rst` & `kolla-9.4.0/doc/source/admin/kolla_api.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/admin/template-override/opendaylight-source.rst` & `kolla-9.4.0/doc/source/admin/template-override/opendaylight-source.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/admin/template-override/ovs-dpdk.rst` & `kolla-9.4.0/doc/source/admin/template-override/ovs-dpdk.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/conf.py` & `kolla-9.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/contributor/CONTRIBUTING.rst` & `kolla-9.4.0/doc/source/contributor/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/contributor/ptl-guide.rst` & `kolla-9.4.0/doc/source/contributor/ptl-guide.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/contributor/release-management.rst` & `kolla-9.4.0/doc/source/contributor/release-management.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/contributor/running-tests.rst` & `kolla-9.4.0/doc/source/contributor/running-tests.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/index.rst` & `kolla-9.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/matrix_aarch64.csv` & `kolla-9.4.0/doc/source/matrix_aarch64.csv`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/doc/source/matrix_x86.csv` & `kolla-9.4.0/doc/source/matrix_x86.csv`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 radvd,C,C,C,C,C,C,N,C
 rally,C,C,C,C,N,C,N,C
 redis,C,T,C,T,C,C,N,C
 rsyslog,C,C,C,C,C,C,N,C
 sahara,C,C,C,C,C,C,N,C
 searchlight,N,C,N,C,N,C,N,C
 senlin,C,C,C,C,C,C,N,C
-sensu,C,C,N,N,C,C,N,N
+sensu,C,C,N,N,N,N,N,N
 skydive,C,C,C,C,C,C,N,C
 solum,N,C,N,C,N,C,N,C
 storm,C,C,C,C,C,C,N,C
 swift,C,C,C,C,C,C,N,C
 tacker,C,T,C,T,N,C,N,C
 telegraf,C,C,C,C,C,C,N,N
 tempest,C,C,C,C,C,C,N,C
```

### Comparing `kolla-9.3.1/doc/source/support_matrix.rst` & `kolla-9.4.0/doc/source/support_matrix.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/almanach/almanach-base/Dockerfile.j2` & `kolla-9.4.0/docker/almanach/almanach-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/aodh/aodh-api/Dockerfile.j2` & `kolla-9.4.0/docker/aodh/aodh-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/aodh/aodh-base/Dockerfile.j2` & `kolla-9.4.0/docker/aodh/aodh-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/aodh/aodh-evaluator/Dockerfile.j2` & `kolla-9.4.0/docker/aodh/aodh-evaluator/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/aodh/aodh-expirer/Dockerfile.j2` & `kolla-9.4.0/docker/aodh/aodh-expirer/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/aodh/aodh-listener/Dockerfile.j2` & `kolla-9.4.0/docker/aodh/aodh-listener/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/aodh/aodh-notifier/Dockerfile.j2` & `kolla-9.4.0/docker/aodh/aodh-notifier/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/barbican/barbican-api/Dockerfile.j2` & `kolla-9.4.0/docker/barbican/barbican-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/barbican/barbican-base/Dockerfile.j2` & `kolla-9.4.0/docker/barbican/barbican-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/barbican/barbican-keystone-listener/Dockerfile.j2` & `kolla-9.4.0/docker/barbican/barbican-keystone-listener/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/barbican/barbican-worker/Dockerfile.j2` & `kolla-9.4.0/docker/barbican/barbican-worker/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/base/Dockerfile.j2` & `kolla-9.4.0/docker/base/Dockerfile.j2`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 FROM {{ base_image }}:{{ base_distro_tag }}
 LABEL maintainer="{{ maintainer }}" name="{{ image_name }}" build-date="{{ build_date }}"
 
+# We use curl in this dockerfile so let configure it before first use
+COPY curlrc /root/.curlrc
+
 {% block base_lang %}
 # NOTE(yoctozepto): use a UTF-8 (Unicode) locale like standard image installs do
 # fixes issues arising from ascii fallback usage
 ENV LANG en_US.UTF-8
 {% endblock %}
 
 {# NOTE(SamYaple): Avoid uid/gid conflicts by creating each user/group up front. #}
@@ -93,14 +96,15 @@
             'rabbitmq_rabbitmq-erlang.repo',
         ] %}
     {% endif %}
 
     {% set base_yum_repo_keys = [
         'https://packages.grafana.com/gpg.key',
         'https://repos.influxdata.com/influxdb.key',
+        'https://github.com/rabbitmq/signing-keys/releases/download/2.0/rabbitmq-release-signing-key.asc',
         'https://packages.treasuredata.com/GPG-KEY-td-agent',
     ] %}
     # FIXME(mgoddard): Not available for CentOS 8 yet.
     {% if distro_package_manager == 'yum' %}
         {% set base_yum_repo_keys = base_yum_repo_keys + [
             'https://artifacts.elastic.co/GPG-KEY-elasticsearch',
         ] %}
@@ -115,14 +119,15 @@
         {% set base_yum_repo_files = base_yum_repo_files + [
             'elasticsearch.repo',
         ] %}
     {% endif %}
 
     {% set base_yum_repo_keys = [
         'https://packages.grafana.com/gpg.key',
+        'https://github.com/rabbitmq/signing-keys/releases/download/2.0/rabbitmq-release-signing-key.asc',
     ] %}
     # FIXME(mgoddard): Not available for CentOS 8 yet.
     {% if distro_package_manager == 'yum' %}
         {% set base_yum_repo_keys = base_yum_repo_keys + [
             'https://artifacts.elastic.co/GPG-KEY-elasticsearch',
         ] %}
     {% endif %}
@@ -159,14 +164,20 @@
 RUN if [[ -e /etc/yum.repos.d/rabbitmq_rabbitmq-server.repo ]]; then \
       sed -i -e 's/\$basearch/x86_64/g' /etc/yum.repos.d/rabbitmq_rabbitmq-server.repo; \
     fi
 {% endif %}
 
 {% block base_centos_repo_overrides_post_copy %}{% endblock %}
 
+{% for key in base_yum_repo_keys | customizable('yum_repo_keys') %}
+{%- if loop.first %}RUN {% else %}    && {% endif -%}
+    rpm --import {{ key }}
+{%- if not loop.last %} \{% endif %}
+{% endfor -%}
+
 # Install what is needed for en_US.UTF-8
 {% block base_centos_distro_sync_and_languages %}
 
 {% if distro_package_manager == 'dnf' %}
 
 {% set base_centos_language_packages = [
     'langpacks-en',
@@ -178,20 +189,14 @@
 
 {% endif %}
 
 {% endblock %}
 
 {{ macros.install_packages(base_yum_url_packages | customizable("yum_url_packages")) }}
 
-{% for key in base_yum_repo_keys | customizable('yum_repo_keys') %}
-{%- if loop.first %}RUN {% else %}    && {% endif -%}
-    rpm --import {{ key }}
-{%- if not loop.last %} \{% endif %}
-{% endfor -%}
-
     {% if install_metatype in ['rdo', 'mixed'] %}
 
 {% for cmd in rpm_setup %}
 {{ cmd }}
 {% endfor %}
 
 {% block base_centos_repo_overrides_post_rpm %}{% endblock %}
@@ -439,14 +444,16 @@
 COPY sources.list.{{ base_distro }} /etc/apt/sources.list
 {% else %}
 COPY sources.list.{{ base_distro }}.{{ base_arch }} /etc/apt/sources.list
 {% endif %}
 COPY sources.list /etc/apt/sources.list.d/kolla-custom.list
 {% endblock %}
 
+{% block base_debian_after_sources_list %}{% endblock %}
+
 {% block base_ubuntu_package_apt_preferences %}
 COPY apt_preferences.{{ base_distro }} /etc/apt/preferences
 COPY apt_preferences /etc/apt/preferences.d/kolla-custom
 {% endblock %}
 
 {% set base_apt_packages = [
    'apt-utils',
@@ -562,15 +569,14 @@
 {% if distro_python_version.startswith('3') %}
 RUN sed -i -e "s+#\!/usr/bin/env python+#\!/usr/bin/env python3+g" /usr/local/bin/kolla_set_configs
 {% endif %}
 COPY start.sh /usr/local/bin/kolla_start
 COPY copy_cacerts.sh /usr/local/bin/kolla_copy_cacerts
 COPY httpd_setup.sh /usr/local/bin/kolla_httpd_setup
 COPY sudoers /etc/sudoers
-COPY curlrc /root/.curlrc
 
 {% if use_dumb_init %}
 
 {% block dumb_init_installation %}
 {% if base_arch == 'x86_64' %}
 
 RUN curl -sSL https://github.com/Yelp/dumb-init/releases/download/v1.2.2/dumb-init_1.2.2_{{debian_arch}} -o /usr/local/bin/dumb-init \
```

### Comparing `kolla-9.3.1/docker/base/apt_preferences.debian` & `kolla-9.4.0/docker/base/apt_preferences.debian`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/base/ceph_master.repo` & `kolla-9.4.0/docker/base/ceph_master.repo`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/base/copy_cacerts.sh` & `kolla-9.4.0/docker/base/copy_cacerts.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/base/httpd_setup.sh` & `kolla-9.4.0/docker/base/httpd_setup.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/base/set_configs.py` & `kolla-9.4.0/docker/base/set_configs.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/base/sources.list.debian` & `kolla-9.4.0/docker/base/sources.list.debian`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Default repos
 deb http://deb.debian.org/debian buster main
 
 # debian security updates
 deb http://security.debian.org/debian-security buster/updates main
 
+# debian updates
+deb http://deb.debian.org/debian buster-updates main
+
 # debian backports
 deb http://deb.debian.org/debian buster-backports main
 
 # elasticsearch (arch:all), logstash (arch:all), kibana (arch:amd64)
 deb [arch=amd64] https://artifacts.elastic.co/packages/5.x/apt stable main
 
 # main docker repo
```

### Comparing `kolla-9.3.1/docker/base/sources.list.ubuntu` & `kolla-9.4.0/docker/base/sources.list.ubuntu`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # For non-x86 architectures we use sources.list.ubuntu.<arch>
 
 # Default repos
-deb http://archive.ubuntu.com/ubuntu/ bionic main universe
-deb http://archive.ubuntu.com/ubuntu/ bionic-updates main universe
-deb http://archive.ubuntu.com/ubuntu/ bionic-security main universe
+deb mirror://mirrors.ubuntu.com/mirrors.txt bionic main universe
+deb mirror://mirrors.ubuntu.com/mirrors.txt bionic-updates main universe
+deb mirror://mirrors.ubuntu.com/mirrors.txt bionic-security main universe
 
 # Backports have a lower priority and must be explicitly installed to be used
 deb http://archive.ubuntu.com/ubuntu/ bionic-backports main universe
 
 # We need to add the repo for the updated packages they provide. The main ones
 # are qemu, libvirt, and openvswitch.
 deb http://ubuntu-cloud.archive.canonical.com/ubuntu bionic-updates/train main
@@ -23,17 +23,14 @@
 
 # Fluentd repo
 deb http://packages.treasuredata.com/3/ubuntu/bionic/ bionic contrib
 
 # Qdrouterd repo
 deb http://ppa.launchpad.net/qpid/released/ubuntu/ bionic main
 
-# Sensu repo
-deb https://sensu.global.ssl.fastly.net/apt bionic main
-
 # Opendaylight repo
 deb http://ppa.launchpad.net/odl-team/carbon/ubuntu xenial main
 
 # rabbitmq repo
 deb https://packagecloud.io/rabbitmq/rabbitmq-server/ubuntu/ bionic main
 
 # MariaDB repo
```

### Comparing `kolla-9.3.1/docker/base/sources.list.ubuntu.aarch64` & `kolla-9.4.0/docker/base/sources.list.ubuntu.aarch64`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/base/sources.list.ubuntu.ppc64le` & `kolla-9.4.0/docker/base/sources.list.ubuntu.ppc64le`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/base/start.sh` & `kolla-9.4.0/docker/base/start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/base/sudoers` & `kolla-9.4.0/docker/base/sudoers`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/bifrost/bifrost-base/Dockerfile.j2` & `kolla-9.4.0/docker/bifrost/bifrost-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/bifrost/bifrost-deploy/Dockerfile.j2` & `kolla-9.4.0/docker/bifrost/bifrost-deploy/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/blazar/blazar-api/Dockerfile.j2` & `kolla-9.4.0/docker/blazar/blazar-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/blazar/blazar-base/Dockerfile.j2` & `kolla-9.4.0/docker/blazar/blazar-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ceilometer/ceilometer-base/Dockerfile.j2` & `kolla-9.4.0/docker/ceilometer/ceilometer-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ceilometer/ceilometer-central/Dockerfile.j2` & `kolla-9.4.0/docker/ceilometer/ceilometer-central/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ceilometer/ceilometer-compute/Dockerfile.j2` & `kolla-9.4.0/docker/ceilometer/ceilometer-compute/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ceilometer/ceilometer-ipmi/Dockerfile.j2` & `kolla-9.4.0/docker/ceilometer/ceilometer-ipmi/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ceilometer/ceilometer-notification/Dockerfile.j2` & `kolla-9.4.0/docker/ceilometer/ceilometer-notification/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ceph/ceph-base/Dockerfile.j2` & `kolla-9.4.0/docker/ceph/ceph-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ceph/ceph-mon/extend_start.sh` & `kolla-9.4.0/docker/ceph/ceph-mon/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ceph/ceph-mon/fetch_ceph_keys.py` & `kolla-9.4.0/docker/ceph/ceph-mon/fetch_ceph_keys.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ceph/ceph-nfs/Dockerfile.j2` & `kolla-9.4.0/docker/ceph/ceph-nfs/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ceph/ceph-osd/extend_start.sh` & `kolla-9.4.0/docker/ceph/ceph-osd/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/certmonger/Dockerfile.j2` & `kolla-9.4.0/docker/certmonger/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/chrony/Dockerfile.j2` & `kolla-9.4.0/docker/chrony/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cinder/cinder-api/Dockerfile.j2` & `kolla-9.4.0/docker/cinder/cinder-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cinder/cinder-api/extend_start.sh` & `kolla-9.4.0/docker/cinder/cinder-api/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cinder/cinder-backup/Dockerfile.j2` & `kolla-9.4.0/docker/cinder/cinder-backup/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cinder/cinder-base/Dockerfile.j2` & `kolla-9.4.0/docker/cinder/cinder-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cinder/cinder-scheduler/Dockerfile.j2` & `kolla-9.4.0/docker/cinder/cinder-scheduler/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cinder/cinder-volume/Dockerfile.j2` & `kolla-9.4.0/docker/cinder/cinder-volume/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cinder/cinder-volume/cinder_sudoers` & `kolla-9.4.0/docker/cinder/cinder-volume/cinder_sudoers`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cloudkitty/cloudkitty-api/Dockerfile.j2` & `kolla-9.4.0/docker/cloudkitty/cloudkitty-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cloudkitty/cloudkitty-base/Dockerfile.j2` & `kolla-9.4.0/docker/cloudkitty/cloudkitty-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cloudkitty/cloudkitty-processor/Dockerfile.j2` & `kolla-9.4.0/docker/cloudkitty/cloudkitty-processor/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/collectd/Dockerfile.j2` & `kolla-9.4.0/docker/collectd/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/congress/congress-base/Dockerfile.j2` & `kolla-9.4.0/docker/congress/congress-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cron/Dockerfile.j2` & `kolla-9.4.0/docker/cron/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cyborg/cyborg-agent/Dockerfile.j2` & `kolla-9.4.0/docker/cyborg/cyborg-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cyborg/cyborg-api/Dockerfile.j2` & `kolla-9.4.0/docker/cyborg/cyborg-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/cyborg/cyborg-base/Dockerfile.j2` & `kolla-9.4.0/docker/cyborg/cyborg-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/designate/designate-api/Dockerfile.j2` & `kolla-9.4.0/docker/designate/designate-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/designate/designate-backend-bind9/Dockerfile.j2` & `kolla-9.4.0/docker/designate/designate-backend-bind9/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/designate/designate-base/Dockerfile.j2` & `kolla-9.4.0/docker/designate/designate-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/designate/designate-central/Dockerfile.j2` & `kolla-9.4.0/docker/designate/designate-central/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/designate/designate-mdns/Dockerfile.j2` & `kolla-9.4.0/docker/designate/designate-mdns/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/designate/designate-producer/Dockerfile.j2` & `kolla-9.4.0/docker/designate/designate-producer/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/designate/designate-sink/Dockerfile.j2` & `kolla-9.4.0/docker/designate/designate-sink/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/designate/designate-worker/Dockerfile.j2` & `kolla-9.4.0/docker/designate/designate-worker/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/dind/Dockerfile.j2` & `kolla-9.4.0/docker/dind/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/dind/start.sh` & `kolla-9.4.0/docker/dind/start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/dragonflow/dragonflow-base/Dockerfile.j2` & `kolla-9.4.0/docker/dragonflow/dragonflow-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ec2-api/Dockerfile.j2` & `kolla-9.4.0/docker/ec2-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/elasticsearch/elasticsearch/Dockerfile.j2` & `kolla-9.4.0/docker/elasticsearch/elasticsearch/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/elasticsearch/elasticsearch-curator/Dockerfile.j2` & `kolla-9.4.0/docker/elasticsearch/elasticsearch-curator/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/elasticsearch6/Dockerfile.j2` & `kolla-9.4.0/docker/elasticsearch6/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/etcd/Dockerfile.j2` & `kolla-9.4.0/docker/etcd/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/fluentd/Dockerfile.j2` & `kolla-9.4.0/docker/fluentd/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/fluentd/extend_start.sh` & `kolla-9.4.0/docker/fluentd/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/fluentd/fluentd_sudoers` & `kolla-9.4.0/docker/fluentd/fluentd_sudoers`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/freezer/freezer-api/Dockerfile.j2` & `kolla-9.4.0/docker/freezer/freezer-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/freezer/freezer-base/Dockerfile.j2` & `kolla-9.4.0/docker/freezer/freezer-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/glance/glance-api/Dockerfile.j2` & `kolla-9.4.0/docker/glance/glance-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/glance/glance-api/extend_start.sh` & `kolla-9.4.0/docker/glance/glance-api/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/glance/glance-base/Dockerfile.j2` & `kolla-9.4.0/docker/glance/glance-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/gnocchi/gnocchi-api/Dockerfile.j2` & `kolla-9.4.0/docker/gnocchi/gnocchi-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/gnocchi/gnocchi-base/Dockerfile.j2` & `kolla-9.4.0/docker/gnocchi/gnocchi-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/gnocchi/gnocchi-metricd/Dockerfile.j2` & `kolla-9.4.0/docker/gnocchi/gnocchi-metricd/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/gnocchi/gnocchi-statsd/Dockerfile.j2` & `kolla-9.4.0/docker/gnocchi/gnocchi-statsd/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/grafana/Dockerfile.j2` & `kolla-9.4.0/docker/grafana/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/haproxy/Dockerfile.j2` & `kolla-9.4.0/docker/haproxy/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/heat/heat-all/Dockerfile.j2` & `kolla-9.4.0/docker/heat/heat-all/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/heat/heat-api/Dockerfile.j2` & `kolla-9.4.0/docker/heat/heat-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/heat/heat-api/extend_start.sh` & `kolla-9.4.0/docker/heat/heat-api/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/heat/heat-api-cfn/Dockerfile.j2` & `kolla-9.4.0/docker/heat/heat-api-cfn/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/heat/heat-base/Dockerfile.j2` & `kolla-9.4.0/docker/heat/heat-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/heat/heat-engine/Dockerfile.j2` & `kolla-9.4.0/docker/heat/heat-engine/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/helm-repository/Dockerfile.j2` & `kolla-9.4.0/docker/helm-repository/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/horizon/Dockerfile.j2` & `kolla-9.4.0/docker/horizon/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/horizon/extend_start.sh` & `kolla-9.4.0/docker/horizon/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/influxdb/Dockerfile.j2` & `kolla-9.4.0/docker/influxdb/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ironic/ironic-api/Dockerfile.j2` & `kolla-9.4.0/docker/ironic/ironic-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ironic/ironic-base/Dockerfile.j2` & `kolla-9.4.0/docker/ironic/ironic-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ironic/ironic-conductor/Dockerfile.j2` & `kolla-9.4.0/docker/ironic/ironic-conductor/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ironic/ironic-pxe/Dockerfile.j2` & `kolla-9.4.0/docker/ironic/ironic-pxe/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ironic/ironic-pxe/extend_start.sh` & `kolla-9.4.0/docker/ironic/ironic-pxe/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ironic-inspector/Dockerfile.j2` & `kolla-9.4.0/docker/ironic-inspector/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/iscsid/Dockerfile.j2` & `kolla-9.4.0/docker/iscsid/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kafka/Dockerfile.j2` & `kolla-9.4.0/docker/kafka/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/karbor/karbor-api/Dockerfile.j2` & `kolla-9.4.0/docker/karbor/karbor-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/karbor/karbor-base/Dockerfile.j2` & `kolla-9.4.0/docker/karbor/karbor-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/keepalived/Dockerfile.j2` & `kolla-9.4.0/docker/keepalived/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/keystone/keystone/Dockerfile.j2` & `kolla-9.4.0/docker/keystone/keystone/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/keystone/keystone/extend_start.sh` & `kolla-9.4.0/docker/keystone/keystone/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/keystone/keystone/keystone_bootstrap.sh` & `kolla-9.4.0/docker/keystone/keystone/keystone_bootstrap.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/keystone/keystone-base/Dockerfile.j2` & `kolla-9.4.0/docker/keystone/keystone-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/keystone/keystone-fernet/Dockerfile.j2` & `kolla-9.4.0/docker/keystone/keystone-fernet/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/keystone/keystone-fernet/fetch_fernet_tokens.py` & `kolla-9.4.0/docker/keystone/keystone-fernet/fetch_fernet_tokens.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/keystone/keystone-fernet/keystone_bootstrap.sh` & `kolla-9.4.0/docker/keystone/keystone-fernet/keystone_bootstrap.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/keystone/keystone-ssh/Dockerfile.j2` & `kolla-9.4.0/docker/keystone/keystone-ssh/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kibana/Dockerfile.j2` & `kolla-9.4.0/docker/kibana/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kibana6/Dockerfile.j2` & `kolla-9.4.0/docker/kibana6/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kolla-toolbox/Dockerfile.j2` & `kolla-9.4.0/docker/kolla-toolbox/Dockerfile.j2`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         'mariadb',
         'mariadb-devel',
         'openssh-clients',
         'openssl-devel',
      ] %}
     {% if distro_package_manager == 'dnf' %}
         {% set kolla_toolbox_packages = kolla_toolbox_packages + [
+            'erlang-22.*',
             'python3-devel',
             'rabbitmq-server-3.7.*'
         ] %}
     {% else %}
         # NOTE(mandre) Remove rabbitmq-server pinning once package dependencies are met
         # https://bugs.launchpad.net/kolla/+bug/1814233
         {% set kolla_toolbox_packages = kolla_toolbox_packages + [
```

### Comparing `kolla-9.3.1/docker/kolla-toolbox/find_disks.py` & `kolla-9.4.0/docker/kolla-toolbox/find_disks.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kolla-toolbox/kolla_keystone_service.py` & `kolla-9.4.0/docker/kolla-toolbox/kolla_keystone_service.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kolla-toolbox/kolla_keystone_user.py` & `kolla-9.4.0/docker/kolla-toolbox/kolla_keystone_user.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kolla-toolbox/kolla_sanity.py` & `kolla-9.4.0/docker/kolla-toolbox/kolla_sanity.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kube/kube-apiserver/Dockerfile.j2` & `kolla-9.4.0/docker/kube/kube-apiserver/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kube/kube-controller-manager/Dockerfile.j2` & `kolla-9.4.0/docker/kube/kube-controller-manager/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kube/kube-discovery/Dockerfile.j2` & `kolla-9.4.0/docker/kube/kube-discovery/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kube/kube-proxy/Dockerfile.j2` & `kolla-9.4.0/docker/kube/kube-proxy/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kube/kube-scheduler/Dockerfile.j2` & `kolla-9.4.0/docker/kube/kube-scheduler/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kubernetes-entrypoint/Dockerfile.j2` & `kolla-9.4.0/docker/kubernetes-entrypoint/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kubetoolbox/Dockerfile.j2` & `kolla-9.4.0/docker/kubetoolbox/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kuryr/kuryr-base/Dockerfile.j2` & `kolla-9.4.0/docker/kuryr/kuryr-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/kuryr/kuryr-libnetwork/Dockerfile.j2` & `kolla-9.4.0/docker/kuryr/kuryr-libnetwork/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/logstash/Dockerfile.j2` & `kolla-9.4.0/docker/logstash/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/logstash6/Dockerfile.j2` & `kolla-9.4.0/docker/logstash6/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/macros.j2` & `kolla-9.4.0/docker/macros.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/magnum/magnum-api/Dockerfile.j2` & `kolla-9.4.0/docker/magnum/magnum-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/magnum/magnum-base/Dockerfile.j2` & `kolla-9.4.0/docker/magnum/magnum-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/magnum/magnum-conductor/Dockerfile.j2` & `kolla-9.4.0/docker/magnum/magnum-conductor/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/manila/manila-api/Dockerfile.j2` & `kolla-9.4.0/docker/manila/manila-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/manila/manila-base/Dockerfile.j2` & `kolla-9.4.0/docker/manila/manila-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/manila/manila-data/Dockerfile.j2` & `kolla-9.4.0/docker/manila/manila-data/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/manila/manila-scheduler/Dockerfile.j2` & `kolla-9.4.0/docker/manila/manila-scheduler/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/manila/manila-share/Dockerfile.j2` & `kolla-9.4.0/docker/manila/manila-share/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/mariadb/Dockerfile.j2` & `kolla-9.4.0/docker/mariadb/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/mariadb/backup.sh` & `kolla-9.4.0/docker/mariadb/backup.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/mariadb/extend_start.sh` & `kolla-9.4.0/docker/mariadb/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/mariadb/security_reset.expect` & `kolla-9.4.0/docker/mariadb/security_reset.expect`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/masakari/masakari-api/Dockerfile.j2` & `kolla-9.4.0/docker/masakari/masakari-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/masakari/masakari-base/Dockerfile.j2` & `kolla-9.4.0/docker/masakari/masakari-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/masakari/masakari-monitors/Dockerfile.j2` & `kolla-9.4.0/docker/masakari/masakari-monitors/Dockerfile.j2`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ADD masakari-monitors-archive /masakari-monitors-source
 
 {% set masakari_monitors_pip_packages = [
     '/masakari-monitors'
 ] %}
 
 RUN ln -s masakari-monitors-source/* masakari-monitors \
-    {% if distro_package_manager == 'dnf' %}&& sed -i -e 's/libvirt-python===.*/libvirt-python===5.10.0/' /requirements/upper-constraints.txt {% endif %}\
+    {% if distro_package_manager == 'dnf' %}&& sed -i -e 's/libvirt-python===.*/libvirt-python===6.10.0/' /requirements/upper-constraints.txt {% endif %}\
     && {{ macros.install_pip(masakari_monitors_pip_packages | customizable("pip_packages")) }} \
     && mkdir -p /etc/masakari-monitors \
     && chown -R masakari: /etc/masakari-monitors
 
 COPY masakari_monitors_sudoers /etc/sudoers.d/kolla_masakari_monitors_sudoers
 
 RUN chmod 750 /etc/sudoers.d \
```

### Comparing `kolla-9.3.1/docker/memcached/Dockerfile.j2` & `kolla-9.4.0/docker/memcached/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/mistral/mistral-api/Dockerfile.j2` & `kolla-9.4.0/docker/mistral/mistral-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/mistral/mistral-base/Dockerfile.j2` & `kolla-9.4.0/docker/mistral/mistral-base/Dockerfile.j2`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ] %}
 
 {% set mistral_base_plugins_pip_packages = [
     '/plugins/*'
 ] %}
 
 RUN ln -s mistral-base-source/* mistral \
-    && {{ macros.install_pip(mistral_base_pip_packages | customizable("pip_packages"), constraints = false) }} \
+    && {{ macros.install_pip(mistral_base_pip_packages | customizable("pip_packages")) }} \
     && mkdir -p /etc/mistral \
     && cp -r /mistral/etc/* /etc/mistral/ \
     && chown -R mistral: /etc/mistral \
     && if [ "$(ls /plugins)" ]; then \
         {{ macros.install_pip(mistral_base_plugins_pip_packages) }}; \
     fi
 {% endif %}
```

### Comparing `kolla-9.3.1/docker/mistral/mistral-engine/Dockerfile.j2` & `kolla-9.4.0/docker/mistral/mistral-engine/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/mistral/mistral-event-engine/Dockerfile.j2` & `kolla-9.4.0/docker/mistral/mistral-event-engine/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/mistral/mistral-executor/Dockerfile.j2` & `kolla-9.4.0/docker/mistral/mistral-executor/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-agent/Dockerfile.j2` & `kolla-9.4.0/docker/monasca/monasca-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-api/Dockerfile.j2` & `kolla-9.4.0/docker/monasca/monasca-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-api/extend_start.sh` & `kolla-9.4.0/docker/monasca/monasca-api/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-base/Dockerfile.j2` & `kolla-9.4.0/docker/monasca/monasca-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-grafana/Dockerfile.j2` & `kolla-9.4.0/docker/monasca/monasca-grafana/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-log-api/Dockerfile.j2` & `kolla-9.4.0/docker/monasca/monasca-log-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-log-api/extend_start.sh` & `kolla-9.4.0/docker/monasca/monasca-log-api/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-notification/Dockerfile.j2` & `kolla-9.4.0/docker/monasca/monasca-notification/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-persister/Dockerfile.j2` & `kolla-9.4.0/docker/monasca/monasca-persister/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-thresh/Dockerfile.j2` & `kolla-9.4.0/docker/monasca/monasca-thresh/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/monasca/monasca-thresh/extend_start.sh` & `kolla-9.4.0/docker/monasca/monasca-thresh/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/mongodb/Dockerfile.j2` & `kolla-9.4.0/docker/mongodb/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/multipathd/Dockerfile.j2` & `kolla-9.4.0/docker/multipathd/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/murano/murano-api/Dockerfile.j2` & `kolla-9.4.0/docker/murano/murano-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/murano/murano-base/Dockerfile.j2` & `kolla-9.4.0/docker/murano/murano-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/murano/murano-engine/Dockerfile.j2` & `kolla-9.4.0/docker/murano/murano-engine/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/networking-baremetal/ironic-neutron-agent/Dockerfile.j2` & `kolla-9.4.0/docker/networking-baremetal/ironic-neutron-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-base/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-base/extend_start.sh` & `kolla-9.4.0/docker/neutron/neutron-base/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-base/neutron_sudoers` & `kolla-9.4.0/docker/neutron/neutron-base/neutron_sudoers`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-bgp-dragent/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-bgp-dragent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-dhcp-agent/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-dhcp-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-infoblox-ipam-agent/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-infoblox-ipam-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-l3-agent/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-l3-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-linuxbridge-agent/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-linuxbridge-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-metadata-agent/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-metadata-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-metadata-agent-ovn/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-metadata-agent-ovn/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-metering-agent/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-metering-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-openvswitch-agent/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-openvswitch-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-server/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-server/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-server/extend_start.sh` & `kolla-9.4.0/docker/neutron/neutron-server/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-server-opendaylight/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-server-opendaylight/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-server-ovn/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-server-ovn/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/neutron/neutron-sriov-agent/Dockerfile.j2` & `kolla-9.4.0/docker/neutron/neutron-sriov-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-api/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-api/extend_start.sh` & `kolla-9.4.0/docker/nova/nova-api/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-base/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-compute/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-compute/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-compute-ironic/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-compute-ironic/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-conductor/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-conductor/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-libvirt/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-libvirt/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-libvirt/extend_start.sh` & `kolla-9.4.0/docker/nova/nova-libvirt/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-novncproxy/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-novncproxy/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-scheduler/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-scheduler/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-serialproxy/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-serialproxy/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-spicehtml5proxy/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-spicehtml5proxy/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/nova/nova-ssh/Dockerfile.j2` & `kolla-9.4.0/docker/nova/nova-ssh/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/novajoin/novajoin-base/Dockerfile.j2` & `kolla-9.4.0/docker/novajoin/novajoin-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/novajoin/novajoin-notifier/Dockerfile.j2` & `kolla-9.4.0/docker/novajoin/novajoin-notifier/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/novajoin/novajoin-server/Dockerfile.j2` & `kolla-9.4.0/docker/novajoin/novajoin-server/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/octavia/octavia-api/Dockerfile.j2` & `kolla-9.4.0/docker/octavia/octavia-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/octavia/octavia-base/Dockerfile.j2` & `kolla-9.4.0/docker/octavia/octavia-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/octavia/octavia-health-manager/Dockerfile.j2` & `kolla-9.4.0/docker/octavia/octavia-health-manager/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/octavia/octavia-housekeeping/Dockerfile.j2` & `kolla-9.4.0/docker/octavia/octavia-housekeeping/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/octavia/octavia-worker/Dockerfile.j2` & `kolla-9.4.0/docker/octavia/octavia-worker/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/opendaylight/Dockerfile.j2` & `kolla-9.4.0/docker/opendaylight/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/openstack-base/Dockerfile.j2` & `kolla-9.4.0/docker/openstack-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/openvswitch/openvswitch-base/Dockerfile.j2` & `kolla-9.4.0/docker/openvswitch/openvswitch-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/openvswitch/openvswitch-db-server/Dockerfile.j2` & `kolla-9.4.0/docker/openvswitch/openvswitch-db-server/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/openvswitch/openvswitch-db-server/start_ovsdb_server.sh` & `kolla-9.4.0/docker/openvswitch/openvswitch-db-server/start_ovsdb_server.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ovn/ovn-base/Dockerfile.j2` & `kolla-9.4.0/docker/ovn/ovn-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ovn/ovn-controller/Dockerfile.j2` & `kolla-9.4.0/docker/ovn/ovn-controller/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ovn/ovn-nb-db-server/Dockerfile.j2` & `kolla-9.4.0/docker/ovn/ovn-nb-db-server/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ovn/ovn-nb-db-server/start_nb_db_server.sh` & `kolla-9.4.0/docker/ovn/ovn-nb-db-server/start_nb_db_server.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ovn/ovn-northd/Dockerfile.j2` & `kolla-9.4.0/docker/ovn/ovn-northd/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ovn/ovn-sb-db-server/Dockerfile.j2` & `kolla-9.4.0/docker/ovn/ovn-sb-db-server/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ovn/ovn-sb-db-server/start_sb_db_server.sh` & `kolla-9.4.0/docker/ovn/ovn-sb-db-server/start_sb_db_server.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ovsdpdk/ovsdpdk/Dockerfile.j2` & `kolla-9.4.0/docker/ovsdpdk/ovsdpdk/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ovsdpdk/ovsdpdk-db/start_ovsdb_server.sh` & `kolla-9.4.0/docker/ovsdpdk/ovsdpdk-db/start_ovsdb_server.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/panko/panko-api/Dockerfile.j2` & `kolla-9.4.0/docker/panko/panko-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/panko/panko-base/Dockerfile.j2` & `kolla-9.4.0/docker/panko/panko-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/placement/placement-api/Dockerfile.j2` & `kolla-9.4.0/docker/placement/placement-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/placement/placement-api/extend_start.sh` & `kolla-9.4.0/docker/placement/placement-api/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/placement/placement-base/Dockerfile.j2` & `kolla-9.4.0/docker/placement/placement-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-alertmanager/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-alertmanager/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-blackbox-exporter/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-blackbox-exporter/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-cadvisor/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-cadvisor/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-elasticsearch-exporter/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-elasticsearch-exporter/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-haproxy-exporter/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-haproxy-exporter/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-memcached-exporter/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-memcached-exporter/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-mtail/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-mtail/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-mysqld-exporter/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-mysqld-exporter/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-node-exporter/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-node-exporter/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-openstack-exporter/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-openstack-exporter/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/prometheus/prometheus-server/Dockerfile.j2` & `kolla-9.4.0/docker/prometheus/prometheus-server/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/ptp/Dockerfile.j2` & `kolla-9.4.0/docker/ptp/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/qdrouterd/Dockerfile.j2` & `kolla-9.4.0/docker/qdrouterd/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/qinling/qinling-api/Dockerfile.j2` & `kolla-9.4.0/docker/qinling/qinling-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/qinling/qinling-base/Dockerfile.j2` & `kolla-9.4.0/docker/qinling/qinling-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/rabbitmq/Dockerfile.j2` & `kolla-9.4.0/docker/rabbitmq/Dockerfile.j2`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 {% block rabbitmq_install %}
 {% if base_package_type == 'rpm' %}
     {% set rabbitmq_packages = [
         'hostname',
     ] %}
     {% if distro_package_manager == 'dnf' %}
         {% set rabbitmq_packages = rabbitmq_packages + [
+            'erlang-22.*',
             'rabbitmq-server-3.7.*'
         ] %}
     {% else %}
         # NOTE(mandre) Remove rabbitmq-server pinning once package dependencies are met
         # https://bugs.launchpad.net/kolla/+bug/1814233
         {% set rabbitmq_packages = rabbitmq_packages + [
             'erlang-hipe',
```

### Comparing `kolla-9.3.1/docker/rabbitmq/extend_start.sh` & `kolla-9.4.0/docker/rabbitmq/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/rabbitmq/rabbitmq_get_gospel_node.py` & `kolla-9.4.0/docker/rabbitmq/rabbitmq_get_gospel_node.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/rabbitmq-3.7.24/Dockerfile.j2` & `kolla-9.4.0/docker/rabbitmq-3.7.24/Dockerfile.j2`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 {% import "macros.j2" as macros with context %}
 
 {{ macros.configure_user(name='rabbitmq') }}
 
 {% block rabbitmq_install %}
 {% if base_package_type == 'rpm' %}
     {% set rabbitmq_packages = [
+        'erlang-22.*',
         'hostname',
         'rabbitmq-server-3.7.24',
     ] %}
 {% endif %}
 
 COPY rabbitmq_rabbitmq-erlang.repo rabbitmq_rabbitmq-server.repo /etc/yum.repos.d/
 RUN rpm --import https://www.rabbitmq.com/rabbitmq-release-signing-key.asc
```

### Comparing `kolla-9.3.1/docker/rabbitmq-3.7.24/extend_start.sh` & `kolla-9.4.0/docker/rabbitmq-3.7.24/extend_start.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/rally/Dockerfile.j2` & `kolla-9.4.0/docker/rally/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/redis/redis/Dockerfile.j2` & `kolla-9.4.0/docker/redis/redis/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/redis/redis-sentinel/Dockerfile.j2` & `kolla-9.4.0/docker/redis/redis-sentinel/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/rsyslog/rsyslog/Dockerfile.j2` & `kolla-9.4.0/docker/rsyslog/rsyslog/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/sahara/sahara-api/Dockerfile.j2` & `kolla-9.4.0/docker/sahara/sahara-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/sahara/sahara-base/Dockerfile.j2` & `kolla-9.4.0/docker/sahara/sahara-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/sahara/sahara-engine/Dockerfile.j2` & `kolla-9.4.0/docker/sahara/sahara-engine/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/searchlight/searchlight-api/Dockerfile.j2` & `kolla-9.4.0/docker/searchlight/searchlight-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/searchlight/searchlight-base/Dockerfile.j2` & `kolla-9.4.0/docker/searchlight/searchlight-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/senlin/senlin-api/Dockerfile.j2` & `kolla-9.4.0/docker/senlin/senlin-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/senlin/senlin-base/Dockerfile.j2` & `kolla-9.4.0/docker/senlin/senlin-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/senlin/senlin-engine/Dockerfile.j2` & `kolla-9.4.0/docker/senlin/senlin-engine/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/sensu/sensu-base/Dockerfile.j2` & `kolla-9.4.0/docker/sensu/sensu-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/sensu/sensu-client/Dockerfile.j2` & `kolla-9.4.0/docker/sensu/sensu-client/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/sensu/sensu-server/Dockerfile.j2` & `kolla-9.4.0/docker/sensu/sensu-server/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/skydive/skydive-agent/Dockerfile.j2` & `kolla-9.4.0/docker/skydive/skydive-agent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/skydive/skydive-analyzer/Dockerfile.j2` & `kolla-9.4.0/docker/skydive/skydive-analyzer/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/skydive/skydive-base/Dockerfile.j2` & `kolla-9.4.0/docker/skydive/skydive-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/solum/solum-api/Dockerfile.j2` & `kolla-9.4.0/docker/solum/solum-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/solum/solum-base/Dockerfile.j2` & `kolla-9.4.0/docker/solum/solum-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/storm/storm-base/Dockerfile.j2` & `kolla-9.4.0/docker/storm/storm-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/swift/swift-account/Dockerfile.j2` & `kolla-9.4.0/docker/swift/swift-account/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/swift/swift-base/Dockerfile.j2` & `kolla-9.4.0/docker/swift/swift-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/swift/swift-base/rootwrap.conf` & `kolla-9.4.0/docker/swift/swift-base/rootwrap.conf`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/swift/swift-container/Dockerfile.j2` & `kolla-9.4.0/docker/swift/swift-container/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/swift/swift-object/Dockerfile.j2` & `kolla-9.4.0/docker/swift/swift-object/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/swift/swift-object-expirer/Dockerfile.j2` & `kolla-9.4.0/docker/swift/swift-object-expirer/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/swift/swift-proxy-server/Dockerfile.j2` & `kolla-9.4.0/docker/swift/swift-proxy-server/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/swift/swift-rsyncd/Dockerfile.j2` & `kolla-9.4.0/docker/swift/swift-rsyncd/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/tacker/tacker-base/Dockerfile.j2` & `kolla-9.4.0/docker/tacker/tacker-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/tacker/tacker-conductor/Dockerfile.j2` & `kolla-9.4.0/docker/tacker/tacker-conductor/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/tacker/tacker-server/Dockerfile.j2` & `kolla-9.4.0/docker/tacker/tacker-server/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/telegraf/Dockerfile.j2` & `kolla-9.4.0/docker/telegraf/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/tempest/Dockerfile.j2` & `kolla-9.4.0/docker/tempest/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/tgtd/Dockerfile.j2` & `kolla-9.4.0/docker/tgtd/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/tripleoclient/Dockerfile.j2` & `kolla-9.4.0/docker/tripleoclient/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/tripleoclient/create_super_user.sh` & `kolla-9.4.0/docker/tripleoclient/create_super_user.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/trove/trove-api/Dockerfile.j2` & `kolla-9.4.0/docker/trove/trove-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/trove/trove-base/Dockerfile.j2` & `kolla-9.4.0/docker/trove/trove-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/trove/trove-conductor/Dockerfile.j2` & `kolla-9.4.0/docker/trove/trove-conductor/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/trove/trove-guestagent/Dockerfile.j2` & `kolla-9.4.0/docker/trove/trove-guestagent/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/trove/trove-taskmanager/Dockerfile.j2` & `kolla-9.4.0/docker/trove/trove-taskmanager/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/vitrage/vitrage-api/Dockerfile.j2` & `kolla-9.4.0/docker/vitrage/vitrage-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/vitrage/vitrage-base/Dockerfile.j2` & `kolla-9.4.0/docker/vitrage/vitrage-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/vitrage/vitrage-graph/Dockerfile.j2` & `kolla-9.4.0/docker/vitrage/vitrage-graph/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/vitrage/vitrage-ml/Dockerfile.j2` & `kolla-9.4.0/docker/vitrage/vitrage-ml/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/vitrage/vitrage-notifier/Dockerfile.j2` & `kolla-9.4.0/docker/vitrage/vitrage-notifier/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/vitrage/vitrage-persistor/Dockerfile.j2` & `kolla-9.4.0/docker/vitrage/vitrage-persistor/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/vmtp/Dockerfile.j2` & `kolla-9.4.0/docker/vmtp/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/watcher/watcher-api/Dockerfile.j2` & `kolla-9.4.0/docker/watcher/watcher-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/watcher/watcher-applier/Dockerfile.j2` & `kolla-9.4.0/docker/watcher/watcher-applier/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/watcher/watcher-base/Dockerfile.j2` & `kolla-9.4.0/docker/watcher/watcher-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/watcher/watcher-engine/Dockerfile.j2` & `kolla-9.4.0/docker/watcher/watcher-engine/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/zaqar/zaqar-base/Dockerfile.j2` & `kolla-9.4.0/docker/zaqar/zaqar-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/zaqar/zaqar-server/Dockerfile.j2` & `kolla-9.4.0/docker/zaqar/zaqar-server/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/zookeeper/Dockerfile.j2` & `kolla-9.4.0/docker/zookeeper/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/zun/zun-api/Dockerfile.j2` & `kolla-9.4.0/docker/zun/zun-api/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/zun/zun-base/Dockerfile.j2` & `kolla-9.4.0/docker/zun/zun-base/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/docker/zun/zun-compute/Dockerfile.j2` & `kolla-9.4.0/docker/zun/zun-compute/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/__init__.py` & `kolla-9.4.0/kolla/__init__.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/cmd/build.py` & `kolla-9.4.0/kolla/cmd/build.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/common/config.py` & `kolla-9.4.0/kolla/common/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,51 +323,51 @@
     'bifrost-base': {
         'type': 'url',
         'location': ('$tarballs_base/bifrost/'
                      'bifrost-7.2.2.tar.gz')},
     'blazar-base': {
         'type': 'url',
         'location': ('$tarballs_base/blazar/'
-                     'blazar-4.0.0.tar.gz')},
+                     'blazar-4.0.1.tar.gz')},
     'ceilometer-base': {
         'type': 'url',
         'location': ('$tarballs_base/ceilometer/'
-                     'ceilometer-13.1.1.tar.gz')},
+                     'ceilometer-13.1.2.tar.gz')},
     'ceilometer-base-plugin-panko': {
         'type': 'url',
         'location': ('$tarballs_base/panko/'
-                     'panko-7.0.0.tar.gz')},
+                     'panko-7.1.0.tar.gz')},
     'cinder-base': {
         'type': 'url',
         'location': ('$tarballs_base/cinder/'
-                     'cinder-15.4.0.tar.gz')},
+                     'cinder-15.6.0.tar.gz')},
     'congress-base': {
         'type': 'url',
         'location': ('$tarballs_base/congress/'
                      'openstack-congress-10.0.0.tar.gz')},
     'cloudkitty-base': {
         'type': 'url',
         'location': ('$tarballs_base/cloudkitty/'
                      'cloudkitty-11.1.0.tar.gz')},
     'cyborg-base': {
         'type': 'url',
         'location': ('$tarballs_base/cyborg/'
-                     'openstack-cyborg-3.0.0.tar.gz')},
+                     'openstack-cyborg-3.0.1.tar.gz')},
     'designate-base': {
         'type': 'url',
         'location': ('$tarballs_base/designate/'
-                     'designate-9.0.1.tar.gz')},
+                     'designate-9.0.2.tar.gz')},
     'dragonflow-base': {
         'type': 'url',
         'location': ('$tarballs_base/dragonflow/'
                      'dragonflow-3.0.0.tar.gz')},
     'ec2-api': {
         'type': 'url',
         'location': ('$tarballs_base/ec2-api/'
-                     'ec2-api-9.0.0.tar.gz')},
+                     'ec2-api-9.0.1.tar.gz')},
     'freezer-api': {
         'type': 'url',
         'location': ('$tarballs_base/freezer-api/'
                      'freezer-api-7.2.0.tar.gz')},
     'freezer-base': {
         'type': 'url',
         'location': ('$tarballs_base/freezer/'
@@ -384,15 +384,15 @@
     'heat-base': {
         'type': 'url',
         'location': ('$tarballs_base/heat/'
                      'openstack-heat-13.1.0.tar.gz')},
     'horizon': {
         'type': 'url',
         'location': ('$tarballs_base/horizon/'
-                     'horizon-16.2.0.tar.gz')},
+                     'horizon-16.2.2.tar.gz')},
     'horizon-plugin-blazar-dashboard': {
         'type': 'url',
         'location': ('$tarballs_base/blazar-dashboard/'
                      'blazar-dashboard-2.0.1.tar.gz')},
     'horizon-plugin-congress-dashboard': {
         'type': 'url',
         'location': ('$tarballs_base/congress-dashboard/'
@@ -424,43 +424,43 @@
     'horizon-plugin-karbor-dashboard': {
         'type': 'url',
         'location': ('$tarballs_base/karbor-dashboard/'
                      'karbor-dashboard-1.3.0.tar.gz')},
     'horizon-plugin-magnum-ui': {
         'type': 'url',
         'location': ('$tarballs_base/magnum-ui/'
-                     'magnum-ui-5.3.0.tar.gz')},
+                     'magnum-ui-5.3.1.tar.gz')},
     'horizon-plugin-manila-ui': {
         'type': 'url',
         'location': ('$tarballs_base/manila-ui/'
                      'manila-ui-2.19.2.tar.gz')},
     'horizon-plugin-masakari-dashboard': {
         'type': 'url',
         'location': ('$tarballs_base/masakari-dashboard/'
                      'masakari-dashboard-1.0.1.tar.gz')},
     'horizon-plugin-mistral-dashboard': {
         'type': 'url',
         'location': ('$tarballs_base/mistral-dashboard/'
-                     'mistral-dashboard-9.0.0.tar.gz')},
+                     'mistral-dashboard-9.0.1.tar.gz')},
     'horizon-plugin-monasca-ui': {
         'type': 'url',
         'location': ('$tarballs_base/monasca-ui/'
-                     'monasca-ui-1.17.1.tar.gz')},
+                     'monasca-ui-1.17.2.tar.gz')},
     'horizon-plugin-murano-dashboard': {
         'type': 'url',
         'location': ('$tarballs_base/murano-dashboard/'
                      'murano-dashboard-8.0.0.tar.gz')},
     'horizon-plugin-neutron-vpnaas-dashboard': {
         'type': 'url',
         'location': ('$tarballs_base/neutron-vpnaas-dashboard/'
                      'neutron-vpnaas-dashboard-1.6.1.tar.gz')},
     'horizon-plugin-octavia-dashboard': {
         'type': 'url',
         'location': ('$tarballs_base/octavia-dashboard/'
-                     'octavia-dashboard-4.0.0.tar.gz')},
+                     'octavia-dashboard-4.0.2.tar.gz')},
     'horizon-plugin-qinling-dashboard': {
         'type': 'url',
         'location': ('$tarballs_base/qinling-dashboard/'
                      'qinling-dashboard-2.0.0.tar.gz')},
     'horizon-plugin-sahara-dashboard': {
         'type': 'url',
         'location': ('$tarballs_base/sahara-dashboard/'
@@ -500,59 +500,59 @@
     'horizon-plugin-zun-ui': {
         'type': 'url',
         'location': ('$tarballs_base/zun-ui/'
                      'zun-ui-4.0.1.tar.gz')},
     'ironic-base': {
         'type': 'url',
         'location': ('$tarballs_base/ironic/'
-                     'ironic-13.0.6.tar.gz')},
+                     'ironic-13.0.7.tar.gz')},
     'ironic-inspector': {
         'type': 'url',
         'location': ('$tarballs_base/ironic-inspector/'
-                     'ironic-inspector-9.2.3.tar.gz')},
+                     'ironic-inspector-9.2.4.tar.gz')},
     'karbor-base': {
         'type': 'url',
         'location': ('$tarballs_base/karbor/'
                      'karbor-1.4.0.tar.gz')},
     'keystone-base': {
         'type': 'url',
         'location': ('$tarballs_base/keystone/'
-                     'keystone-16.0.1.tar.gz')},
+                     'keystone-16.0.2.tar.gz')},
     'kuryr-base': {
         'type': 'url',
         'location': ('$tarballs_base/kuryr/'
                      'kuryr-lib-1.1.1.tar.gz')},
     'kuryr-libnetwork': {
         'type': 'url',
         'location': ('$tarballs_base/kuryr-libnetwork/'
-                     'kuryr-libnetwork-4.0.1.tar.gz')},
+                     'kuryr-libnetwork-4.0.2.tar.gz')},
     'magnum-base': {
         'type': 'url',
         'location': ('$tarballs_base/magnum/'
-                     'magnum-9.4.0.tar.gz')},
+                     'magnum-9.4.1.tar.gz')},
     'manila-base': {
         'type': 'url',
         'location': ('$tarballs_base/manila/'
-                     'manila-9.1.4.tar.gz')},
+                     'manila-9.1.5.tar.gz')},
     'masakari-base': {
         'type': 'url',
         'location': ('$tarballs_base/masakari/'
-                     'masakari-8.1.0.tar.gz')},
+                     'masakari-8.1.2.tar.gz')},
     'masakari-monitors': {
         'type': 'url',
         'location': ('$tarballs_base/masakari-monitors/'
                      'masakari-monitors-8.0.2.tar.gz')},
     'mistral-base': {
         'type': 'url',
         'location': ('$tarballs_base/mistral/'
                      'mistral-9.1.0.tar.gz')},
     'mistral-base-plugin-tacker': {
         'type': 'url',
         'location': ('$tarballs_base/tacker/'
-                     'tacker-2.0.1.tar.gz')},
+                     'tacker-2.0.2.tar.gz')},
     'monasca-agent': {
         'type': 'url',
         'location': ('$tarballs_base/monasca-agent/'
                      'monasca-agent-2.12.1.tar.gz')},
     'monasca-api': {
         'type': 'url',
         'location': ('$tarballs_base/monasca-api/'
@@ -581,19 +581,19 @@
     'monasca-thresh-additions-monasca-common': {
         'type': 'url',
         'location': ('$tarballs_base/monasca-common/'
                      'monasca-common-2.16.1.tar.gz')},
     'murano-base': {
         'type': 'url',
         'location': ('$tarballs_base/murano/'
-                     'murano-8.1.0.tar.gz')},
+                     'murano-8.1.1.tar.gz')},
     'neutron-base': {
         'type': 'url',
         'location': ('$tarballs_base/neutron/'
-                     'neutron-15.3.0.tar.gz')},
+                     'neutron-15.3.4.tar.gz')},
     'neutron-base-plugin-neutron-fwaas': {
         'type': 'url',
         'location': ('$tarballs_base/neutron-fwaas/'
                      'neutron-fwaas-15.0.1.tar.gz')},
     'neutron-base-plugin-networking-ansible': {
         'type': 'url',
         'location': ('$tarballs_base/networking-ansible/'
@@ -605,15 +605,15 @@
     'neutron-base-plugin-networking-generic-switch': {
         'type': 'url',
         'location': ('$tarballs_base/networking-generic-switch/'
                      'networking-generic-switch-2.1.0.tar.gz')},
     'neutron-base-plugin-networking-sfc': {
         'type': 'url',
         'location': ('$tarballs_base/networking-sfc/'
-                     'networking-sfc-9.0.0.tar.gz')},
+                     'networking-sfc-9.0.1.tar.gz')},
     'neutron-base-plugin-vmware-nsx': {
         'type': 'url',
         'location': ('$tarballs_base/vmware-nsx/'
                      'vmware-nsx-15.0.0.tar.gz')},
     'neutron-base-plugin-vpnaas-agent': {
         'type': 'url',
         'location': ('$tarballs_base/neutron-vpnaas/'
@@ -633,15 +633,15 @@
     'neutron-server-opendaylight-plugin-networking-l2gw': {
         'type': 'url',
         'location': ('$tarballs_base/networking-l2gw/'
                      'networking-l2gw-15.0.0.tar.gz')},
     'neutron-server-opendaylight-plugin-networking-sfc': {
         'type': 'url',
         'location': ('$tarballs_base/networking-sfc/'
-                     'networking-sfc-9.0.0.tar.gz')},
+                     'networking-sfc-9.0.1.tar.gz')},
     'neutron-server-plugin-neutron-dynamic-routing': {
         'type': 'url',
         'location': ('$tarballs_base/neutron-dynamic-routing/'
                      'neutron-dynamic-routing-15.0.1.tar.gz')},
     'neutron-server-plugin-vmware-nsxlib': {
         'type': 'url',
         'location': ('$tarballs_base/vmware-nsxlib/'
@@ -649,23 +649,23 @@
     'neutron-vpnaas-agent': {
         'type': 'url',
         'location': ('$tarballs_base/neutron-vpnaas/'
                      'neutron-vpnaas-15.0.0.tar.gz')},
     'neutron-server-ovn-plugin-networking-ovn': {
         'type': 'url',
         'location': ('$tarballs_base/networking-ovn/'
-                     'networking-ovn-7.3.0.tar.gz')},
+                     'networking-ovn-7.4.1.tar.gz')},
     'neutron-metadata-agent-ovn-plugin-networking-ovn': {
         'type': 'url',
         'location': ('$tarballs_base/networking-ovn/'
-                     'networking-ovn-7.3.0.tar.gz')},
+                     'networking-ovn-7.4.1.tar.gz')},
     'nova-base': {
         'type': 'url',
         'location': ('$tarballs_base/nova/'
-                     'nova-20.4.1.tar.gz')},
+                     'nova-20.6.1.tar.gz')},
     'nova-base-plugin-blazar': {
         'type': 'url',
         'location': ('$tarballs_base/blazar-nova/'
                      'blazar-nova-1.3.0.tar.gz')},
     'nova-base-plugin-mksproxy': {
         'type': 'url',
         'location': ('$tarballs_base/nova-mksproxy/'
@@ -673,23 +673,23 @@
     'novajoin-base': {
         'type': 'url',
         'location': ('$tarballs_base/novajoin/'
                      'novajoin-1.2.0.tar.gz')},
     'octavia-base': {
         'type': 'url',
         'location': ('$tarballs_base/octavia/'
-                     'octavia-5.0.3.tar.gz')},
+                     'octavia-5.1.2.tar.gz')},
     'panko-base': {
         'type': 'url',
         'location': ('$tarballs_base/panko/'
-                     'panko-7.0.0.tar.gz')},
+                     'panko-7.1.0.tar.gz')},
     'placement-base': {
         'type': 'url',
         'location': ('$tarballs_base/placement/'
-                     'openstack-placement-2.0.0.tar.gz')},
+                     'openstack-placement-2.0.1.tar.gz')},
     'qinling-base': {
         'type': 'url',
         'location': ('$tarballs_base/qinling/'
                      'qinling-3.0.0.tar.gz')},
     'tempest-plugin-tempest-conf': {
         'type': 'url',
         'location': ('$tarballs_base/python-tempestconf/'
@@ -809,31 +809,31 @@
     'searchlight-base': {
         'type': 'url',
         'location': ('$tarballs_base/searchlight/'
                      'searchlight-7.0.0.tar.gz')},
     'senlin-base': {
         'type': 'url',
         'location': ('$tarballs_base/senlin/'
-                     'senlin-8.0.0.tar.gz')},
+                     'senlin-8.0.1.tar.gz')},
     'solum-base': {
         'type': 'url',
         'location': ('$tarballs_base/solum/'
                      'solum-7.0.0.tar.gz')},
     'swift-base': {
         'type': 'url',
         'location': ('$tarballs_base/swift/'
-                     'swift-2.23.2.tar.gz')},
+                     'swift-2.23.3.tar.gz')},
     'tacker-base': {
         'type': 'url',
         'location': ('$tarballs_base/tacker/'
-                     'tacker-2.0.1.tar.gz')},
+                     'tacker-2.0.2.tar.gz')},
     'tacker-base-plugin-networking-sfc': {
         'type': 'url',
         'location': ('$tarballs_base/networking-sfc/'
-                     'networking-sfc-9.0.0.tar.gz')},
+                     'networking-sfc-9.0.1.tar.gz')},
     'tempest': {
         'type': 'url',
         'location': ('$tarballs_base/tempest/'
                      'tempest-22.1.0.tar.gz')},
     'tripleoclient': {
         'type': 'url',
         'location': ('$tarballs_base/python-tripleoclient/'
@@ -849,23 +849,23 @@
     'vmtp': {
         'type': 'url',
         'location': ('$tarballs_base/vmtp/'
                      'vmtp-master.tar.gz')},
     'watcher-base': {
         'type': 'url',
         'location': ('$tarballs_base/watcher/'
-                     'python-watcher-3.0.1.tar.gz')},
+                     'python-watcher-3.0.2.tar.gz')},
     'zaqar-base': {
         'type': 'url',
         'location': ('$tarballs_base/zaqar/'
                      'zaqar-9.0.1.tar.gz')},
     'zun-base': {
         'type': 'url',
         'location': ('$tarballs_base/zun/'
-                     'zun-4.0.1.tar.gz')}
+                     'zun-4.0.2.tar.gz')}
 }
 
 
 # NOTE(SamYaple): Only increment the UID. Never reuse old or removed UIDs.
 #     Starting point 42400+ was chosen arbitrarily to ensure no conflicts
 USERS = {
     'kolla-user': {
```

### Comparing `kolla-9.3.1/kolla/common/task.py` & `kolla-9.4.0/kolla/common/task.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/common/utils.py` & `kolla-9.4.0/kolla/common/utils.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/exception.py` & `kolla-9.4.0/kolla/exception.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/hacking/checks.py` & `kolla-9.4.0/kolla/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/image/build.py` & `kolla-9.4.0/kolla/image/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,29 +193,28 @@
     'ubuntu': {
         "cyborg-base",
         "elasticsearch6",   # Only required for CentOS 8 migration.
         "logstash6",        # Only required for CentOS 8 migration.
         "kibana6",          # Only required for CentOS 8 migration.
         "qdrouterd",  # There is no qdrouterd package for ubuntu bionic
         "rabbitmq-3.7.24",  # Required only for CentOS 7 to 8 migration
+        "sensu-base",       # upstream dropped Ubuntu repositories
     },
 
     'debian+aarch64': {
         "skydive-base",  # no binary package
     },
     'ubuntu+aarch64': {
-        "sensu-base",    # no binary package
         "skydive-base",  # no binary package
     },
 
     'debian+ppc64le': {
         "skydive-base",  # no binary package
     },
     'ubuntu+ppc64le': {
-        "sensu-base",    # no binary package
         "skydive-base",  # no binary package
     },
 
     'centos+aarch64': {
         "elasticsearch",  # no binary package
         "fluentd",        # no binary package
         "gnocchi-base",   # no python3-boto3 package in HA
@@ -859,14 +858,15 @@
                 sys.exit(1)
 
     def _get_images_dir(self):
         possible_paths = (
             PROJECT_ROOT,
             os.path.join(sys.prefix, 'share/kolla'),
             os.path.join(sys.prefix, 'local/share/kolla'),
+            os.path.join(os.getenv('HOME', ''), '.local/share/kolla'),
             # NOTE(zioproto): When Kolla is used within a snap, the env var
             #                 $SNAP is the directory where the snap is mounted.
             #                 https://github.com/zioproto/snap-kolla
             #                 More info in snap packages https://snapcraft.io
             os.path.join(os.environ.get('SNAP', ''), 'share/kolla'))
 
         for path in possible_paths:
```

### Comparing `kolla-9.3.1/kolla/opts.py` & `kolla-9.4.0/kolla/opts.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/template/filters.py` & `kolla-9.4.0/kolla/template/filters.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/template/methods.py` & `kolla-9.4.0/kolla/template/methods.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/tests/base.py` & `kolla-9.4.0/kolla/tests/base.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/tests/common/test_config.py` & `kolla-9.4.0/kolla/tests/common/test_config.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/tests/test_build.py` & `kolla-9.4.0/kolla/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/tests/test_hacking.py` & `kolla-9.4.0/kolla/tests/test_hacking.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/tests/test_methods.py` & `kolla-9.4.0/kolla/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla/version.py` & `kolla-9.4.0/kolla/version.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/kolla.egg-info/PKG-INFO` & `kolla-9.4.0/kolla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kolla
-Version: 9.3.1
+Version: 9.4.0
 Summary: Kolla OpenStack Deployment
 Home-page: https://docs.openstack.org/kolla/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `kolla-9.3.1/kolla.egg-info/SOURCES.txt` & `kolla-9.4.0/kolla.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 AUTHORS
 ChangeLog
 HACKING.rst
 LICENSE
 README.rst
 bindep.txt
 deliverables.yaml
-lower-constraints.txt
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
 .zuul.d/base.yaml
 .zuul.d/centos.yaml
@@ -706,14 +705,16 @@
 releasenotes/notes/bug-1868574.yaml
 releasenotes/notes/bug-1869319-aa032c1330b540dc.yaml
 releasenotes/notes/bug-1884034-328afb8831779e02.yaml
 releasenotes/notes/bug-1884484-d26488c9c1f3977f.yaml
 releasenotes/notes/bug-1886975-454ac12be3d8e1d3.yaml
 releasenotes/notes/bug-1897948-a0eb6d890eea8061.yaml
 releasenotes/notes/bug-1907213-e0cee8498d19a170.yaml
+releasenotes/notes/bug-1930544-a8926990f3a578a9.yaml
+releasenotes/notes/bug-1931544-5a091735efb6d6dd.yaml
 releasenotes/notes/build-skip-parents-102a82736935f027.yaml
 releasenotes/notes/cadf-notifications-6c102c16090688d5.yaml
 releasenotes/notes/centos-8-950d979507939643.yaml
 releasenotes/notes/centos8-aarch64-not-part-of-release-330893c1f7d5f394.yaml
 releasenotes/notes/ceph-jewel-33caab815946cb4c.yaml
 releasenotes/notes/clean_package_cache-fa08d1808a2f2b49.yaml
 releasenotes/notes/cloudkitty-docker-fb6b3d7e006a0697.yaml
@@ -773,14 +774,15 @@
 releasenotes/notes/kolla_build_skip_existing-92aebdd858a0bfa5.yaml
 releasenotes/notes/kubernetes-for-arm64-b149983c7e11ab60.yaml
 releasenotes/notes/kuryr-libnetwork-1e6ab1916a8a0d10.yaml
 releasenotes/notes/make_init_system_configurable-0ee16808b6e90954.yaml
 releasenotes/notes/mariadb-dumb-init-b23949398fd44021.yaml
 releasenotes/notes/masakari-a047b0387a474186.yaml
 releasenotes/notes/mistral-fix-wrong-service-type-72ff772fc7cf0b82.yaml
+releasenotes/notes/mistral-respect-uc-77aea99b5c6506ba.yaml
 releasenotes/notes/monitoring-ad566513454614db.yaml
 releasenotes/notes/more-flexible-image-skipping-8e1320ed78976026.yaml
 releasenotes/notes/move-manila-share-to-network-node-57c61e757c5b96b2.yaml
 releasenotes/notes/multiple-physical-networks-f2de7444f7e2d145.yaml
 releasenotes/notes/network_mode-build-configuration-5e7c15b84dae9199.yaml
 releasenotes/notes/neutron-sriov-agent-4dae576ca279ef87.yaml
 releasenotes/notes/new_networking_ovn_metadata_agent_kolla_image-6f87ef59cf62cb8f.yaml
@@ -794,14 +796,15 @@
 releasenotes/notes/prefer_headless_jre-005b5a6f17673e33.yaml
 releasenotes/notes/prometheus-alertmanager-3dbe1b8ee3b312ee.yaml
 releasenotes/notes/prometheus-cadvisor-05906b0894651a29.yaml
 releasenotes/notes/prometheus-containers-1599a6417cc6a264.yaml
 releasenotes/notes/prometheus-memcached-exporter-3ca7f701a5069509.yaml
 releasenotes/notes/rabbit-3.6.2-accdb2d3ecd493cc.yaml
 releasenotes/notes/rabbitmq-3.7.24-ba6f071b59000731.yaml
+releasenotes/notes/rabbitmq-packagecloud-c009ff6d0d2bd02d.yaml
 releasenotes/notes/rally-manage-fix-8c98a0beb6dae50e.yaml
 releasenotes/notes/redis-container-810eec9915d426d8.yaml
 releasenotes/notes/redis-sentinel-container-defa09d0ac420f64.yaml
 releasenotes/notes/remove-ceilometer-collector-image-c5d1c4b6463b2ecd.yaml
 releasenotes/notes/remove-crane-ad12c12b633d4d73.yaml
 releasenotes/notes/remove-fedora-44af79f3e061e8d6.yaml
 releasenotes/notes/remove-heat-cloudwatch-api-c71e9deafffdb3e7.yaml
@@ -835,14 +838,15 @@
 releasenotes/notes/tacker-conductor-246d23f8c4a97de0.yaml
 releasenotes/notes/tacker-networking-sfc-138b9fedd09b8728.yaml
 releasenotes/notes/tacker-rpm-binary-137dc2771bdfc5d3.yaml
 releasenotes/notes/templete-override-files-c7489543d92d1811.yaml
 releasenotes/notes/train-prelude-2420ae1363bd92bc.yaml
 releasenotes/notes/ubuntu-sources.list-change-65bb0f936b0ec95b.yaml
 releasenotes/notes/ubuntu-upstream-mariadb-34ce8106811a1f75.yaml
+releasenotes/notes/ubuntu-uses-mirrors-now-0858d579944eea48.yaml
 releasenotes/notes/unbuildable-helm-repository-5e361266659b29d1.yaml
 releasenotes/notes/unicode-locale-018fe01eaccc556d.yaml
 releasenotes/notes/unmount-ceph-osds-43b7b59685bff5b4.yaml
 releasenotes/notes/update-zaqar-images-95a5909b48893698.yaml
 releasenotes/notes/update_rpm_security_fixes-f99a3fa509cb5b3b.yaml
 releasenotes/notes/upgade-to-ubuntu-xenial-93e68d2330e9bd84.yaml
 releasenotes/notes/upgrade-ceph-luminous-415581032d25699e.yaml
```

### Comparing `kolla-9.3.1/releasenotes/notes/add-ceph-disk-init-protection-5b38ce8f1502ff69.yaml` & `kolla-9.4.0/releasenotes/notes/add-ceph-disk-init-protection-5b38ce8f1502ff69.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/notes/add-kubernetes-images-76f5a60e98d09eb7.yaml` & `kolla-9.4.0/releasenotes/notes/add-kubernetes-images-76f5a60e98d09eb7.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/notes/add-networking-baremtal-ed44e0fc04371eb8.yaml` & `kolla-9.4.0/releasenotes/notes/add-networking-baremtal-ed44e0fc04371eb8.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/notes/add-use-dumb-init-config-option-26b47f6d97d7585c.yaml` & `kolla-9.4.0/releasenotes/notes/add-use-dumb-init-config-option-26b47f6d97d7585c.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/notes/bifrost-f080de99005ad38e.yaml` & `kolla-9.4.0/releasenotes/notes/bifrost-f080de99005ad38e.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/notes/bug-1907213-e0cee8498d19a170.yaml` & `kolla-9.4.0/releasenotes/notes/bug-1907213-e0cee8498d19a170.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/notes/centos-8-950d979507939643.yaml` & `kolla-9.4.0/releasenotes/notes/centos-8-950d979507939643.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/notes/deprecate-kubernetes-dbabf9f86c15a0ee.yaml` & `kolla-9.4.0/releasenotes/notes/deprecate-kubernetes-dbabf9f86c15a0ee.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/notes/dockerfile-customizations-26981ebefe3b710b.yaml` & `kolla-9.4.0/releasenotes/notes/dockerfile-customizations-26981ebefe3b710b.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/notes/kolla-host-584270e3aee6dfd6.yaml` & `kolla-9.4.0/releasenotes/notes/kolla-host-584270e3aee6dfd6.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/notes/upgrade-influxdb-for-monasca-202f3cf22ff8597e.yaml` & `kolla-9.4.0/releasenotes/notes/upgrade-influxdb-for-monasca-202f3cf22ff8597e.yaml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/releasenotes/source/conf.py` & `kolla-9.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/requirements.txt` & `kolla-9.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/roles/collect-collectd/files/rrdtool_graph.py` & `kolla-9.4.0/roles/collect-collectd/files/rrdtool_graph.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/roles/collect-collectd/tasks/main.yml` & `kolla-9.4.0/roles/collect-collectd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/roles/collectd/tasks/main.yml` & `kolla-9.4.0/roles/collectd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/setup.cfg` & `kolla-9.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/setup.py` & `kolla-9.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/README.rst` & `kolla-9.4.0/specs/README.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/ansible-multi.rst` & `kolla-9.4.0/specs/ansible-multi.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/containerize-openstack.rst` & `kolla-9.4.0/specs/containerize-openstack.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/ha.svg` & `kolla-9.4.0/specs/ha.svg`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/high-availability.rst` & `kolla-9.4.0/specs/high-availability.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/kolla-ceph-bluestore.rst` & `kolla-9.4.0/specs/kolla-ceph-bluestore.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/kubernetes-deployment.rst` & `kolla-9.4.0/specs/kubernetes-deployment.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/logging-with-heka.rst` & `kolla-9.4.0/specs/logging-with-heka.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/logging-with-heka.svg` & `kolla-9.4.0/specs/logging-with-heka.svg`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/mariadb-backup-recovery.rst` & `kolla-9.4.0/specs/mariadb-backup-recovery.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/specs/template.rst` & `kolla-9.4.0/specs/template.rst`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/test-requirements.txt` & `kolla-9.4.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tests/clients.py` & `kolla-9.4.0/tests/clients.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tests/files/process_build_logs.py` & `kolla-9.4.0/tests/files/process_build_logs.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tests/playbooks/post.yml` & `kolla-9.4.0/tests/playbooks/post.yml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tests/playbooks/pre.yml` & `kolla-9.4.0/tests/playbooks/pre.yml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tests/playbooks/run.yml` & `kolla-9.4.0/tests/playbooks/run.yml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tests/templates/kolla-build.conf.j2` & `kolla-9.4.0/tests/templates/kolla-build.conf.j2`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tests/templates/template_overrides.j2` & `kolla-9.4.0/tests/templates/template_overrides.j2`

 * *Files 24% similar despite different names*

```diff
@@ -9,23 +9,14 @@
 ENV PIP_EXTRA_INDEX_URL {{ nodepool_wheel_mirror }}
 
 RUN echo registry={{ nodepool_npmjs_proxy }} > /etc/npmrc \
     && mkdir -p /usr/etc \
     && ln -s /etc/npmrc /usr/etc/npmrc
 
 {% raw %}
-{% if base_distro == 'ubuntu' %}
-{% endraw %}
-
-# NOTE(hrw): Debian 'buster' and Ubuntu 18.04 refuse to use unsigned repos
-RUN echo 'APT::Get::AllowUnauthenticated "true";' > /etc/apt/apt.conf.d/99allow-unauthenticated \
- && echo 'Acquire::AllowInsecureRepositories "true";' > /etc/apt/apt.conf.d/99allow-insecure-repos
-
-{% raw %}
-{% endif %}
 {% endblock %}
 
 {% block base_centos_repo_overrides_post_copy %}
 {% endraw %}
 
 RUN sed -i \
         -e "s|^\(mirrorlist.*\)|#\1|" \
@@ -68,23 +59,30 @@
         -e "s|^\(metalink.*\)|#\1|" \
         -e "s|^#baseurl=http://download.fedoraproject.org/pub|baseurl=http://{{ nodepool_mirror_host }}|" \
         -e "s|^#baseurl=https://download.fedoraproject.org/pub|baseurl=http://{{ nodepool_mirror_host }}|" \
         /etc/yum.repos.d/epel*.repo \
 {% raw %}
 {% endblock %}
 
-{% block base_footer %}
-{% if base_distro == "ubuntu" %}
+{% block base_debian_after_sources_list %}
+{% if base_distro == "debian" %}
+{% endraw %}
+
+RUN sed -i -e "s|http://deb.debian.org|[trusted=yes] http://{{ nodepool_mirror_host }}|" \
+        -e "s|http://security.debian.org|[trusted=yes] http://{{ nodepool_mirror_host }}|" \
+        /etc/apt/sources.list
+
+{% raw %}
+{% elif base_distro == "ubuntu" %}
 {% endraw %}
 
-## TODO(yoctozepto): replace base repo earlier as well (like RHEL-based do)
-RUN sed -i -e "s|http://archive.ubuntu.com|http://{{ nodepool_mirror_host }}|" \
-        -e "s|http://ubuntu-cloud.archive.canonical.com/ubuntu|http://{{ nodepool_mirror_host }}/ubuntu-cloud-archive|" \
-        /etc/apt/sources.list \
-    && apt-get update
+RUN sed -i -e "s|mirror://mirrors.ubuntu.com/mirrors.txt|[trusted=yes] http://{{ nodepool_mirror_host }}/ubuntu/|" \
+        -e "s|http://ubuntu-cloud.archive.canonical.com/ubuntu|[trusted=yes] http://{{ nodepool_mirror_host }}/ubuntu-cloud-archive|" \
+        -e "s|http://ports.ubuntu.com|[trusted=yes] http://{{ nodepool_mirror_host }}/ubuntu-ports|" \
+        /etc/apt/sources.list
 
 {% raw %}
 {% endif %}
 {% endblock %}
 
 {# Revert to upstream mirrors after build is complete #}
 
@@ -93,15 +91,15 @@
 
 ENV PIP_INDEX_URL=
 ENV PIP_TRUSTED_HOST=
 {% if use_infra_wheels_mirror | default(true) %}
 ENV PIP_EXTRA_INDEX_URL=
 {% endif %}
 
-RUN if [[ -f /usr/etc/npmrc ]]; then \
+RUN if [ -f /usr/etc/npmrc ]; then \
         unlink /usr/etc/npmrc; \
     fi \
     && rm -f /etc/npmrc
 
 {% raw %}
 {% if base_package_type == 'rpm' %}
 {% endraw %}
@@ -124,20 +122,24 @@
         /etc/yum.repos.d/opendaylight.repo \
     && sed -i \
         -e "s|^#baseurl|baseurl|g" \
         /etc/yum.repos.d/CentOS-OpsTools.repo
 {% raw %}
 {% endif %}
 {% elif base_package_type == 'deb' %}
+{% if base_distro == "debian" %}
 {% endraw %}
-RUN rm -f /etc/apt/apt.conf.d/99allow-unauthenticated /etc/apt/apt.conf.d/99allow-insecure-repos
+RUN sed -i -e "s|\[trusted=yes\] http://{{ nodepool_mirror_host }}|http://deb.debian.org|" \
+        -e "s|\[trusted=yes\] http://{{ nodepool_mirror_host }}|http://security.debian.org|" \
+        /etc/apt/sources.list
 {% raw %}
-{% if base_distro == "ubuntu" %}
+{% elif base_distro == "ubuntu" %}
 {% endraw %}
-RUN sed -i -e "s|http://{{ nodepool_mirror_host }}/ubuntu-cloud-archive|http://ubuntu-cloud.archive.canonical.com/ubuntu|" \
-        -e "s|http://{{ nodepool_mirror_host }}|http://archive.ubuntu.com|" \
+RUN sed -i -e "s|\[trusted=yes\] http://{{ nodepool_mirror_host }}/ubuntu/|mirror://mirrors.ubuntu.com/mirrors.txt|" \
+        -e "s|\[trusted=yes\] http://{{ nodepool_mirror_host }}/ubuntu-cloud-archive|http://ubuntu-cloud.archive.canonical.com/ubuntu|" \
+        -e "s|\[trusted=yes\] http://{{ nodepool_mirror_host }}/ubuntu-ports|http://ports.ubuntu.com|" \
         /etc/apt/sources.list
 {% raw %}
 {% endif %}
 {% endif %}
 {% endblock %}
 {% endraw %}
```

### Comparing `kolla-9.3.1/tests/test_build.py` & `kolla-9.4.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tests/test_keystone.py` & `kolla-9.4.0/tests/test_keystone.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tests/test_set_config.py` & `kolla-9.4.0/tests/test_set_config.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tests/vars/zuul.yml` & `kolla-9.4.0/tests/vars/zuul.yml`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tools/build.py` & `kolla-9.4.0/tools/build.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tools/cleanup-images` & `kolla-9.4.0/tools/cleanup-images`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tools/diag` & `kolla-9.4.0/tools/diag`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tools/loc` & `kolla-9.4.0/tools/loc`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tools/pre-commit-hook` & `kolla-9.4.0/tools/pre-commit-hook`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tools/setup_Debian.sh` & `kolla-9.4.0/tools/setup_Debian.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tools/validate-all-file.py` & `kolla-9.4.0/tools/validate-all-file.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tools/validate-binary-build.sh` & `kolla-9.4.0/tools/validate-binary-build.sh`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tools/validate-yaml.py` & `kolla-9.4.0/tools/validate-yaml.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tools/version-check.py` & `kolla-9.4.0/tools/version-check.py`

 * *Files identical despite different names*

### Comparing `kolla-9.3.1/tox.ini` & `kolla-9.4.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -187,14 +187,7 @@
 [flake8]
 show-source = True
 enable-extensions = H203,H106
 exclude=.eggs,.git,.tox,doc
 
 [hacking]
 local-check-factory = kolla.hacking.checks.factory
-
-[testenv:lower-constraints]
-basepython = python3
-deps =
-  -c{toxinidir}/lower-constraints.txt
-  -r{toxinidir}/test-requirements.txt
-  -r{toxinidir}/requirements.txt
```

