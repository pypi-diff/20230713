# Comparing `tmp/mprov_jobserver-0.0.8.tar.gz` & `tmp/mprov_jobserver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mprov_jobserver-0.0.8.tar", last modified: Tue Aug  2 13:30:41 2022, max compression
+gzip compressed data, was "mprov_jobserver-0.0.9.tar", last modified: Tue Aug  2 22:08:06 2022, max compression
```

## Comparing `mprov_jobserver-0.0.8.tar` & `mprov_jobserver-0.0.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.943327 mprov_jobserver-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-08-02 13:30:41.943327 mprov_jobserver-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-02 13:30:35.000000 mprov_jobserver-0.0.8/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-08-02 13:30:41.943327 mprov_jobserver-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.939327 mprov_jobserver-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.939327 mprov_jobserver-0.0.8/src/mprov_jobserver/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10659 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/jobserver.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/mprov_jobserver
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.943327 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dhcp_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dhcp_update.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dns_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dns_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq.py
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.943327 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq_mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq_mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq_mod/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq_mod/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq_mod/dns.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/iamge-delete.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image-sync.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image-update.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     6252 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     7724 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image_update.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.943327 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image_update_mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image_update_mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6054 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image_update_mod/rhel.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/mprov-webserver.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/mprov_webserver.py
--rw-r--r--   0 runner    (1001) docker     (121)     8572 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/nads.py
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/nads.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/pxe_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/pxe_update.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/repo_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     3216 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/repo_update.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.943327 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/repo_update_mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/repo_update_mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/repo_update_mod/rhel.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/script-runner.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    10046 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/script_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.939327 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.943327 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/dnsmasq/
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/dnsmasq/dhcp.conf.j2
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/dnsmasq/dhcp_host.conf.j2
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/dnsmasq/dns.conf.j2
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/dnsmasq/dns_host.conf.j2
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/dnsmasq/ipxe.conf.j2
--rw-r--r--   0 runner    (1001) docker     (121)     3378 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/dnsmasq/menu.ipxe.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.943327 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/image-update/
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/image-update/script-runner.sh
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-02 13:30:27.000000 mprov_jobserver-0.0.8/src/mprov_jobserver/templates/image-update/script-runner.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:30:41.939327 mprov_jobserver-0.0.8/src/mprov_jobserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-08-02 13:30:41.000000 mprov_jobserver-0.0.8/src/mprov_jobserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-08-02 13:30:41.000000 mprov_jobserver-0.0.8/src/mprov_jobserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 13:30:41.000000 mprov_jobserver-0.0.8/src/mprov_jobserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-08-02 13:30:41.000000 mprov_jobserver-0.0.8/src/mprov_jobserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-02 13:30:41.000000 mprov_jobserver-0.0.8/src/mprov_jobserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.627486 mprov_jobserver-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-08-02 22:08:06.627486 mprov_jobserver-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-02 22:08:00.000000 mprov_jobserver-0.0.9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      763 2022-08-02 22:08:06.627486 mprov_jobserver-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.623486 mprov_jobserver-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.623486 mprov_jobserver-0.0.9/src/mprov_jobserver/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10659 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/jobserver.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/mprov_jobserver
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.627486 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dhcp_delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dhcp_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dns_delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dns_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2691 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq.py
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.627486 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq_mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq_mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq_mod/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq_mod/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq_mod/dns.py
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/iamge-delete.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image-sync.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image-update.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image_delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6252 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7724 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image_update.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.627486 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image_update_mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image_update_mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6054 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image_update_mod/rhel.py
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/mprov-webserver.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      935 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/mprov_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8572 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/nads.py
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/nads.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/pxe_delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/pxe_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/repo_delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3216 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/repo_update.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.627486 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/repo_update_mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/repo_update_mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/repo_update_mod/rhel.py
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/script-runner.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    10697 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/script_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.623486 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.627486 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/dnsmasq/
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/dnsmasq/dhcp.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/dnsmasq/dhcp_host.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/dnsmasq/dns.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/dnsmasq/dns_host.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/dnsmasq/ipxe.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (121)     3378 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/dnsmasq/menu.ipxe.j2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.627486 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/image-update/
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/image-update/script-runner.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-02 22:07:55.000000 mprov_jobserver-0.0.9/src/mprov_jobserver/templates/image-update/script-runner.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 22:08:06.623486 mprov_jobserver-0.0.9/src/mprov_jobserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-08-02 22:08:06.000000 mprov_jobserver-0.0.9/src/mprov_jobserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-08-02 22:08:06.000000 mprov_jobserver-0.0.9/src/mprov_jobserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 22:08:06.000000 mprov_jobserver-0.0.9/src/mprov_jobserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-08-02 22:08:06.000000 mprov_jobserver-0.0.9/src/mprov_jobserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-02 22:08:06.000000 mprov_jobserver-0.0.9/src/mprov_jobserver.egg-info/top_level.txt
```

### Comparing `mprov_jobserver-0.0.8/LICENSE` & `mprov_jobserver-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/PKG-INFO` & `mprov_jobserver-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mprov_jobserver
-Version: 0.0.8
+Version: 0.0.9
 Summary: The job server component of mProv
 Home-page: https://github.com/mprov-ng/mprov_jobserver
 Author: Jason Williams
 Author-email: jasonw@jhu.edu
 Project-URL: Bug Tracker, https://github.com/mprov-ng/mprov_jobserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `mprov_jobserver-0.0.8/README.md` & `mprov_jobserver-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/setup.cfg` & `mprov_jobserver-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/setup.py` & `mprov_jobserver-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/app.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/app.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/jobserver.yaml` & `mprov_jobserver-0.0.9/src/mprov_jobserver/jobserver.yaml`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/main.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/main.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq_mod/config.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq_mod/config.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq_mod/dhcp.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq_mod/dhcp.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/dnsmasq_mod/dns.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/dnsmasq_mod/dns.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image_delete.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image_delete.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image_sync.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image_sync.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image_update.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image_update.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/image_update_mod/rhel.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/image_update_mod/rhel.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/mprov_webserver.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/mprov_webserver.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/nads.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/nads.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/plugin.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/pxe_update.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/pxe_update.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/repo_update.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/repo_update.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/repo_update_mod/rhel.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/repo_update_mod/rhel.py`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/plugins/script_runner.py` & `mprov_jobserver-0.0.9/src/mprov_jobserver/plugins/script_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,40 +108,52 @@
       sysimage = False
       system = True
       entityId = socket.gethostname()
     else:
       print("Error: You must specify -i or -s")
       self.printHelp()
       return False
