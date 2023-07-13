# Comparing `tmp/ansible_taskrunner-2.8.3.tar.gz` & `tmp/ansible_taskrunner-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_taskrunner-2.8.3.tar", last modified: Thu Jun 15 18:25:00 2023, max compression
+gzip compressed data, was "ansible_taskrunner-2.8.4.tar", last modified: Thu Jul 13 16:50:42 2023, max compression
```

## Comparing `ansible_taskrunner-2.8.3.tar` & `ansible_taskrunner-2.8.4.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.306056 ansible_taskrunner-2.8.3/
--rw-r--r--   0 etejeda    (501) staff       (20)      313 2022-09-14 03:08:59.000000 ansible_taskrunner-2.8.3/.editorconfig
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.270128 ansible_taskrunner-2.8.3/.github/
--rw-r--r--   0 etejeda    (501) staff       (20)      344 2022-09-14 03:08:56.000000 ansible_taskrunner-2.8.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1558 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)      314 2022-09-14 03:05:03.000000 ansible_taskrunner-2.8.3/.travis.yml
--rw-r--r--   0 etejeda    (501) staff       (20)      175 2022-09-14 03:04:51.000000 ansible_taskrunner-2.8.3/AUTHORS.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     3790 2022-09-14 03:04:49.000000 ansible_taskrunner-2.8.3/CONTRIBUTING.rst
--rw-r--r--   0 etejeda    (501) staff       (20)    26436 2023-03-24 15:57:41.000000 ansible_taskrunner-2.8.3/HISTORY.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1097 2022-09-14 03:04:47.000000 ansible_taskrunner-2.8.3/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)      365 2022-09-14 03:18:38.000000 ansible_taskrunner-2.8.3/MANIFEST.in
--rw-r--r--   0 etejeda    (501) staff       (20)    11310 2023-05-14 18:24:49.000000 ansible_taskrunner-2.8.3/Makefile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)    57555 2023-06-15 18:25:00.306414 ansible_taskrunner-2.8.3/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)    58542 2023-06-15 17:31:39.000000 ansible_taskrunner-2.8.3/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     5182 2023-03-08 21:35:43.000000 ansible_taskrunner-2.8.3/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-06-15 18:24:53.000000 ansible_taskrunner-2.8.3/VERSION.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.273545 ansible_taskrunner-2.8.3/ansible_taskrunner/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2479 2023-03-07 16:10:01.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/cli.py
--rw-r--r--   0 etejeda    (501) staff       (20)      953 2023-06-09 16:20:10.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/config.py
--rw-r--r--   0 etejeda    (501) staff       (20)      922 2023-06-15 18:13:33.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/defaults.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.278517 ansible_taskrunner-2.8.3/ansible_taskrunner/files/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.279522 ansible_taskrunner-2.8.3/ansible_taskrunner/files/cfg/
--rw-r--r--   0 etejeda    (501) staff       (20)      159 2023-01-10 10:27:20.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/files/cfg/default.ini
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.280435 ansible_taskrunner-2.8.3/ansible_taskrunner/files/macros/
--rw-r--r--   0 etejeda    (501) staff       (20)     1116 2023-01-10 10:27:25.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/files/macros/default.mac
--rw-r--r--   0 etejeda    (501) staff       (20)      956 2023-01-10 10:27:29.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/files/start-tutorial.bat
--rw-r--r--   0 etejeda    (501) staff       (20)     1772 2023-01-10 10:27:30.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/files/tasks-console.bat
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.281118 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.281419 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/bastion_mode/
--rw-r--r--   0 etejeda    (501) staff       (20)     1354 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/bastion_mode/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.284340 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/
--rw-r--r--   0 etejeda    (501) staff       (20)     6176 2023-05-11 18:40:41.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2868 2023-03-07 15:21:06.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/click_commands_create_group.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2917 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/click_commands_create_init.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5286 2023-06-15 18:14:32.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/click_commands_create_sub.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5660 2023-03-24 15:45:23.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/click_commands_init_sub.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4667 2023-03-15 18:34:45.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/invocation.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.285295 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/click_extras/
--rw-r--r--   0 etejeda    (501) staff       (20)     9616 2023-05-22 20:24:50.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/click_extras/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2228 2023-03-24 15:54:02.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/click_extras/help.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2512 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/click_extras/options_advanced.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.285703 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/errorhandler/
--rw-r--r--   0 etejeda    (501) staff       (20)      738 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/errorhandler/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.286049 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/formatting/
--rw-r--r--   0 etejeda    (501) staff       (20)      787 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/formatting/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.286391 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/help/
--rw-r--r--   0 etejeda    (501) staff       (20)     2738 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/help/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.287534 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/language/
--rw-r--r--   0 etejeda    (501) staff       (20)      876 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/language/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)       19 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/language/en.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.288157 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/logger/
--rw-r--r--   0 etejeda    (501) staff       (20)      462 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/logger/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.288717 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/proc_mgmt/
--rw-r--r--   0 etejeda    (501) staff       (20)     3334 2023-04-28 19:10:32.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/proc_mgmt/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.290052 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/providers/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/providers/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)    15894 2023-03-13 18:12:26.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/providers/ansible.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2481 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/providers/bash.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2561 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/providers/vagrant.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.292460 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/sshutil/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/sshutil/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5474 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/sshutil/client.py
--rw-r--r--   0 etejeda    (501) staff       (20)    16240 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/sshutil/scp.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2949 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/libs/sshutil/sync.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-09 20:18:59.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/logger.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.292832 ansible_taskrunner-2.8.3/ansible_taskrunner/plugins/
--rw-r--r--   0 etejeda    (501) staff       (20)     1951 2023-01-10 10:29:26.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/plugins/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5089 2023-01-09 21:15:54.000000 ansible_taskrunner-2.8.3/ansible_taskrunner/setup.cx_freeze.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.277544 ansible_taskrunner-2.8.3/ansible_taskrunner.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)    57555 2023-06-15 18:25:00.000000 ansible_taskrunner-2.8.3/ansible_taskrunner.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     2948 2023-06-15 18:25:00.000000 ansible_taskrunner-2.8.3/ansible_taskrunner.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-15 18:25:00.000000 ansible_taskrunner-2.8.3/ansible_taskrunner.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       53 2023-06-15 18:25:00.000000 ansible_taskrunner-2.8.3/ansible_taskrunner.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-15 18:25:00.000000 ansible_taskrunner-2.8.3/ansible_taskrunner.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)      244 2023-06-15 18:25:00.000000 ansible_taskrunner-2.8.3/ansible_taskrunner.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       25 2023-06-15 18:25:00.000000 ansible_taskrunner-2.8.3/ansible_taskrunner.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.297238 ansible_taskrunner-2.8.3/docs/
--rw-r--r--   0 etejeda    (501) staff       (20)      636 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/docs/Makefile
--rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.3/docs/authors.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     5127 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.3/docs/conf.py
--rw-r--r--   0 etejeda    (501) staff       (20)       34 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.3/docs/contributing.rst
--rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.3/docs/history.rst
--rw-r--r--   0 etejeda    (501) staff       (20)      335 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.3/docs/index.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     1261 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.3/docs/installation.rst
--rw-r--r--   0 etejeda    (501) staff       (20)      816 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.3/docs/make.bat
--rw-r--r--   0 etejeda    (501) staff       (20)       28 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.3/docs/readme.rst
--rw-r--r--   0 etejeda    (501) staff       (20)       98 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.3/docs/usage.rst
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.262257 ansible_taskrunner-2.8.3/examples/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.298423 ansible_taskrunner-2.8.3/examples/ansible/
--rw-r--r--   0 etejeda    (501) staff       (20)     5071 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/examples/ansible/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1967 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/examples/ansible/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.3/examples/ansible/config.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.299596 ansible_taskrunner-2.8.3/examples/bash/
--rw-r--r--   0 etejeda    (501) staff       (20)     2933 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/examples/bash/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/examples/bash/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)       44 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.3/examples/bash/config.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.300109 ansible_taskrunner-2.8.3/examples/choice/
--rw-r--r--   0 etejeda    (501) staff       (20)     2300 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/examples/choice/Taskfile.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.301782 ansible_taskrunner-2.8.3/examples/custom-cli-provider/
--rw-r--r--   0 etejeda    (501) staff       (20)     3046 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.3/examples/custom-cli-provider/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/examples/custom-cli-provider/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.3/examples/custom-cli-provider/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      177 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.3/examples/custom-cli-provider/dynamic-import.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.261679 ansible_taskrunner-2.8.3/examples/custom-cli-provider/plugins/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.261785 ansible_taskrunner-2.8.3/examples/custom-cli-provider/plugins/providers/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.302238 ansible_taskrunner-2.8.3/examples/custom-cli-provider/plugins/providers/example/
--rw-r--r--   0 etejeda    (501) staff       (20)     2187 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.3/examples/custom-cli-provider/plugins/providers/example/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.302694 ansible_taskrunner-2.8.3/examples/mutually-exclusive/
--rw-r--r--   0 etejeda    (501) staff       (20)     2354 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/examples/mutually-exclusive/Taskfile.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.303048 ansible_taskrunner-2.8.3/examples/prompt/
--rw-r--r--   0 etejeda    (501) staff       (20)     2275 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/examples/prompt/Taskfile.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.304617 ansible_taskrunner-2.8.3/examples/vagrant/
--rw-r--r--   0 etejeda    (501) staff       (20)     4168 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/examples/vagrant/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1506 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.3/examples/vagrant/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)     3092 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.3/examples/vagrant/Vagrantfile
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.3/examples/vagrant/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-03-07 16:28:11.000000 ansible_taskrunner-2.8.3/requirements_dev.txt
--rw-r--r--   0 etejeda    (501) staff       (20)     1591 2023-06-15 18:25:00.307309 ansible_taskrunner-2.8.3/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)       39 2022-09-14 03:03:38.000000 ansible_taskrunner-2.8.3/setup.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-15 18:25:00.305360 ansible_taskrunner-2.8.3/tests/
--rw-r--r--   0 etejeda    (501) staff       (20)       76 2022-09-14 03:04:16.000000 ansible_taskrunner-2.8.3/tests/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2433 2023-03-13 18:35:06.000000 ansible_taskrunner-2.8.3/tests/test_ansible_taskrunner.py
--rw-r--r--   0 etejeda    (501) staff       (20)      343 2022-09-14 03:17:41.000000 ansible_taskrunner-2.8.3/tox.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.064289 ansible_taskrunner-2.8.4/
+-rw-r--r--   0 etejeda    (501) staff       (20)      313 2022-09-14 03:08:59.000000 ansible_taskrunner-2.8.4/.editorconfig
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.032997 ansible_taskrunner-2.8.4/.github/
+-rw-r--r--   0 etejeda    (501) staff       (20)      344 2022-09-14 03:08:56.000000 ansible_taskrunner-2.8.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1558 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)      314 2022-09-14 03:05:03.000000 ansible_taskrunner-2.8.4/.travis.yml
+-rw-r--r--   0 etejeda    (501) staff       (20)      175 2022-09-14 03:04:51.000000 ansible_taskrunner-2.8.4/AUTHORS.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     3790 2022-09-14 03:04:49.000000 ansible_taskrunner-2.8.4/CONTRIBUTING.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)    26436 2023-03-24 15:57:41.000000 ansible_taskrunner-2.8.4/HISTORY.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1097 2022-09-14 03:04:47.000000 ansible_taskrunner-2.8.4/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)      365 2022-09-14 03:18:38.000000 ansible_taskrunner-2.8.4/MANIFEST.in
+-rw-r--r--   0 etejeda    (501) staff       (20)    11310 2023-05-14 18:24:49.000000 ansible_taskrunner-2.8.4/Makefile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)    59236 2023-07-13 16:50:42.064590 ansible_taskrunner-2.8.4/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)    60289 2023-07-13 16:11:59.000000 ansible_taskrunner-2.8.4/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     5182 2023-03-08 21:35:43.000000 ansible_taskrunner-2.8.4/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-07-13 15:23:20.000000 ansible_taskrunner-2.8.4/VERSION.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.035648 ansible_taskrunner-2.8.4/ansible_taskrunner/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2479 2023-03-07 16:10:01.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/cli.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      953 2023-06-09 16:20:10.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/config.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      922 2023-06-15 18:13:33.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/defaults.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.038842 ansible_taskrunner-2.8.4/ansible_taskrunner/files/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.039311 ansible_taskrunner-2.8.4/ansible_taskrunner/files/cfg/
+-rw-r--r--   0 etejeda    (501) staff       (20)      159 2023-01-10 10:27:20.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/files/cfg/default.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.039828 ansible_taskrunner-2.8.4/ansible_taskrunner/files/macros/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1116 2023-01-10 10:27:25.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/files/macros/default.mac
+-rw-r--r--   0 etejeda    (501) staff       (20)      956 2023-01-10 10:27:29.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/files/start-tutorial.bat
+-rw-r--r--   0 etejeda    (501) staff       (20)     1772 2023-01-10 10:27:30.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/files/tasks-console.bat
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.040273 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.040460 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/bastion_mode/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1354 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/bastion_mode/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.043693 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/
+-rw-r--r--   0 etejeda    (501) staff       (20)     6176 2023-05-11 18:40:41.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2868 2023-03-07 15:21:06.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/click_commands_create_group.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2917 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/click_commands_create_init.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5286 2023-06-15 18:14:32.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/click_commands_create_sub.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5660 2023-03-24 15:45:23.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/click_commands_init_sub.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4667 2023-03-15 18:34:45.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/invocation.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.045341 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/click_extras/
+-rw-r--r--   0 etejeda    (501) staff       (20)    10881 2023-06-15 19:40:30.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/click_extras/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2228 2023-03-24 15:54:02.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/click_extras/help.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2512 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/click_extras/options_advanced.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.045915 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/errorhandler/
+-rw-r--r--   0 etejeda    (501) staff       (20)      738 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/errorhandler/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.046423 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/formatting/
+-rw-r--r--   0 etejeda    (501) staff       (20)      787 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/formatting/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.046843 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/help/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2738 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/help/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.047766 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/language/
+-rw-r--r--   0 etejeda    (501) staff       (20)      876 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/language/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)       19 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/language/en.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.048215 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/logger/
+-rw-r--r--   0 etejeda    (501) staff       (20)      462 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/logger/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.048719 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/proc_mgmt/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3334 2023-04-28 19:10:32.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/proc_mgmt/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.050714 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/providers/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/providers/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    16535 2023-07-13 16:42:47.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/providers/ansible.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2481 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/providers/bash.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2561 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/providers/vagrant.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.052126 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/sshutil/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/sshutil/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5474 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/sshutil/client.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    16240 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/sshutil/scp.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2949 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/libs/sshutil/sync.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-09 20:18:59.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/logger.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.052517 ansible_taskrunner-2.8.4/ansible_taskrunner/plugins/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1951 2023-01-10 10:29:26.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/plugins/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5089 2023-01-09 21:15:54.000000 ansible_taskrunner-2.8.4/ansible_taskrunner/setup.cx_freeze.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.038063 ansible_taskrunner-2.8.4/ansible_taskrunner.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)    59236 2023-07-13 16:50:41.000000 ansible_taskrunner-2.8.4/ansible_taskrunner.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     2948 2023-07-13 16:50:41.000000 ansible_taskrunner-2.8.4/ansible_taskrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-07-13 16:50:41.000000 ansible_taskrunner-2.8.4/ansible_taskrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       53 2023-07-13 16:50:41.000000 ansible_taskrunner-2.8.4/ansible_taskrunner.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-07-13 16:50:41.000000 ansible_taskrunner-2.8.4/ansible_taskrunner.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)      244 2023-07-13 16:50:41.000000 ansible_taskrunner-2.8.4/ansible_taskrunner.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       25 2023-07-13 16:50:41.000000 ansible_taskrunner-2.8.4/ansible_taskrunner.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.056353 ansible_taskrunner-2.8.4/docs/
+-rw-r--r--   0 etejeda    (501) staff       (20)      636 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/docs/Makefile
+-rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.4/docs/authors.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     5127 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.4/docs/conf.py
+-rw-r--r--   0 etejeda    (501) staff       (20)       34 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.4/docs/contributing.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.4/docs/history.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)      335 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.4/docs/index.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     1261 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.4/docs/installation.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)      816 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.4/docs/make.bat
+-rw-r--r--   0 etejeda    (501) staff       (20)       28 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.4/docs/readme.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)       98 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.4/docs/usage.rst
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.024937 ansible_taskrunner-2.8.4/examples/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.057316 ansible_taskrunner-2.8.4/examples/ansible/
+-rw-r--r--   0 etejeda    (501) staff       (20)     5071 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/examples/ansible/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1967 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/examples/ansible/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.4/examples/ansible/config.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.058558 ansible_taskrunner-2.8.4/examples/bash/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2933 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/examples/bash/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/examples/bash/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)       44 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.4/examples/bash/config.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.058999 ansible_taskrunner-2.8.4/examples/choice/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2300 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/examples/choice/Taskfile.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.060409 ansible_taskrunner-2.8.4/examples/custom-cli-provider/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3046 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.4/examples/custom-cli-provider/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/examples/custom-cli-provider/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.4/examples/custom-cli-provider/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      177 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.4/examples/custom-cli-provider/dynamic-import.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.024217 ansible_taskrunner-2.8.4/examples/custom-cli-provider/plugins/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.024332 ansible_taskrunner-2.8.4/examples/custom-cli-provider/plugins/providers/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.060692 ansible_taskrunner-2.8.4/examples/custom-cli-provider/plugins/providers/example/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2187 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.4/examples/custom-cli-provider/plugins/providers/example/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.061013 ansible_taskrunner-2.8.4/examples/mutually-exclusive/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2354 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/examples/mutually-exclusive/Taskfile.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.061392 ansible_taskrunner-2.8.4/examples/prompt/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2275 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/examples/prompt/Taskfile.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.062783 ansible_taskrunner-2.8.4/examples/vagrant/
+-rw-r--r--   0 etejeda    (501) staff       (20)     4168 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/examples/vagrant/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1506 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.4/examples/vagrant/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)     3092 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.4/examples/vagrant/Vagrantfile
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.4/examples/vagrant/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-03-07 16:28:11.000000 ansible_taskrunner-2.8.4/requirements_dev.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)     1591 2023-07-13 16:50:42.065322 ansible_taskrunner-2.8.4/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)       39 2022-09-14 03:03:38.000000 ansible_taskrunner-2.8.4/setup.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 16:50:42.063546 ansible_taskrunner-2.8.4/tests/
+-rw-r--r--   0 etejeda    (501) staff       (20)       76 2022-09-14 03:04:16.000000 ansible_taskrunner-2.8.4/tests/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2433 2023-03-13 18:35:06.000000 ansible_taskrunner-2.8.4/tests/test_ansible_taskrunner.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      343 2022-09-14 03:17:41.000000 ansible_taskrunner-2.8.4/tox.ini
```

### Comparing `ansible_taskrunner-2.8.3/.gitignore` & `ansible_taskrunner-2.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/CONTRIBUTING.rst` & `ansible_taskrunner-2.8.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/HISTORY.md` & `ansible_taskrunner-2.8.4/HISTORY.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/LICENSE` & `ansible_taskrunner-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/Makefile.yaml` & `ansible_taskrunner-2.8.4/Makefile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/PKG-INFO` & `ansible_taskrunner-2.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible_taskrunner
-Version: 2.8.3
+Version: 2.8.4
 Summary: Ansible Task Runner
 Home-page: https://github.com/berttejeda/ansible-taskrunner.git
 Author: Engelbert Tejeda
 Author-email: etejeda@tecknicos.com
 Keywords: ansible,playbook,wrapper,bash,python,click,task-runner,subprocess,yaml,cli,options
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -1771,25 +1771,64 @@
 -e "{'var1':'${var1}'}" \
 -e "{'var2':'${var2}'}" \
 -e "{'var3':'${var3}'}" \
 ... Taskfile.yaml
 ```
 
 [Back To Top](#top)
+<a name="pre_execution"></a>
+
+### pre_execution
+
+Anything defined under the *pre_execution* variable will be evaluated
+**before** all other statements in the underlying shell expression.
+
+As an example, suppose I define the pre_execution variable in the above *Taskfile.yaml*, as follows:
+
+```
+- hosts: myhosts
+  gather_facts: true
+  become: true
+  vars:
+    pre_execution: |-
+      export pxe_var=some_value
+      touch /tmp/.run.lock
+```
+
+Upon invoking the `tasks` command with the `---echo` flag:
+
+- The underlying shell expression would be revealed as:<br />
+
+```
+...
+export pxe_var=some_value
+touch /tmp/.run.lock
+...
+```
+
+The commands above are always placed **before**<br />
+all variables declarations in the underlying shell expresison.
+
+<a name="post_execution"></a>
+
+### post_execution
+
+This is similar to *pre_execution*, except that anything defined under the *post_execution* variable will be evaluated
+**after** all other statements in the underlying shell expression.
+
 <a name="environment_vars"></a>
 
 ### environment_vars
 
 By defining the playbook dictionary variable *environment_vars*,<br />
 the following occurs:
 
 - For each dictionary `key: value` pair:
     - A corresponding `export` statement is defined in the underlying shell expression
 
-
 As an example, suppose I define this variable in the above *Taskfile.yaml*, as follows:
 
 ```
 - hosts: myhosts
   gather_facts: true
   become: true
   vars:
