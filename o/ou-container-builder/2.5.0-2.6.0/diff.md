# Comparing `tmp/ou_container_builder-2.5.0.tar.gz` & `tmp/ou_container_builder-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_container_builder-2.5.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ou_container_builder-2.5.0.tar` & `ou_container_builder-2.6.0.tar`

### file list

```diff
@@ -1,32 +1,912 @@
--rw-r--r--   0        0        0       32 2023-06-14 13:48:53.158242 ou_container_builder-2.5.0/ou_container_builder/__init__.py
--rw-r--r--   0        0        0     1454 2023-06-14 13:48:53.158242 ou_container_builder-2.5.0/ou_container_builder/__main__.py
--rw-r--r--   0        0        0     6189 2023-06-14 13:48:53.158242 ou_container_builder-2.5.0/ou_container_builder/builder.py
--rw-r--r--   0        0        0      158 2023-06-14 13:48:53.158242 ou_container_builder-2.5.0/ou_container_builder/core/__init__.py
--rw-r--r--   0        0        0     1098 2023-06-14 13:48:53.158242 ou_container_builder-2.5.0/ou_container_builder/core/base.py
--rw-r--r--   0        0        0     2435 2023-06-14 13:48:53.158242 ou_container_builder-2.5.0/ou_container_builder/core/content.py
--rw-r--r--   0        0        0      815 2023-06-14 13:48:53.158242 ou_container_builder-2.5.0/ou_container_builder/core/env.py
--rw-r--r--   0        0        0     1137 2023-06-14 13:48:53.158242 ou_container_builder-2.5.0/ou_container_builder/core/hacks.py
--rw-r--r--   0        0        0     3096 2023-06-14 13:48:53.158242 ou_container_builder-2.5.0/ou_container_builder/core/jupyter_server.py
--rw-r--r--   0        0        0     1172 2023-06-14 13:48:53.159242 ou_container_builder-2.5.0/ou_container_builder/core/packages.py
--rw-r--r--   0        0        0     4219 2023-06-14 13:48:53.159242 ou_container_builder-2.5.0/ou_container_builder/core/scripts.py
--rw-r--r--   0        0        0     1522 2023-06-14 13:48:53.159242 ou_container_builder-2.5.0/ou_container_builder/core/services.py
--rw-r--r--   0        0        0     2216 2023-06-14 13:48:53.159242 ou_container_builder-2.5.0/ou_container_builder/core/startup.py
--rw-r--r--   0        0        0     2613 2023-06-14 13:48:53.159242 ou_container_builder-2.5.0/ou_container_builder/core/web_apps.py
--rw-r--r--   0        0        0      152 2023-06-14 13:48:53.159242 ou_container_builder-2.5.0/ou_container_builder/packs/__init__.py
--rw-r--r--   0        0        0     4616 2023-06-14 13:48:53.159242 ou_container_builder-2.5.0/ou_container_builder/packs/code_server.py
--rw-r--r--   0        0        0     1558 2023-06-14 13:48:53.159242 ou_container_builder-2.5.0/ou_container_builder/packs/jupyterlab.py
--rw-r--r--   0        0        0     2895 2023-06-14 13:48:53.159242 ou_container_builder-2.5.0/ou_container_builder/packs/mariadb.py
--rw-r--r--   0        0        0     1853 2023-06-14 13:48:53.159242 ou_container_builder-2.5.0/ou_container_builder/packs/nbclassic.py
--rw-r--r--   0        0        0     2733 2023-06-14 13:48:53.160242 ou_container_builder-2.5.0/ou_container_builder/packs/tutorial_server.py
--rw-r--r--   0        0        0     3766 2023-06-14 13:48:53.160242 ou_container_builder-2.5.0/ou_container_builder/templates/Dockerfile.jinja2
--rw-r--r--   0        0        0      990 2023-06-14 13:48:53.160242 ou_container_builder-2.5.0/ou_container_builder/templates/core/content/content_config.yaml
--rw-r--r--   0        0        0      247 2023-06-14 13:48:53.160242 ou_container_builder-2.5.0/ou_container_builder/templates/core/services/sudoers
--rw-r--r--   0        0        0      140 2023-06-14 13:48:53.160242 ou_container_builder-2.5.0/ou_container_builder/templates/core/startup/home-dir.sudoers
--rw-r--r--   0        0        0      486 2023-06-14 13:48:53.160242 ou_container_builder-2.5.0/ou_container_builder/templates/core/startup/start.sh
--rw-r--r--   0        0        0     4451 2023-06-14 13:48:53.161242 ou_container_builder-2.5.0/ou_container_builder/templates/packs/code_server/vscode.svg
--rw-r--r--   0        0        0      615 2023-06-14 13:48:53.161242 ou_container_builder-2.5.0/ou_container_builder/templates/packs/mariadb/setup.sh
--rw-r--r--   0        0        0      942 2023-06-14 13:48:53.161242 ou_container_builder-2.5.0/ou_container_builder/templates/packs/tutorial-server/production.ini
--rw-r--r--   0        0        0     2142 2023-06-14 13:48:53.161242 ou_container_builder-2.5.0/ou_container_builder/utils.py
--rw-r--r--   0        0        0    12634 2023-06-14 13:48:53.161242 ou_container_builder-2.5.0/ou_container_builder/validator.py
--rw-r--r--   0        0        0      629 2023-06-14 13:48:53.162243 ou_container_builder-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 ou_container_builder-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/Dockerfile
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/prepare_release.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tox.ini
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate_this.py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/pip
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/pip-3.11
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/pip3
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/python -> /usr/bin/python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/wheel
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/wheel3
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/wheel3.11
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.virtualenv
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    23741 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30030 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18328 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    28722 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    18817 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20435 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18442 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    27696 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    27475 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17872 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    32782 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    18864 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0    84101 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   109388 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    32064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35601 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    71556 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53572 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    99195 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35153 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/METADATA
+-rw-r--r--   0        0        0    72198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0   109451 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    80078 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   133344 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    22975 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_importlib.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_itertools.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_normalization.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_path.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_reqs.py
+-rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    19778 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/build_meta.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli-32.exe
+-rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli-64.exe
+-rw-r--r--   0        0        0   137216 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli-arm64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    21087 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/discovery.py
+-rw-r--r--   0        0        0    47046 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/glob.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui-32.exe
+-rw-r--r--   0        0        0    75264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui-64.exe
+-rw-r--r--   0        0        0   137728 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui-arm64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/logging.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    47115 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    39968 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/py312compat.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/py34compat.py
+-rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/warnings.py
+-rw-r--r--   0        0        0     8608 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_log.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0        0        0    19616 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    48643 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    17861 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    50174 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    17899 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8212 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30188 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23577 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    18928 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12085 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    15601 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    18099 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    12951 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    31503 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    16537 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    30153 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0        0        0    26498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    16596 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    87692 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    31965 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0        0        0    28906 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0        0        0    13755 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
+-rw-r--r--   0        0        0    16353 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/expand.py
+-rw-r--r--   0        0        0    19659 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0        0        0    26184 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0        0        0   274907 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/METADATA
+-rw-r--r--   0        0        0    34553 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/__main__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/_setuptools_logging.py
+-rw-r--r--   0        0        0    19868 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/bdist_wheel.py
+-rw-r--r--   0        0        0    16143 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/macosx_libfile.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/metadata.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/util.py
+-rw-r--r--   0        0        0     7674 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/wheelfile.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/__init__.py
+-rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/convert.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/pack.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/tags.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/unpack.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/__init__.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/vendor.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py
+-rw-r--r--   0        0        0    39047 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py
+-rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/METADATA
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/Makefile
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/building.rst
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/conf.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/index.rst
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/installation.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/index.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/main.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/packs.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/utils.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/validator.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core/content.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core/env.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core/scripts.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core/services.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core/web_apps.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/packs/jupyterlab.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/packs/mariadb.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/packs/nbclassic.rst
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/packs/tutorial_server.rst
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/content.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/environment.rst
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/flags.rst
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/hacks.rst
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/image.rst
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/index.rst
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/jupyter_server_config.rst
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/module.rst
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/packages.rst
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/packs.rst
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/scripts.rst
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/server.rst
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/services.rst
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/sources.rst
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/web_apps.rst
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/code-server.rst
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/index.rst
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/jupyterlab.rst
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/mariadb.rst
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/nbclassic.rst
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/tutorial_server.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/__about__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/__init__.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/__main__.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/builder.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/settings.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/utils.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/base.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/content.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/env.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/hacks.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/jupyter_server.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/packages.py
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/scripts.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/services.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/startup.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/web_apps.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/__init__.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/code_server.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/jupyterlab.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/mariadb.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/nbclassic.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/tutorial_server.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/Dockerfile.jinja2
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/core/content/content_config.yaml
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/core/services/sudoers
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/core/startup/home-dir.sudoers
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/core/startup/start.sh
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/packs/code_server/vscode.svg
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/packs/mariadb/setup.sh
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/packs/tutorial-server/production.ini
+-rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/demo-tests.sh
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/run-all.sh
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/code_server/ContainerConfig.yaml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/code_server_pinned/ContainerConfig.yaml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/custom_apt_key_dearmor/ContainerConfig.yaml
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod.conf
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/jupyterlab/v3/ContainerConfig.yaml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/jupyterlab/v4/ContainerConfig.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/mariadb/ContainerConfig.yaml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/nbclassic/ContainerConfig.yaml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/nbclassic/content/Welcome.ipynb
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/openrefine/ContainerConfig.yaml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/tutorial_server/ContainerConfig.yaml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/tutorial_server/content/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_content_settings.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_hacks_settings.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_image_settings.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_module_settings.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_packages_settings.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_scripts_settings.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_server_settings.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_sources_settings.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_webapps_settings.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/util.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.gitignore
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/README.md
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/PKG-INFO
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/__main__.py` & `ou_container_builder-2.6.0/ou_container_builder/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 """The main OU Container Builder commandline application.
 
 Run ``ou-container-builder --help`` for help with the command-line parameters.
 """
 import click
 import os
 
+from pydantic import ValidationError
 from yaml import safe_load
 
-from .builder import run_build
-from .validator import ValidationException
+from ou_container_builder.builder import run_build
 
 
 @click.command()
-@click.option('-c', '--context',
-              default='.',
-              help='Context within which the container will be built',
-              show_default=True)
-@click.option('-b/-nb', '--build/--no-build',
-              default=True,
-              help='Automatically build the container',
-              show_default=True)
-@click.option('--clean/--no-clean',
-              default=True,
-              help='Automatically clean up after building the container',
-              show_default=True)
-@click.option('--tag',
-              multiple=True,
-              help='Automatically tag the generated image')
+@click.option(
+    "-c", "--context", default=".", help="Context within which the container will be built", show_default=True
+)
+@click.option("-b/-nb", "--build/--no-build", default=True, help="Automatically build the container", show_default=True)
+@click.option(
+    "--clean/--no-clean", default=True, help="Automatically clean up after building the container", show_default=True
+)
+@click.option("--tag", multiple=True, help="Automatically tag the generated image")
 def main(context: str, build: bool, clean: bool, tag: list):
     """Build your OU Container."""
-    with open(os.path.join(context, 'ContainerConfig.yaml')) as config_f:
+    with open(os.path.join(context, "ContainerConfig.yaml")) as config_f:
         settings = safe_load(config_f)
     try:
         run_build(settings, context, build, clean, tag)
-    except ValidationException as ve:
-        click.echo(click.style('There are errors in your configuration settings:', fg='red'), err=True)
+    except ValidationError as ve:
+        click.echo(click.style("There are errors in your configuration settings:", fg="red"), err=True)
         click.echo(err=True)
-        for error in ve.errors:
-            click.echo(error, err=True)
+        for error in ve.errors():
+            click.echo(click.style(f"{'.'.join([str(v) for v in error['loc']])}: {error['msg']}", fg="red"), err=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/builder.py` & `ou_container_builder-2.6.0/ou_container_builder/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 """The main OU Container Builder commandline application.
 
 Run ``ou-container-builder --help`` for help with the command-line parameters.
 """
 import os
 import shutil
 import subprocess
-
 from copy import deepcopy
+
 from jinja2 import Environment, PackageLoader
 
-from . import packs, core
-from .validator import validate_settings
+from ou_container_builder import core, packs
+from ou_container_builder.settings import Settings
 
 
 def clean_build(context: str) -> None:
     """Clean the build files.
 
     :param context: The context directory containing the build files.
     :type context: str
     """
-    if os.path.exists(os.path.join(context, 'Dockerfile')):
-        os.unlink(os.path.join(context, 'Dockerfile'))
-    if os.path.exists(os.path.join(context, 'ou-builder-build')):
-        shutil.rmtree(os.path.join(context, 'ou-builder-build'))
+    if os.path.exists(os.path.join(context, "Dockerfile")):
+        os.unlink(os.path.join(context, "Dockerfile"))
+    if os.path.exists(os.path.join(context, "ou-builder-build")):
+        shutil.rmtree(os.path.join(context, "ou-builder-build"))
 
 
 def process_settings(settings: dict) -> dict:
     """Process the settings.
 
     :param settings: The settings provided by the user on the command-line
     :type settings: dict
     :return: The validated settings
     :rtype: dict
     """
     # Setup the base settings
-    settings = core.base.process_settings(validate_settings(settings))
+    settings = core.base.process_settings(Settings(**settings).dict())
     # Handle optional packs
-    if 'packs' in settings:
-        for pack in settings['packs']:
-            if pack['name'] == 'code_server':
-                settings = packs.code_server.process_settings(settings, pack['options'])
-            elif pack['name'] == 'jupyterlab':
-                settings = packs.jupyterlab.process_settings(settings, pack['options'])
-            elif pack['name'] == 'mariadb':
-                settings = packs.mariadb.process_settings(settings, pack['options'])
-            elif pack['name'] == 'nbclassic':
-                settings = packs.nbclassic.process_settings(settings, pack['options'])
-            elif pack['name'] == 'tutorial_server':
-                settings = packs.tutorial_server.process_settings(settings, pack['options'])
+    if "packs" in settings:
+        for pack in settings["packs"]:
+            if pack["name"] == "code_server":
+                settings = packs.code_server.process_settings(settings, pack["options"])
+            elif pack["name"] == "jupyterlab":
+                settings = packs.jupyterlab.process_settings(settings, pack["options"])
+            elif pack["name"] == "mariadb":
+                settings = packs.mariadb.process_settings(settings, pack["options"])
+            elif pack["name"] == "nbclassic":
+                settings = packs.nbclassic.process_settings(settings, pack["options"])
+            elif pack["name"] == "tutorial_server":
+                settings = packs.tutorial_server.process_settings(settings, pack["options"])
     # Handle core packs
     settings = core.env.process_settings(settings)
-    if 'services' in settings:
+    if "services" in settings:
         settings = core.services.process_settings(settings)
-    if 'scripts' in settings:
+    if "scripts" in settings:
         settings = core.scripts.process_settings(settings)
-    if 'web_apps' in settings:
+    if "web_apps" in settings:
         settings = core.web_apps.process_settings(settings)
     settings = core.hacks.process_settings(settings)
     settings = core.jupyter_server.process_settings(settings)
     settings = core.startup.process_settings(settings)
     settings = core.content.process_settings(settings)
     settings = core.packages.process_settings(settings)
-    return validate_settings(settings)
+    return Settings(**settings).dict()
 
 
 def generate_files(settings: dict, context: str, env: Environment, user_settings: dict) -> None:
     """Generate the files required for the Docker build.
 
     :param settings: The validated settings
     :type settings: dict
     :param context: The context directory
     :type context: str
     :param en: The jinja2 environment
     :type env: :class:`~jinja2.environment.Environment`
     """
-    if 'packs' in settings:
-        for pack in settings['packs']:
-            if pack['name'] == 'code_server':
-                packs.code_server.generate_files(context, env, settings, pack['options'])
-            elif pack['name'] == 'jupyterlab':
-                packs.jupyterlab.generate_files(context, env, settings, pack['options'])
-            elif pack['name'] == 'mariadb':
-                packs.mariadb.generate_files(context, env, settings, pack['options'])
-            elif pack['name'] == 'nbclassic':
-                packs.nbclassic.generate_files(context, env, settings, pack['options'])
-            elif pack['name'] == 'tutorial_server':
-                packs.tutorial_server.generate_files(context, env, settings, pack['options'])
+    if "packs" in settings:
+        for pack in settings["packs"]:
+            if pack["name"] == "code_server":
+                packs.code_server.generate_files(context, env, settings, pack["options"])
+            elif pack["name"] == "jupyterlab":
+                packs.jupyterlab.generate_files(context, env, settings, pack["options"])
+            elif pack["name"] == "mariadb":
+                packs.mariadb.generate_files(context, env, settings, pack["options"])
+            elif pack["name"] == "nbclassic":
+                packs.nbclassic.generate_files(context, env, settings, pack["options"])
+            elif pack["name"] == "tutorial_server":
+                packs.tutorial_server.generate_files(context, env, settings, pack["options"])
     core.env.generate_files(context, env, settings)
-    if 'services' in settings:
+    if "services" in settings:
         core.services.generate_files(context, env, settings)
-    if 'scripts' in settings:
+    if "scripts" in settings:
         core.scripts.generate_files(context, env, settings)
-    if 'web_apps' in settings:
+    if "web_apps" in settings:
         core.web_apps.generate_files(context, env, settings)
     core.hacks.generate_files(context, env, settings)
     core.jupyter_server.generate_files(context, env, settings, user_settings)
     core.startup.generate_files(context, env, settings)
     core.content.generate_files(context, env, settings)
     core.packages.generate_files(context, env, settings)
 
     # Generate the Dockerfile
-    with open(os.path.join(context, 'Dockerfile'), 'w') as out_f:
-        tmpl = env.get_template('Dockerfile.jinja2')
+    with open(os.path.join(context, "Dockerfile"), "w") as out_f:
+        tmpl = env.get_template("Dockerfile.jinja2")
         out_f.write(tmpl.render(**settings))
 
 
 def docker_build(context: str, tag: list) -> None:
     """Run the docker build.
 
     :param context: The build context directory
     :type context: str
     :param tag: The tags to apply to the Docker image
     :type tag: list
     """
-    cmd = ['docker', 'build', context]
+    cmd = ["docker", "build", context]
     if tag:
         for t in tag:
-            cmd.append('--tag')
+            cmd.append("--tag")
             cmd.append(t)
     subprocess.run(cmd)
 
 
 def run_build(settings: dict, context: str, build: bool, clean: bool, tag: list) -> None:
     """Run the build process.
 
@@ -139,17 +139,17 @@
     :return: A list with any errors that occured during processing
     :rtype: list
     """
     # Process and validate the settings
     user_settings = deepcopy(settings)  # Todo: fix this in 3.0.0
     settings = process_settings(settings)
     # Setup the build environment
-    env = Environment(loader=PackageLoader('ou_container_builder', 'templates'), autoescape=False)
+    env = Environment(loader=PackageLoader("ou_container_builder", "templates"), autoescape=False)
     clean_build(context)
-    os.makedirs(os.path.join(context, 'ou-builder-build'))
+    os.makedirs(os.path.join(context, "ou-builder-build"))
     # Run the file generation
     generate_files(settings, context, env, user_settings)
 
     if build:
         docker_build(context, tag)
         if clean:
             clean_build(context)
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/core/base.py` & `ou_container_builder-2.6.0/ou_container_builder/core/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """Pack to handle setting up the base settings.
 
 This provides a few minimal initial settings.
 """
 from jinja2 import Environment
 
-from ..utils import merge_settings
+from ou_container_builder.utils import merge_settings
 
 
 def process_settings(settings: dict) -> dict:
     """Process the content core settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    settings = merge_settings({
-        'packages': {
-            'apt': ['libcurl3-gnutls', 'libcurl3-gnutls-dev', 'gnutls-dev', 'gcc', 'build-essential'],
-            'pip': ['pycurl'],
-        }
-    }, settings)
+    settings = merge_settings(
+        {
+            "packages": {
+                "apt": ["libcurl3-gnutls", "libcurl3-gnutls-dev", "gnutls-dev", "gcc", "build-essential"],
+                "pip": ["pycurl"],
+            }
+        },
+        settings,
+    )
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict) -> None:
     """Generate the build files for the base core.
 
     :param context: The context path within which the generation is running
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/core/content.py` & `ou_container_builder-2.6.0/ou_container_builder/core/content.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,62 +4,51 @@
 files are distributed in the container as configured. This also sets the ``ou_container_content`` flag to ensure
 that the OU Container Content application is run upon container startup.
 """
 import os
 
 from jinja2 import Environment
 
-from ..utils import merge_settings, render_template
+from ou_container_builder.utils import merge_settings, render_template
 
 
 def process_settings(settings: dict) -> dict:
     """Process the content core settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    if 'content' in settings and settings['content']:
-        settings = merge_settings(settings, {
-            'flags': {
-                'ou_container_content': True
-            }
-        })
-    if 'flags' in settings and settings['flags']:
-        if 'ou_container_content' in settings['flags'] and settings['flags']['ou_container_content']:
-            settings = merge_settings(settings, {
-                'packages': {
-                    'pip': [
-                        'ou-container-content>=1.1.3'
-                    ]
+    if "content" in settings and settings["content"]:
+        settings = merge_settings(settings, {"flags": {"ou_container_content": True}})
+    if "flags" in settings and settings["flags"]:
+        if "ou_container_content" in settings["flags"] and settings["flags"]["ou_container_content"]:
+            settings = merge_settings(
+                settings,
+                {
+                    "packages": {"pip": ["ou-container-content>=1.1.3"]},
+                    "scripts": {"build": [{"commands": ["ou-container-content prepare"]}]},
                 },
-                'scripts': {
-                    'build': [
-                        {
-                            'commands': [
-                                'ou-container-content prepare'
-                            ]
-                        }
-                    ]
-                }
-            })
+            )
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict) -> None:
     """Generate the build files for the content core.
 
     :param context: The context path within which the generation is running
     :type context: str
     :param env: The Jinja2 environment to use for loading and rendering templates
     :type env: :class:`~jinja2.environment.Environment`
     :param settings: The validated settings
     :type settings: dict
     """
-    if 'flags' in settings and settings['flags']:
-        if 'ou_container_content' in settings['flags'] and settings['flags']['ou_container_content']:
-            render_template(context,
-                            env,
-                            'core/content/content_config.yaml',
-                            os.path.join('ou-builder-build', 'content', 'content_config.yaml'),
-                            settings)
+    if "flags" in settings and settings["flags"]:
+        if "ou_container_content" in settings["flags"] and settings["flags"]["ou_container_content"]:
+            render_template(
+                context,
+                env,
+                "core/content/content_config.yaml",
+                os.path.join("ou-builder-build", "content", "content_config.yaml"),
+                settings,
+            )
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/core/env.py` & `ou_container_builder-2.6.0/ou_container_builder/core/env.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.5.0/ou_container_builder/core/hacks.py` & `ou_container_builder-2.6.0/ou_container_builder/core/hacks.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     """Process the hacks core settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    if 'packages' in settings and 'apt' in settings['packages']:
-        if 'openjdk-11-jdk' in settings['packages']['apt']:
-            if 'hacks' in settings:
-                if 'missing-man1' not in settings['hacks']:
-                    settings['hacks'].append('missing-man1')
+    if "packages" in settings and "apt" in settings["packages"]:
+        if "openjdk-11-jdk" in settings["packages"]["apt"]:
+            if "hacks" in settings:
+                if "missing-man1" not in settings["hacks"]:
+                    settings["hacks"].append("missing-man1")
             else:
-                settings['hacks'] = ['missing-man1']
+                settings["hacks"] = ["missing-man1"]
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict) -> dict:
     """Generate the build files for the hacks core.
 
     :param context: The context path within which the generation is running
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/core/jupyter_server.py` & `ou_container_builder-2.6.0/ou_container_builder/core/jupyter_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,79 @@
 """Pack to handle setting up jupyter_server."""
 import json
 import os.path
 
 from jinja2 import Environment
 
-from ..utils import merge_settings
+from ou_container_builder.utils import merge_settings
 
 
 def process_settings(settings: dict) -> dict:
     """Process the jupyter_server core settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    settings = merge_settings(settings, {
-        'packages': {
-            'apt': [
-                'sudo'
+    settings = merge_settings(
+        settings,
+        {
+            "packages": {"apt": ["sudo"], "pip": ["jupyter_server<4.0.0", "jupyterhub<1.6.0"]},
+            "content": [
+                {
+                    "source": "ou-builder-build/ou_core_config.json",
+                    "target": "/usr/local/etc/jupyter/jupyter_server_config.json",
+                    "overwrite": "always",
+                }
             ],
-            'pip': [
-                'jupyter_server<2.0.0',
-                'jupyterhub<1.6.0'
-            ]
+            "jupyter_server_config": {
+                "ServerApp": {
+                    "ip": "0.0.0.0",
+                    "port": 8888,
+                    "quit_button": False,
+                    "trust_xheaders": True,
+                    "iopub_data_rate_limit": 10000000,
+                },
+                "NotebookApp": {"quit_button": False},
+            },
         },
-        'content': [
+    )
+    if "access_token" in settings["server"] and settings["server"]["access_token"]:
+        settings = merge_settings(
+            settings, {"jupyter_server_config": {"ServerApp": {"token": settings["server"]["access_token"]}}}
+        )
+    if "wrapper_host" in settings["server"] and settings["server"]["wrapper_host"]:
+        settings = merge_settings(
+            settings,
             {
-                'source': 'ou-builder-build/ou_core_config.json',
-                'target': '/usr/local/etc/jupyter/jupyter_server_config.json',
-                'overwrite': 'always'
-            }
-        ],
-        'jupyter_server_config': {
-            'ServerApp': {
-                'ip': '0.0.0.0',
-                'port': 8888,
-                'quit_button': False,
-                'trust_xheaders': True,
-                'iopub_data_rate_limit': 10000000
-            },
-            'NotebookApp': {
-                'quit_button': False
-            }
-        }
-    })
-    if 'access_token' in settings['server'] and settings['server']['access_token']:
-        settings = merge_settings(settings, {
-            'jupyter_server_config': {
-                'ServerApp': {
-                    'token': settings['server']['access_token']
-                }
-            }
-        })
-    if 'wrapper_host' in settings['server'] and settings['server']['wrapper_host']:
-        settings = merge_settings(settings, {
-            'jupyter_server_config': {
-                'ServerApp': {
-                    'tornado_settings': {
-                        'headers': {
-                            'Content-Security-Policy': f"frame-ancestors 'self' {settings['server']['wrapper_host']}",
-                            'Access-Control-Allow-Origin': f'{settings["server"]["wrapper_host"]}',
+                "jupyter_server_config": {
+                    "ServerApp": {
+                        "tornado_settings": {
+                            "headers": {
+                                "Content-Security-Policy": f"frame-ancestors 'self' {settings['server']['wrapper_host']}",
+                                "Access-Control-Allow-Origin": f'{settings["server"]["wrapper_host"]}',
+                            }
                         }
                     }
                 }
-            }
-        })
+            },
+        )
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict, user_settings) -> dict:
     """Generate the build files the jupyter_server core.
 
     :param context: The context path within which the generation is running
     :type context: str
     :param env: The Jinja2 environment to use for loading and rendering templates
     :type env: :class:`~jinja2.environment.Environment`
     :param settings: The validated settings
     :type settings: dict
     """
-    if 'server' in user_settings and 'default_path' in user_settings['server']:
-        settings = merge_settings(settings, {
-            'jupyter_server_config': {
-                'ServerApp': {
-                    'default_url': user_settings['server']['default_path']
-                }
-            }
-        })
-    with open(os.path.join(context, 'ou-builder-build', 'ou_core_config.json'), 'w') as out_f:
-        json.dump(settings['jupyter_server_config'], out_f)
+    if "server" in user_settings and "default_path" in user_settings["server"]:
+        settings = merge_settings(
+            settings, {"jupyter_server_config": {"ServerApp": {"default_url": user_settings["server"]["default_path"]}}}
+        )
+    with open(os.path.join(context, "ou-builder-build", "ou_core_config.json"), "w") as out_f:
+        json.dump(settings["jupyter_server_config"], out_f)
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/core/packages.py` & `ou_container_builder-2.6.0/ou_container_builder/core/packages.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """Pack to handle packages."""
 from jinja2 import Environment
 
-from ..utils import merge_settings
+from ou_container_builder.utils import merge_settings
 
 
 def process_settings(settings: dict) -> dict:
     """Process the env core settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    settings = merge_settings(settings, {
-        'packages': {
-            'apt': ['libcurl3-gnutls'],
-            'pip': ['pycurl'],
-        }
-    })
-
-    if 'packages' in settings:
-        if 'apt' in settings['packages']:
-            settings['packages']['apt'].sort()
-        if 'pip' in settings['packages']:
-            settings['packages']['pip'].sort()
+    settings = merge_settings(
+        settings,
+        {
+            "packages": {
+                "apt": ["libcurl3-gnutls"],
+                "pip": ["pycurl"],
+            }
+        },
+    )
+
+    if "packages" in settings:
+        if "apt" in settings["packages"]:
+            settings["packages"]["apt"].sort()
+        if "pip" in settings["packages"]:
+            settings["packages"]["pip"].sort()
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict) -> dict:
     """Generate the build files for the env core.
 
     :param context: The context path within which the generation is running
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/core/scripts.py` & `ou_container_builder-2.6.0/ou_container_builder/core/scripts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,67 @@
 """Pack to handle scripts."""
 import os
-
 from hashlib import sha256
+
 from jinja2 import Environment
 
-from ..utils import merge_settings
+from ou_container_builder.utils import merge_settings
 
 
 def process_settings(settings: dict) -> dict:
     """Process the env core settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    if 'startup' in settings['scripts']:
-        settings = merge_settings(settings, {
-            'flags': {
-                'ou_container_content': True
-            }
-        })
+    if "startup" in settings["scripts"]:
+        settings = merge_settings(settings, {"flags": {"ou_container_content": True}})
         new_settings = {}
-        for script in settings['scripts']['startup']:
-            if len(script['commands']) > 1:
-                hash = sha256('\n'.join(script['commands']).encode())
-                script_name = f'startup-script-{hash.hexdigest()}'
-                new_settings = merge_settings(new_settings, {
-                    'content': [
-                        {
-                            'source': os.path.join('ou-builder-build', script_name),
-                            'target': f'/usr/bin/{script_name}',
-                            'overwrite': 'always'
-                        }
-                    ],
-                    'scripts': {
-                        'build': [
+        for script in settings["scripts"]["startup"]:
+            if len(script["commands"]) > 1:
+                hash = sha256("\n".join(script["commands"]).encode())
+                script_name = f"startup-script-{hash.hexdigest()}"
+                new_settings = merge_settings(
+                    new_settings,
+                    {
+                        "content": [
                             {
-                                'commands': [f'chmod a+x /usr/bin/{script_name}']
+                                "source": os.path.join("ou-builder-build", script_name),
+                                "target": f"/usr/bin/{script_name}",
+                                "overwrite": "always",
                             }
-                        ]
-                    }
-                })
-                script['commands'] = [
-                    f'/usr/bin/{script_name}'
-                ]
+                        ],
+                        "scripts": {"build": [{"commands": [f"chmod a+x /usr/bin/{script_name}"]}]},
+                    },
+                )
+                script["commands"] = [f"/usr/bin/{script_name}"]
         settings = merge_settings(settings, new_settings)
-    if 'shutdown' in settings['scripts']:
-        settings = merge_settings(settings, {
-            'flags': {
-                'ou_container_content': True
-            }
-        })
+    if "shutdown" in settings["scripts"]:
+        settings = merge_settings(settings, {"flags": {"ou_container_content": True}})
         new_settings = {}
-        for script in settings['scripts']['shutdown']:
-            if len(script['commands']) > 1:
-                hash = sha256('\n'.join(script['commands']).encode())
-                script_name = f'shutdown-script-{hash.hexdigest()}'
-                new_settings = merge_settings(new_settings, {
-                    'content': [
-                        {
-                            'source': os.path.join('ou-builder-build', script_name),
-                            'target': f'/usr/bin/{script_name}',
-                            'overwrite': 'always'
-                        }
-                    ],
-                    'scripts': {
-                        'build': [
+        for script in settings["scripts"]["shutdown"]:
+            if len(script["commands"]) > 1:
+                hash = sha256("\n".join(script["commands"]).encode())
+                script_name = f"shutdown-script-{hash.hexdigest()}"
+                new_settings = merge_settings(
+                    new_settings,
+                    {
+                        "content": [
                             {
-                                'commands': [f'chmod a+x /usr/bin/{script_name}']
+                                "source": os.path.join("ou-builder-build", script_name),
+                                "target": f"/usr/bin/{script_name}",
+                                "overwrite": "always",
                             }
-                        ]
-                    }
-                })
-                script['commands'] = [
-                    f'/usr/bin/{script_name}'
-                ]
+                        ],
+                        "scripts": {"build": [{"commands": [f"chmod a+x /usr/bin/{script_name}"]}]},
+                    },
+                )
+                script["commands"] = [f"/usr/bin/{script_name}"]
         settings = merge_settings(settings, new_settings)
 
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict) -> dict:
     """Generate the build files for the scripts core.
@@ -87,21 +69,21 @@
     :param context: The context path within which the generation is running
     :type context: str
     :param env: The Jinja2 environment to use for loading and rendering templates
     :type env: :class:`~jinja2.environment.Environment`
     :param settings: The validated settings
     :type settings: dict
     """
-    if 'startup' in settings['scripts']:
-        for script in settings['scripts']['startup']:
-            if len(script['commands']) > 1:
-                hash = sha256('\n'.join(script['commands']).encode())
-                script_name = f'startup-script-{hash.hexdigest()}'
-                with open(os.path.join(context, 'ou-builder-build', script_name), 'w') as out_f:
-                    out_f.write('\n'.join(script['commands']))
-    if 'shutdown' in settings['scripts']:
-        for script in settings['scripts']['shutdown']:
-            if len(script['commands']) > 1:
-                hash = sha256('\n'.join(script['commands']).encode())
-                script_name = f'shutdown-script-{hash.hexdigest()}'
-                with open(os.path.join(context, 'ou-builder-build', script_name), 'w') as out_f:
-                    out_f.write('\n'.join(script['commands']))
+    if "startup" in settings["scripts"]:
+        for script in settings["scripts"]["startup"]:
+            if len(script["commands"]) > 1:
+                hash = sha256("\n".join(script["commands"]).encode())
+                script_name = f"startup-script-{hash.hexdigest()}"
+                with open(os.path.join(context, "ou-builder-build", script_name), "w") as out_f:
+                    out_f.write("\n".join(script["commands"]))
+    if "shutdown" in settings["scripts"]:
+        for script in settings["scripts"]["shutdown"]:
+            if len(script["commands"]) > 1:
+                hash = sha256("\n".join(script["commands"]).encode())
+                script_name = f"shutdown-script-{hash.hexdigest()}"
+                with open(os.path.join(context, "ou-builder-build", script_name), "w") as out_f:
+                    out_f.write("\n".join(script["commands"]))
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/core/services.py` & `ou_container_builder-2.6.0/ou_container_builder/core/startup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,60 @@
-"""Pack to setup and run system services.
+"""Pack to handle setting up the startup process in the container.
 
-Automatically generates a sudoers file that ensures that the default user can start and stop all services.
+Generates the startup script and the sudoers file to ensure the user can chown their home-directory.
 """
-import os
+import os.path
 
 from jinja2 import Environment
 
-from ..utils import merge_settings, render_template
+from ou_container_builder.utils import merge_settings, render_template
 
 
 def process_settings(settings: dict) -> dict:
-    """Process the services core settings.
+    """Process the startup core settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    settings = merge_settings(settings, {
-        'content': [
-            {
-                'source': 'ou-builder-build/services/services.sudoers',
-                'target': '/etc/sudoers.d/99-services',
-                'overwrite': 'always'
-            }
-        ],
-        'flags': {
-            'ou_container_content': True
-        }
-    })
+    settings = merge_settings(
+        settings,
+        {
+            "content": [
+                {"source": "ou-builder-build/startup/start.sh", "target": "/usr/bin/start.sh", "overwrite": "always"},
+                {
+                    "source": "ou-builder-build/startup/home-dir.sudoers",
+                    "target": "/etc/sudoers.d/99-home-dir",
+                    "overwrite": "always",
+                },
+            ],
+            "scripts": {
+                "build": [{"commands": ["chmod a+x /usr/bin/start.sh", "chmod 0660 /etc/sudoers.d/99-home-dir"]}]
+            },
+        },
+    )
     return settings
 
 
-def generate_files(context: str, env: Environment, settings: dict) -> None:
-    """Generate the build files for the services core.
+def generate_files(context: str, env: Environment, settings: dict) -> dict:
+    """Generate the build files for the startup core.
 
     :param context: The context path within which the generation is running
     :type context: str
     :param env: The Jinja2 environment to use for loading and rendering templates
     :type env: :class:`~jinja2.environment.Environment`
     :param settings: The validated settings
     :type settings: dict
     """
-    render_template(context,
-                    env,
-                    'core/services/sudoers',
-                    os.path.join('ou-builder-build', 'services', 'services.sudoers'),
-                    settings)
+    # Generate the start script
+    render_template(
+        context, env, "core/startup/start.sh", os.path.join("ou-builder-build", "startup", "start.sh"), settings
+    )
+    # Generate the home-dir chown sudoers
+    render_template(
+        context,
+        env,
+        "core/startup/home-dir.sudoers",
+        os.path.join("ou-builder-build", "startup", "home-dir.sudoers"),
+        settings,
+    )
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/core/web_apps.py` & `ou_container_builder-2.6.0/ou_container_builder/core/web_apps.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 """Pack to handle web_apps setups.
 
 This simply sets the server's default_path, if a web application is set as the default.
 """
 from copy import deepcopy
-from jinja2 import Environment
 from warnings import warn
 
-from ..utils import merge_settings
+from jinja2 import Environment
+
+from ou_container_builder.utils import merge_settings
 
 
 def process_settings(settings: dict) -> dict:
     """Process the env core settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    if len(settings['web_apps']) > 0:
-        settings = merge_settings(settings, {
-            'packages': {
-                'pip': [
-                    'jupyter-server-proxy>=3.2.1,<4.0.0'
-                ]
-            }
-        })
+    if len(settings["web_apps"]) > 0:
+        settings = merge_settings(settings, {"packages": {"pip": ["jupyter-server-proxy>=3.2.1,<4.0.0"]}})
     servers = {}
-    for web_app in settings['web_apps']:
-        if 'cmdline' in web_app:
-            if 'command' in web_app:
-                warn('Both cmdline and command specified for a web_app. As cmdline is deprecated in 2.2.0, command takes preceence.', FutureWarning)  # noqa: E501
+    for web_app in settings["web_apps"]:
+        if "cmdline" in web_app:
+            if "command" in web_app:
+                warn(
+                    "Both cmdline and command specified for a web_app. As cmdline is deprecated in 2.2.0, command takes preceence.",
+                    FutureWarning,
+                )
             else:
-                warn('The cmdline setting for a web_app is deprecated in 2.2.0 and will be removed for version 3.0.0. Use command instead.', FutureWarning)  # noqa: E501
-                web_app['command'] = web_app['cmdline']
-            del web_app['cmdline']
-        elif 'command' not in web_app:
-            warn('No command specified for the web_app')
-        if 'default' in web_app:
-            warn('The default setting in the web_app configuration is deprecated in 2.2.0 and will be removed in 3.0.0. Use server.default_path instead', FutureWarning)  # noqa: E501
-            if web_app['default']:
-                settings = merge_settings(settings, {
-                    'server': {
-                        'default_path': web_app['path']
-                    }
-                })
-            del web_app['default']
-        path = web_app['path']
+                warn(
+                    "The cmdline setting for a web_app is deprecated in 2.2.0 and will be removed for version 3.0.0. Use command instead.",
+                    FutureWarning,
+                )
+                web_app["command"] = web_app["cmdline"]
+            del web_app["cmdline"]
+        elif "command" not in web_app:
+            warn("No command specified for the web_app")
+        if "default" in web_app:
+            warn(
+                "The default setting in the web_app configuration is deprecated in 2.2.0 and will be removed in 3.0.0. Use server.default_path instead",
+                FutureWarning,
+            )
+            if web_app["default"]:
+                settings = merge_settings(settings, {"server": {"default_path": web_app["path"]}})
+            del web_app["default"]
+        path = web_app["path"]
         servers[path] = deepcopy(web_app)
-        del servers[path]['path']
-    settings = merge_settings(settings, {
-        'jupyter_server_config': {
-            'ServerProxy': {
-                'servers': servers
-            }
-        }
-    })
+        del servers[path]["path"]
+    settings = merge_settings(settings, {"jupyter_server_config": {"ServerProxy": {"servers": servers}}})
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict) -> None:
     """Generate the build files for the web_apps core.
 
     :param context: The context path within which the generation is running
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/packs/code_server.py` & `ou_container_builder-2.6.0/ou_container_builder/packs/code_server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,121 @@
 """Pack to install the Code Server interface."""
 import os
-
-from jinja2 import Environment
 from importlib import resources
+from pydantic import BaseModel
+from typing import Literal
 from warnings import warn
 
-from ..utils import merge_settings
+from jinja2 import Environment
+
+from ou_container_builder.utils import merge_settings
+
+
+class Options(BaseModel):
+    version: str = "4.14.1"
+    extensions: list[str] = []
+
+
+class Pack(BaseModel):
+    name: Literal["code_server"]
+    options: Options = Options()
 
 
 def process_settings(settings: dict, pack_settings: dict) -> dict:
     """
     Process the user-provided settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :param pack_settings: The pack-specific settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    if 'version' in pack_settings:
-        version = pack_settings['version']
-    else:
-        version = '4.12.0'
-    warn('Automatically setting the code_server as the default web-app is deprecated in 2.2.0 and will be removed in 3.0.0. Instead set server.default_path explicitly.', FutureWarning)  # noqa: E501
-    settings = merge_settings(settings, {
-        'sources': {
-            'apt': [
-                {
-                    'name': 'nodesource',
-                    'key_url': 'https://deb.nodesource.com/gpgkey/nodesource.gpg.key',
-                    'dearmor': True,
-                    'deb': {
-                        'url': 'https://deb.nodesource.com/node_18.x',
-                        'distribution': 'bullseye',
-                        'component': 'main'
+    version = pack_settings["version"]
+    warn(
+        "Automatically setting the code_server as the default web-app is deprecated in 2.2.0 and will be removed in 3.0.0. Instead set server.default_path explicitly.",
+        FutureWarning,
+    )
+    settings = merge_settings(
+        settings,
+        {
+            "sources": {
+                "apt": [
+                    {
+                        "name": "nodesource",
+                        "key_url": "https://deb.nodesource.com/gpgkey/nodesource.gpg.key",
+                        "dearmor": True,
+                        "deb": {
+                            "url": "https://deb.nodesource.com/node_18.x",
+                            "distribution": "bullseye",
+                            "component": "main",
+                        },
                     }
-                }
-            ],
-        },
-        'packages': {
-            'apt': [
-                'nodejs',
-                'yarn'
+                ],
+            },
+            "packages": {
+                "apt": ["nodejs", "yarn"],
+            },
+            "scripts": {
+                "build": [
+                    {
+                        "commands": [
+                            "cd /opt",
+                            f"curl -L --output code-server.tar.gz https://github.com/coder/code-server/releases/download/v{version}/code-server-{version}-linux-amd64.tar.gz",  # noqa: E501
+                            "tar -zxvf code-server.tar.gz",
+                            f"ln -s /opt/code-server-{version}-linux-amd64/bin/code-server /usr/local/bin",
+                        ]
+                    }
+                ]
+            },
+            "content": [
+                {
+                    "source": "ou-builder-build/packs/code_server/logo.svg",
+                    "target": "/var/lib/code_server/logo.svg",
+                    "overwrite": "always",
+                },
             ],
-        },
-        'scripts': {
-            'build': [
+            "web_apps": [
                 {
-                    'commands': [
-                        'cd /opt',
-                        f'curl -L --output code-server.tar.gz https://github.com/coder/code-server/releases/download/v{version}/code-server-{version}-linux-amd64.tar.gz',  # noqa: E501
-                        'tar -zxvf code-server.tar.gz',
-                        f'ln -s /opt/code-server-{version}-linux-amd64/bin/code-server /usr/local/bin',
-                    ]
+                    "path": "code-server/",
+                    "command": [
+                        "code-server",
+                        "--auth",
+                        "none",
+                        "--disable-update-check",
+                        "--bind-addr",
+                        "0.0.0.0",
+                        "--port",
+                        "{port}",
+                    ],
+                    "timeout": 60,
+                    "default": True,
+                    "new_browser_tab": False,
+                    "launcher_entry": {"title": "VS Code", "icon_path": "/var/lib/code_server/logo.svg"},
                 }
-            ]
+            ],
         },
-        'content': [
+    )
+    if len(pack_settings["extensions"]) > 0:
+        settings = merge_settings(
+            settings,
             {
-                'source': 'ou-builder-build/packs/code_server/logo.svg',
-                'target': '/var/lib/code_server/logo.svg',
-                'overwrite': 'always'
-            },
-        ],
-        'web_apps': [
-            {
-                'path': 'code-server/',
-                'command': [
-                    'code-server',
-                    '--auth',
-                    'none',
-                    '--disable-update-check',
-                    '--bind-addr',
-                    '0.0.0.0',
-                    '--port',
-                    '{port}'
-                ],
-                'timeout': 60,
-                'default': True,
-                'new_browser_tab': False,
-                'launcher_entry': {
-                    'title': 'VS Code',
-                    'icon_path': '/var/lib/code_server/logo.svg'
+                "scripts": {
+                    "build": [
+                        {
+                            "commands": [
+                                f"code-server --install-extension {extension}"
+                                for extension in pack_settings["extensions"]
+                            ]
+                        }
+                    ]
                 }
-            }
-        ],
-    })
-    if 'extensions' in pack_settings and isinstance(pack_settings['extensions'], list):
-        settings = merge_settings(settings, {
-            'scripts': {
-                'build': [
-                    {
-                        'commands': [
-                            f'code-server --install-extension {extension}'
-                            for extension in pack_settings['extensions']
-                        ]
-                    }
-                ]
-            }
-        })
+            },
+        )
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict, pack_settings: dict) -> None:
     """Generate the build files for the code-server pack.
 
     This ensures that the the code-server is installed
@@ -113,15 +125,15 @@
     :param env: The Jinja2 environment to use for loading and rendering templates
     :type env: :class:`~jinja2.environment.Environment`
     :param settings: The validated settings
     :type settings: dict
     :param pack_settings: The validated pack-specific settings
     :type settings: dict
     """
-    source = resources.files('ou_container_builder') / 'templates' / 'packs' / 'code_server' / 'vscode.svg'
-    target_path = os.path.join(context, 'ou-builder-build', 'packs', 'code_server', 'logo.svg')
+    source = resources.files("ou_container_builder") / "templates" / "packs" / "code_server" / "vscode.svg"
+    target_path = os.path.join(context, "ou-builder-build", "packs", "code_server", "logo.svg")
     if not os.path.exists(os.path.dirname(target_path)):
         os.makedirs(os.path.dirname(target_path), exist_ok=True)
     with resources.as_file(source) as in_path:
-        with open(in_path, 'rb') as in_f:
-            with open(target_path, 'wb') as out_f:
+        with open(in_path, "rb") as in_f:
+            with open(target_path, "wb") as out_f:
                 out_f.write(in_f.read())
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/packs/jupyterlab.py` & `ou_container_builder-2.6.0/ou_container_builder/packs/nbclassic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,60 @@
-"""Pack to install the Jupyterlab interface."""
-from jinja2 import Environment
+"""Pack to install the Nbclassic notebook interface."""
 from warnings import warn
 
-from ..utils import merge_settings
+from jinja2 import Environment
+from pydantic import BaseModel
+from typing import Literal
+
+from ou_container_builder.utils import merge_settings
+
+
+class Options(BaseModel):
+    pass
+
+
+class Pack(BaseModel):
+    name: Literal["nbclassic"]
+    options: Options = Options()
 
 
 def process_settings(settings: dict, pack_settings: dict) -> dict:
     """
     Process the user-provided settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :param pack_settings: The pack-specific settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    warn('Automatically setting JupyterLab as the default is deprecated in 2.2.0 and will be removed in 3.0.0. Instead set server.default_path explicitly.', FutureWarning)  # noqa: E501
-    settings = merge_settings(settings, {
-        'packages': {
-            'pip': ['jupyterlab>=3.4.3,<4.0.0']
-        },
-        'server': {
-            'default_path': '/lab'
+    warn(
+        "Automatically setting Nbclassic as the default is deprecated in 2.2.0 and will be removed in 3.0.0. Instead set server.default_path explicitly.",
+        FutureWarning,
+    )
+    settings = merge_settings(
+        settings,
+        {
+            "packages": {"pip": ["nbclassic>=0.4.8,<1.0.0"]},
+            "server": {"default_path": "/tree"},
+            "scripts": {
+                "build": [
+                    {"commands": ["pip uninstall -y notebook", "jupyter server extension enable --system nbclassic"]}
+                ]
+            },
         },
-    })
+    )
     return settings
 
 
-def generate_files(context: str, env: Environment, settings: dict, pack_settings: dict) -> None:
-    """Generate the build files for the jupyterlab pack.
+def generate_files(context: str, env: Environment, settings: dict, pack_settings: dict) -> dict:
+    """Generate the build files for the nbclassic pack.
 
-    This ensures that the the jupyterlab package is installed
+    This ensures that the the nbclassic package is installed
 
     :param context: The context path within which the generation is running
     :type context: str
     :param env: The Jinja2 environment to use for loading and rendering templates
     :type env: :class:`~jinja2.environment.Environment`
     :param settings: The validated settings
     :type settings: dict
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/packs/mariadb.py` & `ou_container_builder-2.6.0/ou_container_builder/packs/mariadb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 """Pack to install the MariaDB database."""
 import os
 
 from jinja2 import Environment
+from pydantic import BaseModel
+from typing import Literal
 
-from ..utils import merge_settings, render_template
+from ou_container_builder.utils import merge_settings, render_template
+
+
+class Options(BaseModel):
+    pass
+
+
+class Pack(BaseModel):
+    name: Literal["mariadb"]
+    options: Options = Options()
 
 
 def process_settings(settings: dict, pack_settings: dict) -> dict:
     """Process the user-provided settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :param pack_settings: The pack-specific settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    settings = merge_settings(settings, {
-        'packages': {
-            'apt': ['mariadb-server', 'sudo']
-        },
-        'scripts': {
-            'build': [
+    settings = merge_settings(
+        settings,
+        {
+            "packages": {"apt": ["mariadb-server", "sudo"]},
+            "scripts": {
+                "build": [
+                    {
+                        "commands": [
+                            "mkdir -p /run/mysqld",
+                            f'sed -e "s#datadir.*=.*#datadir = $HOME/mariadb#" -e "s#user.*=.*#user = {settings["image"]["user"]}#" -i /etc/mysql/mariadb.conf.d/50-server.cnf',  # noqa: E501
+                            f'chown -R {settings["image"]["user"]}: /var/log/mysql /run/mysqld',
+                            "chmod a+x /usr/bin/mariadb-setup.sh",
+                            f'printf "{settings["image"]["user"]} ALL=NOPASSWD: /usr/bin/mariadb-setup.sh\\n" > /etc/sudoers.d/99-mariadb',  # noqa: E501
+                        ]
+                    },
+                ],
+                "startup": [{"commands": ["sudo /usr/bin/mariadb-setup.sh"]}],
+            },
+            "services": ["mariadb"],
+            "content": [
+                {"source": "/var/lib/mysql", "target": "mariadb", "overwrite": "never"},
                 {
-                    'commands': [
-                        'mkdir -p /run/mysqld',
-                        f'sed -e "s#datadir.*=.*#datadir = $HOME/mariadb#" -e "s#user.*=.*#user = {settings["image"]["user"]}#" -i /etc/mysql/mariadb.conf.d/50-server.cnf',  # noqa: E501
-                        f'chown -R {settings["image"]["user"]}: /var/log/mysql /run/mysqld',
-                        'chmod a+x /usr/bin/mariadb-setup.sh',
-                        f'printf "{settings["image"]["user"]} ALL=NOPASSWD: /usr/bin/mariadb-setup.sh\\n" > /etc/sudoers.d/99-mariadb'  # noqa: E501
-                    ]
+                    "source": "ou-builder-build/mariadb/mariadb-setup.sh",
+                    "target": "/usr/bin/mariadb-setup.sh",
+                    "overwrite": "always",
                 },
             ],
-            'startup': [
-                {
-                    'commands': [
-                        'sudo /usr/bin/mariadb-setup.sh'
-                    ]
-                }
-            ]
         },
-        'services': [
-            'mariadb'
-        ],
-        'content': [
-            {
-                'source': '/var/lib/mysql',
-                'target': 'mariadb',
-                'overwrite': 'never'
-            },
-            {
-                'source': 'ou-builder-build/mariadb/mariadb-setup.sh',
-                'target': '/usr/bin/mariadb-setup.sh',
-                'overwrite': 'always'
-            }
-        ]
-    })
+    )
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict, pack_settings: dict) -> None:
     """Generate the build files for the mariadb pack.
 
     This ensures that the the mariadb service is activated and that the configured database is set up in the user's
@@ -70,12 +70,14 @@
     :param env: The Jinja2 environment to use for loading and rendering templates
     :type env: :class:`~jinja2.environment.Environment`
     :param settings: The validated settings
     :type settings: dict
     :param pack_settings: The validated pack-specific settings
     :type settings: dict
     """
-    render_template(context,
-                    env,
-                    'packs/mariadb/setup.sh',
-                    os.path.join('ou-builder-build', 'mariadb', 'mariadb-setup.sh'),
-                    pack_settings)
+    render_template(
+        context,
+        env,
+        "packs/mariadb/setup.sh",
+        os.path.join("ou-builder-build", "mariadb", "mariadb-setup.sh"),
+        pack_settings,
+    )
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/packs/nbclassic.py` & `ou_container_builder-2.6.0/ou_container_builder/packs/jupyterlab.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,67 @@
-"""Pack to install the Nbclassic notebook interface."""
+"""Pack to install the Jupyterlab interface."""
 from jinja2 import Environment
+from pydantic import BaseModel
+from typing import Literal
 from warnings import warn
 
-from ..utils import merge_settings
+from ou_container_builder.utils import merge_settings
+
+
+class Options(BaseModel):
+    version: Literal[3] | Literal[4] = 3
+
+
+class Pack(BaseModel):
+    name: Literal["jupyterlab"]
+    options: Options = Options()
 
 
 def process_settings(settings: dict, pack_settings: dict) -> dict:
     """
     Process the user-provided settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :param pack_settings: The pack-specific settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    warn('Automatically setting Nbclassic as the default is deprecated in 2.2.0 and will be removed in 3.0.0. Instead set server.default_path explicitly.', FutureWarning)  # noqa: E501
-    settings = merge_settings(settings, {
-        'packages': {
-            'pip': ['nbclassic>=0.4.8,<1.0.0']
-        },
-        'server': {
-            'default_path': '/tree'
+    warn(
+        "Automatically setting JupyterLab as the default is deprecated in 2.2.0 and will be removed in 3.0.0. Instead set server.default_path explicitly.",
+        FutureWarning,
+    )
+    if pack_settings["version"] == 3:
+        settings = merge_settings(
+            settings,
+            {
+                "packages": {"pip": ["jupyterlab>=3.4.3,<4.0.0"]},
+            },
+        )
+    elif pack_settings["version"] == 4:
+        settings = merge_settings(
+            settings,
+            {
+                "packages": {"pip": ["jupyterlab>=4.0.2,<5.0.0"]},
+            },
+        )
+    settings = merge_settings(
+        settings,
+        {
+            "server": {"default_path": "/lab"},
         },
-        'scripts': {
-            'build': [
-                {
-                    'commands': [
-                        'pip uninstall -y notebook',
-                        'jupyter server extension enable --system nbclassic'
-                    ]
-                }
-            ]
-        }
-    })
+    )
     return settings
 
 
-def generate_files(context: str, env: Environment, settings: dict, pack_settings: dict) -> dict:
-    """Generate the build files for the nbclassic pack.
+def generate_files(context: str, env: Environment, settings: dict, pack_settings: dict) -> None:
+    """Generate the build files for the jupyterlab pack.
 
-    This ensures that the the nbclassic package is installed
+    This ensures that the the jupyterlab package is installed
 
     :param context: The context path within which the generation is running
     :type context: str
     :param env: The Jinja2 environment to use for loading and rendering templates
     :type env: :class:`~jinja2.environment.Environment`
     :param settings: The validated settings
     :type settings: dict
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/packs/tutorial_server.py` & `ou_container_builder-2.6.0/ou_container_builder/packs/tutorial_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 """Pack to install the tutorial_sever."""
 import os
+from warnings import warn
 
 from jinja2 import Environment
-from warnings import warn
+from pydantic import BaseModel
+from typing import Literal
+
+from ou_container_builder.utils import merge_settings, render_template
 
-from ..utils import merge_settings, render_template
+
+class Pack(BaseModel):
+    name: Literal["tutorial_server"]
+    options: dict = {}
 
 
 def process_settings(settings: dict, pack_settings: dict) -> dict:
     """
     Process the user-provided settings.
 
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :param pack_settings: The pack-specific settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
-    warn('Automatically setting tutorial_server as the default is deprecated in 2.2.0 and will be removed in 3.0.0. Instead set server.default_path explicitly.', FutureWarning)  # noqa: E501
+    warn(
+        "Automatically setting tutorial_server as the default is deprecated in 2.2.0 and will be removed in 3.0.0. Instead set server.default_path explicitly.",
+        FutureWarning,
+    )
     additional_settings = {
-        'packages': {
-            'pip': [
-                'tutorial-server>=1.0.2,<2.0.0',
+        "packages": {
+            "pip": [
+                "tutorial-server>=1.0.2,<2.0.0",
             ]
         },
-        'content': [
+        "content": [
             {
-                'source': 'ou-builder-build/tutorial-server/production.ini',
-                'target': '/etc/tutorial-server/production.ini',
-                'overwrite': 'always'
+                "source": "ou-builder-build/tutorial-server/production.ini",
+                "target": "/etc/tutorial-server/production.ini",
+                "overwrite": "always",
             }
         ],
-        'web_apps': [
+        "web_apps": [
             {
-                'path': '/tutorial-server',
-                'command': [
-                    'python',
-                    '-m',
-                    'tutorial_server',
-                    '--config=/etc/tutorial-server/production.ini',
-                    '--port={port}',
-                    '--basepath={base_url}tutorial-server/'
+                "path": "/tutorial-server",
+                "command": [
+                    "python",
+                    "-m",
+                    "tutorial_server",
+                    "--config=/etc/tutorial-server/production.ini",
+                    "--port={port}",
+                    "--basepath={base_url}tutorial-server/",
                 ],
-                'absolute_url': True,
-                'default': True
+                "absolute_url": True,
+                "default": True,
             }
-        ]
+        ],
     }
-    if 'php-cgi' in pack_settings and pack_settings['php-cgi']:
-        additional_settings['packages']['apt'] = ['php-cgi']
+    if "php-cgi" in pack_settings and pack_settings["php-cgi"]:
+        additional_settings["packages"]["apt"] = ["php-cgi"]
     settings = merge_settings(settings, additional_settings)
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict, pack_settings: dict) -> dict:
     """Generate the build files for the tutorial-server pack.
 
@@ -64,12 +74,14 @@
     :param env: The Jinja2 environment to use for loading and rendering templates
     :type env: :class:`~jinja2.environment.Environment`
     :param settings: The validated settings
     :type settings: dict
     :param pack_settings: The validated pack-specific settings
     :type settings: dict
     """
-    render_template(context,
-                    env,
-                    'packs/tutorial-server/production.ini',
-                    os.path.join('ou-builder-build', 'tutorial-server', 'production.ini'),
-                    dict(**settings, **pack_settings))
+    render_template(
+        context,
+        env,
+        "packs/tutorial-server/production.ini",
+        os.path.join("ou-builder-build", "tutorial-server", "production.ini"),
+        dict(**settings, **pack_settings),
+    )
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/templates/Dockerfile.jinja2` & `ou_container_builder-2.6.0/ou_container_builder/templates/Dockerfile.jinja2`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 ENV USER="{{ image.user }}"
 ENV UID="1000"
 ENV GID="100"
 ENV MODULE_CODE="{{ module.code }}"
 ENV MODULE_PRESENTATION="{{ module.presentation }}"
 ENV HOME="/home/$USER/$MODULE_CODE-$MODULE_PRESENTATION"
 ENV SHELL="/bin/bash"