-
+    entity = None
     if '-b' in sys.argv:
       # someone is asking for post-boot scripts
       scriptMode = 'post-boot'
-    
-    # grab the scripts for this entity.
-    query=""
-    if sysimage:
-      query="systemimages/" + entityId + "/"
+      if not os.path.exists("/tmp/mprov/entity.json"):
+        print("Error: Unable to load /tmp/mprov/entity.json.  Cannot run postboot")
+        sys.exit(1)
+      
+      with open("/tmp/mprov/entity.json", 'r') as entityJSON:
+        entity = json.load(entityJSON)
     else:
-      query="systems/?hostname=" + entityId 
-    # print(self.js.mprovURL + query)
-    response = self.js.session.get( self.js.mprovURL + query)
-    # merge the scripts from distro -> system_groups -> entity
-    try:
-      entity = response.json()
-    except:
-      # if this response was bad, try to grab the nads image 
-      query="systemimages/nads/"
-      response = self.js.session.get( self.js.mprovURL + query )
+      # grab the scripts for this entity.
+      query=""
+      if sysimage:
+        query="systemimages/" + entityId + "/"
+      else:
+        query="systems/?hostname=" + entityId 
+      # print(self.js.mprovURL + query)
+      response = self.js.session.get( self.js.mprovURL + query)
+      # merge the scripts from distro -> system_groups -> entity
       try:
         entity = response.json()