@@ -1814,14 +1853,41 @@
 export MY_ENV_VAR1="${some_path}/${var1}"
 export MY_ENV_VAR2="${some_path}/${var2}"
 ```
 
 These export statements are always placed **after**<br />
 all variables declarations in the underlying shell expresison.
 
+#### ANSIBLE_ Variables
+
+Any variables matching ANSIBLE_.* will automatically be expressed as export statements.
+
+As an example, suppose I define such variables in the above *Taskfile.yaml*, as follows:
+
+```
+- hosts: myhosts
+  gather_facts: true
+  become: true
+  vars:
+    ANSIBLE_VAULT_PASSWORD_FILE: /some/path/some/password_file
+    ANSIBLE_CALLBACK_PLUGINS: /some/other/path/some/plugins
+    # ...
+```
+
+Upon invoking the `tasks` command with the `---echo` flag:
+
+- The underlying shell expression would be revealed as:<br />
+
+```
+var1="value1"
+var2="value2"
+export ANSIBLE_VAULT_PASSWORD_FILE="/some/path/some/password_file"
+export ANSIBLE_CALLBACK_PLUGINS="/some/other/path/some/plugins"
+```
+
 <a name="cli_provider"></a>
 
 ### cli_provider
 
 You can override the underlying command-line provider in two ways:
 
 - Via the tasks config file (see [examples](#examples))
```

