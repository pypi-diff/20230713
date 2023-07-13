# Comparing `tmp/designate-9.0.1.tar.gz` & `tmp/designate-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/designate-9.0.1.tar", last modified: Thu Jun 18 17:09:00 2020, max compression
+gzip compressed data, was "dist/designate-9.0.2.tar", last modified: Tue Feb 16 10:12:41 2021, max compression
```

## Comparing `designate-9.0.1.tar` & `designate-9.0.2.tar`

### file list

```diff
@@ -1,1004 +1,1004 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/etc/designate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/pools.yaml.sample-infoblox
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/rootwrap.conf.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/etc/designate/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/rootwrap.d/bind9.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/rootwrap.d/djbdns.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/rootwrap.d/knot2.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8374 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/policy.yaml.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3278 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/pools.yaml.sample-multiple-pools
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/designate-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/README-designate.conf.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/designate-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/pools.yaml.sample-bind
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/api-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2020-06-18 17:07:15.000000 designate-9.0.1/etc/designate/pools.yaml.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2020-06-18 17:07:15.000000 designate-9.0.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4010 2020-06-18 17:09:00.000000 designate-9.0.1/designate.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-18 17:09:00.000000 designate-9.0.1/designate.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2020-06-18 17:09:00.000000 designate-9.0.1/designate.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2020-06-18 17:09:00.000000 designate-9.0.1/designate.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36276 2020-06-18 17:09:00.000000 designate-9.0.1/designate.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-18 17:09:00.000000 designate-9.0.1/designate.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2020-06-18 17:09:00.000000 designate-9.0.1/designate.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2020-06-18 17:09:00.000000 designate-9.0.1/designate.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4010 2020-06-18 17:09:00.000000 designate-9.0.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2020-06-18 17:07:15.000000 designate-9.0.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2020-06-18 17:07:15.000000 designate-9.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6322 2020-06-18 17:07:15.000000 designate-9.0.1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2020-06-18 17:07:15.000000 designate-9.0.1/rally-jobs/designate-designate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2020-06-18 17:07:15.000000 designate-9.0.1/rally-jobs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/rally-jobs/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2020-06-18 17:07:15.000000 designate-9.0.1/rally-jobs/plugins/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/rally-jobs/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/rally-jobs/extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2020-06-18 17:07:15.000000 designate-9.0.1/rally-jobs/extra/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2020-06-18 17:07:15.000000 designate-9.0.1/ipa-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2020-06-18 17:07:15.000000 designate-9.0.1/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/liberty.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/queens.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1871 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25320 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/stein.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9184 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/source/_templates/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/pool-config-db-45a2cad74e22d95e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/api-mdns-multiple-bind-c78853de46ee587d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/zone_name-null-zone-trasfer-request-response-a2e316872798d1df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/newton-rc-1-eddc78fac760b98a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/pool-listener-6689ffa50345ba6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/pluggable-notifications-bd049b755a2ace9c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      612 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/cfg-notification-remove.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/bug-1827070-service_status-multiple-workers-cf99fe9e4eaf57ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/removing-deprectated-pdns-mysql-backend-1babc968f5778ae6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/bug-1768824-service_statuses-constraint-7a30eb78dc63b86f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/v1-disabled-ffebc0434fa0665f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/multilevel-tlds-3dadd285fed82715.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/fix-recordset-status-204e2747ef47d5ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/removed-pool-manager-a1a9466aceb44b9f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/agent-port-number-c28462562a74cbf9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/djbdns-agent-backend-c84e9eeab48d2e01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/stein-upgrade-checkers-cli-b8518126fff82be6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/attribute-filter-f06a53b61f5fd111.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/remove-v1-api-e38de408c6454de2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/pool_scheduler-32e34dda9484ef9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/removed-deprecated-managed-210a00cdaf975b8f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/service-status-ab0e696c8f5fdef8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/pool-manager-disabled-ff8582b5f86d2360.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/pdns4-tsig-1fda534c01d90138.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/bug-1832799-allow-topic-override-7540c14a10b8e3ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/knot-agent-backend-db2893aa97d85a1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/policy-in-code-8d3f4f89e2ede50f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/mini-dns-tcp-c1a15742f5c71739.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/quotas-validate-project-36a2a88b66bc6d63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/api-dot-json-324038360202e86b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/CAA_NAPTR_records-5e2e466a5bc18a31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/recordset-api-2c82abf569f7623e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/soa_refresh_interval_randomization-fcc1d0d63124699b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/v2-api-quotas-dd7e189cddcf7b96.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/worker-executor-84d983c92dd13b49.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/bug-1755788-txt-spf-validation-d18e43c12691132a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/bug-1828534-ensure-coordination-ids-are-encoded-b5f32b9e16339251.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2020-06-18 17:07:15.000000 designate-9.0.1/releasenotes/notes/new-service-layer-8023c242de89075a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-06-18 17:07:15.000000 designate-9.0.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2020-06-18 17:07:15.000000 designate-9.0.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5326 2020-06-18 17:09:00.000000 designate-9.0.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-06-18 17:07:15.000000 designate-9.0.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2020-06-18 17:07:15.000000 designate-9.0.1/.zuul.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/devstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/devstack/upgrade/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5185 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/upgrade/resources.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3527 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/upgrade/upgrade.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      748 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/upgrade/shutdown.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/upgrade/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/devstack/designate_plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2948 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-pdns4-mysql-db.sql
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4559 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-dynect
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3555 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-agent-msdns
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5226 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-bind9
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1444 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-agent-fake
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-infoblox
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-fake
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4119 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-agent-knot2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5538 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-pdns4
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3035 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-agent
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2876 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-pdns4-pgsql-db.sql
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4356 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-akamai
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3981 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/designate_plugins/backend-designate
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1914 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/statsd_mock_server.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13735 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/plugin.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      121 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/networking_test_monitor_tc.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21224 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/networking_test.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/devstack/gate/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2216 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/gate/post_test_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      784 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/gate/gate_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1212 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/gate/run_tempest_tests.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1014 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/gate/run_cli_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4001 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/settings
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9292 2020-06-18 17:07:15.000000 designate-9.0.1/devstack/exercise.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/records_mass_create.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/contrib/archive/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/contrib/archive/backends/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/contrib/archive/backends/impl_ipa/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2160 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/archive/backends/impl_ipa/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17158 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/archive/backends/impl_ipa/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5400 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/archive/backends/impl_multi.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4056 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/fixleadingzeros.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7230 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/zoneextractor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/contrib/designate-ext-samplehandler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/.gitignore
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/contrib/designate-ext-samplehandler/designate_ext_samplehandler/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/contrib/designate-ext-samplehandler/designate_ext_samplehandler/notification_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2740 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/designate_ext_samplehandler/notification_handler/sample.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/designate_ext_samplehandler/notification_handler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/designate_ext_samplehandler/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/designate_ext_samplehandler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/setup.cfg
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      781 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/designate-ext-samplehandler/README.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      901 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/dns_dump_raw.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1038 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/dns_dump_server.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      978 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/dns_dump_dnspy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1237 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/consume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/dns_dump_hex_to_text.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/contrib/djbdns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/djbdns/tinydns.service
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2552 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/djbdns/tinydns.init
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/contrib/vagrant/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5345 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/vagrant/Vagrantfile
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1613 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/vagrant/setup_ubuntu_devstack
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3537 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/vagrant/local.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/vagrant/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81609 2020-06-18 17:07:15.000000 designate-9.0.1/contrib/public_suffix_list.dat
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/playbooks/legacy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/playbooks/legacy/grenade-devstack-designate-pdns4/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2385 2020-06-18 17:07:15.000000 designate-9.0.1/playbooks/legacy/grenade-devstack-designate-pdns4/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-06-18 17:07:15.000000 designate-9.0.1/playbooks/legacy/grenade-devstack-designate-pdns4/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/playbooks/designate-pdns4/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2020-06-18 17:07:15.000000 designate-9.0.1/playbooks/designate-pdns4/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/playbooks/designate-bind9/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2020-06-18 17:07:15.000000 designate-9.0.1/playbooks/designate-bind9/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1698 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6133 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/cli/designate-manage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2110 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/cli/designate-status.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1309 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/examples/basic-pools-sample.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35901 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/images/Designate-Arch.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44979 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/images/Designate-PowerDNS-Detail.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36741 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/images/Designate-MultiZone.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    96455 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/images/Designate-Simple.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/_extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/_extra/.htaccess
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9397 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/user/manage-ptr-records.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/user/secondary-zones.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/user/rest/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/user/rest/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3700 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/user/rest/admin/quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/user/rest.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1710 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/notifications.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6200 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6107 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/multiple-pools.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/support-matrix.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/support-matrix.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3015 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/blacklists.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3063 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/pool-scheduler.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/admin/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3938 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/djbdns_agent.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2746 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/pdns4.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5199 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/knot2_agent.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/agent.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/bind9.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/admin/backends/sample_yaml_snippets/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/sample_yaml_snippets/pdns4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/sample_yaml_snippets/bind.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/sample_yaml_snippets/agent.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3397 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/gdnsd_agent.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3423 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/infoblox.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4412 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/backends/msdns_agent.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4572 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/troubleshooting.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/admin/upgrades/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1515 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/upgrades/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/upgrades/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2899 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/upgrades/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/upgrades/kilo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4489 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/upgrades/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4709 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/production-guidelines.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/admin/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/samples/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/samples/policy-yaml.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/samples/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2157 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/tlds.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4650 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/pools.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6656 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/admin/ha.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7649 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/ubuntu-dev.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6413 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/getting-involved.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5435 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/contributor/sourcedoc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/sourcedoc/central.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/sourcedoc/backend.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/sourcedoc/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/sourcedoc/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3314 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/sourcedoc/objects.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/sourcedoc/quota.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/sourcedoc/storage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/sourcedoc/mdns.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/sourcedoc/sink.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/metrics.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15898 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/gmr.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1564 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/related.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7272 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/devstack.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3259 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/contributor/integrations.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6511 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/install/install-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/install/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6384 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/install/install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2340 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/install/verify.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6388 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/install/install-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      624 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/install/next-steps.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/install/common_prerequisites.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5108 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/install/create-zone.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/install/get_started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9277 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/source/diagrams/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/diagrams/Designate-PowerDNS-Detail.dia
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/diagrams/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/diagrams/Designate-MultiZone.dia
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3028 2020-06-18 17:07:15.000000 designate-9.0.1/doc/source/diagrams/Designate-Simple.dia
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2020-06-18 17:07:15.000000 designate-9.0.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/ext/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/doc/ext/assets/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2020-06-18 17:07:15.000000 designate-9.0.1/doc/ext/assets/support-matrix.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2020-06-18 17:07:15.000000 designate-9.0.1/doc/ext/assets/support-matrix.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2020-06-18 17:07:15.000000 designate-9.0.1/doc/ext/custom_css.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15252 2020-06-18 17:07:15.000000 designate-9.0.1/doc/ext/support_matrix.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/doc/ext/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/roles/pdns4-logs-conf/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/roles/pdns4-logs-conf/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2020-06-18 17:07:15.000000 designate-9.0.1/roles/pdns4-logs-conf/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/roles/pdns4-logs-conf/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2020-06-18 17:07:15.000000 designate-9.0.1/roles/pdns4-logs-conf/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/roles/bind-logs-conf/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/roles/bind-logs-conf/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2020-06-18 17:07:15.000000 designate-9.0.1/roles/bind-logs-conf/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/roles/bind-logs-conf/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2020-06-18 17:07:15.000000 designate-9.0.1/roles/bind-logs-conf/defaults/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   108005 2020-06-18 17:08:59.000000 designate-9.0.1/ChangeLog
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2210 2020-06-18 17:07:15.000000 designate-9.0.1/designate/cmd/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2020-06-18 17:07:15.000000 designate-9.0.1/designate/cmd/producer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2020-06-18 17:07:15.000000 designate-9.0.1/designate/cmd/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2020-06-18 17:07:15.000000 designate-9.0.1/designate/cmd/sink.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2020-06-18 17:07:15.000000 designate-9.0.1/designate/cmd/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2020-06-18 17:07:15.000000 designate-9.0.1/designate/cmd/central.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2020-06-18 17:07:15.000000 designate-9.0.1/designate/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2020-06-18 17:07:15.000000 designate-9.0.1/designate/cmd/mdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1446 2020-06-18 17:07:15.000000 designate-9.0.1/designate/cmd/worker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3414 2020-06-18 17:07:15.000000 designate-9.0.1/designate/cmd/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2837 2020-06-18 17:07:15.000000 designate-9.0.1/designate/schema/_validators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2020-06-18 17:07:15.000000 designate-9.0.1/designate/schema/resolvers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6547 2020-06-18 17:07:15.000000 designate-9.0.1/designate/schema/format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3901 2020-06-18 17:07:15.000000 designate-9.0.1/designate/schema/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1040 2020-06-18 17:07:15.000000 designate-9.0.1/designate/schema/validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/private_codes.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12111 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_dynect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4771 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_bind9.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9008 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_akamai.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3783 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_pdns4.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6648 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/backend/agent_backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4495 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/agent_backend/impl_bind9.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/agent_backend/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3825 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/agent_backend/impl_msdns.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11340 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/agent_backend/impl_djbdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7949 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/agent_backend/impl_gdnsd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8512 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/agent_backend/impl_denominator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/agent_backend/impl_fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/agent_backend/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7539 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/agent_backend/impl_knot2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3066 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/backend/impl_infoblox/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7830 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_infoblox/object_manipulator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3158 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_infoblox/ibexceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9311 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_infoblox/connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_infoblox/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3180 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_designate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      958 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1137 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3540 2020-06-18 17:07:15.000000 designate-9.0.1/designate/backend/impl_nsd4.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7668 2020-06-18 17:07:15.000000 designate-9.0.1/designate/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1686 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_mx.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6535 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_spf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1554 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/pool_target.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1383 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/zone_attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/pool_ns_record.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15353 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1664 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/zone_transfer_accept.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2051 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_naptr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/blacklist.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/zone_export.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/pool_attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_ptr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3309 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/record.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_aaaa.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1735 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/pool_target_master.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9063 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/recordset.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/objects/adapters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13385 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/objects/adapters/yaml/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/yaml/pool_target.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/yaml/pool_ns_record.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2593 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/yaml/pool_attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/yaml/pool_target_master.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3366 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/yaml/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2605 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/yaml/pool_target_option.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/yaml/pool_also_notify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/yaml/pool_nameserver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/yaml/pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/yaml/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/objects/adapters/api_v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2810 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/zone_attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1710 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/pool_ns_record.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2025 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/zone_transfer_accept.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1929 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/blacklist.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2252 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/zone_export.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2906 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/pool_attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/record.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2103 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5346 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5160 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/zone_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1747 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/tld.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1723 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/tsigkey.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2782 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/zone_master.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4763 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/validation_error.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/zone_transfer_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1884 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/api_v2/service_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/adapters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17585 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2278 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_txt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1372 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/pool_target_option.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1560 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_caa.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_cname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1309 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/tenant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1324 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/pool_also_notify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_ns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1570 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/zone_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1874 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_sshfp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1324 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/pool_nameserver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2009 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2177 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_soa.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3798 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_a.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/tld.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1821 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/tsigkey.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/zone_master.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/validation_error.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/zone_transfer_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/rrdata_srv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2020-06-18 17:07:15.000000 designate-9.0.1/designate/objects/service_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5852 2020-06-18 17:07:15.000000 designate-9.0.1/designate/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/hacking/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/producer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3278 2020-06-18 17:07:15.000000 designate-9.0.1/designate/producer/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8640 2020-06-18 17:07:15.000000 designate-9.0.1/designate/producer/tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/producer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13578 2020-06-18 17:07:15.000000 designate-9.0.1/designate/service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/notification_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1195 2020-06-18 17:07:15.000000 designate-9.0.1/designate/notification_handler/fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7533 2020-06-18 17:07:15.000000 designate-9.0.1/designate/notification_handler/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2020-06-18 17:07:15.000000 designate-9.0.1/designate/notification_handler/neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2020-06-18 17:07:15.000000 designate-9.0.1/designate/notification_handler/nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2020-06-18 17:07:15.000000 designate-9.0.1/designate/notification_handler/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1755 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/api/v2/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/api/v2/controllers/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/api/v2/controllers/zones/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/zones/nameservers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/api/v2/controllers/zones/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4544 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/zones/tasks/exports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3994 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/zones/tasks/imports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/zones/tasks/abandon.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3548 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/zones/tasks/transfer_accepts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5924 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/zones/tasks/transfer_requests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1627 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/zones/tasks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1428 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/zones/tasks/xfr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5778 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/zones/recordsets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6897 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/zones/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4994 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4721 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/blacklists.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/errors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2510 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4672 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/tsigkeys.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1883 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4295 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/tlds.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5895 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/rest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2253 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/recordsets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3261 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/floatingips.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2999 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/reverse.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/controllers/service_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2355 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/patches.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/v2/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13628 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/middleware.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/api/admin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/api/admin/views/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/api/admin/views/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/views/extensions/reports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/views/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/views/extensions/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6714 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/views/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/views/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/api/admin/controllers/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/api/admin/controllers/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1553 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/controllers/extensions/tenants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/controllers/extensions/target_sync.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/controllers/extensions/reports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/controllers/extensions/zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/controllers/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/controllers/extensions/export.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2615 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/controllers/extensions/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1535 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/controllers/extensions/counts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1716 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/controllers/root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/controllers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1423 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1336 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/admin/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2020-06-18 17:07:15.000000 designate-9.0.1/designate/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2020-06-18 17:07:15.000000 designate-9.0.1/designate/policy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3261 2020-06-18 17:07:15.000000 designate-9.0.1/designate/locale/en_GB/LC_MESSAGES/designate.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/worker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2596 2020-06-18 17:07:15.000000 designate-9.0.1/designate/worker/processing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6407 2020-06-18 17:07:15.000000 designate-9.0.1/designate/worker/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6504 2020-06-18 17:07:15.000000 designate-9.0.1/designate/worker/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/worker/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21370 2020-06-18 17:07:15.000000 designate-9.0.1/designate/worker/tasks/zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3924 2020-06-18 17:07:15.000000 designate-9.0.1/designate/worker/tasks/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/worker/tasks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2448 2020-06-18 17:07:15.000000 designate-9.0.1/designate/worker/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2447 2020-06-18 17:07:15.000000 designate-9.0.1/designate/worker/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/worker/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2765 2020-06-18 17:07:15.000000 designate-9.0.1/designate/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3609 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/infoblox.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1317 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5602 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/producer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2319 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/network_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4049 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/sink.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1465 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/bind9.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1276 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/akamai.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/msdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4712 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/gdnsd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/denominator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/central.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/knot2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1705 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/djbdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2738 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/heartbeat_emitter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/metrics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2158 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1301 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/dynect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2190 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/mdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/coordination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2745 2020-06-18 17:07:15.000000 designate-9.0.1/designate/conf/worker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/scheduler/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/scheduler/filters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2020-06-18 17:07:15.000000 designate-9.0.1/designate/scheduler/filters/random_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2939 2020-06-18 17:07:15.000000 designate-9.0.1/designate/scheduler/filters/pool_id_attribute_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1944 2020-06-18 17:07:15.000000 designate-9.0.1/designate/scheduler/filters/in_doubt_default_pool_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1620 2020-06-18 17:07:15.000000 designate-9.0.1/designate/scheduler/filters/fallback_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4680 2020-06-18 17:07:15.000000 designate-9.0.1/designate/scheduler/filters/attribute_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1709 2020-06-18 17:07:15.000000 designate-9.0.1/designate/scheduler/filters/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/scheduler/filters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2020-06-18 17:07:15.000000 designate-9.0.1/designate/scheduler/filters/default_pool_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2983 2020-06-18 17:07:15.000000 designate-9.0.1/designate/scheduler/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2020-06-18 17:07:15.000000 designate-9.0.1/designate/scheduler/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/sink/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4089 2020-06-18 17:07:15.000000 designate-9.0.1/designate/sink/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/sink/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/network_api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2630 2020-06-18 17:07:15.000000 designate-9.0.1/designate/network_api/fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3931 2020-06-18 17:07:15.000000 designate-9.0.1/designate/network_api/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4329 2020-06-18 17:07:15.000000 designate-9.0.1/designate/network_api/neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2020-06-18 17:07:15.000000 designate-9.0.1/designate/network_api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/metrics_client/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1769 2020-06-18 17:07:15.000000 designate-9.0.1/designate/metrics_client/noop.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/metrics_client/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22750 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19977 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/091_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/072_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/095_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/073_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/088_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/102_support_caa_records.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/087_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/079_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/084_add_delayed_notify_column.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/101_support_naptr_records.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15140 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/070_liberty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3371 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/085_add_zone_attributes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/094_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4915 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/086_new_pools_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1395 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/083_change_managed_column_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/099_add_rrset_indexes_for_filtering_perf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/089_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/075_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/081_add_FKs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/071_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/092_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1776 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/097_add_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4514 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/080_domain_to_zone_rename.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/093_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/074_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/100_unique_service_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/078_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/090_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/096_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/098_fix_service_charset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/077_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2108 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/082_unique_ns_record.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/076_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/migrate.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    71910 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/impl_sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3903 2020-06-18 17:07:15.000000 designate-9.0.1/designate/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8026 2020-06-18 17:07:15.000000 designate-9.0.1/designate/rpc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/mdns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2650 2020-06-18 17:07:15.000000 designate-9.0.1/designate/mdns/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2020-06-18 17:07:15.000000 designate-9.0.1/designate/mdns/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5273 2020-06-18 17:07:15.000000 designate-9.0.1/designate/mdns/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/mdns/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13036 2020-06-18 17:07:15.000000 designate-9.0.1/designate/mdns/notify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2020-06-18 17:07:15.000000 designate-9.0.1/designate/mdns/xfr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16754 2020-06-18 17:07:15.000000 designate-9.0.1/designate/mdns/handler.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/resources/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/resources/schemas/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/resources/schemas/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1777 2020-06-18 17:07:15.000000 designate-9.0.1/designate/resources/schemas/admin/quota.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/resources/wsdl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15420 2020-06-18 17:07:15.000000 designate-9.0.1/designate/resources/wsdl/EnhancedDNS.xml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/resources/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1484 2020-06-18 17:07:15.000000 designate-9.0.1/designate/resources/templates/bind9-zone.jinja2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2020-06-18 17:07:15.000000 designate-9.0.1/designate/resources/templates/dnsmasq-zone.jinja2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2020-06-18 17:07:15.000000 designate-9.0.1/designate/resources/templates/export-zone.jinja2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7184 2020-06-18 17:07:15.000000 designate-9.0.1/designate/notifications.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/central/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   105702 2020-06-18 17:07:15.000000 designate-9.0.1/designate/central/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21044 2020-06-18 17:07:15.000000 designate-9.0.1/designate/central/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/central/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_central/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_central/test_decorator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_central/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   136143 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_central/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_producer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5446 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_producer/test_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_producer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_producer/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_quota/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3125 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_quota/test_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_quota/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4127 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_quota/test_quota.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_mdns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8634 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_mdns/test_notify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36606 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_mdns/test_handler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_mdns/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6434 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_mdns/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7425 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_middleware.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_api/test_v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12589 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_zone_transfers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9810 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_floatingips.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7092 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_import_export.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6209 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_blacklists.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27493 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7484 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_tlds.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13963 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13258 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_tsigkeys.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3380 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_service_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2084 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_hostheaders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40067 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/test_recordsets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5274 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_v2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_api/test_admin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_api/test_admin/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5891 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_admin/extensions/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_admin/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6168 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_admin/extensions/test_reports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5175 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_admin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1082 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_api/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/resources/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/resources/sample_notifications/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/resources/sample_notifications/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/neutron/port.delete.start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/neutron/port.create.start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      583 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/neutron/port.delete.end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/neutron/port.create.end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      985 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/neutron/floatingip.update.end_associate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/neutron/floatingip.delete.start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      907 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/neutron/floatingip.update.end_disassociate.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3642 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/network.floating_ip.deallocate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6860 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/network.floating_ip.associate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4660 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/compute.instance.create.start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7061 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.scheduled.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6237 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/compute.instance.create.end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4635 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/compute.instance.delete.start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6893 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3640 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/network.floating_ip.allocate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3644 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/network.floating_ip.disassociate.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/compute.instance.shutdown.end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4636 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/sample_notifications/nova/compute.instance.shutdown.start.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/resources/pools_yaml/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/pools_yaml/pools.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/pools_yaml/sample_output.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/pools_yaml/multiple-pools.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/resources/zonefiles/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/zonefiles/two_example.com.zone
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/zonefiles/nosoa_example.com.zone
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/zonefiles/malformed_example.com.zone
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/zonefiles/example.com.zone
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/zonefiles/noorigin_example.com.zone
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/resources/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/test_central/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15757 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/test_central/test_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/test_central/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    80980 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/test_central/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3066 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/test_upgrade_checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4419 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/backend/test_nsd4.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8053 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/backend/test_bind9.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10073 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/backend/test_pdns4.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5288 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/backend/test_infoblox.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8709 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/backend/test_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/backend/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4791 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/backend/test_dynect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4804 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/backend/test_designate.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4538 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_caa_object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10925 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5922 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_yaml_adapters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_rrdata_txt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5370 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1441 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_naptr_object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27019 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2649 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_adapters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_rrdata_a.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_rrdata_spf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1452 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_mx_object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2084 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/objects/test_sshfp_object.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/producer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8072 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/producer/test_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/producer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2882 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/producer/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3441 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/test_context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/notification_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1931 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/notification_handler/test_fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/notification_handler/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5633 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/api/test_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/api/test_api_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/api/test_admin_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/test_conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/test_heartbeat.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/scheduler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13641 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/scheduler/test_filters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3388 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/scheduler/test_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/sink/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2844 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/sink/test_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/sink/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/sink/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/workers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/workers/test_processing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/workers/test_base_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/workers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22539 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/workers/test_zone_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8977 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/workers/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/metrics/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4522 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/metrics/test_metrics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/metrics/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/mdns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9430 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/mdns/test_notify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13822 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/mdns/test_handler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/mdns/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3099 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/mdns/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4186 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/test_service_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2688 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2610 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7849 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/test_handler.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/unit/agent/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2693 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/backends/test_gdnsd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4527 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/backends/test_bind9.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7761 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/backends/test_knot2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4501 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/backends/test_djbdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/backends/test_fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4683 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/backends/test_msdns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6160 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/backends/test_denominator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2672 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/agent/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10125 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/test_dnsutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16370 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/unit/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4601 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_storage/test_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   120771 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_storage/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_network_api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2019 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_network_api/test_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_network_api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17661 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_schema/test_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_schema/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4101 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27092 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7146 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_coordination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9185 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/tests/test_notification_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5441 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_notification_handler/test_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_notification_handler/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1185 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_notification_handler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8143 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_notification_handler/test_nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4343 2020-06-18 17:07:15.000000 designate-9.0.1/designate/tests/test_hookpoints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2020-06-18 17:07:15.000000 designate-9.0.1/designate/hookpoints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2020-06-18 17:07:15.000000 designate-9.0.1/designate/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2020-06-18 17:07:15.000000 designate-9.0.1/designate/loggingutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12886 2020-06-18 17:07:15.000000 designate-9.0.1/designate/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/common/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3603 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2275 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/zone_transfer_accept.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/blacklist.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2447 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/zone_export.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/record.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1687 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2767 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2054 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/diagnostics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/tenant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2280 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/zone_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2051 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2069 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/tld.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2249 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/tsigkey.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2878 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/zone_transfer_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1417 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/policies/service_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3033 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2300 2020-06-18 17:07:15.000000 designate-9.0.1/designate/metrics.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2020-06-18 17:07:15.000000 designate-9.0.1/designate/sqlalchemy/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24196 2020-06-18 17:07:15.000000 designate-9.0.1/designate/sqlalchemy/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5091 2020-06-18 17:07:15.000000 designate-9.0.1/designate/sqlalchemy/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2020-06-18 17:07:15.000000 designate-9.0.1/designate/sqlalchemy/session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2020-06-18 17:07:15.000000 designate-9.0.1/designate/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12431 2020-06-18 17:07:15.000000 designate-9.0.1/designate/dnsutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10064 2020-06-18 17:07:15.000000 designate-9.0.1/designate/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2020-06-18 17:07:15.000000 designate-9.0.1/designate/agent/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9391 2020-06-18 17:07:15.000000 designate-9.0.1/designate/agent/handler.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/quota/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2020-06-18 17:07:15.000000 designate-9.0.1/designate/quota/impl_noop.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2556 2020-06-18 17:07:15.000000 designate-9.0.1/designate/quota/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3145 2020-06-18 17:07:15.000000 designate-9.0.1/designate/quota/impl_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      966 2020-06-18 17:07:15.000000 designate-9.0.1/designate/quota/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2020-06-18 17:07:15.000000 designate-9.0.1/designate/coordination.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/designate/manage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2020-06-18 17:07:15.000000 designate-9.0.1/designate/manage/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5835 2020-06-18 17:07:15.000000 designate-9.0.1/designate/manage/tlds.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7048 2020-06-18 17:07:15.000000 designate-9.0.1/designate/manage/pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:15.000000 designate-9.0.1/designate/manage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1762 2020-06-18 17:07:15.000000 designate-9.0.1/designate/manage/database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2961 2020-06-18 17:07:15.000000 designate-9.0.1/designate/service_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9735 2020-06-18 17:09:00.000000 designate-9.0.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2951 2020-06-18 17:07:15.000000 designate-9.0.1/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2304 2020-06-18 17:07:15.000000 designate-9.0.1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2020-06-18 17:07:15.000000 designate-9.0.1/.coveragerc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/tools/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/tools/mysql_pending_notify_bench/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2420 2020-06-18 17:07:15.000000 designate-9.0.1/tools/mysql_pending_notify_bench/runner
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3148 2020-06-18 17:07:15.000000 designate-9.0.1/tools/mysql_pending_notify_bench/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5959 2020-06-18 17:07:15.000000 designate-9.0.1/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2020-06-18 17:07:15.000000 designate-9.0.1/tools/with_venv.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      132 2020-06-18 17:07:15.000000 designate-9.0.1/tools/pretty_flake8.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2020-06-18 17:07:15.000000 designate-9.0.1/tools/install_venv.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4497 2020-06-18 17:07:15.000000 designate-9.0.1/tools/pretty_flake8.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-blacklist.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6672 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-zone-ownership-transfer-request.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18834 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4348 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-tld.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3883 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-quota.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5384 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-tsigkey.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5111 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-zone-export.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-limits.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7411 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-zone.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/zones/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/update-zone-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/update-zone-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/show-zone-transfer-request-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/update-zone-transfer-request-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/show-zone-export-content.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/list-zones-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/create-zone-transfer-request-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/update-zone-transfer-request-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/show-zone-import-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/list-zone-transfer-request-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/create-zone-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/list-zone-import-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/create-zone-transfer-accept-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/list-zone-export-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/show-zone-nameservers-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/list-zone-transfer-accept-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/create-zone-transfer-request-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/create-zone-export-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/show-zone-export-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/create-zone-transfer-accept-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/create-zone-import-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/zone-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/zones/delete-zone-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/blacklists/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/blacklists/list-blacklists-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/blacklists/create-blacklist-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/blacklists/update-blacklist-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/blacklists/update-blacklist-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/blacklists/blacklist-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/quotas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/quotas/set-quotas-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/quotas/set-quotas-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/quotas/get-quotas-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/reverse_floatingips/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/reverse_floatingips/unset-ptr-record-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      958 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/reverse_floatingips/list-ptr-record-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/reverse_floatingips/set-ptr-record-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/reverse_floatingips/ptr-record-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/tsigkeys/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1599 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/tsigkeys/list-tsigkeys-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/tsigkeys/update-tsigkey-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/tsigkeys/tsigkey-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/tsigkeys/update-tsigkey-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/tsigkeys/create-tsigkey-request.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/versions/get-versions-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/recordsets/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/list-recordset-in-zone-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/delete-recordset-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/create-srv-recordset-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/create-mx-recordset-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/create-recordset-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/create-srv-recordset-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/create-recordset-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/create-mx-recordset-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/create-sshfp-recordset-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/show-recordset-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/create-spf-recordset-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/list-all-recordset-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/update-recordset-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/create-sshfp-recordset-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/create-spf-recordset-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/recordsets/update-recordset-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/limits/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/limits/get-limits-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/service_status/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/service_status/service_status_list.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/tlds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/tlds/update-tld-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/tlds/update-tld-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/tlds/tld-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/tlds/create-tld-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/tlds/list-tlds-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:00.000000 designate-9.0.1/api-ref/source/samples/pools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/pools/list-pools-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/samples/pools/show-pool-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3862 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-zone-ownership-transfer-accept.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1564 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1866 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-zone-tasks.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7478 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      591 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-version.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-pool.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4256 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-reverse-floatingips.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-service-status.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14014 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-recordset.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3951 2020-06-18 17:07:15.000000 designate-9.0.1/api-ref/source/dns-api-v2-zone-import.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2020-06-18 17:07:15.000000 designate-9.0.1/designate.sublime-project
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.228425 designate-9.0.2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2021-02-16 10:12:08.000000 designate-9.0.2/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2021-02-16 10:12:08.000000 designate-9.0.2/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4249 2021-02-16 10:12:08.000000 designate-9.0.2/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9842 2021-02-16 10:12:40.000000 designate-9.0.2/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2021-02-16 10:12:08.000000 designate-9.0.2/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   108269 2021-02-16 10:12:40.000000 designate-9.0.2/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-02-16 10:12:08.000000 designate-9.0.2/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4010 2021-02-16 10:12:41.228425 designate-9.0.2/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2304 2021-02-16 10:12:08.000000 designate-9.0.2/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.056433 designate-9.0.2/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.080432 designate-9.0.2/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7478 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-blacklist.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-limits.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-pool.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3883 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-quota.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14014 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-recordset.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4256 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-reverse-floatingips.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-service-status.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4348 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-tld.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5384 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-tsigkey.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      591 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-version.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5111 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-zone-export.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3951 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-zone-import.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3862 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-zone-ownership-transfer-accept.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6672 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-zone-ownership-transfer-request.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1866 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-zone-tasks.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7411 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/dns-api-v2-zone.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18834 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.056433 designate-9.0.2/api-ref/source/samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.080432 designate-9.0.2/api-ref/source/samples/blacklists/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/blacklists/blacklist-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/blacklists/create-blacklist-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/blacklists/list-blacklists-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/blacklists/update-blacklist-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/blacklists/update-blacklist-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.080432 designate-9.0.2/api-ref/source/samples/limits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/limits/get-limits-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.080432 designate-9.0.2/api-ref/source/samples/pools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/pools/list-pools-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/pools/show-pool-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.080432 designate-9.0.2/api-ref/source/samples/quotas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/quotas/get-quotas-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/quotas/set-quotas-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/quotas/set-quotas-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.084432 designate-9.0.2/api-ref/source/samples/recordsets/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/create-mx-recordset-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/create-mx-recordset-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/create-recordset-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/create-recordset-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/create-spf-recordset-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/create-spf-recordset-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/create-srv-recordset-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/create-srv-recordset-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/create-sshfp-recordset-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/create-sshfp-recordset-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/delete-recordset-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/list-all-recordset-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/list-recordset-in-zone-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/show-recordset-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/update-recordset-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/recordsets/update-recordset-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.084432 designate-9.0.2/api-ref/source/samples/reverse_floatingips/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      958 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/reverse_floatingips/list-ptr-record-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/reverse_floatingips/ptr-record-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/reverse_floatingips/set-ptr-record-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/reverse_floatingips/unset-ptr-record-request.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.084432 designate-9.0.2/api-ref/source/samples/service_status/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/service_status/service_status_list.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.084432 designate-9.0.2/api-ref/source/samples/tlds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/tlds/create-tld-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/tlds/list-tlds-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/tlds/tld-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/tlds/update-tld-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/tlds/update-tld-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.088431 designate-9.0.2/api-ref/source/samples/tsigkeys/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/tsigkeys/create-tsigkey-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1599 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/tsigkeys/list-tsigkeys-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/tsigkeys/tsigkey-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/tsigkeys/update-tsigkey-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/tsigkeys/update-tsigkey-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.088431 designate-9.0.2/api-ref/source/samples/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/versions/get-versions-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.092431 designate-9.0.2/api-ref/source/samples/zones/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/create-zone-export-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/create-zone-import-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/create-zone-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/create-zone-transfer-accept-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/create-zone-transfer-accept-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/create-zone-transfer-request-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/create-zone-transfer-request-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/delete-zone-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/list-zone-export-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/list-zone-import-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/list-zone-transfer-accept-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/list-zone-transfer-request-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/list-zones-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/show-zone-export-content.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/show-zone-export-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/show-zone-import-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/show-zone-nameservers-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/show-zone-transfer-request-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/update-zone-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/update-zone-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/update-zone-transfer-request-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/update-zone-transfer-request-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/samples/zones/zone-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1564 2021-02-16 10:12:08.000000 designate-9.0.2/api-ref/source/status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-02-16 10:12:08.000000 designate-9.0.2/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.092431 designate-9.0.2/contrib/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.056433 designate-9.0.2/contrib/archive/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.092431 designate-9.0.2/contrib/archive/backends/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.092431 designate-9.0.2/contrib/archive/backends/impl_ipa/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17158 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/archive/backends/impl_ipa/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2160 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/archive/backends/impl_ipa/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5400 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/archive/backends/impl_multi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1237 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/consume.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.096431 designate-9.0.2/contrib/designate-ext-samplehandler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.096431 designate-9.0.2/contrib/designate-ext-samplehandler/designate_ext_samplehandler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/designate_ext_samplehandler/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.096431 designate-9.0.2/contrib/designate-ext-samplehandler/designate_ext_samplehandler/notification_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/designate_ext_samplehandler/notification_handler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2740 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/designate_ext_samplehandler/notification_handler/sample.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/designate_ext_samplehandler/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/setup.cfg
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      781 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/designate-ext-samplehandler/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.096431 designate-9.0.2/contrib/djbdns/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2552 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/djbdns/tinydns.init
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/djbdns/tinydns.service
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      978 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/dns_dump_dnspy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/dns_dump_hex_to_text.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      901 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/dns_dump_raw.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1038 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/dns_dump_server.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4056 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/fixleadingzeros.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    81609 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/public_suffix_list.dat
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/records_mass_create.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.096431 designate-9.0.2/contrib/vagrant/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/vagrant/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5345 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/vagrant/Vagrantfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3537 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/vagrant/local.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1613 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/vagrant/setup_ubuntu_devstack
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7230 2021-02-16 10:12:08.000000 designate-9.0.2/contrib/zoneextractor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.100431 designate-9.0.2/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2021-02-16 10:12:08.000000 designate-9.0.2/designate/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.100431 designate-9.0.2/designate/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9391 2021-02-16 10:12:08.000000 designate-9.0.2/designate/agent/handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2021-02-16 10:12:08.000000 designate-9.0.2/designate/agent/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.104431 designate-9.0.2/designate/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.104431 designate-9.0.2/designate/api/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1423 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1336 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/app.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.104431 designate-9.0.2/designate/api/admin/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/controllers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.104431 designate-9.0.2/designate/api/admin/controllers/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/controllers/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1535 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/controllers/extensions/counts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/controllers/extensions/export.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2615 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/controllers/extensions/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/controllers/extensions/reports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/controllers/extensions/target_sync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1553 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/controllers/extensions/tenants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/controllers/extensions/zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1716 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/controllers/root.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.104431 designate-9.0.2/designate/api/admin/views/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/views/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6714 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/views/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.104431 designate-9.0.2/designate/api/admin/views/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/views/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/views/extensions/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/admin/views/extensions/reports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13628 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.108431 designate-9.0.2/designate/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/app.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.108431 designate-9.0.2/designate/api/v2/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4721 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/blacklists.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1883 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/errors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3261 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/floatingips.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4994 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2999 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2253 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/recordsets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5895 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/rest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/reverse.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2510 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/service_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4295 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/tlds.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4672 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/tsigkeys.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.108431 designate-9.0.2/designate/api/v2/controllers/zones/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6897 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/zones/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/zones/nameservers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5778 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/zones/recordsets.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.112430 designate-9.0.2/designate/api/v2/controllers/zones/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1627 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/zones/tasks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/zones/tasks/abandon.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4544 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/zones/tasks/exports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3994 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/zones/tasks/imports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3548 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/zones/tasks/transfer_accepts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5924 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/zones/tasks/transfer_requests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1428 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/controllers/zones/tasks/xfr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2355 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/v2/patches.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1755 2021-02-16 10:12:08.000000 designate-9.0.2/designate/api/versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.112430 designate-9.0.2/designate/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1137 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6648 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.116430 designate-9.0.2/designate/backend/agent_backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/agent_backend/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/agent_backend/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4495 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/agent_backend/impl_bind9.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8512 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/agent_backend/impl_denominator.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11340 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/agent_backend/impl_djbdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/agent_backend/impl_fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7949 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/agent_backend/impl_gdnsd.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7539 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/agent_backend/impl_knot2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3825 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/agent_backend/impl_msdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3066 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9008 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_akamai.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4771 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_bind9.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3180 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_designate.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12111 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_dynect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      958 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.116430 designate-9.0.2/designate/backend/impl_infoblox/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_infoblox/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9311 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_infoblox/connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3158 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_infoblox/ibexceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7830 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_infoblox/object_manipulator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3540 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_nsd4.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/impl_pdns4.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2021-02-16 10:12:08.000000 designate-9.0.2/designate/backend/private_codes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.116430 designate-9.0.2/designate/central/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/central/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21044 2021-02-16 10:12:08.000000 designate-9.0.2/designate/central/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   105882 2021-02-16 10:12:08.000000 designate-9.0.2/designate/central/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.116430 designate-9.0.2/designate/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2021-02-16 10:12:08.000000 designate-9.0.2/designate/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2021-02-16 10:12:08.000000 designate-9.0.2/designate/cmd/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2021-02-16 10:12:08.000000 designate-9.0.2/designate/cmd/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2021-02-16 10:12:08.000000 designate-9.0.2/designate/cmd/central.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3414 2021-02-16 10:12:08.000000 designate-9.0.2/designate/cmd/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2021-02-16 10:12:08.000000 designate-9.0.2/designate/cmd/mdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2021-02-16 10:12:08.000000 designate-9.0.2/designate/cmd/producer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2021-02-16 10:12:08.000000 designate-9.0.2/designate/cmd/sink.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2210 2021-02-16 10:12:08.000000 designate-9.0.2/designate/cmd/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1446 2021-02-16 10:12:08.000000 designate-9.0.2/designate/cmd/worker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.120430 designate-9.0.2/designate/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3033 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/keystone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.120430 designate-9.0.2/designate/common/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2051 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2054 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/blacklist.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/diagnostics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1687 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/record.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2767 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1417 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/service_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/tenant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2069 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/tld.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2249 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/tsigkey.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3603 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2447 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/zone_export.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2280 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/zone_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2275 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/zone_transfer_accept.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2878 2021-02-16 10:12:08.000000 designate-9.0.2/designate/common/policies/zone_transfer_request.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.128430 designate-9.0.2/designate/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2158 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1276 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/akamai.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4712 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1465 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/bind9.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/central.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/denominator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1705 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/djbdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1301 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/dynect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/gdnsd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/heartbeat_emitter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3609 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/infoblox.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/knot2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2190 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/mdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/metrics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/msdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2319 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/network_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2738 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5602 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/producer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1317 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4049 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/sink.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2745 2021-02-16 10:12:08.000000 designate-9.0.2/designate/conf/worker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7668 2021-02-16 10:12:08.000000 designate-9.0.2/designate/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7721 2021-02-16 10:12:08.000000 designate-9.0.2/designate/coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12431 2021-02-16 10:12:08.000000 designate-9.0.2/designate/dnsutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10064 2021-02-16 10:12:08.000000 designate-9.0.2/designate/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.128430 designate-9.0.2/designate/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5852 2021-02-16 10:12:08.000000 designate-9.0.2/designate/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2021-02-16 10:12:08.000000 designate-9.0.2/designate/hookpoints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2021-02-16 10:12:08.000000 designate-9.0.2/designate/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.060433 designate-9.0.2/designate/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.060433 designate-9.0.2/designate/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.128430 designate-9.0.2/designate/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3261 2021-02-16 10:12:08.000000 designate-9.0.2/designate/locale/en_GB/LC_MESSAGES/designate.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2021-02-16 10:12:08.000000 designate-9.0.2/designate/loggingutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.128430 designate-9.0.2/designate/manage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/manage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2021-02-16 10:12:08.000000 designate-9.0.2/designate/manage/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1762 2021-02-16 10:12:08.000000 designate-9.0.2/designate/manage/database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7048 2021-02-16 10:12:08.000000 designate-9.0.2/designate/manage/pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5835 2021-02-16 10:12:08.000000 designate-9.0.2/designate/manage/tlds.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.128430 designate-9.0.2/designate/mdns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/mdns/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2021-02-16 10:12:08.000000 designate-9.0.2/designate/mdns/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16754 2021-02-16 10:12:08.000000 designate-9.0.2/designate/mdns/handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13036 2021-02-16 10:12:08.000000 designate-9.0.2/designate/mdns/notify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5273 2021-02-16 10:12:08.000000 designate-9.0.2/designate/mdns/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2650 2021-02-16 10:12:08.000000 designate-9.0.2/designate/mdns/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2021-02-16 10:12:08.000000 designate-9.0.2/designate/mdns/xfr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2300 2021-02-16 10:12:08.000000 designate-9.0.2/designate/metrics.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.128430 designate-9.0.2/designate/metrics_client/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/metrics_client/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1769 2021-02-16 10:12:08.000000 designate-9.0.2/designate/metrics_client/noop.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.128430 designate-9.0.2/designate/network_api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2021-02-16 10:12:08.000000 designate-9.0.2/designate/network_api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3931 2021-02-16 10:12:08.000000 designate-9.0.2/designate/network_api/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2630 2021-02-16 10:12:08.000000 designate-9.0.2/designate/network_api/fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4329 2021-02-16 10:12:08.000000 designate-9.0.2/designate/network_api/neutron.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.132429 designate-9.0.2/designate/notification_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2021-02-16 10:12:08.000000 designate-9.0.2/designate/notification_handler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7533 2021-02-16 10:12:08.000000 designate-9.0.2/designate/notification_handler/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1195 2021-02-16 10:12:08.000000 designate-9.0.2/designate/notification_handler/fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2021-02-16 10:12:08.000000 designate-9.0.2/designate/notification_handler/neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2021-02-16 10:12:08.000000 designate-9.0.2/designate/notification_handler/nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7184 2021-02-16 10:12:08.000000 designate-9.0.2/designate/notifications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.140429 designate-9.0.2/designate/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3798 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.140429 designate-9.0.2/designate/objects/adapters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.144429 designate-9.0.2/designate/objects/adapters/api_v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5160 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/blacklist.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1929 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1747 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2906 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/pool_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1710 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/pool_ns_record.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2103 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/record.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5346 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1884 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/service_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/tld.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1723 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/tsigkey.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4763 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/validation_error.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2810 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/zone_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2252 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/zone_export.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/zone_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2782 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/zone_master.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2025 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/zone_transfer_accept.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/api_v2/zone_transfer_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13385 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.144429 designate-9.0.2/designate/objects/adapters/yaml/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/yaml/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3366 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/yaml/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/yaml/pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/yaml/pool_also_notify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2593 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/yaml/pool_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/yaml/pool_nameserver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/yaml/pool_ns_record.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/yaml/pool_target.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/yaml/pool_target_master.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2605 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/adapters/yaml/pool_target_option.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17585 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/blacklist.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15353 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2009 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1324 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/pool_also_notify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/pool_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1324 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/pool_nameserver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/pool_ns_record.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1554 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/pool_target.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/pool_target_master.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1372 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/pool_target_option.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1735 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3309 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/record.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9063 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_a.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_aaaa.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1560 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_caa.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_cname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1686 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_mx.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2051 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_naptr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_ns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_ptr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2177 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_soa.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_spf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_srv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1874 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_sshfp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2278 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/rrdata_txt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/service_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1309 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/tenant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/tld.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1821 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/tsigkey.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/validation_error.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6535 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1383 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/zone_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/zone_export.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1570 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/zone_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/zone_master.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1664 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/zone_transfer_accept.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2021-02-16 10:12:08.000000 designate-9.0.2/designate/objects/zone_transfer_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2765 2021-02-16 10:12:08.000000 designate-9.0.2/designate/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2021-02-16 10:12:08.000000 designate-9.0.2/designate/policy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.144429 designate-9.0.2/designate/producer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/producer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3278 2021-02-16 10:12:08.000000 designate-9.0.2/designate/producer/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8640 2021-02-16 10:12:08.000000 designate-9.0.2/designate/producer/tasks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.144429 designate-9.0.2/designate/quota/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      966 2021-02-16 10:12:08.000000 designate-9.0.2/designate/quota/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2556 2021-02-16 10:12:08.000000 designate-9.0.2/designate/quota/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2021-02-16 10:12:08.000000 designate-9.0.2/designate/quota/impl_noop.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3145 2021-02-16 10:12:08.000000 designate-9.0.2/designate/quota/impl_storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.060433 designate-9.0.2/designate/resources/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.060433 designate-9.0.2/designate/resources/schemas/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.144429 designate-9.0.2/designate/resources/schemas/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1777 2021-02-16 10:12:08.000000 designate-9.0.2/designate/resources/schemas/admin/quota.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.148429 designate-9.0.2/designate/resources/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1484 2021-02-16 10:12:08.000000 designate-9.0.2/designate/resources/templates/bind9-zone.jinja2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2021-02-16 10:12:08.000000 designate-9.0.2/designate/resources/templates/dnsmasq-zone.jinja2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2021-02-16 10:12:08.000000 designate-9.0.2/designate/resources/templates/export-zone.jinja2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.148429 designate-9.0.2/designate/resources/wsdl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15420 2021-02-16 10:12:08.000000 designate-9.0.2/designate/resources/wsdl/EnhancedDNS.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8026 2021-02-16 10:12:08.000000 designate-9.0.2/designate/rpc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.148429 designate-9.0.2/designate/scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2021-02-16 10:12:08.000000 designate-9.0.2/designate/scheduler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2983 2021-02-16 10:12:08.000000 designate-9.0.2/designate/scheduler/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.148429 designate-9.0.2/designate/scheduler/filters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/scheduler/filters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4680 2021-02-16 10:12:08.000000 designate-9.0.2/designate/scheduler/filters/attribute_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1709 2021-02-16 10:12:08.000000 designate-9.0.2/designate/scheduler/filters/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2021-02-16 10:12:08.000000 designate-9.0.2/designate/scheduler/filters/default_pool_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1620 2021-02-16 10:12:08.000000 designate-9.0.2/designate/scheduler/filters/fallback_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1944 2021-02-16 10:12:08.000000 designate-9.0.2/designate/scheduler/filters/in_doubt_default_pool_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2939 2021-02-16 10:12:08.000000 designate-9.0.2/designate/scheduler/filters/pool_id_attribute_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2021-02-16 10:12:08.000000 designate-9.0.2/designate/scheduler/filters/random_filter.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.148429 designate-9.0.2/designate/schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3901 2021-02-16 10:12:08.000000 designate-9.0.2/designate/schema/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2837 2021-02-16 10:12:08.000000 designate-9.0.2/designate/schema/_validators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6547 2021-02-16 10:12:08.000000 designate-9.0.2/designate/schema/format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2021-02-16 10:12:08.000000 designate-9.0.2/designate/schema/resolvers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1040 2021-02-16 10:12:08.000000 designate-9.0.2/designate/schema/validators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13578 2021-02-16 10:12:08.000000 designate-9.0.2/designate/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2961 2021-02-16 10:12:08.000000 designate-9.0.2/designate/service_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.148429 designate-9.0.2/designate/sink/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/sink/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4089 2021-02-16 10:12:08.000000 designate-9.0.2/designate/sink/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.152428 designate-9.0.2/designate/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24196 2021-02-16 10:12:08.000000 designate-9.0.2/designate/sqlalchemy/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2021-02-16 10:12:08.000000 designate-9.0.2/designate/sqlalchemy/session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2021-02-16 10:12:08.000000 designate-9.0.2/designate/sqlalchemy/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5091 2021-02-16 10:12:08.000000 designate-9.0.2/designate/sqlalchemy/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.152428 designate-9.0.2/designate/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3903 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22750 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.152428 designate-9.0.2/designate/storage/impl_sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71910 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.152428 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/migrate.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.160428 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15199 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/070_liberty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/071_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/072_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/073_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/074_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/075_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/076_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/077_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/078_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/079_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4514 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/080_domain_to_zone_rename.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/081_add_FKs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2108 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/082_unique_ns_record.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1395 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/083_change_managed_column_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/084_add_delayed_notify_column.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3371 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/085_add_zone_attributes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4915 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/086_new_pools_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/087_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/088_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/089_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/090_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/091_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/092_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/093_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/094_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/095_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/096_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1776 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/097_add_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/098_fix_service_charset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/099_add_rrset_indexes_for_filtering_perf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/100_unique_service_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/101_support_naptr_records.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/102_support_caa_records.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19977 2021-02-16 10:12:08.000000 designate-9.0.2/designate/storage/impl_sqlalchemy/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.160428 designate-9.0.2/designate/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27092 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9185 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.160428 designate-9.0.2/designate/tests/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.160428 designate-9.0.2/designate/tests/resources/pools_yaml/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/pools_yaml/multiple-pools.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/pools_yaml/pools.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/pools_yaml/sample_output.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.064433 designate-9.0.2/designate/tests/resources/sample_notifications/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.160428 designate-9.0.2/designate/tests/resources/sample_notifications/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/neutron/floatingip.delete.start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      985 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/neutron/floatingip.update.end_associate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      907 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/neutron/floatingip.update.end_disassociate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/neutron/port.create.end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/neutron/port.create.start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      583 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/neutron/port.delete.end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/neutron/port.delete.start.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.164428 designate-9.0.2/designate/tests/resources/sample_notifications/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6237 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/compute.instance.create.end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4660 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/compute.instance.create.start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4635 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/compute.instance.delete.start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/compute.instance.shutdown.end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4636 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/compute.instance.shutdown.start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3640 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/network.floating_ip.allocate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/network.floating_ip.associate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3642 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/network.floating_ip.deallocate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3644 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/network.floating_ip.disassociate.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6893 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7061 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.scheduled.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6860 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.start.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.164428 designate-9.0.2/designate/tests/resources/zonefiles/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/zonefiles/example.com.zone
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/zonefiles/malformed_example.com.zone
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/zonefiles/noorigin_example.com.zone
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/zonefiles/nosoa_example.com.zone
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/resources/zonefiles/two_example.com.zone
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.164428 designate-9.0.2/designate/tests/test_api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.164428 designate-9.0.2/designate/tests/test_api/test_admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5175 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_admin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.168428 designate-9.0.2/designate/tests/test_api/test_admin/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_admin/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5891 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_admin/extensions/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6168 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_admin/extensions/test_reports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7425 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1082 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.168428 designate-9.0.2/designate/tests/test_api/test_v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5274 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6209 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_blacklists.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9810 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_floatingips.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2084 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_hostheaders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7092 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_import_export.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13963 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40067 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_recordsets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3380 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_service_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7484 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_tlds.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13258 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_tsigkeys.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12589 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_zone_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27493 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_api/test_v2/test_zones.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.168428 designate-9.0.2/designate/tests/test_backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_backend/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.168428 designate-9.0.2/designate/tests/test_central/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_central/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_central/test_decorator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   136143 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_central/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7146 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4343 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_hookpoints.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.172428 designate-9.0.2/designate/tests/test_mdns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_mdns/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36606 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_mdns/test_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8634 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_mdns/test_notify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6434 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_mdns/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.172428 designate-9.0.2/designate/tests/test_network_api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_network_api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2019 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_network_api/test_neutron.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.172428 designate-9.0.2/designate/tests/test_notification_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1185 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_notification_handler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_notification_handler/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5441 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_notification_handler/test_neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8143 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_notification_handler/test_nova.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.172428 designate-9.0.2/designate/tests/test_producer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_producer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_producer/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5446 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_producer/test_tasks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.172428 designate-9.0.2/designate/tests/test_quota/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_quota/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4127 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_quota/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3125 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_quota/test_storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.172428 designate-9.0.2/designate/tests/test_schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_schema/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17661 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_schema/test_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4101 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_sqlalchemy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.172428 designate-9.0.2/designate/tests/test_storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   120771 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4601 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/test_storage/test_sqlalchemy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.176427 designate-9.0.2/designate/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2610 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.176427 designate-9.0.2/designate/tests/unit/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.176427 designate-9.0.2/designate/tests/unit/agent/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4527 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/backends/test_bind9.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6160 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/backends/test_denominator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4501 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/backends/test_djbdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/backends/test_fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2693 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/backends/test_gdnsd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7761 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/backends/test_knot2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4683 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/backends/test_msdns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7849 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/test_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2672 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/agent/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.180427 designate-9.0.2/designate/tests/unit/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/api/test_admin_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/api/test_api_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5633 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/api/test_middleware.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.180427 designate-9.0.2/designate/tests/unit/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/backend/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8709 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/backend/test_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8053 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/backend/test_bind9.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4804 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/backend/test_designate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4791 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/backend/test_dynect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5288 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/backend/test_infoblox.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4419 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/backend/test_nsd4.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10896 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/backend/test_pdns4.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.180427 designate-9.0.2/designate/tests/unit/mdns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/mdns/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13822 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/mdns/test_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9430 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/mdns/test_notify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3099 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/mdns/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.180427 designate-9.0.2/designate/tests/unit/metrics/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/metrics/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4522 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/metrics/test_metrics.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.180427 designate-9.0.2/designate/tests/unit/notification_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/notification_handler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1931 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/notification_handler/test_fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.184427 designate-9.0.2/designate/tests/unit/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2649 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_adapters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27019 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4538 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_caa_object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1452 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_mx_object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1441 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_naptr_object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10925 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_rrdata_a.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_rrdata_spf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_rrdata_txt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2084 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_sshfp_object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5922 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_yaml_adapters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5370 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/objects/test_zone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.184427 designate-9.0.2/designate/tests/unit/producer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/producer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2882 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/producer/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8072 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/producer/test_tasks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.184427 designate-9.0.2/designate/tests/unit/scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/scheduler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3388 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/scheduler/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13641 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/scheduler/test_filters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.184427 designate-9.0.2/designate/tests/unit/sink/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/sink/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2844 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/sink/test_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/sink/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.184427 designate-9.0.2/designate/tests/unit/test_central/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/test_central/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    80980 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/test_central/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15757 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/test_central/test_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/test_conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3441 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10125 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/test_dnsutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/test_heartbeat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4186 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/test_service_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3066 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/test_upgrade_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16370 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2688 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.188427 designate-9.0.2/designate/tests/unit/workers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/workers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/workers/test_base_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/workers/test_processing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8977 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/workers/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22539 2021-02-16 10:12:08.000000 designate-9.0.2/designate/tests/unit/workers/test_zone_tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12886 2021-02-16 10:12:08.000000 designate-9.0.2/designate/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2021-02-16 10:12:08.000000 designate-9.0.2/designate/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.188427 designate-9.0.2/designate/worker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6504 2021-02-16 10:12:08.000000 designate-9.0.2/designate/worker/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/worker/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2596 2021-02-16 10:12:08.000000 designate-9.0.2/designate/worker/processing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2448 2021-02-16 10:12:08.000000 designate-9.0.2/designate/worker/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6407 2021-02-16 10:12:08.000000 designate-9.0.2/designate/worker/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.188427 designate-9.0.2/designate/worker/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/designate/worker/tasks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3924 2021-02-16 10:12:08.000000 designate-9.0.2/designate/worker/tasks/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21370 2021-02-16 10:12:08.000000 designate-9.0.2/designate/worker/tasks/zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2447 2021-02-16 10:12:08.000000 designate-9.0.2/designate/worker/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.100431 designate-9.0.2/designate.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4010 2021-02-16 10:12:40.000000 designate-9.0.2/designate.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36276 2021-02-16 10:12:41.000000 designate-9.0.2/designate.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-16 10:12:40.000000 designate-9.0.2/designate.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2021-02-16 10:12:40.000000 designate-9.0.2/designate.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-16 10:12:40.000000 designate-9.0.2/designate.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-02-16 10:12:40.000000 designate-9.0.2/designate.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1186 2021-02-16 10:12:40.000000 designate-9.0.2/designate.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2021-02-16 10:12:40.000000 designate-9.0.2/designate.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2021-02-16 10:12:08.000000 designate-9.0.2/designate.sublime-project
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.188427 designate-9.0.2/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.192427 designate-9.0.2/devstack/designate_plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3035 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-agent
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1444 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-agent-fake
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4119 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-agent-knot2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3555 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-agent-msdns
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4356 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-akamai
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5226 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-bind9
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3981 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-designate
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4559 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-dynect
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-fake
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-infoblox
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5538 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-pdns4
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2948 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-pdns4-mysql-db.sql
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2876 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/designate_plugins/backend-pdns4-pgsql-db.sql
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9292 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/exercise.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.192427 designate-9.0.2/devstack/gate/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      784 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/gate/gate_hook.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2216 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/gate/post_test_hook.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1014 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/gate/run_cli_tests.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1212 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/gate/run_tempest_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21224 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/networking_test.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      121 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/networking_test_monitor_tc.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13878 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4001 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/settings
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1914 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/statsd_mock_server.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.192427 designate-9.0.2/devstack/upgrade/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5185 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/upgrade/resources.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/upgrade/settings
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      748 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/upgrade/shutdown.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3527 2021-02-16 10:12:08.000000 designate-9.0.2/devstack/upgrade/upgrade.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.192427 designate-9.0.2/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.196426 designate-9.0.2/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/doc/ext/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.196426 designate-9.0.2/doc/ext/assets/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2021-02-16 10:12:08.000000 designate-9.0.2/doc/ext/assets/support-matrix.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2021-02-16 10:12:08.000000 designate-9.0.2/doc/ext/assets/support-matrix.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2021-02-16 10:12:08.000000 designate-9.0.2/doc/ext/custom_css.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15252 2021-02-16 10:12:08.000000 designate-9.0.2/doc/ext/support_matrix.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2021-02-16 10:12:08.000000 designate-9.0.2/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.196426 designate-9.0.2/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.196426 designate-9.0.2/doc/source/_extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/_extra/.htaccess
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.196426 designate-9.0.2/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.200426 designate-9.0.2/doc/source/admin/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.200426 designate-9.0.2/doc/source/admin/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/agent.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/bind9.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3938 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/djbdns_agent.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3397 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/gdnsd_agent.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3423 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/infoblox.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5199 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/knot2_agent.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4412 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/msdns_agent.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2746 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/pdns4.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.200426 designate-9.0.2/doc/source/admin/backends/sample_yaml_snippets/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/sample_yaml_snippets/agent.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/sample_yaml_snippets/bind.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/backends/sample_yaml_snippets/pdns4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3015 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/blacklists.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6656 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/ha.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6107 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/multiple-pools.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1710 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/notifications.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3063 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/pool-scheduler.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4650 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/pools.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4709 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/production-guidelines.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6200 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/quotas.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.200426 designate-9.0.2/doc/source/admin/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/samples/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/samples/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/samples/policy-yaml.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/support-matrix.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/support-matrix.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2157 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/tlds.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4572 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/troubleshooting.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.204426 designate-9.0.2/doc/source/admin/upgrades/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/upgrades/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/upgrades/kilo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2899 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/upgrades/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4489 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/upgrades/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1515 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/admin/upgrades/ocata.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.204426 designate-9.0.2/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6133 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/cli/designate-manage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2110 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/cli/designate-status.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9277 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.204426 designate-9.0.2/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1698 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.204426 designate-9.0.2/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5435 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7272 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/devstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6413 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/getting-involved.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15898 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/gmr.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3259 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/integrations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/metrics.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1564 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/related.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.208426 designate-9.0.2/doc/source/contributor/sourcedoc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/sourcedoc/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/sourcedoc/backend.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/sourcedoc/central.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/sourcedoc/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/sourcedoc/mdns.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3314 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/sourcedoc/objects.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/sourcedoc/quota.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/sourcedoc/sink.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/sourcedoc/storage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7649 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/contributor/ubuntu-dev.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.208426 designate-9.0.2/doc/source/diagrams/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/diagrams/Designate-MultiZone.dia
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/diagrams/Designate-PowerDNS-Detail.dia
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3028 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/diagrams/Designate-Simple.dia
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/diagrams/README
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.208426 designate-9.0.2/doc/source/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1309 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/examples/basic-pools-sample.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.208426 designate-9.0.2/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35901 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/images/Designate-Arch.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36741 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/images/Designate-MultiZone.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44979 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/images/Designate-PowerDNS-Detail.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    96455 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/images/Designate-Simple.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.208426 designate-9.0.2/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/install/common_prerequisites.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5108 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/install/create-zone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/install/get_started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      624 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6511 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/install/install-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6388 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/install/install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6384 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/install/install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/install/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/install/next-steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2340 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/install/verify.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.212426 designate-9.0.2/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9397 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/user/manage-ptr-records.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.068432 designate-9.0.2/doc/source/user/rest/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.212426 designate-9.0.2/doc/source/user/rest/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3700 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/user/rest/admin/quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/user/rest.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2021-02-16 10:12:08.000000 designate-9.0.2/doc/source/user/secondary-zones.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.068432 designate-9.0.2/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.212426 designate-9.0.2/etc/designate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/README-designate.conf.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/api-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/designate-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/designate-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8374 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/policy.yaml.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/pools.yaml.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/pools.yaml.sample-bind
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/pools.yaml.sample-infoblox
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3278 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/pools.yaml.sample-multiple-pools
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/rootwrap.conf.sample
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.212426 designate-9.0.2/etc/designate/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/rootwrap.d/bind9.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/rootwrap.d/djbdns.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-02-16 10:12:08.000000 designate-9.0.2/etc/designate/rootwrap.d/knot2.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2021-02-16 10:12:08.000000 designate-9.0.2/ipa-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3017 2021-02-16 10:12:08.000000 designate-9.0.2/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.068432 designate-9.0.2/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.212426 designate-9.0.2/playbooks/designate-bind9/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-02-16 10:12:08.000000 designate-9.0.2/playbooks/designate-bind9/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.212426 designate-9.0.2/playbooks/designate-pdns4/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2021-02-16 10:12:08.000000 designate-9.0.2/playbooks/designate-pdns4/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.068432 designate-9.0.2/playbooks/legacy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.212426 designate-9.0.2/playbooks/legacy/grenade-devstack-designate-pdns4/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-16 10:12:08.000000 designate-9.0.2/playbooks/legacy/grenade-devstack-designate-pdns4/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2385 2021-02-16 10:12:08.000000 designate-9.0.2/playbooks/legacy/grenade-devstack-designate-pdns4/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.216426 designate-9.0.2/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2021-02-16 10:12:08.000000 designate-9.0.2/rally-jobs/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2021-02-16 10:12:08.000000 designate-9.0.2/rally-jobs/designate-designate.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.216426 designate-9.0.2/rally-jobs/extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-02-16 10:12:08.000000 designate-9.0.2/rally-jobs/extra/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.216426 designate-9.0.2/rally-jobs/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-02-16 10:12:08.000000 designate-9.0.2/rally-jobs/plugins/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/rally-jobs/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.068432 designate-9.0.2/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/CAA_NAPTR_records-5e2e466a5bc18a31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/agent-port-number-c28462562a74cbf9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/api-dot-json-324038360202e86b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/api-mdns-multiple-bind-c78853de46ee587d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/attribute-filter-f06a53b61f5fd111.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/bug-1755788-txt-spf-validation-d18e43c12691132a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/bug-1768824-service_statuses-constraint-7a30eb78dc63b86f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/bug-1827070-service_status-multiple-workers-cf99fe9e4eaf57ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/bug-1828534-ensure-coordination-ids-are-encoded-b5f32b9e16339251.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/bug-1832799-allow-topic-override-7540c14a10b8e3ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      612 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/cfg-notification-remove.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/djbdns-agent-backend-c84e9eeab48d2e01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/fix-recordset-status-204e2747ef47d5ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/knot-agent-backend-db2893aa97d85a1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/mini-dns-tcp-c1a15742f5c71739.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/multilevel-tlds-3dadd285fed82715.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/new-service-layer-8023c242de89075a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/newton-rc-1-eddc78fac760b98a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/pdns4-tsig-1fda534c01d90138.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/pluggable-notifications-bd049b755a2ace9c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/policy-in-code-8d3f4f89e2ede50f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/pool-config-db-45a2cad74e22d95e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/pool-listener-6689ffa50345ba6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/pool-manager-disabled-ff8582b5f86d2360.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/pool_scheduler-32e34dda9484ef9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/quotas-validate-project-36a2a88b66bc6d63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/recordset-api-2c82abf569f7623e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/remove-v1-api-e38de408c6454de2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/removed-deprecated-managed-210a00cdaf975b8f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/removed-pool-manager-a1a9466aceb44b9f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/removing-deprectated-pdns-mysql-backend-1babc968f5778ae6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/service-status-ab0e696c8f5fdef8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/soa_refresh_interval_randomization-fcc1d0d63124699b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/stein-upgrade-checkers-cli-b8518126fff82be6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/v1-disabled-ffebc0434fa0665f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/v2-api-quotas-dd7e189cddcf7b96.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/worker-executor-84d983c92dd13b49.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/notes/zone_name-null-zone-trasfer-request-response-a2e316872798d1df.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9184 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.072432 designate-9.0.2/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.072432 designate-9.0.2/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25320 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.072432 designate-9.0.2/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1871 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.072432 designate-9.0.2/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-02-16 10:12:08.000000 designate-9.0.2/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1981 2021-02-16 10:12:08.000000 designate-9.0.2/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.072432 designate-9.0.2/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.072432 designate-9.0.2/roles/bind-logs-conf/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/roles/bind-logs-conf/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-02-16 10:12:08.000000 designate-9.0.2/roles/bind-logs-conf/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/roles/bind-logs-conf/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2021-02-16 10:12:08.000000 designate-9.0.2/roles/bind-logs-conf/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.072432 designate-9.0.2/roles/pdns4-logs-conf/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/roles/pdns4-logs-conf/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-02-16 10:12:08.000000 designate-9.0.2/roles/pdns4-logs-conf/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.224425 designate-9.0.2/roles/pdns4-logs-conf/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2021-02-16 10:12:08.000000 designate-9.0.2/roles/pdns4-logs-conf/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5326 2021-02-16 10:12:41.228425 designate-9.0.2/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-02-16 10:12:08.000000 designate-9.0.2/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2021-02-16 10:12:08.000000 designate-9.0.2/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.228425 designate-9.0.2/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2021-02-16 10:12:08.000000 designate-9.0.2/tools/install_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5959 2021-02-16 10:12:08.000000 designate-9.0.2/tools/install_venv_common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-16 10:12:41.228425 designate-9.0.2/tools/mysql_pending_notify_bench/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3148 2021-02-16 10:12:08.000000 designate-9.0.2/tools/mysql_pending_notify_bench/README
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2420 2021-02-16 10:12:08.000000 designate-9.0.2/tools/mysql_pending_notify_bench/runner
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4497 2021-02-16 10:12:08.000000 designate-9.0.2/tools/pretty_flake8.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      132 2021-02-16 10:12:08.000000 designate-9.0.2/tools/pretty_flake8.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2021-02-16 10:12:08.000000 designate-9.0.2/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6322 2021-02-16 10:12:08.000000 designate-9.0.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `designate-9.0.1/etc/designate/pools.yaml.sample-infoblox` & `designate-9.0.2/etc/designate/pools.yaml.sample-infoblox`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/etc/designate/rootwrap.conf.sample` & `designate-9.0.2/etc/designate/rootwrap.conf.sample`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/etc/designate/policy.yaml.sample` & `designate-9.0.2/etc/designate/policy.yaml.sample`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/etc/designate/pools.yaml.sample-multiple-pools` & `designate-9.0.2/etc/designate/pools.yaml.sample-multiple-pools`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/etc/designate/pools.yaml.sample-bind` & `designate-9.0.2/etc/designate/pools.yaml.sample-bind`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/etc/designate/api-paste.ini` & `designate-9.0.2/etc/designate/api-paste.ini`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/etc/designate/pools.yaml.sample` & `designate-9.0.2/etc/designate/pools.yaml.sample`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/test-requirements.txt` & `designate-9.0.2/test-requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 oslotest>=3.2.0 # Apache-2.0
 requests-mock>=1.2.0 # Apache-2.0
 testtools>=2.2.0 # MIT
 testscenarios>=0.4 # Apache-2.0/BSD
 WebTest>=2.0.27 # MIT
 tempest>=17.1.0 # Apache-2.0
 # Bandit security code scanner