+ENV CARGO_HOME="/opt/cargo"
+ENV PATH="$PATH:/opt/cargo/bin"
 {% if environment %}
   {% for env in environment %}
 ENV {{ env.name }}="{{ env.value }}"
   {% endfor %}
 {% endif %}
 {% endblock %}
 
@@ -28,14 +30,16 @@
     useradd -u $UID -g $GID -d $HOME -m -s /bin/bash $USER
 {% endblock %}
 
 RUN DEBIAN_FRONTEND=noninteractive apt-get update -y && \
     DEBIAN_FRONTEND=noninteractive apt-get dist-upgrade -y && \
     DEBIAN_FRONTEND=noninteractive apt-get install -y tini{% if sources and sources.apt %} curl gnupg{% endif %}
 
+RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
+
 {% block hacks %}
   {% if hacks %}
     {% if 'missing-man1' in hacks %}
 RUN mkdir -p /usr/share/man/man1
     {% endif %}
   {% endif %}
 {% endblock %}
@@ -60,15 +64,15 @@
   {% if packages and packages.apt %}
 RUN DEBIAN_FRONTEND=noninteractive apt-get install -y {{ ' '.join(packages.apt) }}
   {% endif %}
 {% endblock %}
 
 {% block pip %}
   {% if packages and packages.pip %}