### Comparing `ansible_taskrunner-2.8.3/README.md` & `ansible_taskrunner-2.8.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1747,25 +1747,64 @@
 -e "{'var1':'${var1}'}" \
 -e "{'var2':'${var2}'}" \
 -e "{'var3':'${var3}'}" \
 ... Taskfile.yaml
 ```
 
 [Back To Top](#top)
+<a name="pre_execution"></a>
+
+### pre_execution
+
+Anything defined under the *pre_execution* variable will be evaluated
+**before** all other statements in the underlying shell expression.
+
+As an example, suppose I define the pre_execution variable in the above *Taskfile.yaml*, as follows:
+
+```
+- hosts: myhosts
+  gather_facts: true
+  become: true
+  vars:
+    pre_execution: |-
+      export pxe_var=some_value
+      touch /tmp/.run.lock
+```
+
+Upon invoking the `tasks` command with the `---echo` flag:
+
+- The underlying shell expression would be revealed as:<br />
+
+```
+...
+export pxe_var=some_value
+touch /tmp/.run.lock
+...
+```
+
+The commands above are always placed **before**<br />
+all variables declarations in the underlying shell expresison.
+
+<a name="post_execution"></a>
+
+### post_execution
+
+This is similar to *pre_execution*, except that anything defined under the *post_execution* variable will be evaluated
+**after** all other statements in the underlying shell expression.
+
 <a name="environment_vars"></a>
 
 ### environment_vars
 
 By defining the playbook dictionary variable *environment_vars*,<br />
 the following occurs:
 
 - For each dictionary `key: value` pair:
     - A corresponding `export` statement is defined in the underlying shell expression
 
-
 As an example, suppose I define this variable in the above *Taskfile.yaml*, as follows:
 
 ```
 - hosts: myhosts
   gather_facts: true
   become: true
   vars:
@@ -1790,14 +1829,41 @@
 export MY_ENV_VAR1="${some_path}/${var1}"
 export MY_ENV_VAR2="${some_path}/${var2}"
 ```
 
 These export statements are always placed **after**<br />
 all variables declarations in the underlying shell expresison.
 
+#### ANSIBLE_ Variables
+
+Any variables matching ANSIBLE_.* will automatically be expressed as export statements.
+
+As an example, suppose I define such variables in the above *Taskfile.yaml*, as follows:
+
+```
+- hosts: myhosts
+  gather_facts: true
+  become: true
+  vars:
+    ANSIBLE_VAULT_PASSWORD_FILE: /some/path/some/password_file
+    ANSIBLE_CALLBACK_PLUGINS: /some/other/path/some/plugins
+    # ...
+```
+
+Upon invoking the `tasks` command with the `---echo` flag:
+
+- The underlying shell expression would be revealed as:<br />
+
+```
+var1="value1"
+var2="value2"
+export ANSIBLE_VAULT_PASSWORD_FILE="/some/path/some/password_file"
+export ANSIBLE_CALLBACK_PLUGINS="/some/other/path/some/plugins"
+```
+
 <a name="cli_provider"></a>
 
 ### cli_provider
 
 You can override the underlying command-line provider in two ways:
 
 - Via the tasks config file (see [examples](#examples))
```

