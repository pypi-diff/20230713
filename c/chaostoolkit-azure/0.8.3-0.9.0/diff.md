# Comparing `tmp/chaostoolkit-azure-0.8.3.tar.gz` & `tmp/chaostoolkit-azure-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chaostoolkit-azure-0.8.3.tar", last modified: Thu May 14 11:58:07 2020, max compression
+gzip compressed data, was "dist/chaostoolkit-azure-0.9.0.tar", last modified: Mon Mar 15 21:13:48 2021, max compression
```

## Comparing `chaostoolkit-azure-0.8.3.tar` & `chaostoolkit-azure-0.9.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      163 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaosazure/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaosazure/machine/
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/machine/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1705 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/machine/probes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18854 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/machine/actions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/machine/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaosazure/aks/
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/aks/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3532 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/aks/actions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/aks/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaosazure/common/
--rw-rw-r--   0 travis    (2000) travis    (2000)      905 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/cleanse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1210 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/cloud.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaosazure/common/compute/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3025 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/compute/command.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/compute/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4493 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaosazure/common/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)      238 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/scripts/network_latency.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      532 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/scripts/cpu_stress_test.ps1
--rw-rw-r--   0 travis    (2000) travis    (2000)      280 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/scripts/cpu_stress_test.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/scripts/burn_io.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/scripts/fill_disk.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      300 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/scripts/fill_disk.ps1
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaosazure/common/resources/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2370 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/resources/graph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/resources/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/common/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaosazure/webapp/
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/webapp/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1592 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/webapp/probes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4671 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/webapp/actions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/webapp/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaosazure/auth/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3524 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/auth/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1142 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/auth/authentication.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2809 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaosazure/vmss/
--rw-rw-r--   0 travis    (2000) travis    (2000)      444 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/vmss/records.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/vmss/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      969 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/vmss/probes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17049 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/vmss/actions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/vmss/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3548 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/chaosazure/vmss/fetcher.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10888 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     7772 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/requirements-dev.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaostoolkit_azure.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10888 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaostoolkit_azure.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaostoolkit_azure.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaostoolkit_azure.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaostoolkit_azure.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/chaostoolkit_azure.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      114 2020-05-14 11:58:07.000000 chaostoolkit-azure-0.8.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     5680 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     2122 2020-05-14 11:57:39.000000 chaostoolkit-azure-0.8.3/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      163 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      123 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaosazure/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaosazure/machine/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/machine/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1705 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/machine/probes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18892 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/machine/actions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/machine/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaosazure/aks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/aks/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3532 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/aks/actions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/aks/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaosazure/common/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      905 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/cleanse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1210 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/cloud.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaosazure/common/compute/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3063 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/compute/command.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/compute/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4493 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaosazure/common/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      238 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/scripts/network_latency.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      532 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/scripts/cpu_stress_test.ps1
+-rw-rw-r--   0 travis    (2000) travis    (2000)      280 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/scripts/cpu_stress_test.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/scripts/burn_io.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/scripts/fill_disk.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      300 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/scripts/fill_disk.ps1
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaosazure/common/resources/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2339 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/resources/graph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/resources/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/common/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaosazure/webapp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/webapp/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1592 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/webapp/probes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4766 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/webapp/actions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/webapp/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaosazure/auth/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3524 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/auth/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1142 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/auth/authentication.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3825 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaosazure/vmss/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      444 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/vmss/records.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/vmss/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      969 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/vmss/probes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17144 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/vmss/actions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/vmss/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3586 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/chaosazure/vmss/fetcher.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10888 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7772 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/requirements-dev.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaostoolkit_azure.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10888 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaostoolkit_azure.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaostoolkit_azure.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaostoolkit_azure.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaostoolkit_azure.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      124 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/chaostoolkit_azure.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      176 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/pytest.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)      114 2021-03-15 21:13:48.000000 chaostoolkit-azure-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6132 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2122 2021-03-15 21:13:14.000000 chaostoolkit-azure-0.9.0/setup.py
```

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/machine/probes.py` & `chaostoolkit-azure-0.9.0/chaosazure/machine/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/machine/actions.py` & `chaostoolkit-azure-0.9.0/chaosazure/machine/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from chaoslib.exceptions import FailedActivity
 from chaoslib.types import Configuration, Secrets
 from logzero import logger
 
-from chaosazure import init_client
+from chaosazure import init_compute_management_client
 from chaosazure.common import cleanse
 from chaosazure.common.compute import command
 from chaosazure.machine.constants import RES_TYPE_VM
 from chaosazure.common.resources.graph import fetch_resources
 
 __all__ = ["delete_machines", "stop_machines", "restart_machines",
            "start_machines", "stress_cpu", "fill_disk", "network_latency",
@@ -517,8 +517,8 @@
         logger.debug(
             "Fetched virtual machines: {}".format(
                 [x['name'] for x in machines]))
     return machines
 
 
 def __compute_mgmt_client(secrets, configuration):
-    return init_client(secrets, configuration)
+    return init_compute_management_client(secrets, configuration)
```

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/aks/actions.py` & `chaostoolkit-azure-0.9.0/chaosazure/aks/actions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/common/cleanse.py` & `chaostoolkit-azure-0.9.0/chaosazure/common/cleanse.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/common/cloud.py` & `chaostoolkit-azure-0.9.0/chaosazure/common/cloud.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/common/compute/command.py` & `chaostoolkit-azure-0.9.0/chaosazure/common/compute/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from chaoslib.exceptions import FailedActivity, InterruptExecution
 from logzero import logger
 
