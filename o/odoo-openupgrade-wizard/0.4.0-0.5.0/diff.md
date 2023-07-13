# Comparing `tmp/odoo-openupgrade-wizard-0.4.0.tar.gz` & `tmp/odoo_openupgrade_wizard-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo-openupgrade-wizard-0.4.0.tar", max compression
+gzip compressed data, was "odoo_openupgrade_wizard-0.5.0.tar", max compression
```

## Comparing `odoo-openupgrade-wizard-0.4.0.tar` & `odoo_openupgrade_wizard-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0    10019 2023-02-28 08:21:53.360949 odoo-openupgrade-wizard-0.4.0/README.md
--rw-r--r--   0        0        0      131 2022-06-16 09:40:44.931869 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/__init__.py
--rw-r--r--   0        0        0      142 2022-06-16 09:40:44.931869 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/__main__.py
--rw-r--r--   0        0        0     4109 2022-10-11 10:38:47.295516 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli.py
--rw-r--r--   0        0        0      546 2022-10-11 10:38:47.295516 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_copydb.py
--rw-r--r--   0        0        0     1825 2023-02-28 08:21:53.360949 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_docker_build.py
--rw-r--r--   0        0        0     2525 2023-02-28 10:04:38.122789 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_estimate_workload.py
--rw-r--r--   0        0        0      866 2022-10-10 09:10:06.188877 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_execute_script_python.py
--rw-r--r--   0        0        0      864 2022-10-10 09:10:06.188877 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_execute_script_sql.py
--rw-r--r--   0        0        0     4618 2022-10-10 09:10:06.188877 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_generate_module_analysis.py
--rw-r--r--   0        0        0      880 2022-10-10 09:10:06.188877 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_get_code.py
--rw-r--r--   0        0        0     5549 2023-01-03 14:06:21.050633 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_init.py
--rw-r--r--   0        0        0     2814 2022-10-11 10:38:47.295516 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_install_from_csv.py
--rw-r--r--   0        0        0     3066 2022-10-10 09:10:06.192877 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_options.py
--rw-r--r--   0        0        0     1900 2023-02-28 08:21:53.360949 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_pull_submodule.py
--rw-r--r--   0        0        0     1981 2022-10-11 10:38:47.295516 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_run.py
--rw-r--r--   0        0        0     1297 2023-03-16 19:57:18.432283 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_upgrade.py
--rw-r--r--   0        0        0     8322 2023-01-03 14:06:21.054633 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/configuration_version_dependant.py
--rw-r--r--   0        0        0       14 2022-10-10 09:10:06.192877 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/.gitignore.j2
--rw-r--r--   0        0        0     4978 2023-02-28 10:04:38.122789 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/analysis.html.j2
--rw-r--r--   0        0        0     1538 2023-03-17 11:32:42.709156 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/config.yml.j2
--rw-r--r--   0        0        0        0 2022-10-11 10:38:47.295516 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/custom-postgres.conf.j2
--rw-r--r--   0        0        0       10 2022-10-10 09:10:06.192877 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/modules.csv.j2
--rw-r--r--   0        0        0     1709 2023-02-28 08:21:53.360949 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/11.0/Dockerfile
--rw-r--r--   0        0        0     1708 2023-02-28 08:21:53.360949 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/12.0/Dockerfile
--rw-r--r--   0        0        0     1707 2023-02-28 08:21:53.364950 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/13.0/Dockerfile
--rw-r--r--   0        0        0     1557 2023-02-28 08:21:53.364950 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/14.0/Dockerfile
--rw-r--r--   0        0        0     1557 2023-02-28 08:21:53.364950 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/15.0/Dockerfile
--rw-r--r--   0        0        0     1557 2023-02-28 08:21:53.364950 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/16.0/Dockerfile
--rw-r--r--   0        0        0        0 2022-10-10 09:10:06.196878 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/extra_debian_requirements.txt.j2
--rw-r--r--   0        0        0      355 2023-01-03 14:06:21.054633 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/extra_python_requirements.txt.j2
--rw-r--r--   0        0        0      314 2022-10-13 20:03:07.334219 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/odoo.conf.j2
--rw-r--r--   0        0        0     1303 2022-10-10 09:10:06.196878 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/repos.yml.j2
--rw-r--r--   0        0        0      179 2022-10-10 09:10:06.196878 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/scripts/post-migration.py.j2
--rw-r--r--   0        0        0        0 2022-10-10 09:10:06.196878 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/scripts/pre-migration.sql.j2
--rw-r--r--   0        0        0      339 2022-10-11 10:38:47.295516 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_click_odoo_contrib.py
--rw-r--r--   0        0        0     4358 2023-03-16 19:57:18.432283 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_docker.py
--rw-r--r--   0        0        0    11134 2023-02-28 08:21:53.364950 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_odoo.py
--rw-r--r--   0        0        0     4898 2022-10-11 10:38:47.299516 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_odoo_instance.py
--rw-r--r--   0        0        0    29405 2023-03-17 11:32:42.717156 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_odoo_module.py
--rw-r--r--   0        0        0     5513 2022-10-11 10:38:47.299516 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_postgres.py
--rw-r--r--   0        0        0     3224 2023-03-17 11:32:42.721156 odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_system.py
--rw-r--r--   0        0        0     1549 2023-03-17 11:33:03.805270 odoo-openupgrade-wizard-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    12174 2023-03-17 11:34:17.159632 odoo-openupgrade-wizard-0.4.0/setup.py
--rw-r--r--   0        0        0    11463 2023-03-17 11:34:17.162065 odoo-openupgrade-wizard-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    14826 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/README.md
+-rw-r--r--   0        0        0      131 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/__init__.py
+-rw-r--r--   0        0        0      142 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/__main__.py
+-rw-r--r--   0        0        0     4269 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli.py
+-rw-r--r--   0        0        0      546 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_copydb.py
+-rw-r--r--   0        0        0     1825 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_docker_build.py
+-rw-r--r--   0        0        0     3160 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_dumpdb.py
+-rw-r--r--   0        0        0     2525 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_estimate_workload.py
+-rw-r--r--   0        0        0      866 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_execute_script_python.py
+-rw-r--r--   0        0        0      864 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_execute_script_sql.py
+-rw-r--r--   0        0        0     4618 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_generate_module_analysis.py
+-rw-r--r--   0        0        0      880 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_get_code.py
+-rw-r--r--   0        0        0     5549 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_init.py
+-rw-r--r--   0        0        0     2814 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_install_from_csv.py
+-rw-r--r--   0        0        0     3066 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_options.py
+-rw-r--r--   0        0        0      727 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_psql.py
+-rw-r--r--   0        0        0     1900 2023-07-13 19:20:51.236372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_pull_submodule.py
+-rw-r--r--   0        0        0     1981 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_run.py
+-rw-r--r--   0        0        0     1297 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_upgrade.py
+-rw-r--r--   0        0        0     8322 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/configuration_version_dependant.py
+-rw-r--r--   0        0        0       14 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/.gitignore.j2
+-rw-r--r--   0        0        0     4978 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/analysis.html.j2
+-rw-r--r--   0        0        0     1538 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/config.yml.j2
+-rw-r--r--   0        0        0        0 2023-07-13 19:20:51.263373 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/custom-postgres.conf.j2
+-rw-r--r--   0        0        0       10 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/modules.csv.j2
+-rw-r--r--   0        0        0     1918 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/11.0/Dockerfile
+-rw-r--r--   0        0        0     1917 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/12.0/Dockerfile
+-rw-r--r--   0        0        0     1707 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/13.0/Dockerfile
+-rw-r--r--   0        0        0     1557 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/14.0/Dockerfile
+-rw-r--r--   0        0        0     1557 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/15.0/Dockerfile
+-rw-r--r--   0        0        0     1557 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/16.0/Dockerfile
+-rw-r--r--   0        0        0        0 2023-07-13 19:20:51.263373 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/extra_debian_requirements.txt.j2
+-rw-r--r--   0        0        0      355 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/extra_python_requirements.txt.j2
+-rw-r--r--   0        0        0      314 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/odoo.conf.j2
+-rw-r--r--   0        0        0     1303 2023-07-13 19:20:51.237372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/repos.yml.j2
+-rw-r--r--   0        0        0      179 2023-07-13 19:20:51.238372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/scripts/post-migration.py.j2
+-rw-r--r--   0        0        0        0 2023-07-13 19:20:51.263373 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/scripts/pre-migration.sql.j2
+-rw-r--r--   0        0        0      339 2023-07-13 19:20:51.238372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_click_odoo_contrib.py
+-rw-r--r--   0        0        0     4700 2023-07-13 19:20:51.238372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_docker.py
+-rw-r--r--   0        0        0    11134 2023-07-13 19:20:51.238372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_odoo.py
+-rw-r--r--   0        0        0     4898 2023-07-13 19:20:51.238372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_odoo_instance.py
+-rw-r--r--   0        0        0    29405 2023-07-13 19:20:51.238372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_odoo_module.py
+-rw-r--r--   0        0        0     7340 2023-07-13 19:20:51.238372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_postgres.py
+-rw-r--r--   0        0        0     4273 2023-07-13 19:20:51.238372 odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_system.py
+-rw-r--r--   0        0        0     1549 2023-07-13 19:20:51.239372 odoo_openupgrade_wizard-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    16372 1970-01-01 00:00:00.000000 odoo_openupgrade_wizard-0.5.0/PKG-INFO
```

### Comparing `odoo-openupgrade-wizard-0.4.0/README.md` & `odoo_openupgrade_wizard-0.5.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [![Gitlab CI](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/badges/main/pipeline.svg)](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/-/pipelines)
 [![codecov](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/badges/main/coverage.svg)](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 
-
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/odoo-openupgrade-wizard)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/odoo-openupgrade-wizard)
+![GitLab last commit](https://img.shields.io/gitlab/last-commit/34780558)
+![GitLab stars](https://img.shields.io/gitlab/stars/34780558?style=social)
 
 # odoo-openupgrade-wizard
 
 Odoo Openupgrade Wizard is a tool that helps developpers to make major
 upgrade of Odoo Community Edition. (formely OpenERP).
 It works with Openupgrade OCA tools. (https://github.com/oca/openupgrade)
 
@@ -19,14 +22,32 @@
 It will create a migration environment (with all the code available)
 and provides helpers to run (and replay) migrations until it works.
 
 * To develop and contribute to the library, refer to the ``DEVELOP.md`` file.
 * Refer to the ``ROADMAP.md`` file to see the current limitation, bugs, and task to do.
 * See authors in the ``CONTRIBUTORS.md`` file.
 
+# Table of Contents
+
+* [Installation](#installation)
+* [Usage](#usage)
+    * [Command ``init``](#command-init)
+    * [Command ``pull-submodule``](#command-pull-submodule)
+    * [Command ``get-code``](#command-get-code)
+    * [Command ``docker-build``](#command-docker-build)
+    * [Command ``run`` (BETA)](#command-run)
+    * [Command ``install-from-csv``](#command-install-from-csv)
+    * [Command ``upgrade`` (BETA)](#command-upgrade)
+    * [Command ``generate-module-analysis`` (BETA)](#command-generate-module-analysis)
+    * [Command ``estimate-workload`` (BETA)](#command-estimate-workload)
+    * [Command ``psql``](#command-psql)
+    * [Command ``dumpdb``](#command-dumpdb)
+
+<a name="installation"/>
+
 # Installation
 
 **Prerequites:**
 
 * The tools run on debian system
 * You should have docker installed on your system
 * Some features require extra packages. To have all the features available run:
@@ -37,21 +58,25 @@
 
 To install it simply run :
 
 ``pipx install odoo-openupgrade-wizard``
 
 (See alternative installation in ``DEVELOP.md`` file.)
 
+<a name="usage"/>
+
 # Usage
 
 **Note:**
 
 the term ``odoo-openupgrade-wizard`` can be replaced by ``oow``
 in all the command lines below.
 
+<a name="command-init"/>
+
 ## Command: ``init``
 
 ```
 odoo-openupgrade-wizard init\
   --initial-version=10.0\
   --final-version=12.0\
   --project-name=my-customer-10-12\
@@ -142,14 +167,16 @@
 **Note:**
 
 - In your repos.yml, preserve ``openupgrade`` and ``server-tools`` repositories
   to have all the features of the librairies available.
 - In your repos.yml file, the odoo project should be in ``./src/odoo``
   and the openupgrade project should be in ``./src/openupgrade/`` folder.
 
+<a name="command-pull-submodule"/>
+
 ## Command: ``pull-submodule``
 
 **Prerequites:** init
 
 if you already have a repos.yml file on github / gitlab, it can be convenient to
 synchronize the repository, instead of copy past the ``repos.yml`` manually.
 
@@ -165,14 +192,16 @@
 
 then run following command :
 
 ```
 odoo-openupgrade-wizard pull-submodule
 ```
 
+<a name="command-get-code"/>
+
 ## Command: ``get-code``
 
 **Prerequites:** init
 
 ```
 odoo-openupgrade-wizard get-code
 ```
@@ -191,15 +220,15 @@
 
 if you want to update the code of some given versions, you can provide an extra parameter:
 
 ```
 odoo-openupgrade-wizard get-code --versions 10.0,11.0
 ```
 
-
+<a name="command-docker-build"/>
 
 ## Command: ``docker-build``
 
 **Prerequites:** init + get-code
 
 This will build local docker images that will be used in the following steps.
 
@@ -221,14 +250,15 @@
   an extra parameter: ``--versions 10.0,12.0``
 
 **Note**
 
 * This step could take a big while also !
 
 
+<a name="command-run"/>
 
 ## Command: ``run`` (BETA)
 
 **Prerequites:** init + get-code + build
 
 ```
 odoo-openupgrade-wizard run\
@@ -248,14 +278,15 @@
 
 * You can add ``--init-modules=purchase,sale`` to install modules.
 
 * You can add ``stop-after-init`` flag to turn off the process at the end
   of the installation.
 
 
+<a name="command-install-from-csv"/>
 
 ## Command: ``install-from-csv``
 
 **Prerequites:** init + get-code + build
 
 ```
 odoo-openupgrade-wizard install-from-csv\
@@ -269,14 +300,15 @@
 
 To get a correct ``modules.csv`` file, the following query can be used:
 ```
 psql -c "copy (select name, shortdesc from ir_module_module where state = 'installed' order by 1) to stdout csv" coopiteasy
 ```
 
 
+<a name="command-upgrade"/>
 
 ## Command: ``upgrade`` (BETA)
 
 **Prerequites:** init + get-code + build
 
 ```
 odoo-openupgrade-wizard upgrade\
@@ -296,14 +328,15 @@
 **Optional arguments**
 
 * You can add ``--first-step=2`` to start at the second step.
 
 * You can add ``--last-step=3`` to end at the third step.
 
 
+<a name="command-generate-module-analysis"/>
 
 ## Command: ``generate-module-analysis`` (BETA)
 
 **Prerequites:** init + get-code + build
 
 ```
 odoo-openupgrade-wizard generate-module-analysis\
@@ -314,14 +347,15 @@
 
 Realize an analyze between the target version (in parameter via the step argument)
 and the previous version. It will generate analysis_file.txt files present
 in OpenUpgrade project.
 You can also use this fonction to analyze differences for custom / OCA modules
 between several versions, in case of refactoring.
 
+<a name="command-estimate-workload"/>
 
 ## Command: ``estimate-workload``
 
 **Prerequites:** init + get-code
 
 ```
 odoo-openupgrade-wizard estimate-workload
@@ -329,7 +363,121 @@
 
 Generate an HTML file name ``analysis.html`` with all the information regarding
 the work to do for the migration.
 - checks that the modules are present in each version. (by managing the
   renaming or merging of modules)
 - check that the analysis and migration have been done for the official
   modules present in odoo/odoo
+
+<a name="command-psql"/>
+
+## Command: ``psql``
+
+**Prerequites:** init
+
+```
+odoo-openupgrade-wizard psql
+    --database DB_NAME
+    --command "SQL_REQUEST"
+```
+
+Execute an SQL Request on the target database.
+
+**Optional arguments**
+
+* If no ``database`` is provided, default ``postgres`` database will be used. exemple:
+
+```
+odoo-openupgrade-wizard psql --command "\l";
+```
+Result:
+```
+                              List of databases
+    Name    | Owner | Encoding |  Collate   |   Ctype    | Access privileges
+------------+-------+----------+------------+------------+-------------------
+ postgres   | odoo  | UTF8     | en_US.utf8 | en_US.utf8 |
+ template0  | odoo  | UTF8     | en_US.utf8 | en_US.utf8 | =c/odoo          +
+            |       |          |            |            | odoo=CTc/odoo
+ template1  | odoo  | UTF8     | en_US.utf8 | en_US.utf8 | =c/odoo          +
+            |       |          |            |            | odoo=CTc/odoo
+ test_psql  | odoo  | UTF8     | en_US.utf8 | en_US.utf8 |
+
+```
+
+* if you execute request that return long result, you can choose to select ``pager`` or ``-no-pager``
+  option to display the result via the click function ``echo_via_pager``.
+  (see : https://click.palletsprojects.com/en/8.1.x/utils/#pager-support)
+
+Note : Pager is enabled by default.
+
+
+* you can pass extra psql arguments inline.
+
+```
+odoo-openupgrade-wizard psql
+    --database=test_psql
+    --command "select id, name from res_partner where name ilike '%admin%';"
+    -H
+```
+Result:
+```
+<table border="1">
+  <tr>
+    <th align="center">id</th>
+    <th align="center">name</th>
+  </tr>
+  <tr valign="top">
+    <td align="right">3</td>
+    <td align="left">Administrator</td>
+  </tr>
+</table>
+<p>(1 row)<br />
+</p>
+
+```
+
+See all the options here https://www.postgresql.org/docs/current/app-psql.html
+
+<a name="command-dumpdb"/>
+
+## Command: ``dumpdb``
+
+**Prerequites:** init
+
+```
+odoo-openupgrade-wizard dumpdb
+    --database DB_NAME
+    --database-path DATABASE_PATH
+    --filestore-path FILESTORE_PATH
+```
+
+Dump the database DB_NAME to DATABASE_PATH and export the filestore
+related to DB_NAME into FILESTORE_PATH. To choose the format of the
+backup files look at the `--database-format` and `--filestore-format`.
+
+*WARNING*: DATABASE_PATH should be a sub directory of the project path
+in orter to have the postgresql container able to write the dump file.
+For example, the project path is `/path/to/myproject` (where you run the
+`init` command), then DATABASE_PATH can be any of the subdirectory of
+`/path/to/myproject`.
+
+**Optional arguments**
+
+* To chose the database format use `--database-format`. Format can be
+  one of the following:
+      - `p` for plain sql text
+      - `c` for custom compressed backup of `pg_dump`
+      - `d` for directory structure
+      - `t` for a tar version of the directory structure
+  See also https://www.postgresql.org/docs/current/app-pgdump.html
+  The default database format is `c`.
+
+* To chose the filestore format use `--filestore-format`. Format can be
+  one of the following:
+      - `d` copy of the directory structure
+      - `t` tar version of the directory structure (not compressed)
+      - `tgz` tar version of the directory structure compressed with gzip.
+  The default filestore format is `tgz`.
+
+* By default, if database file or filestore file already exists, the
+  command will fail, preserving the existing dump. If you need to
+  overwrite the existing files, the `--force` option can be used.
```

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 import yaml
 from click_loglevel import LogLevel
 from loguru import logger
 
 import odoo_openupgrade_wizard
 from odoo_openupgrade_wizard.cli.cli_copydb import copydb
 from odoo_openupgrade_wizard.cli.cli_docker_build import docker_build
+from odoo_openupgrade_wizard.cli.cli_dumpdb import dumpdb
 from odoo_openupgrade_wizard.cli.cli_estimate_workload import estimate_workload
 from odoo_openupgrade_wizard.cli.cli_execute_script_python import (
     execute_script_python,
 )
 from odoo_openupgrade_wizard.cli.cli_execute_script_sql import (
     execute_script_sql,
 )
 from odoo_openupgrade_wizard.cli.cli_generate_module_analysis import (
     generate_module_analysis,
 )
 from odoo_openupgrade_wizard.cli.cli_get_code import get_code
 from odoo_openupgrade_wizard.cli.cli_init import init
 from odoo_openupgrade_wizard.cli.cli_install_from_csv import install_from_csv
+from odoo_openupgrade_wizard.cli.cli_psql import psql
 from odoo_openupgrade_wizard.cli.cli_pull_submodule import pull_submodule
 from odoo_openupgrade_wizard.cli.cli_run import run
 from odoo_openupgrade_wizard.cli.cli_upgrade import upgrade
 from odoo_openupgrade_wizard.tools.tools_system import ensure_folder_exists
 
 
 @click.group()
@@ -102,17 +104,19 @@
             ctx.obj["config"] = config
     elif ctx.invoked_subcommand != "init":
         raise
 
 
 main.add_command(copydb)
 main.add_command(docker_build)
+main.add_command(dumpdb)
 main.add_command(estimate_workload)
 main.add_command(execute_script_python)
 main.add_command(execute_script_sql)
 main.add_command(generate_module_analysis)
 main.add_command(get_code)
 main.add_command(init)
 main.add_command(install_from_csv)
+main.add_command(psql)
 main.add_command(pull_submodule)
 main.add_command(run)
 main.add_command(upgrade)
```

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_copydb.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_copydb.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_docker_build.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_docker_build.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_estimate_workload.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_estimate_workload.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_execute_script_python.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_execute_script_python.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_execute_script_sql.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_execute_script_sql.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_generate_module_analysis.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_generate_module_analysis.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_get_code.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_get_code.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_init.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_init.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_install_from_csv.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_install_from_csv.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_options.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_options.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_pull_submodule.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_pull_submodule.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_run.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_run.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/cli/cli_upgrade.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/cli/cli_upgrade.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/configuration_version_dependant.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/configuration_version_dependant.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/analysis.html.j2` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/analysis.html.j2`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/config.yml.j2` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/config.yml.j2`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/11.0/Dockerfile` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/13.0/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# <OOW> : Copy of https://github.com/odoo/odoo/blob/11.0/setup/package.dfsrc
-FROM debian:stretch
+# <OOW> : Copy of https://github.com/odoo/odoo/blob/13.0/setup/package.dfsrc
+FROM debian:buster
 
 RUN apt-get update && \
     apt-get install -y locales && \
     rm -rf /var/lib/apt/lists/*
 
 # Reconfigure locales such that postgresql uses UTF-8 encoding
 RUN dpkg-reconfigure locales && \
@@ -14,15 +14,15 @@
 RUN apt-get update -qq &&  \
     apt-get upgrade -qq -y && \
     apt-get install \
         postgresql \
         postgresql-server-dev-all \
         postgresql-client \
         adduser \
-        node-less \
+        libsass1 \
         libxml2-dev \
         libxslt1-dev \
         libldap2-dev \
         libsasl2-dev \
         libssl-dev \
         libjpeg-dev \
         zlib1g-dev \
```

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/12.0/Dockerfile` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/15.0/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# <OOW> : Copy of https://github.com/odoo/odoo/blob/12.0/setup/package.dfsrc
-FROM debian:stretch
+# <OOW> : Copy of https://github.com/odoo/odoo/blob/15.0/setup/package.dfsrc
+FROM debian:buster
 
 RUN apt-get update && \
     apt-get install -y locales && \
     rm -rf /var/lib/apt/lists/*
 
 # Reconfigure locales such that postgresql uses UTF-8 encoding
 RUN dpkg-reconfigure locales && \
@@ -14,23 +14,16 @@
 RUN apt-get update -qq &&  \
     apt-get upgrade -qq -y && \
     apt-get install \
         postgresql \
         postgresql-server-dev-all \
         postgresql-client \
         adduser \
-        libsass0 \
-        libxml2-dev \
-        libxslt1-dev \
         libldap2-dev \
         libsasl2-dev \
-        libssl-dev \
-        libjpeg-dev \
-        zlib1g-dev \
-        python3-dev \
         python3-pip \
         python3-wheel \
         build-essential \
         python3 -y && \
     rm -rf /var/lib/apt/lists/*
 
 # <OOW> Install Debian packages
```

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/13.0/Dockerfile` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/14.0/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# <OOW> : Copy of https://github.com/odoo/odoo/blob/13.0/setup/package.dfsrc
+# <OOW> : Copy of https://github.com/odoo/odoo/blob/14.0/setup/package.dfsrc
 FROM debian:buster
 
 RUN apt-get update && \
     apt-get install -y locales && \
     rm -rf /var/lib/apt/lists/*
 
 # Reconfigure locales such that postgresql uses UTF-8 encoding
@@ -14,23 +14,16 @@
 RUN apt-get update -qq &&  \
     apt-get upgrade -qq -y && \
     apt-get install \
         postgresql \
         postgresql-server-dev-all \
         postgresql-client \
         adduser \
-        libsass1 \
-        libxml2-dev \
-        libxslt1-dev \
         libldap2-dev \
         libsasl2-dev \
-        libssl-dev \
-        libjpeg-dev \
-        zlib1g-dev \
-        python3-dev \
         python3-pip \
         python3-wheel \
         build-essential \
         python3 -y && \
     rm -rf /var/lib/apt/lists/*
 
 # <OOW> Install Debian packages
```

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/14.0/Dockerfile` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/16.0/Dockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# <OOW> : Copy of https://github.com/odoo/odoo/blob/14.0/setup/package.dfsrc
+# <OOW> : Copy of https://github.com/odoo/odoo/blob/16.0/setup/package.dfsrc
 FROM debian:buster
 
 RUN apt-get update && \
     apt-get install -y locales && \
     rm -rf /var/lib/apt/lists/*
 
 # Reconfigure locales such that postgresql uses UTF-8 encoding
```

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/15.0/Dockerfile` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/12.0/Dockerfile`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-# <OOW> : Copy of https://github.com/odoo/odoo/blob/15.0/setup/package.dfsrc
-FROM debian:buster
+# <OOW> : Copy of https://github.com/odoo/odoo/blob/12.0/setup/package.dfsrc
+FROM debian:stretch
+
+RUN sed -i -- 's/security.debian.org/archive.debian.org/g' /etc/apt/**.list
+RUN sed -i -- 's/deb.debian.org/archive.debian.org/g' /etc/apt/**.list
+RUN sed -i -- 's/stretch-updates/stretch/g' /etc/apt/**.list
 
 RUN apt-get update && \
     apt-get install -y locales && \
     rm -rf /var/lib/apt/lists/*
 
 # Reconfigure locales such that postgresql uses UTF-8 encoding
 RUN dpkg-reconfigure locales && \
@@ -14,16 +18,23 @@
 RUN apt-get update -qq &&  \
     apt-get upgrade -qq -y && \
     apt-get install \
         postgresql \
         postgresql-server-dev-all \
         postgresql-client \
         adduser \
+        libsass0 \
+        libxml2-dev \
+        libxslt1-dev \
         libldap2-dev \
         libsasl2-dev \
+        libssl-dev \
+        libjpeg-dev \
+        zlib1g-dev \
+        python3-dev \
         python3-pip \
         python3-wheel \
         build-essential \
         python3 -y && \
     rm -rf /var/lib/apt/lists/*
 
 # <OOW> Install Debian packages
```

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/16.0/Dockerfile` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/11.0/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-# <OOW> : Copy of https://github.com/odoo/odoo/blob/16.0/setup/package.dfsrc
-FROM debian:buster
+# <OOW> : Copy of https://github.com/odoo/odoo/blob/11.0/setup/package.dfsrc
+FROM debian:stretch
+
+RUN sed -i -- 's/security.debian.org/archive.debian.org/g' /etc/apt/**.list
+RUN sed -i -- 's/deb.debian.org/archive.debian.org/g' /etc/apt/**.list
+RUN sed -i -- 's/stretch-updates/stretch/g' /etc/apt/**.list
 
 RUN apt-get update && \
     apt-get install -y locales && \
     rm -rf /var/lib/apt/lists/*
 
 # Reconfigure locales such that postgresql uses UTF-8 encoding
 RUN dpkg-reconfigure locales && \
@@ -14,16 +18,23 @@
 RUN apt-get update -qq &&  \
     apt-get upgrade -qq -y && \
     apt-get install \
         postgresql \
         postgresql-server-dev-all \
         postgresql-client \
         adduser \
+        node-less \
+        libxml2-dev \
+        libxslt1-dev \
         libldap2-dev \
         libsasl2-dev \
+        libssl-dev \
+        libjpeg-dev \
+        zlib1g-dev \
+        python3-dev \
         python3-pip \
         python3-wheel \
         build-essential \
         python3 -y && \
     rm -rf /var/lib/apt/lists/*
 
 # <OOW> Install Debian packages
```

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/templates/odoo/repos.yml.j2` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/templates/odoo/repos.yml.j2`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_docker.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import time
+
 import docker
 from loguru import logger
 
 
 def get_docker_client():
     return docker.from_env()
 
@@ -82,14 +84,23 @@
         links=links,
         detach=detach,
         auto_remove=auto_remove,
     )
     if detach:
         logger.debug("Container %s launched." % image_name)
     elif auto_remove:
+        # Workaround to avoid
+        # "Conflict. The container name xxx is already in use"
+        # Because it seems that the container name is not freed when the
+        # run command completes
+        while client.containers.list(
+            all=True, filters={"name": container_name}
+        ):
+            time.sleep(1)
+
         logger.debug("Container closed.")
 
     return container
 
 
 def exec_container(container, command):
     debug_docker_command = "docker exec %s" % (container.name)
```

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_odoo.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_odoo.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_odoo_instance.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_odoo_instance.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_odoo_module.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_odoo_module.py`

 * *Files identical despite different names*

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_postgres.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_postgres.py`

 * *Files 18% similar despite different names*

```diff
@@ -100,35 +100,43 @@
         "Executing the script '%s' in postgres container"
         " on database %s" % (relative_path, database)
     )
     exec_container(container, command)
 
 
 def execute_sql_request(ctx, request, database="postgres"):
+    psql_args = ("--tuples-only",)
+    output = execute_psql_command(ctx, request, database, psql_args)
+    lines = output.split("\n")
+    result = []
+    for line in lines:
+        if not line:
+            continue
+        result.append([x.strip() for x in line.split("|")])
+    return result
+
+
+def execute_psql_command(
+    ctx, request: str, database: str = None, psql_args: tuple = ()
+):
+    """Execute psql request in postgres container with psql_args on database"""
     container = get_postgres_container(ctx)
     command = (
         "psql"
         " --username=odoo"
-        " --dbname={database}"
-        " --tuples-only"
-        ' --command "{request}"'
-    ).format(database=database, request=request)
+        f" --dbname={database or 'postgres'}"
+        f' --command "{request}"'
+        f" {' '.join(psql_args)}"
+    )
     logger.debug(
-        "Executing the following command in postgres container"
-        " on database %s \n %s" % (database, request)
+        "Executing the following command in postgres container\n"
+        "%s" % (command)
     )
     docker_result = exec_container(container, command)
-
-    lines = docker_result.output.decode("utf-8").split("\n")
-    result = []
-    for line in lines:
-        if not line:
-            continue
-        result.append([x.strip() for x in line.split("|")])
-    return result
+    return docker_result.output.decode("utf-8")
 
 
 def ensure_database(ctx, database: str, state="present"):
     """
     - Connect to postgres container.
     - Check if the database exist.
     - if doesn't exists and state == 'present', create it.
@@ -168,7 +176,62 @@
             if os.path.isfile(os.path.join(script_folder, f))
             and f[-4:] == ".sql"
         ]
         sql_files = sorted(sql_files)
 
     for sql_file in sql_files:
         execute_sql_file(ctx, database, sql_file)
+
+
+def chown_to_local_user(ctx, filepath: os.PathLike):
+    """Chown a filepath in the postgres container to the local user"""
+    container = get_postgres_container(ctx)
+    user_uid = os.getuid()
+    command = "chown -R {uid}:{uid} {filepath}".format(
+        uid=user_uid, filepath=filepath
+    )
+    logger.debug(
+        "Executing the following command in postgres container: %s"
+        % (command,)
+    )
+    chown_result = exec_container(container, command)
+    return chown_result.output.decode("utf8")
+
+
+def execute_pg_dump(
+    ctx,
+    database: str,
+    dumpformat: str,
+    filename: str,
+    pg_dump_args="--no-owner",
+):
+    """Execute pg_dump command on the postgres container and dump the
+    result to dumpfile.
+    """
+    if pg_dump_args and not isinstance(pg_dump_args, str):
+        pg_dump_args = " ".join(pg_dump_args)
+    container = get_postgres_container(ctx)
+    # Generate path for the output file
+    filepath = Path("/env") / Path(filename)
+    # Generate pg_dump command
+    command = (
+        "pg_dump"
+        " --username=odoo"
+        " --format {dumpformat}"
+        " --file {filepath}"
+        " {pg_dump_args}"
+        " {database}"
+    ).format(
+        dumpformat=dumpformat,
+        filepath=filepath,
+        database=database,
+        pg_dump_args=pg_dump_args,
+    )
+    logger.debug(
+        "Executing the following command in postgres container: %s"
+        % (command,)
+    )
+    pg_dump_result = exec_container(container, command)
+
+    chown_to_local_user(ctx, filepath)
+
+    return pg_dump_result.output.decode("utf8")
```

### Comparing `odoo-openupgrade-wizard-0.4.0/odoo_openupgrade_wizard/tools/tools_system.py` & `odoo_openupgrade_wizard-0.5.0/odoo_openupgrade_wizard/tools/tools_system.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import argparse
 import os
+import shutil
 import subprocess
+import tarfile
 from pathlib import Path
 
 import importlib_resources
 from git_aggregator import main as gitaggregate_cmd
 from git_aggregator.utils import working_directory_keeper
 from jinja2 import Template
 from loguru import logger
@@ -105,7 +107,40 @@
 def get_local_user_id():
     return os.getuid()
 
 
 def execute_check_output(args_list, working_directory=False):
     logger.debug("Execute %s" % " ".join(args_list))
     subprocess.check_output(args_list, cwd=working_directory)
+
+
+def dump_filestore(
+    ctx,
+    database: str,
+    destpath: os.PathLike,
+    copyformat: str = "d",
+):
+    """Copy filestore of database to destpath using copyformat.
+    copyformat can be 'd' for directory, a normal copy, or 't' for a
+    copy into a tar achive, or 'tgz' to copy to a compressed tar file.
+    """
+    valid_format = ("d", "t", "tgz", "txz")
+    if copyformat not in valid_format:
+        raise ValueError(
+            f"copyformat should be one of the following {valid_format}"
+        )
+
+    filestore_folder_path = ctx.obj["env_folder_path"] / "filestore/filestore"
+    filestore_path = filestore_folder_path / database
+
+    if copyformat == "d":
+        shutil.copytree(filestore_path, destpath)
+
+    elif copyformat.startswith("t"):
+        wmode = "w"
+        if copyformat.endswith("gz"):
+            wmode += ":gz"
+        elif copyformat.endswith("xz"):
+            wmode += ":xz"
+
+        with tarfile.open(destpath, wmode) as tar:
+            tar.add(filestore_path, arcname="filestore")
```

### Comparing `odoo-openupgrade-wizard-0.4.0/pyproject.toml` & `odoo_openupgrade_wizard-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odoo-openupgrade-wizard"
-version = "0.4.0"
+version = "0.5.0"
 description = "CLI tool to manage Odoo Major Upgrades"
 authors = [
     "GRAP, Groupement Régional Alimentaire de Proximité",
 ]
 maintainers = [
     "Sylvain LE GAL",
 ]
```

### Comparing `odoo-openupgrade-wizard-0.4.0/PKG-INFO` & `odoo_openupgrade_wizard-0.5.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: odoo-openupgrade-wizard
-Version: 0.4.0
+Version: 0.5.0
 Summary: CLI tool to manage Odoo Major Upgrades
 Home-page: https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard
 License: AGPLv3+
 Keywords: cli,odoo,openupgrade
 Author: GRAP, Groupement Régional Alimentaire de Proximité
 Maintainer: Sylvain LE GAL
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Odoo
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
 Requires-Dist: GitPython (>=3.1,<4.0)
 Requires-Dist: click (>=7.0,<8.0)
 Requires-Dist: click-loglevel (>=0.4,<0.5)
 Requires-Dist: docker (>=5.0,<6.0)
 Requires-Dist: git-aggregator (>=2.1,<3.0)
 Requires-Dist: importlib-resources (>=5.4,<6.0)
 Requires-Dist: jinja2 (>=3.0,<4.0)
@@ -34,15 +36,18 @@
 Project-URL: Repository, https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard
 Description-Content-Type: text/markdown
 
 [![Gitlab CI](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/badges/main/pipeline.svg)](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/-/pipelines)
 [![codecov](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/badges/main/coverage.svg)](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 
-
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/odoo-openupgrade-wizard)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/odoo-openupgrade-wizard)
+![GitLab last commit](https://img.shields.io/gitlab/last-commit/34780558)
+![GitLab stars](https://img.shields.io/gitlab/stars/34780558?style=social)
 
 # odoo-openupgrade-wizard
 
 Odoo Openupgrade Wizard is a tool that helps developpers to make major
 upgrade of Odoo Community Edition. (formely OpenERP).
 It works with Openupgrade OCA tools. (https://github.com/oca/openupgrade)
 
@@ -55,14 +60,32 @@
 It will create a migration environment (with all the code available)
 and provides helpers to run (and replay) migrations until it works.
 
 * To develop and contribute to the library, refer to the ``DEVELOP.md`` file.
 * Refer to the ``ROADMAP.md`` file to see the current limitation, bugs, and task to do.
 * See authors in the ``CONTRIBUTORS.md`` file.
 
+# Table of Contents
+
+* [Installation](#installation)
+* [Usage](#usage)
+    * [Command ``init``](#command-init)
+    * [Command ``pull-submodule``](#command-pull-submodule)
+    * [Command ``get-code``](#command-get-code)
+    * [Command ``docker-build``](#command-docker-build)
+    * [Command ``run`` (BETA)](#command-run)
+    * [Command ``install-from-csv``](#command-install-from-csv)
+    * [Command ``upgrade`` (BETA)](#command-upgrade)
+    * [Command ``generate-module-analysis`` (BETA)](#command-generate-module-analysis)
+    * [Command ``estimate-workload`` (BETA)](#command-estimate-workload)
+    * [Command ``psql``](#command-psql)
+    * [Command ``dumpdb``](#command-dumpdb)
+
+<a name="installation"/>
+
 # Installation
 
 **Prerequites:**
 
 * The tools run on debian system
 * You should have docker installed on your system
 * Some features require extra packages. To have all the features available run:
@@ -73,21 +96,25 @@
 
 To install it simply run :
 
 ``pipx install odoo-openupgrade-wizard``
 
 (See alternative installation in ``DEVELOP.md`` file.)
 
+<a name="usage"/>
+
 # Usage
 
 **Note:**
 
 the term ``odoo-openupgrade-wizard`` can be replaced by ``oow``
 in all the command lines below.
 
+<a name="command-init"/>
+
 ## Command: ``init``
 
 ```
 odoo-openupgrade-wizard init\
   --initial-version=10.0\
   --final-version=12.0\
   --project-name=my-customer-10-12\
@@ -178,14 +205,16 @@
 **Note:**
 
 - In your repos.yml, preserve ``openupgrade`` and ``server-tools`` repositories
   to have all the features of the librairies available.
 - In your repos.yml file, the odoo project should be in ``./src/odoo``
   and the openupgrade project should be in ``./src/openupgrade/`` folder.
 
+<a name="command-pull-submodule"/>
+
 ## Command: ``pull-submodule``
 
 **Prerequites:** init
 
 if you already have a repos.yml file on github / gitlab, it can be convenient to
 synchronize the repository, instead of copy past the ``repos.yml`` manually.
 
@@ -201,14 +230,16 @@
 
 then run following command :
 
 ```
 odoo-openupgrade-wizard pull-submodule
 ```
 
+<a name="command-get-code"/>
+
 ## Command: ``get-code``
 
 **Prerequites:** init
 
 ```
 odoo-openupgrade-wizard get-code
 ```
@@ -227,15 +258,15 @@
 
 if you want to update the code of some given versions, you can provide an extra parameter:
 
 ```
 odoo-openupgrade-wizard get-code --versions 10.0,11.0
 ```
 
-
+<a name="command-docker-build"/>
 
 ## Command: ``docker-build``
 
 **Prerequites:** init + get-code
 
 This will build local docker images that will be used in the following steps.
 
@@ -257,14 +288,15 @@
   an extra parameter: ``--versions 10.0,12.0``
 
 **Note**
 
 * This step could take a big while also !
 
 
+<a name="command-run"/>
 
 ## Command: ``run`` (BETA)
 
 **Prerequites:** init + get-code + build
 
 ```
 odoo-openupgrade-wizard run\
@@ -284,14 +316,15 @@
 
 * You can add ``--init-modules=purchase,sale`` to install modules.
 
 * You can add ``stop-after-init`` flag to turn off the process at the end
   of the installation.
 
 
+<a name="command-install-from-csv"/>
 
 ## Command: ``install-from-csv``
 
 **Prerequites:** init + get-code + build
 
 ```
 odoo-openupgrade-wizard install-from-csv\
@@ -305,14 +338,15 @@
 
 To get a correct ``modules.csv`` file, the following query can be used:
 ```
 psql -c "copy (select name, shortdesc from ir_module_module where state = 'installed' order by 1) to stdout csv" coopiteasy
 ```
 
 
+<a name="command-upgrade"/>
 
 ## Command: ``upgrade`` (BETA)
 
 **Prerequites:** init + get-code + build
 
 ```
 odoo-openupgrade-wizard upgrade\
@@ -332,14 +366,15 @@
 **Optional arguments**
 
 * You can add ``--first-step=2`` to start at the second step.
 
 * You can add ``--last-step=3`` to end at the third step.
 
 
+<a name="command-generate-module-analysis"/>
 
 ## Command: ``generate-module-analysis`` (BETA)
 
 **Prerequites:** init + get-code + build
 
 ```
 odoo-openupgrade-wizard generate-module-analysis\
@@ -350,14 +385,15 @@
 
 Realize an analyze between the target version (in parameter via the step argument)
 and the previous version. It will generate analysis_file.txt files present
 in OpenUpgrade project.
 You can also use this fonction to analyze differences for custom / OCA modules
 between several versions, in case of refactoring.
 
+<a name="command-estimate-workload"/>
 
 ## Command: ``estimate-workload``
 
 **Prerequites:** init + get-code
 
 ```
 odoo-openupgrade-wizard estimate-workload
@@ -366,7 +402,121 @@
 Generate an HTML file name ``analysis.html`` with all the information regarding
 the work to do for the migration.
 - checks that the modules are present in each version. (by managing the
   renaming or merging of modules)
 - check that the analysis and migration have been done for the official
   modules present in odoo/odoo
 
+<a name="command-psql"/>
+
+## Command: ``psql``
+
+**Prerequites:** init
+
+```
+odoo-openupgrade-wizard psql
+    --database DB_NAME
+    --command "SQL_REQUEST"
+```
+
+Execute an SQL Request on the target database.
+
+**Optional arguments**
+
+* If no ``database`` is provided, default ``postgres`` database will be used. exemple:
+
+```
+odoo-openupgrade-wizard psql --command "\l";
+```
+Result:
+```
+                              List of databases
+    Name    | Owner | Encoding |  Collate   |   Ctype    | Access privileges
+------------+-------+----------+------------+------------+-------------------
+ postgres   | odoo  | UTF8     | en_US.utf8 | en_US.utf8 |
+ template0  | odoo  | UTF8     | en_US.utf8 | en_US.utf8 | =c/odoo          +
+            |       |          |            |            | odoo=CTc/odoo
+ template1  | odoo  | UTF8     | en_US.utf8 | en_US.utf8 | =c/odoo          +
+            |       |          |            |            | odoo=CTc/odoo
+ test_psql  | odoo  | UTF8     | en_US.utf8 | en_US.utf8 |
+
+```
+
+* if you execute request that return long result, you can choose to select ``pager`` or ``-no-pager``
+  option to display the result via the click function ``echo_via_pager``.
+  (see : https://click.palletsprojects.com/en/8.1.x/utils/#pager-support)
+
+Note : Pager is enabled by default.
+
+
+* you can pass extra psql arguments inline.
+
+```
+odoo-openupgrade-wizard psql
+    --database=test_psql
+    --command "select id, name from res_partner where name ilike '%admin%';"
+    -H
+```
+Result:
+```
+<table border="1">
+  <tr>
+    <th align="center">id</th>
+    <th align="center">name</th>
+  </tr>
+  <tr valign="top">
+    <td align="right">3</td>
+    <td align="left">Administrator</td>
+  </tr>
+</table>
+<p>(1 row)<br />
+</p>
+
+```
+
+See all the options here https://www.postgresql.org/docs/current/app-psql.html
+
+<a name="command-dumpdb"/>
+
+## Command: ``dumpdb``
+
+**Prerequites:** init
+
+```
+odoo-openupgrade-wizard dumpdb
+    --database DB_NAME
+    --database-path DATABASE_PATH
+    --filestore-path FILESTORE_PATH
+```
+
+Dump the database DB_NAME to DATABASE_PATH and export the filestore
+related to DB_NAME into FILESTORE_PATH. To choose the format of the
+backup files look at the `--database-format` and `--filestore-format`.
+
+*WARNING*: DATABASE_PATH should be a sub directory of the project path
+in orter to have the postgresql container able to write the dump file.
+For example, the project path is `/path/to/myproject` (where you run the
+`init` command), then DATABASE_PATH can be any of the subdirectory of
+`/path/to/myproject`.
+
+**Optional arguments**
+
+* To chose the database format use `--database-format`. Format can be
+  one of the following:
+      - `p` for plain sql text
+      - `c` for custom compressed backup of `pg_dump`
+      - `d` for directory structure
+      - `t` for a tar version of the directory structure
+  See also https://www.postgresql.org/docs/current/app-pgdump.html
+  The default database format is `c`.
+
+* To chose the filestore format use `--filestore-format`. Format can be
+  one of the following:
+      - `d` copy of the directory structure
+      - `t` tar version of the directory structure (not compressed)
+      - `tgz` tar version of the directory structure compressed with gzip.
+  The default filestore format is `tgz`.
+
+* By default, if database file or filestore file already exists, the
+  command will fail, preserving the existing dump. If you need to
+  overwrite the existing files, the `--force` option can be used.
+
```