-bandit>=1.1.0 # Apache-2.0
+bandit>=1.1.0,<1.6.3;python_version=='2.7' # Apache-2.0
+bandit>=1.1.0;python_version>='3.5' # Apache-2.0
 zake>=0.1.6 # Apache-2.0
 doc8>=0.6.0 # Apache-2.0
 Pygments>=2.2.0 # BSD license
```

### Comparing `designate-9.0.1/designate.egg-info/PKG-INFO` & `designate-9.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: designate
-Version: 9.0.1
+Version: 9.0.2
 Summary: DNS as a Service
 Home-page: https://docs.openstack.org/designate/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `designate-9.0.1/designate.egg-info/entry_points.txt` & `designate-9.0.2/designate.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate.egg-info/SOURCES.txt` & `designate-9.0.2/designate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate.egg-info/requires.txt` & `designate-9.0.2/designate.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 Babel!=2.4.0,>=2.3.4
-eventlet!=0.18.3,!=0.20.1,!=0.21.0,!=0.23.0,!=0.25.0,>=0.18.2
 Flask!=0.11,>=0.10
-greenlet>=0.4.10
 Jinja2>=2.10
+Paste>=2.0.2
+PasteDeploy>=1.5.0
+SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,>=1.0.10
+WebOb>=1.7.1
+Werkzeug>=0.9
+debtcollector>=1.2.0
+eventlet!=0.18.3,!=0.20.1,!=0.21.0,!=0.23.0,!=0.25.0,>=0.18.2
+futurist>=1.2.0
+greenlet>=0.4.10
 jsonschema>=2.6.0
 keystoneauth1>=3.4.0
 keystonemiddleware>=4.17.0