-RUN if [ "$TARGETPLATFORM" = "linux/arm/v7" ]; then pip install --no-cache-dir --extra-index-url=https://www.piwheels.org/simple {% for package in packages.pip %}"{{ package }}" {% endfor %}; else pip install --no-cache-dir {% for package in packages.pip %}"{{ package }}" {% endfor %}; fi
+RUN pip install --no-cache-dir --extra-index-url=https://www.piwheels.org/simple {% for package in packages.pip %}"{{ package }}" {% endfor %}
   {% endif %}
 {% endblock %}
 
 {% block content%}
   {% if flags and flags.ou_container_content %}
 RUN mkdir -p /etc/module-content/data
 COPY ou-builder-build/content/content_config.yaml /etc/module-content/config.yaml
```

### Comparing `ou_container_builder-2.5.0/ou_container_builder/templates/core/content/content_config.yaml` & `ou_container_builder-2.6.0/ou_container_builder/templates/core/content/content_config.yaml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.5.0/ou_container_builder/templates/packs/code_server/vscode.svg` & `ou_container_builder-2.6.0/ou_container_builder/templates/packs/code_server/vscode.svg`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.5.0/ou_container_builder/templates/packs/mariadb/setup.sh` & `ou_container_builder-2.6.0/ou_container_builder/templates/packs/mariadb/setup.sh`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.5.0/ou_container_builder/templates/packs/tutorial-server/production.ini` & `ou_container_builder-2.6.0/ou_container_builder/templates/packs/tutorial-server/production.ini`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.5.0/ou_container_builder/utils.py` & `ou_container_builder-2.6.0/ou_container_builder/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Utility functions."""
 import os
-
 from copy import deepcopy
+
 from jinja2 import Environment
 
 
 def merge_settings(base: dict, new: dict) -> dict:
     """Return a new dictionary created by merging the settings from ``new`` into ``base``.
 
     :param base: The base dictionary to merge into
@@ -46,13 +46,13 @@
     :type output_path: str
     :param variables: The variables to pass to the template
     :type variables: dict
     """
     target_path = os.path.join(context, output_path)
     if not os.path.exists(os.path.dirname(target_path)):
         os.makedirs(os.path.dirname(target_path), exist_ok=True)
-    with open(target_path, 'w') as out_f:
+    with open(target_path, "w") as out_f:
         tmpl = env.get_template(template_path)
         rendered = tmpl.render(**variables)
-        if not rendered.endswith('\n'):
-            rendered = f'{rendered}\n'
+        if not rendered.endswith("\n"):
+            rendered = f"{rendered}\n"
         out_f.write(rendered)
```