### Comparing `ansible_taskrunner-2.8.3/Taskfile.yaml` & `ansible_taskrunner-2.8.4/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/cli.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/config.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/config.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/defaults.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/defaults.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/files/macros/default.mac` & `ansible_taskrunner-2.8.4/ansible_taskrunner/files/macros/default.mac`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/files/start-tutorial.bat` & `ansible_taskrunner-2.8.4/ansible_taskrunner/files/start-tutorial.bat`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/files/tasks-console.bat` & `ansible_taskrunner-2.8.4/ansible_taskrunner/files/tasks-console.bat`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/bastion_mode/__init__.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/bastion_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/__init__.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/click_commands_create_group.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/click_commands_create_group.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/click_commands_create_init.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/click_commands_create_init.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/click_commands_create_sub.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/click_commands_create_sub.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/click_commands_init_sub.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/click_commands_init_sub.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/cli/invocation.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/cli/invocation.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/click_extras/__init__.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/click_extras/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,19 @@
             option_is_flag = bool(option.get('is_flag', False))
             option_is_hidden = bool(option.get('is_hidden', False))
             option_show_choices = bool(option.get('show_choices', True))
             option_show_envvar = bool(option.get('env_var_show', True))
             option_supports_counting = bool(option.get('allow_counting', False))
             option_supports_multiple = bool(option.get('allow_multiple', False))
             option_value_from_env = option.get('env_var', None)