+monasca-statsd>=1.1.0
 netaddr>=0.7.18
-oslo.config>=5.2.0
+os-win>=3.0.0
 oslo.concurrency>=3.26.0
+oslo.config>=5.2.0
+oslo.context>=2.19.2
+oslo.db>=4.27.0
+oslo.i18n>=3.15.3
+oslo.log>=3.36.0
 oslo.messaging>=5.29.0
 oslo.middleware>=3.31.0
-oslo.log>=3.36.0
+oslo.policy>=1.30.0
 oslo.reports>=1.18.0
 oslo.rootwrap>=5.8.0
 oslo.serialization!=2.19.1,>=2.18.0
 oslo.service!=1.28.1,>=1.24.0
 oslo.upgradecheck>=0.1.0
 oslo.utils>=3.33.0
 oslo.versionedobjects>=1.31.2
-Paste>=2.0.2
-PasteDeploy>=1.5.0
 pbr!=2.1.0,>=2.0.0
 pecan!=1.0.2,!=1.0.3,!=1.0.4,!=1.2,>=1.0.0
 python-designateclient>=2.7.0
 python-neutronclient>=6.7.0
 requests>=2.14.2
-tenacity>=4.4.0
 six>=1.10.0
-SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,>=1.0.10
 sqlalchemy-migrate>=0.11.0
 stevedore>=1.20.0
 suds-jurko>=0.6