-from chaosazure import init_client
+from chaosazure import init_compute_management_client
 from chaosazure.machine.constants import OS_LINUX, OS_WINDOWS, RES_TYPE_VM
 from chaosazure.vmss.constants import RES_TYPE_VMSS_VM
 
 UNSUPPORTED_WINDOWS_SCRIPTS = ['network_latency', 'burn_io']
 
 
 def prepare_path(machine: dict, path: str):
@@ -37,15 +37,15 @@
     with open(file_path) as file_path:
         script_content = file_path.read()
         return command_id, script_content
 
 
 def run(resource_group: str, compute: dict, timeout: int, parameters: dict,
         secrets, configuration):
-    client = init_client(secrets, configuration)
+    client = init_compute_management_client(secrets, configuration)
 
     compute_type = compute.get('type').lower()
     if compute_type == RES_TYPE_VMSS_VM.lower():
         poller = client.virtual_machine_scale_set_vms.run_command(
             resource_group, compute['scale_set'],
             compute['instance_id'], parameters)
```

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/common/config.py` & `chaostoolkit-azure-0.9.0/chaosazure/common/config.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/common/scripts/cpu_stress_test.ps1` & `chaostoolkit-azure-0.9.0/chaosazure/common/scripts/cpu_stress_test.ps1`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/common/resources/graph.py` & `chaostoolkit-azure-0.9.0/chaosazure/common/resources/graph.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from typing import List
 
-from azure.mgmt.resourcegraph.models \
-    import QueryRequest, ErrorResponseException
+from azure.core.exceptions import HttpResponseError
+from azure.mgmt.resourcegraph.models import QueryRequest
 from chaoslib.exceptions import InterruptExecution
 from chaoslib.types import Secrets, Configuration
 from logzero import logger
 
 from chaosazure import init_resource_graph_client
 from chaosazure.common.config import load_configuration
 
@@ -17,18 +17,18 @@
     _query = __query_from(resource_type, input_query)
     _query_request = __query_request_from(_query, configuration)
 
     # prepare resource graph client
     try:
         client = init_resource_graph_client(secrets)
         resources = client.resources(_query_request)
-    except ErrorResponseException as e:
-        msg = e.inner_exception.error.code
-        if e.inner_exception.error.details:
-            for d in e.inner_exception.error.details:
+    except HttpResponseError as e:
+        msg = e.error.code
+        if e.error.details:
+            for d in e.error.details:
                 msg += ": " + str(d)
         raise InterruptExecution(msg)
 
     # prepare results
     results = __to_dicts(resources.data, client.api_version)
     return results