-            option_default_value = option.get('default', None)
+            if not option_is_flag:
+                option_default_value = option.get('default', None)
+            else:
+                option_default_value = None
+
             mutually_exclusive_with = option.get('mutually_exclusive_with', '')
             required_if = option.get('required_if', '')
             not_required_if = option.get('not_required_if', '')
 
             if mutually_exclusive_with and option_required:
                 logger.warning(f"Not honoring mutual exclusivity of option '{option_name}' " + \
                                f"and options with variables {mutually_exclusive_with}, as 'required' must be False")
@@ -176,32 +180,56 @@
                     f' NOTE: This argument is optional when related options are specified: [{ex_str}]'
                 else:
                     option_help_effective = ''
             else:
                 option_class = self.default_option_class
                 special_options = {}
 
-            option = click.option(
-                *param_declarations,
-                option_variable,
-                cls=option_class,
-                confirmation_prompt=option_confirm_prompt,
-                count=option_supports_counting,
-                envvar=option_value_from_env,
-                nargs=option_nargs,
-                default=option_default_value,
-                help=option_help_effective,
-                hide_input=option_secure,
-                hidden=option_is_hidden,
-                is_flag=option_is_flag,
-                prompt=option_prompt,
-                prompt_required=option_prompt_required,
-                multiple=option_supports_multiple,
-                required=option_required,
-                show_choices=option_show_choices,
-                show_envvar=option_show_envvar,
-                show_default=option_show_default,
-                type=self.get_option_type(option),
-                **special_options,
-            )
+            if not option_is_flag:
+                option = click.option(
+                    *param_declarations,
+                    option_variable,
+                    cls=option_class,
+                    confirmation_prompt=option_confirm_prompt,
+                    count=option_supports_counting,
+                    default=option_default_value,
+                    envvar=option_value_from_env,
+                    nargs=option_nargs,
+                    help=option_help_effective,
+                    hide_input=option_secure,
+                    hidden=option_is_hidden,
+                    is_flag=option_is_flag,
+                    prompt=option_prompt,
+                    prompt_required=option_prompt_required,
+                    multiple=option_supports_multiple,
+                    required=option_required,
+                    show_choices=option_show_choices,
+                    show_envvar=option_show_envvar,
+                    show_default=option_show_default,
+                    type=self.get_option_type(option),
+                    **special_options,
+                )
+            else:
+                option = click.option(
+                    *param_declarations,
+                    option_variable,
+                    cls=option_class,
+                    confirmation_prompt=option_confirm_prompt,
+                    count=option_supports_counting,
+                    envvar=option_value_from_env,
+                    nargs=option_nargs,
+                    help=option_help_effective,
+                    hide_input=option_secure,
+                    hidden=option_is_hidden,
+                    is_flag=option_is_flag,
+                    prompt=option_prompt,
+                    prompt_required=option_prompt_required,
+                    multiple=option_supports_multiple,
+                    required=option_required,
+                    show_choices=option_show_choices,
+                    show_envvar=option_show_envvar,
+                    show_default=option_show_default,
+                    type=self.get_option_type(option),
+                    **special_options,
+                )
             func = option(func)
         return func