-      except: 
-        print("Error: Unable to get information from mPCC.")
-        exit(1)
+      except:
+        # if this response was bad, try to grab the nads image 
+        query="systemimages/nads/"
+        response = self.js.session.get( self.js.mprovURL + query )
+        try:
+          entity = response.json()
+        except: 
+          print("Error: Unable to get information from mPCC.")
+          exit(1)
 
+    if entity == None:
+      print("Error: Entity Not loaded.")
+      exit(1)
+    if "name" not in entity:
+      print("Error: Corrupted entity found, cannot continue.")
+      exit(1)
     # we should iterate in all the scripts.  Let's process that into a dependancy tree.
     scriptDeps = {}
     scripts = {}
     # osdistro scripts first
     for script in entity['osdistro']['scripts']:
       deps=[]
       if script['scriptType']['slug'] != scriptMode:
@@ -183,45 +195,48 @@
     # distro first
     
     # print(entity['osdistro']['config_params'])
     tmpYamlDict = yaml.safe_load(entity['osdistro']['config_params'])
     if tmpYamlDict is not None:
       try:
         if type(tmpYamlDict) is list:
-          for dict in tmpYamlDict:
-            yaml_merged.update(dict)
+          for dict_entry in tmpYamlDict:
+            yaml_merged.update(dict_entry)
         else: 
             yaml_merged.update(tmpYamlDict)
       except:
         pass
     
     # print(yaml_merged)
     # then the system groups
     for group in entity['systemgroups']:
       # print(group['config_params'])
       tmpYamlDict = yaml.safe_load(group['config_params'])
       if tmpYamlDict is not None:
         try:
           if type(tmpYamlDict) is list:
-            for dict in tmpYamlDict:
-              yaml_merged.update(dict)
+            for dict_entry in tmpYamlDict:
+              yaml_merged.update(dict_entry)
           else:
               yaml_merged.update(tmpYamlDict)
         except:
           pass  
     # and finally the system/image params
     # print(yaml_merged)
     # print(yaml.safe_load(entity['config_params']))
-    tmpYamlDict = yaml.safe_load(entity['config_params'])
+    if type(entity['config_params']) is dict:
+      tmpYamlDict = entity['config_params']
+    else:
+      tmpYamlDict = yaml.safe_load(entity['config_params'])
     # print(tmpYamlDict)
     if tmpYamlDict is not None:
       try:
         if type(tmpYamlDict) is list:
-          for dict in tmpYamlDict:
-            yaml_merged.update(dict)
+          for dict_entry in tmpYamlDict:
+            yaml_merged.update(dict_entry)
         else: 
           yaml_merged.update(tmpYamlDict)
       except:
         pass
               
     # print(yaml_merged)
     entity['config_params'] = yaml_merged
```

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/templates/dnsmasq/dhcp.conf.j2` & `mprov_jobserver-0.0.9/src/mprov_jobserver/templates/dnsmasq/dhcp.conf.j2`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/templates/dnsmasq/ipxe.conf.j2` & `mprov_jobserver-0.0.9/src/mprov_jobserver/templates/dnsmasq/ipxe.conf.j2`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver/templates/dnsmasq/menu.ipxe.j2` & `mprov_jobserver-0.0.9/src/mprov_jobserver/templates/dnsmasq/menu.ipxe.j2`

 * *Files identical despite different names*

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver.egg-info/PKG-INFO` & `mprov_jobserver-0.0.9/src/mprov_jobserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mprov-jobserver
-Version: 0.0.8
+Version: 0.0.9
 Summary: The job server component of mProv
 Home-page: https://github.com/mprov-ng/mprov_jobserver
 Author: Jason Williams
 Author-email: jasonw@jhu.edu
 Project-URL: Bug Tracker, https://github.com/mprov-ng/mprov_jobserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `mprov_jobserver-0.0.8/src/mprov_jobserver.egg-info/SOURCES.txt` & `mprov_jobserver-0.0.9/src/mprov_jobserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