-WebOb>=1.7.1
-oslo.db>=4.27.0
-oslo.i18n>=3.15.3
-oslo.context>=2.19.2
-oslo.policy>=1.30.0
-Werkzeug>=0.9
-python-memcached>=1.56
+tenacity>=4.4.0
 tooz>=1.58.0
-debtcollector>=1.2.0
-os-win>=3.0.0
-monasca-statsd>=1.1.0
-futurist>=1.2.0
 
 [:(python_version=='2.7')]
 dnspython>=1.14.0
+python-memcached>=1.56
 
 [:(python_version>='3.0')]
 dnspython3!=1.13.0,!=1.14.0,>=1.12.0
+
+[:(python_version>='3.4')]
+python-memcached>=1.58
```

### Comparing `designate-9.0.1/PKG-INFO` & `designate-9.0.2/designate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: designate
-Version: 9.0.1
+Version: 9.0.2
 Summary: DNS as a Service
 Home-page: https://docs.openstack.org/designate/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `designate-9.0.1/CONTRIBUTING.rst` & `designate-9.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/tox.ini` & `designate-9.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/rally-jobs/designate-designate.yaml` & `designate-9.0.2/rally-jobs/designate-designate.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/rally-jobs/README.rst` & `designate-9.0.2/rally-jobs/README.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `designate-9.0.2/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `designate-9.0.2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `designate-9.0.2/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/source/conf.py` & `designate-9.0.2/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/notes/pool-config-db-45a2cad74e22d95e.yaml` & `designate-9.0.2/releasenotes/notes/pool-config-db-45a2cad74e22d95e.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/notes/api-mdns-multiple-bind-c78853de46ee587d.yaml` & `designate-9.0.2/releasenotes/notes/api-mdns-multiple-bind-c78853de46ee587d.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/notes/newton-rc-1-eddc78fac760b98a.yaml` & `designate-9.0.2/releasenotes/notes/newton-rc-1-eddc78fac760b98a.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/notes/pool-listener-6689ffa50345ba6e.yaml` & `designate-9.0.2/releasenotes/notes/pool-listener-6689ffa50345ba6e.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/notes/pluggable-notifications-bd049b755a2ace9c.yaml` & `designate-9.0.2/releasenotes/notes/pluggable-notifications-bd049b755a2ace9c.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/notes/cfg-notification-remove.yaml` & `designate-9.0.2/releasenotes/notes/cfg-notification-remove.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/notes/policy-in-code-8d3f4f89e2ede50f.yaml` & `designate-9.0.2/releasenotes/notes/policy-in-code-8d3f4f89e2ede50f.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/releasenotes/notes/bug-1828534-ensure-coordination-ids-are-encoded-b5f32b9e16339251.yaml` & `designate-9.0.2/releasenotes/notes/bug-1828534-ensure-coordination-ids-are-encoded-b5f32b9e16339251.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/LICENSE` & `designate-9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/requirements.txt` & `designate-9.0.2/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -40,13 +40,14 @@
 dnspython>=1.14.0;python_version=='2.7' # http://www.dnspython.org/LICENSE
 dnspython3!=1.13.0,!=1.14.0,>=1.12.0;python_version>='3.0' # http://www.dnspython.org/LICENSE
 oslo.db>=4.27.0 # Apache-2.0
 oslo.i18n>=3.15.3 # Apache-2.0
 oslo.context>=2.19.2 # Apache-2.0
 oslo.policy>=1.30.0 # Apache-2.0
 Werkzeug>=0.9 # BSD License