```

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/click_extras/help.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/click_extras/help.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/click_extras/options_advanced.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/click_extras/options_advanced.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/errorhandler/__init__.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/errorhandler/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/formatting/__init__.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/help/__init__.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/help/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/language/__init__.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/language/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/proc_mgmt/__init__.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/proc_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/providers/ansible.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/providers/ansible.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         """Invoke commands according to provider"""
 
         args = kwargs.get('args')
         available_vars = kwargs.get('available_vars', {})
         bastion_settings = kwargs.get('bastion_settings', {})
         cli_functions = kwargs.get('cli_functions')
         extra_vars = kwargs.get('extra_vars', '')
-        shell_functions = kwargs.get('shell_functions', [])
+        shell_functions = '# Embedded Shell Functions' + '\n' + kwargs.get('shell_functions', '')
         debug = kwargs.get('debug', False)
         provider_vars = kwargs.get('provider_vars', {})
         provider_vars_string_block = kwargs.get('provider_vars_string_block', '')
         invocation = kwargs.get('invocation', {})
         prefix = kwargs.get('prefix', '')
         raw_args = kwargs.get('raw_args', '')
         suppress_output = kwargs.get('suppress_output')
@@ -272,28 +272,42 @@
                 f'{trap}\n' + \
                 f'if [[ "$inventory_is_ephemeral" == "True" ]];then\n' + \
                 f'echo -e """${{inventory_expression}}"""' + \
                 f'| while read line;do\n eval "echo -e ${{line}}" >> "{effective_inventory_file_path}";\ndone\n' + \
                 'fi;\n'
         else:
             inventory_command = ''
-        anc = ansi_colors.strip()
-        psb = re.sub(r'(ANSIBLE_)(.*?)=', 'export \\1\\2=', provider_vars_string_block)
-        inc = inventory_command
-        pre_commands = f'{anc}\n{psb}\n{shell_functions}\n{inc}'
+        anc = '# ANSI Colors' + '\n' + ansi_colors.strip()
+        _pexe = available_vars.get('pre_execution', '')
+        if _pexe:
+            pexe = '# Pre-Execution' + '\n' + _pexe
+        else:
+            pexe = _pexe
+        _poxe = available_vars.get('post_execution', '')
+        if _poxe:
+            poxe = '# Post-Execution' + '\n' + _poxe
+        else:
+            poxe = _poxe
+        _psb = re.sub(r'(ANSIBLE_)(.*?)=', 'export \\1\\2=', provider_vars_string_block)
+        psb = '# Provider-Vars' + '\n' + _psb.replace('export export', 'export')
+        if inventory_command:
+            inc = '# Inventory Command' + '\n' + inventory_command
+        else:
+            inc = inventory_command
+        pre_commands = f'{anc}\n{pexe}\n{psb}\n{shell_functions}\n{inc}'
         apc = ansible_playbook_command
         inf = effective_inventory_file_path
         opt = ' \\\n'.join(ansible_extra_options)
         pb = yaml_input_file
         arg = args
         raw = raw_args
         ev = extra_vars
         ansible_command_strings = [apc, '${__ansible_run_flags__}', f'-i {inf}', opt, arg, ev, raw, pb]
-        ansible_command = ' '.join(s for s in ansible_command_strings if s)
-        command = f'{pre_commands} {ansible_command}'
+        ansible_command = '# Ansible Command(s)' + '\n' + ' '.join(s for s in ansible_command_strings if s)
+        command = f'{pre_commands} {ansible_command} \n{poxe}'
         # Command invocation
         result = None
         if prefix == 'echo':
             logger.debug("ECHO MODE ON")
             print(command)
         else:
             if bastion_settings.get('enabled'):
```

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/providers/bash.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/providers/bash.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/providers/vagrant.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/providers/vagrant.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/sshutil/client.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/sshutil/client.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/sshutil/scp.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/sshutil/scp.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/libs/sshutil/sync.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/libs/sshutil/sync.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/logger.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/logger.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/plugins/__init__.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner/setup.cx_freeze.py` & `ansible_taskrunner-2.8.4/ansible_taskrunner/setup.cx_freeze.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner.egg-info/PKG-INFO` & `ansible_taskrunner-2.8.4/ansible_taskrunner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-taskrunner
-Version: 2.8.3
+Version: 2.8.4
 Summary: Ansible Task Runner
 Home-page: https://github.com/berttejeda/ansible-taskrunner.git
 Author: Engelbert Tejeda
 Author-email: etejeda@tecknicos.com
 Keywords: ansible,playbook,wrapper,bash,python,click,task-runner,subprocess,yaml,cli,options
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -1771,25 +1771,64 @@
 -e "{'var1':'${var1}'}" \
 -e "{'var2':'${var2}'}" \
 -e "{'var3':'${var3}'}" \
 ... Taskfile.yaml
 ```
 
 [Back To Top](#top)
+<a name="pre_execution"></a>
+
+### pre_execution
+
+Anything defined under the *pre_execution* variable will be evaluated
+**before** all other statements in the underlying shell expression.
+
+As an example, suppose I define the pre_execution variable in the above *Taskfile.yaml*, as follows:
+
+```
+- hosts: myhosts
+  gather_facts: true
+  become: true
+  vars:
+    pre_execution: |-
+      export pxe_var=some_value
+      touch /tmp/.run.lock
+```
+
+Upon invoking the `tasks` command with the `---echo` flag:
+
+- The underlying shell expression would be revealed as:<br />
+
+```
+...
+export pxe_var=some_value
+touch /tmp/.run.lock
+...
+```
+
+The commands above are always placed **before**<br />
+all variables declarations in the underlying shell expresison.
+
+<a name="post_execution"></a>
+
+### post_execution
+
+This is similar to *pre_execution*, except that anything defined under the *post_execution* variable will be evaluated
+**after** all other statements in the underlying shell expression.
+
 <a name="environment_vars"></a>
 
 ### environment_vars
 
 By defining the playbook dictionary variable *environment_vars*,<br />
 the following occurs:
 
 - For each dictionary `key: value` pair:
     - A corresponding `export` statement is defined in the underlying shell expression
 
-
 As an example, suppose I define this variable in the above *Taskfile.yaml*, as follows:
 
 ```
 - hosts: myhosts
   gather_facts: true
   become: true
   vars:
@@ -1814,14 +1853,41 @@
 export MY_ENV_VAR1="${some_path}/${var1}"
 export MY_ENV_VAR2="${some_path}/${var2}"
 ```
 
 These export statements are always placed **after**<br />
 all variables declarations in the underlying shell expresison.
 
+#### ANSIBLE_ Variables
+
+Any variables matching ANSIBLE_.* will automatically be expressed as export statements.
+
+As an example, suppose I define such variables in the above *Taskfile.yaml*, as follows:
+
+```
+- hosts: myhosts
+  gather_facts: true
+  become: true
+  vars:
+    ANSIBLE_VAULT_PASSWORD_FILE: /some/path/some/password_file
+    ANSIBLE_CALLBACK_PLUGINS: /some/other/path/some/plugins
+    # ...
+```
+
+Upon invoking the `tasks` command with the `---echo` flag:
+
+- The underlying shell expression would be revealed as:<br />
+
+```
+var1="value1"
+var2="value2"
+export ANSIBLE_VAULT_PASSWORD_FILE="/some/path/some/password_file"
+export ANSIBLE_CALLBACK_PLUGINS="/some/other/path/some/plugins"
+```
+
 <a name="cli_provider"></a>
 
 ### cli_provider
 
 You can override the underlying command-line provider in two ways:
 
 - Via the tasks config file (see [examples](#examples))
```

### Comparing `ansible_taskrunner-2.8.3/ansible_taskrunner.egg-info/SOURCES.txt` & `ansible_taskrunner-2.8.4/ansible_taskrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/docs/Makefile` & `ansible_taskrunner-2.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/docs/conf.py` & `ansible_taskrunner-2.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/docs/installation.rst` & `ansible_taskrunner-2.8.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/docs/make.bat` & `ansible_taskrunner-2.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/ansible/README.md` & `ansible_taskrunner-2.8.4/examples/ansible/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/ansible/Taskfile.yaml` & `ansible_taskrunner-2.8.4/examples/ansible/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/bash/README.md` & `ansible_taskrunner-2.8.4/examples/bash/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/bash/Taskfile.yaml` & `ansible_taskrunner-2.8.4/examples/bash/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/choice/Taskfile.yaml` & `ansible_taskrunner-2.8.4/examples/choice/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/custom-cli-provider/README.md` & `ansible_taskrunner-2.8.4/examples/custom-cli-provider/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/custom-cli-provider/Taskfile.yaml` & `ansible_taskrunner-2.8.4/examples/custom-cli-provider/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/custom-cli-provider/plugins/providers/example/__init__.py` & `ansible_taskrunner-2.8.4/examples/custom-cli-provider/plugins/providers/example/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/mutually-exclusive/Taskfile.yaml` & `ansible_taskrunner-2.8.4/examples/mutually-exclusive/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/prompt/Taskfile.yaml` & `ansible_taskrunner-2.8.4/examples/prompt/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/vagrant/README.md` & `ansible_taskrunner-2.8.4/examples/vagrant/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/vagrant/Taskfile.yaml` & `ansible_taskrunner-2.8.4/examples/vagrant/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/examples/vagrant/Vagrantfile` & `ansible_taskrunner-2.8.4/examples/vagrant/Vagrantfile`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/setup.cfg` & `ansible_taskrunner-2.8.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.3/tests/test_ansible_taskrunner.py` & `ansible_taskrunner-2.8.4/tests/test_ansible_taskrunner.py`

 * *Files identical despite different names*