```

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/webapp/probes.py` & `chaostoolkit-azure-0.9.0/chaosazure/webapp/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/webapp/actions.py` & `chaostoolkit-azure-0.9.0/chaosazure/webapp/actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 
 from chaoslib import Secrets, Configuration
 from chaoslib.exceptions import FailedActivity
 from logzero import logger
 
-from chaosazure import init_client
+from chaosazure import init_website_management_client
 from chaosazure.common.resources.graph import fetch_resources
 from chaosazure.webapp.constants import RES_TYPE_WEBAPP
 
 
 __all__ = ["stop_webapp", "restart_webapp", "start_webapp", "delete_webapp"]
 
 
@@ -29,15 +29,15 @@
     logger.debug(
         "Start stop_webapp: configuration='{}', filter='{}'".format(
             configuration, filter))
 
     choice = __fetch_webapp_at_random(filter, configuration, secrets)
 
     logger.debug("Stopping web app: {}".format(choice['name']))
-    client = init_client(secrets, configuration)
+    client = init_website_management_client(secrets, configuration)
     client.web_apps.stop(choice['resourceGroup'], choice['name'])
 
 
 def restart_webapp(filter: str = None,
                    configuration: Configuration = None,
                    secrets: Secrets = None):
     """
@@ -54,15 +54,15 @@
     logger.debug(
         "Start restart_webapp: configuration='{}', filter='{}'".format(
             configuration, filter))
 
     choice = __fetch_webapp_at_random(filter, configuration, secrets)
 
     logger.debug("Restarting web app: {}".format(choice['name']))
-    client = init_client(secrets, configuration)
+    client = init_website_management_client(secrets, configuration)
     client.web_apps.restart(choice['resourceGroup'], choice['name'])
 
 
 def start_webapp(filter: str = None,
                  configuration: Configuration = None,
                  secrets: Secrets = None):
     """
@@ -79,15 +79,15 @@
     logger.debug(
         "Start start_webapp: configuration='{}', filter='{}'".format(
             configuration, filter))
 
     choice = __fetch_webapp_at_random(filter, configuration, secrets)
 
     logger.debug("Starting web app: {}".format(choice['name']))
-    client = init_client(secrets, configuration)
+    client = init_website_management_client(secrets, configuration)
     client.web_apps.start(choice['resourceGroup'], choice['name'])
 
 
 def delete_webapp(filter: str = None,
                   configuration: Configuration = None,
                   secrets: Secrets = None):
     """
@@ -107,15 +107,15 @@
     logger.debug(
         "Start delete_webapp: configuration='{}', filter='{}'".format(
             configuration, filter))
 
     choice = __fetch_webapp_at_random(filter, configuration, secrets)
 
     logger.debug("Deleting web app: {}".format(choice['name']))
-    client = init_client(secrets, configuration)
+    client = init_website_management_client(secrets, configuration)
     client.web_apps.delete(choice['resourceGroup'], choice['name'])
 
 
 def fetch_webapps(filter, configuration, secrets):
     webapps = fetch_resources(filter, RES_TYPE_WEBAPP, secrets, configuration)
     if not webapps:
         logger.warning("No web apps found")
```

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/auth/__init__.py` & `chaostoolkit-azure-0.9.0/chaosazure/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/auth/authentication.py` & `chaostoolkit-azure-0.9.0/chaosazure/auth/authentication.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/__init__.py` & `chaostoolkit-azure-0.9.0/chaosazure/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,92 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for chaostoolkit-azure."""
 
 from typing import List
 
 from azure.mgmt.compute import ComputeManagementClient
+from azure.mgmt.web import WebSiteManagementClient
 from azure.mgmt.resourcegraph import ResourceGraphClient
 from chaoslib.discovery import (discover_actions, discover_probes,
                                 initialize_discovery_result)
 from chaoslib.types import (Configuration, DiscoveredActivities, Discovery,
                             Secrets)
 from logzero import logger
 
 from chaosazure.auth import auth
 from chaosazure.common.config import load_configuration, load_secrets
 
 __all__ = [
-    "discover", "__version__", "init_client",
-    "init_resource_graph_client"
+    "discover", "__version__", "init_compute_management_client",
+    "init_website_management_client", "init_resource_graph_client"
 ]
-__version__ = '0.8.3'
+__version__ = '0.9.0'
 
 
 def discover(discover_system: bool = True) -> Discovery:
     """
     Discover Azure capabilities offered by this extension.
     """
     logger.info("Discovering capabilities from chaostoolkit-azure")
 
     discovery = initialize_discovery_result(
         "chaostoolkit-azure", __version__, "azure")
     discovery["activities"].extend(__load_exported_activities())
     return discovery
 
 
-def init_client(
+def init_compute_management_client(
         experiment_secrets: Secrets,
         experiment_configuration: Configuration) -> ComputeManagementClient:
-
+    """
+    Initializes Compute management client for virtual machine,
+    and virtual machine scale sets resources under Azure Resource manager.
+    """
     secrets = load_secrets(experiment_secrets)
     configuration = load_configuration(experiment_configuration)
     with auth(secrets) as authentication:
         base_url = secrets.get('cloud').endpoints.resource_manager
         client = ComputeManagementClient(
             credentials=authentication,
             subscription_id=configuration.get('subscription_id'),
             base_url=base_url)
 
         return client
 
 
+def init_website_management_client(
+        experiment_secrets: Secrets,
+        experiment_configuration: Configuration) -> WebSiteManagementClient:
+    """
+    Initializes Website management client for webapp resource under Azure
+    Resource manager.
+    """
+    secrets = load_secrets(experiment_secrets)
+    configuration = load_configuration(experiment_configuration)
+    with auth(secrets) as authentication:
+        base_url = secrets.get('cloud').endpoints.resource_manager
+        client = WebSiteManagementClient(
+            credentials=authentication,
+            subscription_id=configuration.get('subscription_id'),
+            base_url=base_url)
+
+        return client
+
+
 def init_resource_graph_client(
         experiment_secrets: Secrets) -> ResourceGraphClient:
-
+    """
+    Initializes Resource Graph client.
+    """
     secrets = load_secrets(experiment_secrets)
     with auth(secrets) as authentication:
         base_url = secrets.get('cloud').endpoints.resource_manager
         client = ResourceGraphClient(
-            credentials=authentication,
+            credential=authentication,
             base_url=base_url)
 
         return client
 
 
 ###############################################################################
 # Private functions
```

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/vmss/probes.py` & `chaostoolkit-azure-0.9.0/chaosazure/vmss/probes.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/vmss/actions.py` & `chaostoolkit-azure-0.9.0/chaosazure/vmss/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable, Mapping
 
 from chaoslib import Configuration, Secrets
 from logzero import logger
 
-from chaosazure import init_client
+from chaosazure import init_compute_management_client
 from chaosazure.common import cleanse
 from chaosazure.common.compute import command
 from chaosazure.vmss.fetcher import fetch_vmss, fetch_instances
 from chaosazure.vmss.records import Records
 
 __all__ = [
     "delete_vmss", "restart_vmss", "stop_vmss", "deallocate_vmss",
@@ -44,15 +44,15 @@
         instances_records = Records()
         instances = fetch_instances(scale_set, instance_criteria,
                                     configuration, secrets)
 
         for instance in instances:
             logger.debug(
                 "Deleting instance: {}".format(instance['name']))
-            client = init_client(secrets, configuration)
+            client = init_compute_management_client(secrets, configuration)
             client.virtual_machine_scale_set_vms.delete(
                 scale_set['resourceGroup'],
                 scale_set['name'],
                 instance['instance_id'])
             instances_records.add(cleanse.vmss_instance(instance))
 
         scale_set['virtualMachines'] = instances_records.output()
@@ -86,15 +86,15 @@
         instances_records = Records()
         instances = fetch_instances(scale_set, instance_criteria,
                                     configuration, secrets)
 
         for instance in instances:
             logger.debug(
                 "Restarting instance: {}".format(instance['name']))
-            client = init_client(secrets, configuration)
+            client = init_compute_management_client(secrets, configuration)
             client.virtual_machine_scale_set_vms.restart(
                 scale_set['resourceGroup'],
                 scale_set['name'],
                 instance['instance_id'])
             instances_records.add(cleanse.vmss_instance(instance))
 
         scale_set['virtualMachines'] = instances_records.output()
@@ -150,15 +150,15 @@
         instances_records = Records()
         instances = fetch_instances(scale_set, instance_criteria,
                                     configuration, secrets)
 
         for instance in instances:
             logger.debug(
                 "Stopping instance: {}".format(instance['name']))
-            client = init_client(secrets, configuration)
+            client = init_compute_management_client(secrets, configuration)
             client.virtual_machine_scale_set_vms.power_off(
                 scale_set['resourceGroup'],
                 scale_set['name'],
                 instance['instance_id'])
             instances_records.add(cleanse.vmss_instance(instance))
 
         scale_set['virtualMachines'] = instances_records.output()
@@ -192,15 +192,15 @@
         instances_records = Records()
         instances = fetch_instances(scale_set, instance_criteria,
                                     configuration, secrets)
 
         for instance in instances:
             logger.debug(
                 "Deallocating instance: {}".format(instance['name']))
-            client = init_client(secrets, configuration)
+            client = init_compute_management_client(secrets, configuration)
             client.virtual_machine_scale_set_vms.deallocate(
                 scale_set['resourceGroup'],
                 scale_set['name'],
                 instance['instance_id'])
             instances_records.add(cleanse.vmss_instance(instance))
 
         scale_set['virtualMachines'] = instances_records.output()
```

### Comparing `chaostoolkit-azure-0.8.3/chaosazure/vmss/fetcher.py` & `chaostoolkit-azure-0.9.0/chaosazure/vmss/fetcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 from typing import Any, Dict, Iterable, Mapping, List
 
 from chaoslib import Configuration, Secrets
 from chaoslib.exceptions import FailedActivity
 from logzero import logger
 
-from chaosazure import init_client
+from chaosazure import init_compute_management_client
 from chaosazure.common.resources.graph import fetch_resources
 from chaosazure.vmss.constants import RES_TYPE_VMSS
 
 
 def fetch_instances(scale_set, instance_criteria,
                     configuration, secrets) -> List[Dict[str, Any]]:
     if not instance_criteria:
@@ -58,15 +58,15 @@
 
 
 #############################################################################
 # Private helper functions
 #############################################################################
 def __fetch_vmss_instances(choice, configuration, secrets) -> List[Dict]:
     vmss_instances = []
-    client = init_client(secrets, configuration)
+    client = init_compute_management_client(secrets, configuration)
     pages = client.virtual_machine_scale_set_vms.list(
         choice['resourceGroup'], choice['name'])
     first_page = pages.advance_page()
     vmss_instances.extend(list(first_page))
 
     while True:
         try:
```

### Comparing `chaostoolkit-azure-0.8.3/PKG-INFO` & `chaostoolkit-azure-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-azure
-Version: 0.8.3
+Version: 0.9.0
 Summary: Chaos Toolkit Extension for Microsoft Azure
 Home-page: https://chaostoolkit.org
 Author: chaostoolkit Team
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Description: # Chaos Toolkit Extension for Azure
```

### Comparing `chaostoolkit-azure-0.8.3/README.md` & `chaostoolkit-azure-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/chaostoolkit_azure.egg-info/PKG-INFO` & `chaostoolkit-azure-0.9.0/chaostoolkit_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-azure
-Version: 0.8.3
+Version: 0.9.0
 Summary: Chaos Toolkit Extension for Microsoft Azure
 Home-page: https://chaostoolkit.org
 Author: chaostoolkit Team
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Description: # Chaos Toolkit Extension for Azure
```

### Comparing `chaostoolkit-azure-0.8.3/chaostoolkit_azure.egg-info/SOURCES.txt` & `chaostoolkit-azure-0.9.0/chaostoolkit_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/LICENSE` & `chaostoolkit-azure-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-azure-0.8.3/CHANGELOG.md` & `chaostoolkit-azure-0.9.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 # Changelog
 
 ## [Unreleased][]
-[Unreleased]: https://github.com/chaostoolkit-incubator/chaostoolkit-azure/compare/0.8.3...HEAD
+[Unreleased]: https://github.com/chaostoolkit-incubator/chaostoolkit-azure/compare/0.9.0...HEAD
+
+## [0.9.0][] - 2021-03-15
+
+[0.9.0]: https://github.com/chaostoolkit-incubator/chaostoolkit-azure/compare/0.8.3...0.9.0
+
+### Added
+
+-   Individual Azure managemnt clients for website and compute resources
+
+### Changed
+
+-   Moved to support new Microsoft Azure python package dependencies. Now importt
+    the msrestazure package.
+-   Renamed `credentials` to `credential` for the `ResourceGraphClient` call
+
+### Removed
+
+-   Removed common init_client
 
 ## [0.8.3][] - 2020-05-14
 
 [0.8.3]: https://github.com/chaostoolkit-incubator/chaostoolkit-azure/compare/0.8.2...0.8.3
 
 ### Added
```

### Comparing `chaostoolkit-azure-0.8.3/setup.py` & `chaostoolkit-azure-0.9.0/setup.py`

 * *Files identical despite different names*