-python-memcached>=1.56 # PSF
+python-memcached>=1.56;python_version=='2.7' # PSF
+python-memcached>=1.58;python_version>='3.4' # PSF
 tooz>=1.58.0 # Apache-2.0
 debtcollector>=1.2.0 # Apache-2.0
 os-win>=3.0.0 # Apache-2.0
 monasca-statsd>=1.1.0 # Apache-2.0
 futurist>=1.2.0 # Apache-2.0
```

### Comparing `designate-9.0.1/setup.cfg` & `designate-9.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/setup.py` & `designate-9.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/.zuul.yaml` & `designate-9.0.2/.zuul.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         c-bak: false
       tox_envlist: all
       tempest_test_regex: |
         designate_tempest_plugin.*
     required-projects: &base_required_projects
       - openstack/designate
       - openstack/designate-dashboard
-      - openstack/designate-tempest-plugin
+      - name: openstack/designate-tempest-plugin
+        override-checkout: 0.7.0
       - openstack/python-designateclient
     timeout: 4200
     irrelevant-files: &base_irrelevant_files
       - ^.*\.rst$
       - ^api-ref/.*$
       - ^doc/.*$
       - ^etc/.*$
@@ -107,15 +108,16 @@
     name: designate-grenade-pdns4
     parent: legacy-dsvm-base
     required-projects:
       - openstack/grenade
       - openstack/devstack-gate
       - openstack/designate
       - openstack/designate-dashboard
-      - openstack/designate-tempest-plugin
+      - name: openstack/designate-tempest-plugin
+        override-checkout: 0.7.0
       - openstack/python-designateclient
     run: playbooks/legacy/grenade-devstack-designate-pdns4/run.yaml
     post-run: playbooks/legacy/grenade-devstack-designate-pdns4/post.yaml
     timeout: 10800
     irrelevant-files:
       - ^.*\.rst$
       - ^api-ref/.*$
```

### Comparing `designate-9.0.1/devstack/upgrade/resources.sh` & `designate-9.0.2/devstack/upgrade/resources.sh`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/upgrade/upgrade.sh` & `designate-9.0.2/devstack/upgrade/upgrade.sh`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/upgrade/shutdown.sh` & `designate-9.0.2/devstack/upgrade/shutdown.sh`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/upgrade/settings` & `designate-9.0.2/devstack/upgrade/settings`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-pdns4-mysql-db.sql` & `designate-9.0.2/devstack/designate_plugins/backend-pdns4-mysql-db.sql`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-dynect` & `designate-9.0.2/devstack/designate_plugins/backend-dynect`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-agent-msdns` & `designate-9.0.2/devstack/designate_plugins/backend-agent-msdns`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-bind9` & `designate-9.0.2/devstack/designate_plugins/backend-bind9`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-agent-fake` & `designate-9.0.2/devstack/designate_plugins/backend-agent-fake`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-infoblox` & `designate-9.0.2/devstack/designate_plugins/backend-infoblox`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-fake` & `designate-9.0.2/devstack/designate_plugins/backend-fake`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-agent-knot2` & `designate-9.0.2/devstack/designate_plugins/backend-agent-knot2`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-pdns4` & `designate-9.0.2/devstack/designate_plugins/backend-pdns4`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-agent` & `designate-9.0.2/devstack/designate_plugins/backend-agent`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-pdns4-pgsql-db.sql` & `designate-9.0.2/devstack/designate_plugins/backend-pdns4-pgsql-db.sql`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-akamai` & `designate-9.0.2/devstack/designate_plugins/backend-akamai`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/designate_plugins/backend-designate` & `designate-9.0.2/devstack/designate_plugins/backend-designate`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/statsd_mock_server.py` & `designate-9.0.2/devstack/statsd_mock_server.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/plugin.sh` & `designate-9.0.2/devstack/plugin.sh`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,19 @@
         # bind-utils package provides `dig`
         install_package libcap bind-utils
     fi
 
     git_clone $DESIGNATE_REPO $DESIGNATE_DIR $DESIGNATE_BRANCH
     setup_develop $DESIGNATE_DIR
 
+    # Install reqs for tooz driver
+    if [[ "$DESIGNATE_COORDINATION_URL" =~ "memcached" ]]; then
+        pip_install_gr "pymemcache"
+    fi
+
     install_designate_backend
 }
 
 # install_designateclient - Collect source and prepare
 function install_designateclient {
     if use_library_from_git "python-designateclient"; then
         git_clone_by_name "python-designateclient"
```

### Comparing `designate-9.0.1/devstack/networking_test.py` & `designate-9.0.2/devstack/networking_test.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/README.rst` & `designate-9.0.2/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/gate/post_test_hook.sh` & `designate-9.0.2/devstack/gate/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/gate/gate_hook.sh` & `designate-9.0.2/devstack/gate/gate_hook.sh`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/gate/run_tempest_tests.sh` & `designate-9.0.2/devstack/gate/run_tempest_tests.sh`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/gate/run_cli_tests.sh` & `designate-9.0.2/devstack/gate/run_cli_tests.sh`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/settings` & `designate-9.0.2/devstack/settings`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/devstack/exercise.sh` & `designate-9.0.2/devstack/exercise.sh`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/records_mass_create.py` & `designate-9.0.2/contrib/records_mass_create.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/archive/backends/impl_ipa/auth.py` & `designate-9.0.2/contrib/archive/backends/impl_ipa/auth.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/archive/backends/impl_ipa/__init__.py` & `designate-9.0.2/contrib/archive/backends/impl_ipa/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/archive/backends/impl_multi.py` & `designate-9.0.2/contrib/archive/backends/impl_multi.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/fixleadingzeros.py` & `designate-9.0.2/contrib/fixleadingzeros.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/zoneextractor.py` & `designate-9.0.2/contrib/zoneextractor.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/designate-ext-samplehandler/designate_ext_samplehandler/notification_handler/sample.py` & `designate-9.0.2/contrib/designate-ext-samplehandler/designate_ext_samplehandler/notification_handler/sample.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/designate-ext-samplehandler/designate_ext_samplehandler/version.py` & `designate-9.0.2/contrib/designate-ext-samplehandler/designate_ext_samplehandler/version.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/designate-ext-samplehandler/setup.cfg` & `designate-9.0.2/contrib/designate-ext-samplehandler/setup.cfg`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/designate-ext-samplehandler/setup.py` & `designate-9.0.2/contrib/designate-ext-samplehandler/setup.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/dns_dump_raw.py` & `designate-9.0.2/contrib/dns_dump_raw.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/dns_dump_server.py` & `designate-9.0.2/contrib/dns_dump_server.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/dns_dump_dnspy.py` & `designate-9.0.2/contrib/dns_dump_dnspy.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/consume.py` & `designate-9.0.2/contrib/consume.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/dns_dump_hex_to_text.py` & `designate-9.0.2/contrib/dns_dump_hex_to_text.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/djbdns/tinydns.service` & `designate-9.0.2/contrib/djbdns/tinydns.service`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/djbdns/tinydns.init` & `designate-9.0.2/contrib/djbdns/tinydns.init`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/vagrant/Vagrantfile` & `designate-9.0.2/contrib/vagrant/Vagrantfile`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/vagrant/setup_ubuntu_devstack` & `designate-9.0.2/contrib/vagrant/setup_ubuntu_devstack`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/vagrant/local.conf` & `designate-9.0.2/contrib/vagrant/local.conf`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/contrib/public_suffix_list.dat` & `designate-9.0.2/contrib/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/playbooks/legacy/grenade-devstack-designate-pdns4/run.yaml` & `designate-9.0.2/playbooks/legacy/grenade-devstack-designate-pdns4/run.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/configuration/index.rst` & `designate-9.0.2/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/cli/designate-manage.rst` & `designate-9.0.2/doc/source/cli/designate-manage.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/cli/designate-status.rst` & `designate-9.0.2/doc/source/cli/designate-status.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/examples/basic-pools-sample.yaml` & `designate-9.0.2/doc/source/examples/basic-pools-sample.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/images/Designate-Arch.png` & `designate-9.0.2/doc/source/images/Designate-Arch.png`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/images/Designate-PowerDNS-Detail.png` & `designate-9.0.2/doc/source/images/Designate-PowerDNS-Detail.png`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/images/Designate-MultiZone.png` & `designate-9.0.2/doc/source/images/Designate-MultiZone.png`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/images/Designate-Simple.svg` & `designate-9.0.2/doc/source/images/Designate-Simple.svg`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/user/manage-ptr-records.rst` & `designate-9.0.2/doc/source/user/manage-ptr-records.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/user/secondary-zones.rst` & `designate-9.0.2/doc/source/user/secondary-zones.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/user/rest/admin/quotas.rst` & `designate-9.0.2/doc/source/user/rest/admin/quotas.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/user/rest.rst` & `designate-9.0.2/doc/source/user/rest.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/notifications.rst` & `designate-9.0.2/doc/source/admin/notifications.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/quotas.rst` & `designate-9.0.2/doc/source/admin/quotas.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/multiple-pools.rst` & `designate-9.0.2/doc/source/admin/multiple-pools.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/support-matrix.ini` & `designate-9.0.2/doc/source/admin/support-matrix.ini`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/blacklists.rst` & `designate-9.0.2/doc/source/admin/blacklists.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/pool-scheduler.rst` & `designate-9.0.2/doc/source/admin/pool-scheduler.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/backends/djbdns_agent.rst` & `designate-9.0.2/doc/source/admin/backends/djbdns_agent.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/backends/pdns4.rst` & `designate-9.0.2/doc/source/admin/backends/pdns4.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/backends/knot2_agent.rst` & `designate-9.0.2/doc/source/admin/backends/knot2_agent.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/backends/agent.rst` & `designate-9.0.2/doc/source/admin/backends/agent.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/backends/bind9.rst` & `designate-9.0.2/doc/source/admin/backends/bind9.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/backends/index.rst` & `designate-9.0.2/doc/source/admin/backends/index.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/backends/sample_yaml_snippets/pdns4.yaml` & `designate-9.0.2/doc/source/admin/backends/sample_yaml_snippets/pdns4.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/backends/gdnsd_agent.rst` & `designate-9.0.2/doc/source/admin/backends/gdnsd_agent.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/backends/infoblox.rst` & `designate-9.0.2/doc/source/admin/backends/infoblox.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/backends/msdns_agent.rst` & `designate-9.0.2/doc/source/admin/backends/msdns_agent.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/troubleshooting.rst` & `designate-9.0.2/doc/source/admin/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/upgrades/ocata.rst` & `designate-9.0.2/doc/source/admin/upgrades/ocata.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/upgrades/mitaka.rst` & `designate-9.0.2/doc/source/admin/upgrades/mitaka.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/upgrades/kilo.rst` & `designate-9.0.2/doc/source/admin/upgrades/kilo.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/upgrades/newton.rst` & `designate-9.0.2/doc/source/admin/upgrades/newton.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/production-guidelines.rst` & `designate-9.0.2/doc/source/admin/production-guidelines.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/tlds.rst` & `designate-9.0.2/doc/source/admin/tlds.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/pools.rst` & `designate-9.0.2/doc/source/admin/pools.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/admin/ha.rst` & `designate-9.0.2/doc/source/admin/ha.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/index.rst` & `designate-9.0.2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/ubuntu-dev.rst` & `designate-9.0.2/doc/source/contributor/ubuntu-dev.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/getting-involved.rst` & `designate-9.0.2/doc/source/contributor/getting-involved.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/architecture.rst` & `designate-9.0.2/doc/source/contributor/architecture.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/index.rst` & `designate-9.0.2/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/sourcedoc/backend.rst` & `designate-9.0.2/doc/source/contributor/sourcedoc/backend.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/sourcedoc/objects.rst` & `designate-9.0.2/doc/source/contributor/sourcedoc/objects.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/sourcedoc/mdns.rst` & `designate-9.0.2/doc/source/contributor/sourcedoc/mdns.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/gmr.rst` & `designate-9.0.2/doc/source/contributor/gmr.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/related.rst` & `designate-9.0.2/doc/source/contributor/related.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/devstack.rst` & `designate-9.0.2/doc/source/contributor/devstack.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/contributor/integrations.rst` & `designate-9.0.2/doc/source/contributor/integrations.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/install/install-obs.rst` & `designate-9.0.2/doc/source/install/install-obs.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/install/install-ubuntu.rst` & `designate-9.0.2/doc/source/install/install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/install/verify.rst` & `designate-9.0.2/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/install/install-rdo.rst` & `designate-9.0.2/doc/source/install/install-rdo.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/install/index.rst` & `designate-9.0.2/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/install/common_prerequisites.rst` & `designate-9.0.2/doc/source/install/common_prerequisites.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/install/create-zone.rst` & `designate-9.0.2/doc/source/install/create-zone.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/install/get_started.rst` & `designate-9.0.2/doc/source/install/get_started.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/conf.py` & `designate-9.0.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/diagrams/Designate-PowerDNS-Detail.dia` & `designate-9.0.2/doc/source/diagrams/Designate-PowerDNS-Detail.dia`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/diagrams/Designate-MultiZone.dia` & `designate-9.0.2/doc/source/diagrams/Designate-MultiZone.dia`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/source/diagrams/Designate-Simple.dia` & `designate-9.0.2/doc/source/diagrams/Designate-Simple.dia`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/requirements.txt` & `designate-9.0.2/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/ext/custom_css.py` & `designate-9.0.2/doc/ext/custom_css.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/doc/ext/support_matrix.py` & `designate-9.0.2/doc/ext/support_matrix.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/roles/pdns4-logs-conf/tasks/main.yaml` & `designate-9.0.2/roles/pdns4-logs-conf/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/roles/bind-logs-conf/tasks/main.yaml` & `designate-9.0.2/roles/bind-logs-conf/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/ChangeLog` & `designate-9.0.2/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+9.0.2
+-----
+
+* [stable-only] Cap bandit to 1.6.2 and fix requirements
+* pdns4 backend: check if zone exists before attempting delete
+* fix database sync always get the wrong  value
+* Pin version of designate-tempest-plugin
+* Adding distributed locking to central
+
 9.0.1
 -----
 
 * Fixing services getting stuck on shutdown
 * Improve sink recordset creation
 * Remove unused legacy playbooks
 * Use Tempest 'all' tox env
```

### Comparing `designate-9.0.1/designate/cmd/status.py` & `designate-9.0.2/designate/cmd/status.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/cmd/producer.py` & `designate-9.0.2/designate/cmd/producer.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/cmd/agent.py` & `designate-9.0.2/designate/cmd/agent.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/cmd/sink.py` & `designate-9.0.2/designate/cmd/sink.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/cmd/api.py` & `designate-9.0.2/designate/cmd/api.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/cmd/central.py` & `designate-9.0.2/designate/cmd/central.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/cmd/__init__.py` & `designate-9.0.2/designate/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/cmd/mdns.py` & `designate-9.0.2/designate/cmd/mdns.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/cmd/worker.py` & `designate-9.0.2/designate/cmd/worker.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/cmd/manage.py` & `designate-9.0.2/designate/cmd/manage.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/schema/_validators.py` & `designate-9.0.2/designate/schema/_validators.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/schema/resolvers.py` & `designate-9.0.2/designate/schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/schema/format.py` & `designate-9.0.2/designate/schema/format.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/schema/__init__.py` & `designate-9.0.2/designate/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/schema/validators.py` & `designate-9.0.2/designate/schema/validators.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/private_codes.py` & `designate-9.0.2/designate/backend/private_codes.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_dynect.py` & `designate-9.0.2/designate/backend/impl_dynect.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_bind9.py` & `designate-9.0.2/designate/backend/impl_bind9.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_akamai.py` & `designate-9.0.2/designate/backend/impl_akamai.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_pdns4.py` & `designate-9.0.2/designate/backend/impl_pdns4.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,21 @@
         self.mdns_api.notify_zone_changed(
             context, zone, self.host, self.port, self.timeout,
             self.retry_interval, self.max_retries, self.delay)
 
     def delete_zone(self, context, zone):
         """Delete a DNS zone"""
 
-        try:
-            requests.delete(
-                self._build_url(zone.name),
-                headers=self.headers
-            ).raise_for_status()
-        except requests.HTTPError as e:
-            raise exceptions.Backend(e)
+        # First verify that the zone exists -- If it's not present
+        #  in the backend then we can just declare victory.
+        if self._check_zone_exists(zone):
+            try:
+                requests.delete(
+                    self._build_url(zone.name),
+                    headers=self.headers
+                ).raise_for_status()
+            except requests.HTTPError as e:
+                raise exceptions.Backend(e)
+        else:
+            LOG.warning("Trying to delete zone %s but that zone is not "
+                        "present in the pdns backend. Assuming success.",
+                        zone)
```

### Comparing `designate-9.0.1/designate/backend/agent.py` & `designate-9.0.2/designate/backend/agent.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/agent_backend/impl_bind9.py` & `designate-9.0.2/designate/backend/agent_backend/impl_bind9.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/agent_backend/base.py` & `designate-9.0.2/designate/backend/agent_backend/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/agent_backend/impl_msdns.py` & `designate-9.0.2/designate/backend/agent_backend/impl_msdns.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/agent_backend/impl_djbdns.py` & `designate-9.0.2/designate/backend/agent_backend/impl_djbdns.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/agent_backend/impl_gdnsd.py` & `designate-9.0.2/designate/backend/agent_backend/impl_gdnsd.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/agent_backend/impl_denominator.py` & `designate-9.0.2/designate/backend/agent_backend/impl_denominator.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/agent_backend/impl_fake.py` & `designate-9.0.2/designate/backend/agent_backend/impl_fake.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/agent_backend/__init__.py` & `designate-9.0.2/designate/backend/agent_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/agent_backend/impl_knot2.py` & `designate-9.0.2/designate/backend/agent_backend/impl_knot2.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/base.py` & `designate-9.0.2/designate/backend/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_infoblox/object_manipulator.py` & `designate-9.0.2/designate/backend/impl_infoblox/object_manipulator.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_infoblox/ibexceptions.py` & `designate-9.0.2/designate/backend/impl_infoblox/ibexceptions.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_infoblox/connector.py` & `designate-9.0.2/designate/backend/impl_infoblox/connector.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_infoblox/__init__.py` & `designate-9.0.2/designate/backend/impl_infoblox/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_designate.py` & `designate-9.0.2/designate/backend/impl_designate.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_fake.py` & `designate-9.0.2/designate/backend/impl_fake.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/__init__.py` & `designate-9.0.2/designate/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/backend/impl_nsd4.py` & `designate-9.0.2/designate/backend/impl_nsd4.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/context.py` & `designate-9.0.2/designate/context.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_mx.py` & `designate-9.0.2/designate/objects/rrdata_mx.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/zone.py` & `designate-9.0.2/designate/objects/zone.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_spf.py` & `designate-9.0.2/designate/objects/rrdata_spf.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/pool_target.py` & `designate-9.0.2/designate/objects/pool_target.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/zone_attribute.py` & `designate-9.0.2/designate/objects/zone_attribute.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/pool_ns_record.py` & `designate-9.0.2/designate/objects/pool_ns_record.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/fields.py` & `designate-9.0.2/designate/objects/fields.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/zone_transfer_accept.py` & `designate-9.0.2/designate/objects/zone_transfer_accept.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/floating_ip.py` & `designate-9.0.2/designate/objects/floating_ip.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_naptr.py` & `designate-9.0.2/designate/objects/rrdata_naptr.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/blacklist.py` & `designate-9.0.2/designate/objects/blacklist.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/zone_export.py` & `designate-9.0.2/designate/objects/zone_export.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/pool_attribute.py` & `designate-9.0.2/designate/objects/pool_attribute.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_ptr.py` & `designate-9.0.2/designate/objects/rrdata_ptr.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/record.py` & `designate-9.0.2/designate/objects/record.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_aaaa.py` & `designate-9.0.2/designate/objects/rrdata_aaaa.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/quota.py` & `designate-9.0.2/designate/objects/quota.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/pool_target_master.py` & `designate-9.0.2/designate/objects/pool_target_master.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/recordset.py` & `designate-9.0.2/designate/objects/recordset.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/base.py` & `designate-9.0.2/designate/objects/adapters/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/yaml/pool_target.py` & `designate-9.0.2/designate/objects/adapters/yaml/pool_target.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/yaml/pool_ns_record.py` & `designate-9.0.2/designate/objects/adapters/yaml/pool_ns_record.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/yaml/pool_attribute.py` & `designate-9.0.2/designate/objects/adapters/yaml/pool_attribute.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/yaml/pool_target_master.py` & `designate-9.0.2/designate/objects/adapters/yaml/pool_target_master.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/yaml/base.py` & `designate-9.0.2/designate/objects/adapters/yaml/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/yaml/pool_target_option.py` & `designate-9.0.2/designate/objects/adapters/yaml/pool_target_option.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/yaml/pool_also_notify.py` & `designate-9.0.2/designate/objects/adapters/yaml/pool_also_notify.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/yaml/pool_nameserver.py` & `designate-9.0.2/designate/objects/adapters/yaml/pool_nameserver.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/yaml/pool.py` & `designate-9.0.2/designate/objects/adapters/yaml/pool.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/zone.py` & `designate-9.0.2/designate/objects/adapters/api_v2/zone.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/zone_attribute.py` & `designate-9.0.2/designate/objects/adapters/api_v2/zone_attribute.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/pool_ns_record.py` & `designate-9.0.2/designate/objects/adapters/api_v2/pool_ns_record.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/zone_transfer_accept.py` & `designate-9.0.2/designate/objects/adapters/api_v2/zone_transfer_accept.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/floating_ip.py` & `designate-9.0.2/designate/objects/adapters/api_v2/floating_ip.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/blacklist.py` & `designate-9.0.2/designate/objects/adapters/api_v2/blacklist.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/zone_export.py` & `designate-9.0.2/designate/objects/adapters/api_v2/zone_export.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/pool_attribute.py` & `designate-9.0.2/designate/objects/adapters/api_v2/pool_attribute.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/record.py` & `designate-9.0.2/designate/objects/adapters/api_v2/record.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/quota.py` & `designate-9.0.2/designate/objects/adapters/api_v2/quota.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/recordset.py` & `designate-9.0.2/designate/objects/adapters/api_v2/recordset.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/base.py` & `designate-9.0.2/designate/objects/adapters/api_v2/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/zone_import.py` & `designate-9.0.2/designate/objects/adapters/api_v2/zone_import.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/pool.py` & `designate-9.0.2/designate/objects/adapters/api_v2/pool.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/tld.py` & `designate-9.0.2/designate/objects/adapters/api_v2/tld.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/tsigkey.py` & `designate-9.0.2/designate/objects/adapters/api_v2/tsigkey.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/zone_master.py` & `designate-9.0.2/designate/objects/adapters/api_v2/zone_master.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/validation_error.py` & `designate-9.0.2/designate/objects/adapters/api_v2/validation_error.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/zone_transfer_request.py` & `designate-9.0.2/designate/objects/adapters/api_v2/zone_transfer_request.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/api_v2/service_status.py` & `designate-9.0.2/designate/objects/adapters/api_v2/service_status.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/adapters/__init__.py` & `designate-9.0.2/designate/objects/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/base.py` & `designate-9.0.2/designate/objects/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_txt.py` & `designate-9.0.2/designate/objects/rrdata_txt.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/pool_target_option.py` & `designate-9.0.2/designate/objects/pool_target_option.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_caa.py` & `designate-9.0.2/designate/objects/rrdata_caa.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_cname.py` & `designate-9.0.2/designate/objects/rrdata_cname.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/tenant.py` & `designate-9.0.2/designate/objects/tenant.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/pool_also_notify.py` & `designate-9.0.2/designate/objects/pool_also_notify.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_ns.py` & `designate-9.0.2/designate/objects/rrdata_ns.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/zone_import.py` & `designate-9.0.2/designate/objects/zone_import.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_sshfp.py` & `designate-9.0.2/designate/objects/rrdata_sshfp.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/pool_nameserver.py` & `designate-9.0.2/designate/objects/pool_nameserver.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/server.py` & `designate-9.0.2/designate/objects/server.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/pool.py` & `designate-9.0.2/designate/objects/pool.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_soa.py` & `designate-9.0.2/designate/objects/rrdata_soa.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/__init__.py` & `designate-9.0.2/designate/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_a.py` & `designate-9.0.2/designate/objects/rrdata_a.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/tld.py` & `designate-9.0.2/designate/objects/tld.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/tsigkey.py` & `designate-9.0.2/designate/objects/tsigkey.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/zone_master.py` & `designate-9.0.2/designate/objects/zone_master.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/validation_error.py` & `designate-9.0.2/designate/objects/validation_error.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/zone_transfer_request.py` & `designate-9.0.2/designate/objects/zone_transfer_request.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/rrdata_srv.py` & `designate-9.0.2/designate/objects/rrdata_srv.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/objects/service_status.py` & `designate-9.0.2/designate/objects/service_status.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/hacking/checks.py` & `designate-9.0.2/designate/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/producer/service.py` & `designate-9.0.2/designate/producer/service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/producer/tasks.py` & `designate-9.0.2/designate/producer/tasks.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/service.py` & `designate-9.0.2/designate/service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/notification_handler/fake.py` & `designate-9.0.2/designate/notification_handler/fake.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/notification_handler/base.py` & `designate-9.0.2/designate/notification_handler/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/notification_handler/neutron.py` & `designate-9.0.2/designate/notification_handler/neutron.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/notification_handler/nova.py` & `designate-9.0.2/designate/notification_handler/nova.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/notification_handler/__init__.py` & `designate-9.0.2/designate/notification_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/versions.py` & `designate-9.0.2/designate/api/versions.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/zones/nameservers.py` & `designate-9.0.2/designate/api/v2/controllers/zones/nameservers.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/zones/tasks/exports.py` & `designate-9.0.2/designate/api/v2/controllers/zones/tasks/exports.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/zones/tasks/imports.py` & `designate-9.0.2/designate/api/v2/controllers/zones/tasks/imports.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/zones/tasks/abandon.py` & `designate-9.0.2/designate/api/v2/controllers/zones/tasks/abandon.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/zones/tasks/transfer_accepts.py` & `designate-9.0.2/designate/api/v2/controllers/zones/tasks/transfer_accepts.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/zones/tasks/transfer_requests.py` & `designate-9.0.2/designate/api/v2/controllers/zones/tasks/transfer_requests.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/zones/tasks/__init__.py` & `designate-9.0.2/designate/api/v2/controllers/zones/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/zones/tasks/xfr.py` & `designate-9.0.2/designate/api/v2/controllers/zones/tasks/xfr.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/zones/recordsets.py` & `designate-9.0.2/designate/api/v2/controllers/zones/recordsets.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/zones/__init__.py` & `designate-9.0.2/designate/api/v2/controllers/zones/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/pools.py` & `designate-9.0.2/designate/api/v2/controllers/pools.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/blacklists.py` & `designate-9.0.2/designate/api/v2/controllers/blacklists.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/errors.py` & `designate-9.0.2/designate/api/v2/controllers/errors.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/root.py` & `designate-9.0.2/designate/api/v2/controllers/root.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/tsigkeys.py` & `designate-9.0.2/designate/api/v2/controllers/tsigkeys.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/common.py` & `designate-9.0.2/designate/api/v2/controllers/common.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/tlds.py` & `designate-9.0.2/designate/api/v2/controllers/tlds.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/rest.py` & `designate-9.0.2/designate/api/v2/controllers/rest.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/limits.py` & `designate-9.0.2/designate/api/v2/controllers/limits.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/recordsets.py` & `designate-9.0.2/designate/api/v2/controllers/recordsets.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/floatingips.py` & `designate-9.0.2/designate/api/v2/controllers/floatingips.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/quotas.py` & `designate-9.0.2/designate/api/v2/controllers/quotas.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/reverse.py` & `designate-9.0.2/designate/api/v2/controllers/reverse.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/controllers/service_status.py` & `designate-9.0.2/designate/api/v2/controllers/service_status.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/patches.py` & `designate-9.0.2/designate/api/v2/patches.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/__init__.py` & `designate-9.0.2/designate/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/v2/app.py` & `designate-9.0.2/designate/api/v2/app.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/service.py` & `designate-9.0.2/designate/api/service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/middleware.py` & `designate-9.0.2/designate/api/middleware.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/views/extensions/reports.py` & `designate-9.0.2/designate/api/admin/views/extensions/reports.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/views/extensions/quotas.py` & `designate-9.0.2/designate/api/admin/views/extensions/quotas.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/views/base.py` & `designate-9.0.2/designate/api/admin/views/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/controllers/extensions/tenants.py` & `designate-9.0.2/designate/api/admin/controllers/extensions/tenants.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/controllers/extensions/target_sync.py` & `designate-9.0.2/designate/api/admin/controllers/extensions/target_sync.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/controllers/extensions/reports.py` & `designate-9.0.2/designate/api/admin/controllers/extensions/reports.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/controllers/extensions/zones.py` & `designate-9.0.2/designate/api/admin/controllers/extensions/zones.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/controllers/extensions/export.py` & `designate-9.0.2/designate/api/admin/controllers/extensions/export.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/controllers/extensions/quotas.py` & `designate-9.0.2/designate/api/admin/controllers/extensions/quotas.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/controllers/extensions/counts.py` & `designate-9.0.2/designate/api/admin/controllers/extensions/counts.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/controllers/root.py` & `designate-9.0.2/designate/api/admin/controllers/root.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/__init__.py` & `designate-9.0.2/designate/api/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/api/admin/app.py` & `designate-9.0.2/designate/api/admin/app.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/i18n.py` & `designate-9.0.2/designate/i18n.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/policy.py` & `designate-9.0.2/designate/policy.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/locale/en_GB/LC_MESSAGES/designate.po` & `designate-9.0.2/designate/locale/en_GB/LC_MESSAGES/designate.po`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/worker/processing.py` & `designate-9.0.2/designate/worker/processing.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/worker/service.py` & `designate-9.0.2/designate/worker/service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/worker/README.md` & `designate-9.0.2/designate/worker/README.md`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/worker/tasks/zone.py` & `designate-9.0.2/designate/worker/tasks/zone.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/worker/tasks/base.py` & `designate-9.0.2/designate/worker/tasks/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/worker/rpcapi.py` & `designate-9.0.2/designate/worker/rpcapi.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/worker/utils.py` & `designate-9.0.2/designate/worker/utils.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/plugin.py` & `designate-9.0.2/designate/plugin.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/infoblox.py` & `designate-9.0.2/designate/conf/infoblox.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/proxy.py` & `designate-9.0.2/designate/conf/proxy.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/producer.py` & `designate-9.0.2/designate/conf/producer.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/agent.py` & `designate-9.0.2/designate/conf/agent.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/network_api.py` & `designate-9.0.2/designate/conf/network_api.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/sink.py` & `designate-9.0.2/designate/conf/sink.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/bind9.py` & `designate-9.0.2/designate/conf/bind9.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/akamai.py` & `designate-9.0.2/designate/conf/akamai.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/msdns.py` & `designate-9.0.2/designate/conf/msdns.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/base.py` & `designate-9.0.2/designate/conf/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/api.py` & `designate-9.0.2/designate/conf/api.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/gdnsd.py` & `designate-9.0.2/designate/conf/gdnsd.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/denominator.py` & `designate-9.0.2/designate/conf/denominator.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/central.py` & `designate-9.0.2/designate/conf/central.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/keystone.py` & `designate-9.0.2/designate/conf/keystone.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/knot2.py` & `designate-9.0.2/designate/conf/knot2.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/djbdns.py` & `designate-9.0.2/designate/conf/djbdns.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/storage.py` & `designate-9.0.2/designate/conf/storage.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/opts.py` & `designate-9.0.2/designate/conf/opts.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/heartbeat_emitter.py` & `designate-9.0.2/designate/conf/heartbeat_emitter.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/metrics.py` & `designate-9.0.2/designate/conf/metrics.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/__init__.py` & `designate-9.0.2/designate/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/dynect.py` & `designate-9.0.2/designate/conf/dynect.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/mdns.py` & `designate-9.0.2/designate/conf/mdns.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/coordination.py` & `designate-9.0.2/designate/conf/coordination.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/conf/worker.py` & `designate-9.0.2/designate/conf/worker.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/scheduler/filters/random_filter.py` & `designate-9.0.2/designate/scheduler/filters/random_filter.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/scheduler/filters/pool_id_attribute_filter.py` & `designate-9.0.2/designate/scheduler/filters/pool_id_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/scheduler/filters/in_doubt_default_pool_filter.py` & `designate-9.0.2/designate/scheduler/filters/in_doubt_default_pool_filter.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/scheduler/filters/fallback_filter.py` & `designate-9.0.2/designate/scheduler/filters/fallback_filter.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/scheduler/filters/attribute_filter.py` & `designate-9.0.2/designate/scheduler/filters/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/scheduler/filters/base.py` & `designate-9.0.2/designate/scheduler/filters/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/scheduler/filters/default_pool_filter.py` & `designate-9.0.2/designate/scheduler/filters/default_pool_filter.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/scheduler/base.py` & `designate-9.0.2/designate/scheduler/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/scheduler/__init__.py` & `designate-9.0.2/designate/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/sink/service.py` & `designate-9.0.2/designate/sink/service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/network_api/fake.py` & `designate-9.0.2/designate/network_api/fake.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/network_api/base.py` & `designate-9.0.2/designate/network_api/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/network_api/neutron.py` & `designate-9.0.2/designate/network_api/neutron.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/network_api/__init__.py` & `designate-9.0.2/designate/network_api/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/metrics_client/noop.py` & `designate-9.0.2/designate/metrics_client/noop.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/base.py` & `designate-9.0.2/designate/storage/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/tables.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/tables.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/091_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/087_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/072_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/071_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/095_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/088_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/073_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/072_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/088_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/089_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/102_support_caa_records.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/102_support_caa_records.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/087_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/090_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/079_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/073_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/084_add_delayed_notify_column.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/084_add_delayed_notify_column.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/101_support_naptr_records.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/101_support_naptr_records.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/070_liberty.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/070_liberty.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 from sqlalchemy import (Table, MetaData, Column, String, Text, Integer,
                         SmallInteger, CHAR, DateTime, Enum, Boolean, Unicode,
                         UniqueConstraint, ForeignKeyConstraint, Index)
 
 from oslo_config import cfg
 from oslo_utils import timeutils
 
+from designate.conf import central
 from designate.sqlalchemy.types import UUID
 
 
 CONF = cfg.CONF
+central.register_opts(CONF)
 
 RESOURCE_STATUSES = ['ACTIVE', 'PENDING', 'DELETED', 'ERROR']
 RECORD_TYPES = ['A', 'AAAA', 'CNAME', 'MX', 'SRV', 'TXT', 'SPF', 'NS', 'PTR',
                 'SSHFP', 'SOA']
 TASK_STATUSES = ['ACTIVE', 'PENDING', 'DELETED', 'ERROR', 'COMPLETE']
 TSIG_ALGORITHMS = ['hmac-md5', 'hmac-sha1', 'hmac-sha224', 'hmac-sha256',
                    'hmac-sha384', 'hmac-sha512']
@@ -363,15 +365,15 @@
 def default_shard(context, id_col):
     return int(context.current_parameters[id_col][0:3], 16)
 
 
 def upgrade(migrate_engine):
     metadata.bind = migrate_engine
 
-    default_pool_id = cfg.CONF['service:central'].default_pool_id
+    default_pool_id = CONF['service:central'].default_pool_id
 
     with migrate_engine.begin() as conn:
         if migrate_engine.name == "mysql":
             conn.execute("SET foreign_key_checks = 0;")
 
         pools.create()
         pool_ns_records.create()
```

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/085_add_zone_attributes.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/085_add_zone_attributes.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/094_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/091_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/086_new_pools_tables.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/086_new_pools_tables.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/083_change_managed_column_types.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/083_change_managed_column_types.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/099_add_rrset_indexes_for_filtering_perf.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/099_add_rrset_indexes_for_filtering_perf.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/089_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/092_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/075_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/074_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/081_add_FKs.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/081_add_FKs.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/071_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/075_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/092_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/093_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/097_add_services.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/097_add_services.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/080_domain_to_zone_rename.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/080_domain_to_zone_rename.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/093_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/094_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/074_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/076_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/100_unique_service_status.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/100_unique_service_status.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/078_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/077_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/090_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/095_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/096_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/096_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/098_fix_service_charset.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/098_fix_service_charset.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/077_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/078_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/082_unique_ns_record.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/082_unique_ns_record.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/versions/076_placeholder.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/versions/079_placeholder.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/utils.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/utils.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/migrate.cfg` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/migrate.cfg`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/migrate_repo/manage.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/migrate_repo/manage.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/impl_sqlalchemy/__init__.py` & `designate-9.0.2/designate/storage/impl_sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/storage/__init__.py` & `designate-9.0.2/designate/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/rpc.py` & `designate-9.0.2/designate/rpc.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/mdns/service.py` & `designate-9.0.2/designate/mdns/service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/mdns/base.py` & `designate-9.0.2/designate/mdns/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/mdns/rpcapi.py` & `designate-9.0.2/designate/mdns/rpcapi.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/mdns/notify.py` & `designate-9.0.2/designate/mdns/notify.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/mdns/xfr.py` & `designate-9.0.2/designate/mdns/xfr.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/mdns/handler.py` & `designate-9.0.2/designate/mdns/handler.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/resources/schemas/admin/quota.json` & `designate-9.0.2/designate/resources/schemas/admin/quota.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/resources/wsdl/EnhancedDNS.xml` & `designate-9.0.2/designate/resources/wsdl/EnhancedDNS.xml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/resources/templates/bind9-zone.jinja2` & `designate-9.0.2/designate/resources/templates/bind9-zone.jinja2`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/notifications.py` & `designate-9.0.2/designate/notifications.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/central/service.py` & `designate-9.0.2/designate/central/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 import six
 from eventlet import tpool
 from dns import zone as dnszone
 from dns import exception as dnsexception
 from oslo_config import cfg
 import oslo_messaging as messaging
 from oslo_log import log as logging
-from oslo_concurrency import lockutils
 
 from designate import context as dcontext
+from designate import coordination
 from designate import exceptions
 from designate import dnsutils
 from designate import network_api
 from designate import notifications
 from designate import objects
 from designate import policy
 from designate import quota
@@ -113,15 +113,15 @@
             else:
                 raise Exception('Failed to determine zone id for '
                                 'synchronized operation')
 
             if zone_id in ZONE_LOCKS.held:
                 return f(self, *args, **kwargs)
 
-            with lockutils.lock(lock_name):
+            with self.coordination.get_lock(lock_name):
                 try:
                     ZONE_LOCKS.held.add(zone_id)
                     return f(self, *args, **kwargs)
                 finally:
                     ZONE_LOCKS.held.remove(zone_id)
 
         sync_wrapper.__wrapped_function = f
@@ -194,14 +194,18 @@
         self._quota = None
 
         super(Service, self).__init__(
             self.service_name, cfg.CONF['service:central'].topic,
             threads=cfg.CONF['service:central'].threads,
         )
 
+        self.coordination = coordination.Coordination(
+            self.service_name, self.tg
+        )
+
         self.network_api = network_api.get_network_api(cfg.CONF.network_api)
 
     @property
     def scheduler(self):
         if not self._scheduler:
             # Get a scheduler instance
             self._scheduler = scheduler.get_scheduler(storage=self.storage)
@@ -229,16 +233,18 @@
     def start(self):
         if (cfg.CONF['service:central'].managed_resource_tenant_id ==
                 "00000000-0000-0000-0000-000000000000"):
             LOG.warning("Managed Resource Tenant ID is not properly "
                         "configured")
 
         super(Service, self).start()
+        self.coordination.start()
 
     def stop(self, graceful=True):
+        self.coordination.stop()
         super(Service, self).stop(graceful)
 
     @property
     def mdns_api(self):
         return mdns_rpcapi.MdnsAPI.get_instance()
 
     @property
```

### Comparing `designate-9.0.1/designate/central/rpcapi.py` & `designate-9.0.2/designate/central/rpcapi.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_central/test_decorator.py` & `designate-9.0.2/designate/tests/test_central/test_decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,54 +5,64 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
+import mock
+from oslo_concurrency import lockutils
 from oslo_log import log as logging
 
 from designate import exceptions
 from designate import utils
 from designate.central import service
 from designate.objects import record
 from designate.objects import zone
 from designate.tests.test_central import CentralTestCase
 
 LOG = logging.getLogger(__name__)
 
 
+class FakeCoordination(object):
+    def get_lock(self, name):
+        return lockutils.lock(name)
+
+
 class CentralDecoratorTests(CentralTestCase):
     def test_synchronized_zone_exception_raised(self):
         @service.synchronized_zone()
         def mock_get_zone(cls, index, zone):
             self.assertEqual(service.ZONE_LOCKS.held, {zone.id})
             if index % 3 == 0:
                 raise exceptions.ZoneNotFound()
 
         for index in range(9):
             try:
-                mock_get_zone(object, index,
+                mock_get_zone(mock.Mock(coordination=FakeCoordination()),
+                              index,
                               zone.Zone(id=utils.generate_uuid()))
             except exceptions.ZoneNotFound:
                 pass
 
     def test_synchronized_zone_recursive_decorator_call(self):
         @service.synchronized_zone()
         def mock_create_record(cls, context, record):
             self.assertEqual(service.ZONE_LOCKS.held, {record.zone_id})
             mock_get_zone(cls, context, zone.Zone(id=record.zone_id))
 
         @service.synchronized_zone()
         def mock_get_zone(cls, context, zone):
             self.assertEqual(service.ZONE_LOCKS.held, {zone.id})
 
-        mock_create_record(object, self.get_context(),
+        mock_create_record(mock.Mock(coordination=FakeCoordination()),
+                           self.get_context(),
                            record=record.Record(zone_id=utils.generate_uuid()))
-        mock_get_zone(object, self.get_context(),
+        mock_get_zone(mock.Mock(coordination=FakeCoordination()),
+                      self.get_context(),
                       zone=zone.Zone(id=utils.generate_uuid()))
 
     def test_synchronized_zone_raises_exception_when_no_zone_provided(self):
         @service.synchronized_zone(new_zone=False)
         def mock_not_creating_new_zone(cls, context, record):
             pass
```

### Comparing `designate-9.0.1/designate/tests/test_central/__init__.py` & `designate-9.0.2/designate/tests/test_central/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_central/test_service.py` & `designate-9.0.2/designate/tests/test_central/test_service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_producer/test_tasks.py` & `designate-9.0.2/designate/tests/test_producer/test_tasks.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_producer/test_service.py` & `designate-9.0.2/designate/tests/test_producer/test_service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_quota/test_storage.py` & `designate-9.0.2/designate/tests/test_quota/test_storage.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_quota/test_quota.py` & `designate-9.0.2/designate/tests/test_quota/test_quota.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_mdns/test_notify.py` & `designate-9.0.2/designate/tests/test_mdns/test_notify.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_mdns/test_handler.py` & `designate-9.0.2/designate/tests/test_mdns/test_handler.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_mdns/__init__.py` & `designate-9.0.2/designate/tests/test_mdns/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_mdns/test_service.py` & `designate-9.0.2/designate/tests/test_mdns/test_service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_middleware.py` & `designate-9.0.2/designate/tests/test_api/test_middleware.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_zone_transfers.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_zone_transfers.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_floatingips.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_floatingips.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_import_export.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_import_export.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_blacklists.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_blacklists.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_zones.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_zones.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_limits.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_limits.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_tlds.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_tlds.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_pools.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_pools.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_tsigkeys.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_tsigkeys.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_service_status.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_service_status.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_hostheaders.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_hostheaders.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/test_recordsets.py` & `designate-9.0.2/designate/tests/test_api/test_v2/test_recordsets.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_v2/__init__.py` & `designate-9.0.2/designate/tests/test_api/test_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_admin/extensions/test_quotas.py` & `designate-9.0.2/designate/tests/test_api/test_admin/extensions/test_quotas.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_admin/extensions/test_reports.py` & `designate-9.0.2/designate/tests/test_api/test_admin/extensions/test_reports.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_admin/__init__.py` & `designate-9.0.2/designate/tests/test_api/test_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/__init__.py` & `designate-9.0.2/designate/tests/test_api/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_api/test_service.py` & `designate-9.0.2/designate/tests/test_api/test_service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/neutron/port.delete.start.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/neutron/port.delete.start.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/neutron/port.create.start.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/neutron/port.create.start.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/neutron/port.delete.end.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/neutron/port.delete.end.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/neutron/port.create.end.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/neutron/port.create.end.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/neutron/floatingip.update.end_associate.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/neutron/floatingip.update.end_associate.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/neutron/floatingip.delete.start.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/neutron/floatingip.delete.start.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/neutron/floatingip.update.end_disassociate.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/neutron/floatingip.update.end_disassociate.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/network.floating_ip.deallocate.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/network.floating_ip.deallocate.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.start.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.start.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/network.floating_ip.associate.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/network.floating_ip.associate.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/compute.instance.create.start.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/compute.instance.create.start.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.scheduled.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.scheduled.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/compute.instance.create.end.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/compute.instance.create.end.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/compute.instance.delete.start.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/compute.instance.delete.start.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.end.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/scheduler.run_instance.end.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/network.floating_ip.allocate.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/network.floating_ip.allocate.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/network.floating_ip.disassociate.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/network.floating_ip.disassociate.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/compute.instance.shutdown.end.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/compute.instance.shutdown.end.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/sample_notifications/nova/compute.instance.shutdown.start.json` & `designate-9.0.2/designate/tests/resources/sample_notifications/nova/compute.instance.shutdown.start.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/pools_yaml/pools.yaml` & `designate-9.0.2/designate/tests/resources/pools_yaml/pools.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/pools_yaml/sample_output.yaml` & `designate-9.0.2/designate/tests/resources/pools_yaml/sample_output.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/pools_yaml/multiple-pools.yaml` & `designate-9.0.2/designate/tests/resources/pools_yaml/multiple-pools.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/zonefiles/two_example.com.zone` & `designate-9.0.2/designate/tests/resources/zonefiles/two_example.com.zone`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/zonefiles/nosoa_example.com.zone` & `designate-9.0.2/designate/tests/resources/zonefiles/nosoa_example.com.zone`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/zonefiles/malformed_example.com.zone` & `designate-9.0.2/designate/tests/resources/zonefiles/malformed_example.com.zone`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/zonefiles/example.com.zone` & `designate-9.0.2/designate/tests/resources/zonefiles/example.com.zone`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/zonefiles/noorigin_example.com.zone` & `designate-9.0.2/designate/tests/resources/zonefiles/noorigin_example.com.zone`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/resources/__init__.py` & `designate-9.0.2/designate/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_backend/__init__.py` & `designate-9.0.2/designate/tests/test_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/test_central/test_notifications.py` & `designate-9.0.2/designate/tests/unit/test_central/test_notifications.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/test_central/test_basic.py` & `designate-9.0.2/designate/tests/unit/test_central/test_basic.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/test_upgrade_checks.py` & `designate-9.0.2/designate/tests/unit/test_upgrade_checks.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/backend/test_nsd4.py` & `designate-9.0.2/designate/tests/unit/backend/test_nsd4.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/backend/test_bind9.py` & `designate-9.0.2/designate/tests/unit/backend/test_bind9.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/backend/test_pdns4.py` & `designate-9.0.2/designate/tests/unit/backend/test_pdns4.py`

 * *Files 5% similar despite different names*

```diff
@@ -281,27 +281,53 @@
         )
 
     @requests_mock.mock()
     def test_delete_zone_success(self, req_mock):
         req_mock.delete(
             '%s/localhost/zones/example.com.' % self.base_address,
         )
+        req_mock.get(
+            '%s/localhost/zones/%s' % (self.base_address, self.zone.name),
+            status_code=200,
+        )
+
+        self.backend.delete_zone(self.context, self.zone)
+
+        self.assertEqual(
+            req_mock.last_request.headers.get('X-API-Key'), 'api_key'
+        )
+
+    @requests_mock.mock()
+    def test_delete_zone_missing(self, req_mock):
+        req_mock.delete(
+            '%s/localhost/zones/example.com.' % self.base_address,
+        )
+
+        # pdns returns 422 if asked about a zone that doesn't exist.
+        req_mock.get(
+            '%s/localhost/zones/%s' % (self.base_address, self.zone.name),
+            status_code=422,
+        )
 
         self.backend.delete_zone(self.context, self.zone)
 
         self.assertEqual(
             req_mock.last_request.headers.get('X-API-Key'), 'api_key'
         )
 
     @requests_mock.mock()
     def test_delete_zone_fail(self, req_mock):
         req_mock.delete(
             '%s/localhost/zones/example.com.' % self.base_address,
             status_code=500,
         )
+        req_mock.get(
+            '%s/localhost/zones/%s' % (self.base_address, self.zone.name),
+            status_code=200,
+        )
 
         self.assertRaisesRegexp(
             exceptions.Backend,
             '500 Server Error: None for url: '
             '%s/localhost/zones' % self.base_address,
             self.backend.delete_zone, self.context, self.zone
         )
```

### Comparing `designate-9.0.1/designate/tests/unit/backend/test_infoblox.py` & `designate-9.0.2/designate/tests/unit/backend/test_infoblox.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/backend/test_agent.py` & `designate-9.0.2/designate/tests/unit/backend/test_agent.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/backend/test_dynect.py` & `designate-9.0.2/designate/tests/unit/backend/test_dynect.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/backend/test_designate.py` & `designate-9.0.2/designate/tests/unit/backend/test_designate.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_caa_object.py` & `designate-9.0.2/designate/tests/unit/objects/test_caa_object.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_recordset.py` & `designate-9.0.2/designate/tests/unit/objects/test_recordset.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_yaml_adapters.py` & `designate-9.0.2/designate/tests/unit/objects/test_yaml_adapters.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_rrdata_txt.py` & `designate-9.0.2/designate/tests/unit/objects/test_rrdata_txt.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_zone.py` & `designate-9.0.2/designate/tests/unit/objects/test_zone.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_naptr_object.py` & `designate-9.0.2/designate/tests/unit/objects/test_naptr_object.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_base.py` & `designate-9.0.2/designate/tests/unit/objects/test_base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_adapters.py` & `designate-9.0.2/designate/tests/unit/objects/test_adapters.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_rrdata_a.py` & `designate-9.0.2/designate/tests/unit/objects/test_rrdata_a.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_rrdata_spf.py` & `designate-9.0.2/designate/tests/unit/objects/test_rrdata_spf.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_mx_object.py` & `designate-9.0.2/designate/tests/unit/objects/test_mx_object.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/objects/test_sshfp_object.py` & `designate-9.0.2/designate/tests/unit/objects/test_sshfp_object.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/producer/test_tasks.py` & `designate-9.0.2/designate/tests/unit/producer/test_tasks.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/producer/test_service.py` & `designate-9.0.2/designate/tests/unit/producer/test_service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/test_context.py` & `designate-9.0.2/designate/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/notification_handler/test_fake.py` & `designate-9.0.2/designate/tests/unit/notification_handler/test_fake.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/api/test_middleware.py` & `designate-9.0.2/designate/tests/unit/api/test_middleware.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/api/test_api_v2.py` & `designate-9.0.2/designate/tests/unit/api/test_api_v2.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/api/test_admin_api.py` & `designate-9.0.2/designate/tests/unit/api/test_admin_api.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/test_conf.py` & `designate-9.0.2/designate/tests/unit/test_conf.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/test_heartbeat.py` & `designate-9.0.2/designate/tests/unit/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/scheduler/test_filters.py` & `designate-9.0.2/designate/tests/unit/scheduler/test_filters.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/scheduler/test_basic.py` & `designate-9.0.2/designate/tests/unit/scheduler/test_basic.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/sink/test_notifications.py` & `designate-9.0.2/designate/tests/unit/sink/test_notifications.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/sink/test_service.py` & `designate-9.0.2/designate/tests/unit/sink/test_service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/workers/test_processing.py` & `designate-9.0.2/designate/tests/unit/workers/test_processing.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/workers/test_base_task.py` & `designate-9.0.2/designate/tests/unit/workers/test_base_task.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/workers/test_zone_tasks.py` & `designate-9.0.2/designate/tests/unit/workers/test_zone_tasks.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/workers/test_service.py` & `designate-9.0.2/designate/tests/unit/workers/test_service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/metrics/test_metrics.py` & `designate-9.0.2/designate/tests/unit/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/mdns/test_notify.py` & `designate-9.0.2/designate/tests/unit/mdns/test_notify.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/mdns/test_handler.py` & `designate-9.0.2/designate/tests/unit/mdns/test_handler.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/mdns/test_service.py` & `designate-9.0.2/designate/tests/unit/mdns/test_service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/test_service_status.py` & `designate-9.0.2/designate/tests/unit/test_service_status.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/utils.py` & `designate-9.0.2/designate/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/__init__.py` & `designate-9.0.2/designate/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/agent/test_handler.py` & `designate-9.0.2/designate/tests/unit/agent/test_handler.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/agent/backends/test_gdnsd.py` & `designate-9.0.2/designate/tests/unit/agent/backends/test_gdnsd.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/agent/backends/test_bind9.py` & `designate-9.0.2/designate/tests/unit/agent/backends/test_bind9.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/agent/backends/test_knot2.py` & `designate-9.0.2/designate/tests/unit/agent/backends/test_knot2.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/agent/backends/test_djbdns.py` & `designate-9.0.2/designate/tests/unit/agent/backends/test_djbdns.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/agent/backends/test_fake.py` & `designate-9.0.2/designate/tests/unit/agent/backends/test_fake.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/agent/backends/__init__.py` & `designate-9.0.2/designate/tests/unit/agent/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/agent/backends/test_msdns.py` & `designate-9.0.2/designate/tests/unit/agent/backends/test_msdns.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/agent/backends/test_denominator.py` & `designate-9.0.2/designate/tests/unit/agent/backends/test_denominator.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/agent/test_service.py` & `designate-9.0.2/designate/tests/unit/agent/test_service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/test_dnsutils.py` & `designate-9.0.2/designate/tests/unit/test_dnsutils.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/unit/test_utils.py` & `designate-9.0.2/designate/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_storage/test_sqlalchemy.py` & `designate-9.0.2/designate/tests/test_storage/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_storage/__init__.py` & `designate-9.0.2/designate/tests/test_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_network_api/test_neutron.py` & `designate-9.0.2/designate/tests/test_network_api/test_neutron.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_schema/test_format.py` & `designate-9.0.2/designate/tests/test_schema/test_format.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_schema/__init__.py` & `designate-9.0.2/designate/tests/test_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_sqlalchemy.py` & `designate-9.0.2/designate/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/__init__.py` & `designate-9.0.2/designate/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_coordination.py` & `designate-9.0.2/designate/tests/test_coordination.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/fixtures.py` & `designate-9.0.2/designate/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_notification_handler/test_neutron.py` & `designate-9.0.2/designate/tests/test_notification_handler/test_neutron.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_notification_handler/test_base.py` & `designate-9.0.2/designate/tests/test_notification_handler/test_base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_notification_handler/__init__.py` & `designate-9.0.2/designate/tests/test_notification_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_notification_handler/test_nova.py` & `designate-9.0.2/designate/tests/test_notification_handler/test_nova.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/tests/test_hookpoints.py` & `designate-9.0.2/designate/tests/test_hookpoints.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/hookpoints.py` & `designate-9.0.2/designate/hookpoints.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/version.py` & `designate-9.0.2/designate/version.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/loggingutils.py` & `designate-9.0.2/designate/loggingutils.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/utils.py` & `designate-9.0.2/designate/utils.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/config.py` & `designate-9.0.2/designate/common/config.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/zone.py` & `designate-9.0.2/designate/common/policies/zone.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/context.py` & `designate-9.0.2/designate/common/policies/context.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/zone_transfer_accept.py` & `designate-9.0.2/designate/common/policies/zone_transfer_accept.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/blacklist.py` & `designate-9.0.2/designate/common/policies/blacklist.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/zone_export.py` & `designate-9.0.2/designate/common/policies/zone_export.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/record.py` & `designate-9.0.2/designate/common/policies/record.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/quota.py` & `designate-9.0.2/designate/common/policies/quota.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/recordset.py` & `designate-9.0.2/designate/common/policies/recordset.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/base.py` & `designate-9.0.2/designate/common/policies/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/diagnostics.py` & `designate-9.0.2/designate/common/policies/diagnostics.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/tenant.py` & `designate-9.0.2/designate/common/policies/tenant.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/zone_import.py` & `designate-9.0.2/designate/common/policies/zone_import.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/pool.py` & `designate-9.0.2/designate/common/policies/pool.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/__init__.py` & `designate-9.0.2/designate/common/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/tld.py` & `designate-9.0.2/designate/common/policies/tld.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/tsigkey.py` & `designate-9.0.2/designate/common/policies/tsigkey.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/zone_transfer_request.py` & `designate-9.0.2/designate/common/policies/zone_transfer_request.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/policies/service_status.py` & `designate-9.0.2/designate/common/policies/service_status.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/common/keystone.py` & `designate-9.0.2/designate/common/keystone.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/metrics.py` & `designate-9.0.2/designate/metrics.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/sqlalchemy/types.py` & `designate-9.0.2/designate/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/sqlalchemy/base.py` & `designate-9.0.2/designate/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/sqlalchemy/utils.py` & `designate-9.0.2/designate/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/sqlalchemy/session.py` & `designate-9.0.2/designate/sqlalchemy/session.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/__init__.py` & `designate-9.0.2/designate/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/dnsutils.py` & `designate-9.0.2/designate/dnsutils.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/exceptions.py` & `designate-9.0.2/designate/exceptions.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/agent/service.py` & `designate-9.0.2/designate/agent/service.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/agent/handler.py` & `designate-9.0.2/designate/agent/handler.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/quota/impl_noop.py` & `designate-9.0.2/designate/quota/impl_noop.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/quota/base.py` & `designate-9.0.2/designate/quota/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/quota/impl_storage.py` & `designate-9.0.2/designate/quota/impl_storage.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/quota/__init__.py` & `designate-9.0.2/designate/quota/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/coordination.py` & `designate-9.0.2/designate/coordination.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import math
 import time
 
+from oslo_concurrency import lockutils
 from oslo_log import log
 import tenacity
 import tooz.coordination
 
 import designate.conf
 from designate.utils import generate_uuid
 
@@ -47,14 +48,22 @@
     def coordinator(self):
         return self._coordinator
 
     @property
     def started(self):
         return self._started
 
+    def get_lock(self, name):
+        if self._coordinator:
+            # NOTE(eandersson): Workaround until tooz handles the conversion.
+            if not isinstance(name, bytes):
+                name = name.encode('ascii')
+            return self._coordinator.get_lock(name)
+        return lockutils.lock(name)
+
     def start(self):
         self.coordination_id = ":".join([CONF.host, generate_uuid()])
 
         if CONF.coordination.backend_url is not None:
             backend_url = CONF.coordination.backend_url
 
             self._coordinator = tooz.coordination.get_coordinator(
```

### Comparing `designate-9.0.1/designate/manage/base.py` & `designate-9.0.2/designate/manage/base.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/manage/tlds.py` & `designate-9.0.2/designate/manage/tlds.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/manage/pool.py` & `designate-9.0.2/designate/manage/pool.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/manage/database.py` & `designate-9.0.2/designate/manage/database.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate/service_status.py` & `designate-9.0.2/designate/service_status.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/AUTHORS` & `designate-9.0.2/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Alexander Maretskiy <amaretskiy@mirantis.com>
 Alexandra Settle <a.settle@outlook.com>
 Alexandra Settle <asettle@suse.com>
 Alin Balutoiu <abalutoiu@cloudbasesolutions.com>
 Alok Jani <alokjani.web@gmail.com>
 Andreas Jaeger <aj@suse.com>
 Andreas Jaeger <aj@suse.de>
+Andrew Bogott <abogott@wikimedia.org>
 Andrew Ruthven <puck@catalyst.net.nz>
 Andrew Spiers <andrew@andrewspiers.net>
 Andrey Perminov <d1pro@yandex.ru>
 Angus Lees <gus@inodes.org>
 Anusree <anusree.a04@gmail.com>
 Arjun Baindur <xagent@gmail.com>
 Artom Lifshitz <artom.lifshitz@enovance.com>
@@ -53,14 +54,15 @@
 Dirk Mueller <dirk@dmllr.de>
 Dmitry Galkin <galkindmitrii@gmail.com>
 Doug Hellmann <doug@doughellmann.com>
 Dougal Matthews <dougal@redhat.com>
 Dr. Jens Harbott <j.harbott@x-ion.de>
 Duong Ha-Quang <duonghq@vn.fujitsu.com>
 Elena Ezhova <eezhova@mirantis.com>
+Elod Illes <elod.illes@est.tech>
 Endre Karlson <endre.karlson@gmail.com>
 Endre Karlson <endre.karlson@hp.com>
 Endre Karlson <endre.karlson@hpe.com>
 Eric Larson <eric.larson@rackspace.com>
 Eric Larson <eric@ionrock.org>
 Erik Olof Gunnar Andersson <eandersson@blizzard.com>
 Erik Olof Gunnar Andersson <me@eandersson.net>
@@ -245,13 +247,14 @@
 swetha-chandrasekaran <swetha.chandrasekaran@hp.com>
 taoguo <guotao.bj@inspur.com>
 twm2016 <TM2086@att.com>
 venkatamahesh <venkatamaheshkotha@gmail.com>
 vishal mahajan <vishal.mahajan@nectechnologies.in>
 wangqi <wang.qi@99cloud.net>
 wengjiangang <weng.jiangang@zte.com.cn>
+wu.chunyang <wuchunyang@yovole.com>
 zhang.lei <zhang.lei@99cloud.net>
 zhangdebo <zhangdebo@inspur.com>
 zhangyanxian <zhang.yanxian@zte.com.cn>
 zhangyanxian <zhangyanxianmail@163.com>
 zhouhenglc <zhouhenglc@inspur.com>
 Łukasz Jernaś <deejay1@srem.org>
```

### Comparing `designate-9.0.1/lower-constraints.txt` & `designate-9.0.2/lower-constraints.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,23 +28,23 @@
 dogpile.cache==0.6.5
 dulwich==0.19.0
 enum-compat==0.0.2
 eventlet==0.18.2
 extras==1.0.0
 fasteners==0.14.1
 fixtures==3.0.0
-flake8==2.5.5
+flake8==2.6.0
 Flask==0.10
 funcparserlib==0.3.6
 future==0.16.0
 futurist==1.2.0
 gitdb2==2.0.3
 GitPython==2.1.8
 greenlet==0.4.10
-hacking==0.12.0
+hacking==1.1.0
 idna==2.6
 imagesize==1.0.0
 iso8601==0.1.12
 itsdangerous==0.24
 Jinja2==2.10
 jmespath==0.9.3
 jsonpatch==1.21
@@ -114,15 +114,16 @@
 PyNaCl==1.2.1
 pyparsing==2.2.0
 pyperclip==1.6.0
 python-dateutil==2.7.0
 python-designateclient==2.7.0
 python-editor==1.0.3
 python-keystoneclient==3.15.0
-python-memcached==1.56
+python-memcached==1.56;python_version=='2.7'
+python-memcached==1.58;python_version>='3.4'
 python-mimeparse==1.6.0
 python-neutronclient==6.7.0
 python-subunit==1.2.0
 pytz==2018.3
 PyYAML==3.12
 reno==2.7.0
 repoze.lru==0.7
```

### Comparing `designate-9.0.1/README.rst` & `designate-9.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/tools/mysql_pending_notify_bench/runner` & `designate-9.0.2/tools/mysql_pending_notify_bench/runner`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/tools/mysql_pending_notify_bench/README` & `designate-9.0.2/tools/mysql_pending_notify_bench/README`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/tools/install_venv_common.py` & `designate-9.0.2/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/tools/install_venv.py` & `designate-9.0.2/tools/install_venv.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/tools/pretty_flake8.py` & `designate-9.0.2/tools/pretty_flake8.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-blacklist.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-blacklist.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-zone-ownership-transfer-request.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-zone-ownership-transfer-request.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/parameters.yaml` & `designate-9.0.2/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-tld.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-tld.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-quota.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-quota.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-tsigkey.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-tsigkey.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-zone-export.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-zone-export.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-limits.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-limits.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-zone.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-zone.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/index.rst` & `designate-9.0.2/api-ref/source/index.rst`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/update-zone-response.json` & `designate-9.0.2/api-ref/source/samples/zones/update-zone-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/list-zones-response.json` & `designate-9.0.2/api-ref/source/samples/zones/list-zones-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/show-zone-import-response.json` & `designate-9.0.2/api-ref/source/samples/zones/show-zone-import-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/list-zone-transfer-request-response.json` & `designate-9.0.2/api-ref/source/samples/zones/list-zone-transfer-request-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/list-zone-import-response.json` & `designate-9.0.2/api-ref/source/samples/zones/list-zone-import-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/list-zone-export-response.json` & `designate-9.0.2/api-ref/source/samples/zones/list-zone-export-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/list-zone-transfer-accept-response.json` & `designate-9.0.2/api-ref/source/samples/zones/list-zone-transfer-accept-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/show-zone-export-response.json` & `designate-9.0.2/api-ref/source/samples/zones/show-zone-export-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/create-zone-transfer-accept-response.json` & `designate-9.0.2/api-ref/source/samples/zones/create-zone-transfer-accept-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/zone-response.json` & `designate-9.0.2/api-ref/source/samples/zones/zone-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/zones/delete-zone-response.json` & `designate-9.0.2/api-ref/source/samples/zones/delete-zone-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/blacklists/list-blacklists-response.json` & `designate-9.0.2/api-ref/source/samples/blacklists/list-blacklists-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/reverse_floatingips/list-ptr-record-response.json` & `designate-9.0.2/api-ref/source/samples/reverse_floatingips/list-ptr-record-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/tsigkeys/list-tsigkeys-response.json` & `designate-9.0.2/api-ref/source/samples/tsigkeys/list-tsigkeys-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/recordsets/list-recordset-in-zone-response.json` & `designate-9.0.2/api-ref/source/samples/recordsets/list-recordset-in-zone-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/recordsets/delete-recordset-response.json` & `designate-9.0.2/api-ref/source/samples/recordsets/delete-recordset-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/recordsets/create-mx-recordset-response.json` & `designate-9.0.2/api-ref/source/samples/recordsets/create-mx-recordset-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/recordsets/create-srv-recordset-response.json` & `designate-9.0.2/api-ref/source/samples/recordsets/create-srv-recordset-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/recordsets/create-recordset-response.json` & `designate-9.0.2/api-ref/source/samples/recordsets/create-recordset-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/recordsets/show-recordset-response.json` & `designate-9.0.2/api-ref/source/samples/recordsets/show-recordset-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/recordsets/create-spf-recordset-response.json` & `designate-9.0.2/api-ref/source/samples/recordsets/create-spf-recordset-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/recordsets/list-all-recordset-response.json` & `designate-9.0.2/api-ref/source/samples/recordsets/list-all-recordset-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/recordsets/create-sshfp-recordset-response.json` & `designate-9.0.2/api-ref/source/samples/recordsets/create-sshfp-recordset-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/recordsets/update-recordset-response.json` & `designate-9.0.2/api-ref/source/samples/recordsets/update-recordset-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/service_status/service_status_list.json` & `designate-9.0.2/api-ref/source/samples/service_status/service_status_list.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/tlds/list-tlds-response.json` & `designate-9.0.2/api-ref/source/samples/tlds/list-tlds-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/samples/pools/list-pools-response.json` & `designate-9.0.2/api-ref/source/samples/pools/list-pools-response.json`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-zone-ownership-transfer-accept.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-zone-ownership-transfer-accept.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/status.yaml` & `designate-9.0.2/api-ref/source/status.yaml`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-zone-tasks.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-zone-tasks.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/conf.py` & `designate-9.0.2/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-version.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-version.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-pool.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-pool.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-reverse-floatingips.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-reverse-floatingips.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-service-status.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-service-status.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-recordset.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-recordset.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/api-ref/source/dns-api-v2-zone-import.inc` & `designate-9.0.2/api-ref/source/dns-api-v2-zone-import.inc`

 * *Files identical despite different names*

### Comparing `designate-9.0.1/designate.sublime-project` & `designate-9.0.2/designate.sublime-project`

 * *Files identical despite different names*

