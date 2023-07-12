# Comparing `tmp/fedrq-0.8.0.tar.gz` & `tmp/fedrq-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedrq-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fedrq-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fedrq-0.8.0.tar` & `fedrq-0.9.0.tar`

### file list

```diff
@@ -1,116 +1,131 @@
--rw-r--r--   0        0        0      749 2023-06-16 02:38:20.599415 fedrq-0.8.0/.builds/epel9.yml
--rw-r--r--   0        0        0     2348 2023-06-19 17:25:09.703310 fedrq-0.8.0/.builds/main.yml
--rw-r--r--   0        0        0     1187 2023-06-19 21:38:24.304734 fedrq-0.8.0/.builds/mockbuild-37.yml
--rw-r--r--   0        0        0      791 2023-06-21 01:13:53.672190 fedrq-0.8.0/.builds/mockbuild.yml
--rw-r--r--   0        0        0      264 2023-06-16 02:40:08.756301 fedrq-0.8.0/.copr/Makefile
-lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.8.0/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
-lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.8.0/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
-lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.8.0/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
-lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.8.0/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
--rw-r--r--   0        0        0      268 2023-06-06 22:57:17.280340 fedrq-0.8.0/.gitignore
--rw-r--r--   0        0        0     2553 2023-06-16 02:38:20.601415 fedrq-0.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    17337 2022-12-13 02:49:11.735043 fedrq-0.8.0/LICENSES/GPL-2.0-or-later.txt
--rw-r--r--   0        0        0     1078 2022-12-13 02:49:11.735043 fedrq-0.8.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     2427 2023-02-19 18:37:34.747046 fedrq-0.8.0/LICENSES/PSF-2.0.txt
--rw-r--r--   0        0        0     1211 2023-02-19 18:37:34.747046 fedrq-0.8.0/LICENSES/Unlicense.txt
--rw-r--r--   0        0        0    13420 2023-06-21 14:13:12.284398 fedrq-0.8.0/NEWS.md
--rw-r--r--   0        0        0       89 2023-03-18 21:16:55.983019 fedrq-0.8.0/NEWS.md.license
--rw-r--r--   0        0        0    12144 2023-03-27 04:19:29.833647 fedrq-0.8.0/README.md
--rwxr-xr-x   0        0        0      687 2023-06-06 22:57:17.280340 fedrq-0.8.0/contrib/add_frag.py
--rwxr-xr-x   0        0        0      906 2023-03-19 23:05:00.923501 fedrq-0.8.0/contrib/api_examples/a_noarch_bash.py
--rwxr-xr-x   0        0        0     2502 2023-03-19 23:05:00.924501 fedrq-0.8.0/contrib/api_examples/ftbfs_retirements.py
--rw-r--r--   0        0        0      630 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/main.yaml
--rw-r--r--   0        0        0      183 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/roles/configure/handlers/main.yaml
--rw-r--r--   0        0        0      885 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/roles/configure/tasks/main.yml
--rw-r--r--   0        0        0      163 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
--rw-r--r--   0        0        0      415 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
--rw-r--r--   0        0        0      156 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/vars.yaml
--rwxr-xr-x   0        0        0      914 2023-06-06 22:57:17.280340 fedrq-0.8.0/contrib/fedoraify.py
--rw-r--r--   0        0        0     5728 2023-06-06 22:57:17.280340 fedrq-0.8.0/doc/API/Summary.md
--rw-r--r--   0        0        0      147 2023-03-19 23:07:21.353951 fedrq-0.8.0/doc/API/backends/base.md
--rw-r--r--   0        0        0      343 2023-06-06 22:57:17.280340 fedrq-0.8.0/doc/API/backends/dnf.md
--rw-r--r--   0        0        0      532 2023-06-06 22:57:17.280340 fedrq-0.8.0/doc/API/backends/libdnf5.md
--rw-r--r--   0        0        0      133 2023-03-19 23:07:21.353951 fedrq-0.8.0/doc/API/config.md
--rw-r--r--   0        0        0      145 2023-03-19 23:07:21.353951 fedrq-0.8.0/doc/API/release_repo.md
-lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.8.0/doc/News.md -> ../NEWS.md
--rw-r--r--   0        0        0     3322 2023-06-06 22:57:17.280340 fedrq-0.8.0/doc/dnf-repoquery-diff.md
--rw-r--r--   0        0        0    16162 2023-06-06 22:57:17.281340 fedrq-0.8.0/doc/fedrq.1.scd
--rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.8.0/doc/fedrq.1.scd.license
--rw-r--r--   0        0        0     4958 2023-06-06 22:57:17.281340 fedrq-0.8.0/doc/fedrq.5.scd
--rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.8.0/doc/fedrq.5.scd.license
-lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.8.0/doc/index.md -> ../README.md
--rw-r--r--   0        0        0      193 2023-06-16 02:38:20.601415 fedrq-0.8.0/fedrq.rpmlintrc
--rw-r--r--   0        0        0     3567 2023-06-21 14:13:11.838399 fedrq-0.8.0/fedrq.spec
--rw-r--r--   0        0        0     2169 2023-06-06 22:57:17.281340 fedrq-0.8.0/mkdocs.yml
--rw-r--r--   0        0        0     6722 2023-06-21 14:11:42.850542 fedrq-0.8.0/noxfile.py
--rw-r--r--   0        0        0     3455 2023-06-21 01:22:32.983394 fedrq-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      532 2023-03-18 19:37:34.178930 fedrq-0.8.0/ruff.toml
--rw-r--r--   0        0        0      371 2023-06-21 14:13:05.594408 fedrq-0.8.0/src/fedrq/__init__.py
--rw-r--r--   0        0        0      219 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/__main__.py
--rw-r--r--   0        0        0     1713 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/_compat.py
--rw-r--r--   0        0        0      173 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/_config.py
--rw-r--r--   0        0        0     1181 2023-06-16 02:38:20.603415 fedrq-0.8.0/src/fedrq/_utils.py
--rw-r--r--   0        0        0     2526 2023-06-16 02:38:20.604415 fedrq-0.8.0/src/fedrq/backends/__init__.py
--rw-r--r--   0        0        0    14489 2023-06-20 21:21:53.608401 fedrq-0.8.0/src/fedrq/backends/base.py
--rw-r--r--   0        0        0      630 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/backends/dnf/__init__.py
--rw-r--r--   0        0        0     6949 2023-06-06 22:57:17.282340 fedrq-0.8.0/src/fedrq/backends/dnf/backend.py
--rw-r--r--   0        0        0      741 2023-06-19 17:06:43.021535 fedrq-0.8.0/src/fedrq/backends/libdnf5/__init__.py
--rw-r--r--   0        0        0    28272 2023-06-20 21:21:16.516440 fedrq-0.8.0/src/fedrq/backends/libdnf5/backend.py
--rw-r--r--   0        0        0     2111 2023-06-18 22:08:35.139910 fedrq-0.8.0/src/fedrq/cli/__init__.py
--rw-r--r--   0        0        0    15896 2023-06-20 21:21:53.609401 fedrq-0.8.0/src/fedrq/cli/base.py
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.8.0/src/fedrq/cli/commands/__init__.py
--rw-r--r--   0        0        0     2854 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/cli/commands/pkgs.py
--rw-r--r--   0        0        0     1489 2023-06-06 22:57:17.282340 fedrq-0.8.0/src/fedrq/cli/commands/repolist.py
--rw-r--r--   0        0        0     2425 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/cli/commands/subpkgs.py
--rw-r--r--   0        0        0    10843 2023-06-06 00:02:46.964960 fedrq-0.8.0/src/fedrq/cli/commands/whatrequires.py
--rw-r--r--   0        0        0    13071 2023-06-19 17:26:45.758192 fedrq-0.8.0/src/fedrq/cli/formatters.py
--rw-r--r--   0        0        0    16472 2023-06-16 02:38:20.606415 fedrq-0.8.0/src/fedrq/config.py
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.8.0/src/fedrq/data/__init__.py
--rw-r--r--   0        0        0     7326 2023-06-20 21:21:53.609401 fedrq-0.8.0/src/fedrq/data/releases.toml
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/__init__.py
--rw-r--r--   0        0        0     2053 2023-06-06 22:57:17.282340 fedrq-0.8.0/src/fedrq/data/repos/almalinux.repo
--rw-r--r--   0        0        0      639 2023-03-27 04:19:29.835647 fedrq-0.8.0/src/fedrq/data/repos/amazonlinux.repo
--rw-r--r--   0        0        0     1386 2023-06-06 22:57:17.282340 fedrq-0.8.0/src/fedrq/data/repos/centos-stream-compose.repo
--rw-r--r--   0        0        0     1850 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/centos-stream.repo
--rw-r--r--   0        0        0     1494 2023-06-06 22:57:17.283340 fedrq-0.8.0/src/fedrq/data/repos/centos-stream8-compose.repo
--rw-r--r--   0        0        0     1599 2023-03-18 19:37:34.184930 fedrq-0.8.0/src/fedrq/data/repos/centos-stream8.repo
--rw-r--r--   0        0        0     1342 2023-06-20 21:21:53.609401 fedrq-0.8.0/src/fedrq/data/repos/centos7.repo
--rw-r--r--   0        0        0     1809 2023-06-06 22:57:17.283340 fedrq-0.8.0/src/fedrq/data/repos/eln.repo
--rw-r--r--   0        0        0     2158 2023-06-06 22:57:17.283340 fedrq-0.8.0/src/fedrq/data/repos/epel.repo
--rw-r--r--   0        0        0    14146 2023-06-06 22:57:17.283340 fedrq-0.8.0/src/fedrq/data/repos/fedora-eln.repo
--rw-r--r--   0        0        0     2402 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/fedora-rawhide.repo
--rw-r--r--   0        0        0     1480 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/fedora-updates-testing.repo
--rw-r--r--   0        0        0     1422 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/fedora-updates.repo
--rw-r--r--   0        0        0     1375 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/fedora.repo
--rw-r--r--   0        0        0      425 2023-06-06 22:57:17.283340 fedrq-0.8.0/src/fedrq/data/repos/rawhide-buildroot.repo
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/py.typed
--rw-r--r--   0        0        0     8912 2023-06-19 17:26:45.758192 fedrq-0.8.0/src/fedrq/release_repo.py
--rw-r--r--   0        0        0      994 2023-06-20 21:21:53.609401 fedrq-0.8.0/src/fedrq/repoquery.py
--rw-r--r--   0        0        0      154 2023-02-19 18:37:34.753046 fedrq-0.8.0/tests/.gitignore
--rw-r--r--   0        0        0        0 2023-06-06 22:57:17.283340 fedrq-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     2948 2023-06-16 02:38:20.607415 fedrq-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-06 22:57:17.283340 fedrq-0.8.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     1775 2023-06-16 02:38:20.607415 fedrq-0.8.0/tests/integration/test_backends.py
--rw-r--r--   0        0        0      771 2023-06-16 02:38:20.608415 fedrq-0.8.0/tests/integration/test_pkgs.py
--rw-r--r--   0        0        0     1292 2023-06-20 21:34:55.966590 fedrq-0.8.0/tests/integration/test_subpkgs.py
--rw-r--r--   0        0        0     1761 2023-06-16 02:38:20.609415 fedrq-0.8.0/tests/integration/test_whatrequires.py
--rw-r--r--   0        0        0     1370 2023-06-16 02:38:20.609415 fedrq-0.8.0/tests/integration/test_whatrequires_src.py
--rw-r--r--   0        0        0        0 2023-06-06 22:57:17.283340 fedrq-0.8.0/tests/test_data/__init__.py
--rw-r--r--   0        0        0      332 2023-02-19 18:37:34.753046 fedrq-0.8.0/tests/test_data/_template.spec
--rwxr-xr-x   0        0        0     1449 2023-02-19 18:37:34.754046 fedrq-0.8.0/tests/test_data/build.sh
--rw-r--r--   0        0        0     1130 2023-02-19 18:37:34.754046 fedrq-0.8.0/tests/test_data/repos/repo1/specs/e1/packageb.spec
--rw-r--r--   0        0        0     1060 2023-02-19 18:37:34.754046 fedrq-0.8.0/tests/test_data/repos/repo1/specs/packagea.spec
--rw-r--r--   0        0        0     1156 2023-02-19 18:37:34.754046 fedrq-0.8.0/tests/test_data/repos/repo1/specs/packageb.spec
--rw-r--r--   0        0        0        0 2023-06-06 22:57:17.283340 fedrq-0.8.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     2128 2023-06-16 02:38:20.610415 fedrq-0.8.0/tests/unit/test_checkconfig.py
--rw-r--r--   0        0        0     7163 2023-06-16 02:38:20.611415 fedrq-0.8.0/tests/unit/test_command.py
--rw-r--r--   0        0        0     7780 2023-06-20 21:20:35.641482 fedrq-0.8.0/tests/unit/test_formatters.py
--rw-r--r--   0        0        0     3361 2023-06-20 21:34:58.442587 fedrq-0.8.0/tests/unit/test_pkgs.py
--rw-r--r--   0        0        0     1681 2023-06-16 02:38:20.612415 fedrq-0.8.0/tests/unit/test_release.py
--rw-r--r--   0        0        0      449 2023-06-16 02:38:20.612415 fedrq-0.8.0/tests/unit/test_repo.py
--rw-r--r--   0        0        0      640 2023-06-16 02:38:20.613415 fedrq-0.8.0/tests/unit/test_repolist.py
--rw-r--r--   0        0        0     1325 2023-06-16 02:38:20.613415 fedrq-0.8.0/tests/unit/test_repoquery.py
--rw-r--r--   0        0        0     2712 2023-06-16 02:38:20.614415 fedrq-0.8.0/tests/unit/test_subbpkgs.py
--rw-r--r--   0        0        0     4088 2023-06-16 02:38:20.614415 fedrq-0.8.0/tests/unit/test_whatrequires.py
--rw-r--r--   0        0        0      689 2023-06-16 02:38:20.615415 fedrq-0.8.0/tests/unit/test_whatrequires_src.py
--rw-r--r--   0        0        0    14335 1970-01-01 00:00:00.000000 fedrq-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      749 2023-06-26 23:03:24.118349 fedrq-0.9.0/.builds/epel9.yml
+-rw-r--r--   0        0        0     2348 2023-06-26 23:03:24.118349 fedrq-0.9.0/.builds/main.yml
+-rw-r--r--   0        0        0     1187 2023-06-26 23:03:24.118349 fedrq-0.9.0/.builds/mockbuild-37.yml
+-rw-r--r--   0        0        0      791 2023-06-26 23:03:24.118349 fedrq-0.9.0/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      264 2023-06-26 23:03:24.118349 fedrq-0.9.0/.copr/Makefile
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-0.9.0/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-0.9.0/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-0.9.0/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.119349 fedrq-0.9.0/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0      268 2023-06-26 23:03:24.119349 fedrq-0.9.0/.gitignore
+-rw-r--r--   0        0        0     2553 2023-06-26 23:03:24.119349 fedrq-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    17337 2023-06-26 23:03:24.120349 fedrq-0.9.0/LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2023-06-26 23:03:24.120349 fedrq-0.9.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2427 2023-06-26 23:03:24.120349 fedrq-0.9.0/LICENSES/PSF-2.0.txt
+-rw-r--r--   0        0        0     1211 2023-06-26 23:03:24.120349 fedrq-0.9.0/LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0    14474 2023-06-29 17:37:52.842689 fedrq-0.9.0/NEWS.md
+-rw-r--r--   0        0        0       89 2023-06-26 23:03:24.120349 fedrq-0.9.0/NEWS.md.license
+-rw-r--r--   0        0        0    12644 2023-06-29 17:31:29.461913 fedrq-0.9.0/README.md
+-rwxr-xr-x   0        0        0      687 2023-06-26 23:03:24.121349 fedrq-0.9.0/contrib/add_frag.py
+-rwxr-xr-x   0        0        0      906 2023-06-26 23:03:24.121349 fedrq-0.9.0/contrib/api_examples/a_noarch_bash.py
+-rwxr-xr-x   0        0        0     2502 2023-06-26 23:03:24.121349 fedrq-0.9.0/contrib/api_examples/ftbfs_retirements.py
+-rw-r--r--   0        0        0      548 2023-06-28 23:32:16.904799 fedrq-0.9.0/contrib/container/Containerfile
+-rw-r--r--   0        0        0      573 2023-06-29 17:14:01.127260 fedrq-0.9.0/contrib/container/Containerfile.rhel
+-rw-r--r--   0        0        0      759 2023-06-28 23:32:16.904799 fedrq-0.9.0/contrib/container/build.yml
+-rw-r--r--   0        0        0      446 2023-06-29 17:17:07.001666 fedrq-0.9.0/contrib/container/rhel.toml
+-rw-r--r--   0        0        0      630 2023-06-26 23:03:24.121349 fedrq-0.9.0/contrib/deploy-docsite/main.yaml
+-rw-r--r--   0        0        0      183 2023-06-26 23:03:24.122349 fedrq-0.9.0/contrib/deploy-docsite/roles/configure/handlers/main.yaml
+-rw-r--r--   0        0        0      885 2023-06-26 23:03:24.122349 fedrq-0.9.0/contrib/deploy-docsite/roles/configure/tasks/main.yml
+-rw-r--r--   0        0        0      163 2023-06-26 23:03:24.122349 fedrq-0.9.0/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
+-rw-r--r--   0        0        0      415 2023-06-26 23:03:24.122349 fedrq-0.9.0/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
+-rw-r--r--   0        0        0      156 2023-06-26 23:03:24.123349 fedrq-0.9.0/contrib/deploy-docsite/vars.yaml
+-rwxr-xr-x   0        0        0      914 2023-06-26 23:03:24.123349 fedrq-0.9.0/contrib/fedoraify.py
+-rw-r--r--   0        0        0     5728 2023-06-26 23:03:24.123349 fedrq-0.9.0/doc/API/Summary.md
+-rw-r--r--   0        0        0      147 2023-06-26 23:03:24.123349 fedrq-0.9.0/doc/API/backends/base.md
+-rw-r--r--   0        0        0      343 2023-06-26 23:03:24.123349 fedrq-0.9.0/doc/API/backends/dnf.md
+-rw-r--r--   0        0        0      532 2023-06-26 23:03:24.123349 fedrq-0.9.0/doc/API/backends/libdnf5.md
+-rw-r--r--   0        0        0      133 2023-06-26 23:03:24.123349 fedrq-0.9.0/doc/API/config.md
+-rw-r--r--   0        0        0      145 2023-06-26 23:03:24.124349 fedrq-0.9.0/doc/API/release_repo.md
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.124349 fedrq-0.9.0/doc/News.md -> ../NEWS.md
+-rw-r--r--   0        0        0     3322 2023-06-26 23:03:24.124349 fedrq-0.9.0/doc/dnf-repoquery-diff.md
+-rw-r--r--   0        0        0    16598 2023-06-29 16:24:22.948766 fedrq-0.9.0/doc/fedrq.1.scd
+-rw-r--r--   0        0        0       98 2023-06-26 23:03:24.124349 fedrq-0.9.0/doc/fedrq.1.scd.license
+-rw-r--r--   0        0        0     4958 2023-06-26 23:03:24.124349 fedrq-0.9.0/doc/fedrq.5.scd
+-rw-r--r--   0        0        0       98 2023-06-26 23:03:24.125349 fedrq-0.9.0/doc/fedrq.5.scd.license
+lrwxr-xr-x   0        0        0        0 2023-06-26 23:03:24.125349 fedrq-0.9.0/doc/index.md -> ../README.md
+-rw-r--r--   0        0        0      193 2023-06-26 23:03:24.125349 fedrq-0.9.0/fedrq.rpmlintrc
+-rw-r--r--   0        0        0     3641 2023-06-29 17:37:52.482691 fedrq-0.9.0/fedrq.spec
+-rw-r--r--   0        0        0     2169 2023-06-26 23:03:24.125349 fedrq-0.9.0/mkdocs.yml
+-rw-r--r--   0        0        0     6722 2023-06-29 03:33:21.071453 fedrq-0.9.0/noxfile.py
+-rw-r--r--   0        0        0     3496 2023-06-29 16:24:22.847766 fedrq-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      532 2023-06-26 23:03:24.126349 fedrq-0.9.0/ruff.toml
+-rw-r--r--   0        0        0      371 2023-06-29 17:37:47.357707 fedrq-0.9.0/src/fedrq/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-26 23:03:24.126349 fedrq-0.9.0/src/fedrq/__main__.py
+-rw-r--r--   0        0        0     2822 2023-06-28 23:32:16.252803 fedrq-0.9.0/src/fedrq/_archive.py
+-rw-r--r--   0        0        0     1713 2023-06-26 23:03:24.126349 fedrq-0.9.0/src/fedrq/_compat.py
+-rw-r--r--   0        0        0      173 2023-06-26 23:03:24.126349 fedrq-0.9.0/src/fedrq/_config.py
+-rw-r--r--   0        0        0     1268 2023-06-28 23:32:16.468802 fedrq-0.9.0/src/fedrq/_utils.py
+-rw-r--r--   0        0        0     2526 2023-06-26 23:03:24.127349 fedrq-0.9.0/src/fedrq/backends/__init__.py
+-rw-r--r--   0        0        0    14850 2023-06-29 16:24:22.745766 fedrq-0.9.0/src/fedrq/backends/base.py
+-rw-r--r--   0        0        0      630 2023-06-26 23:03:24.127349 fedrq-0.9.0/src/fedrq/backends/dnf/__init__.py
+-rw-r--r--   0        0        0     7039 2023-06-29 02:38:33.991820 fedrq-0.9.0/src/fedrq/backends/dnf/backend.py
+-rw-r--r--   0        0        0      741 2023-06-26 23:03:24.128349 fedrq-0.9.0/src/fedrq/backends/libdnf5/__init__.py
+-rw-r--r--   0        0        0    29790 2023-06-29 16:40:18.859715 fedrq-0.9.0/src/fedrq/backends/libdnf5/backend.py
+-rw-r--r--   0        0        0     2313 2023-06-28 23:32:16.795800 fedrq-0.9.0/src/fedrq/cli/__init__.py
+-rw-r--r--   0        0        0    17914 2023-06-28 23:32:16.688800 fedrq-0.9.0/src/fedrq/cli/base.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.129349 fedrq-0.9.0/src/fedrq/cli/commands/__init__.py
+-rw-r--r--   0        0        0     5672 2023-06-28 23:32:16.795800 fedrq-0.9.0/src/fedrq/cli/commands/download.py
+-rw-r--r--   0        0        0     1926 2023-06-28 23:32:16.577801 fedrq-0.9.0/src/fedrq/cli/commands/pkgs.py
+-rw-r--r--   0        0        0     1425 2023-06-28 23:32:16.688800 fedrq-0.9.0/src/fedrq/cli/commands/repolist.py
+-rw-r--r--   0        0        0     2394 2023-06-28 23:32:16.688800 fedrq-0.9.0/src/fedrq/cli/commands/subpkgs.py
+-rw-r--r--   0        0        0    10020 2023-06-28 23:32:16.688800 fedrq-0.9.0/src/fedrq/cli/commands/whatrequires.py
+-rw-r--r--   0        0        0    13218 2023-06-28 02:09:36.446265 fedrq-0.9.0/src/fedrq/cli/formatters.py
+-rw-r--r--   0        0        0    16472 2023-06-26 23:03:24.131349 fedrq-0.9.0/src/fedrq/config.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.131349 fedrq-0.9.0/src/fedrq/data/__init__.py
+-rw-r--r--   0        0        0     9322 2023-06-28 02:09:36.446265 fedrq-0.9.0/src/fedrq/data/releases.toml
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.131349 fedrq-0.9.0/src/fedrq/data/repos/__init__.py
+-rw-r--r--   0        0        0     2053 2023-06-26 23:03:24.131349 fedrq-0.9.0/src/fedrq/data/repos/almalinux.repo
+-rw-r--r--   0        0        0      639 2023-06-26 23:03:24.131349 fedrq-0.9.0/src/fedrq/data/repos/amazonlinux.repo
+-rw-r--r--   0        0        0     1386 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/centos-stream-compose.repo
+-rw-r--r--   0        0        0     1850 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/centos-stream.repo
+-rw-r--r--   0        0        0     1494 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/centos-stream8-compose.repo
+-rw-r--r--   0        0        0     1599 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/centos-stream8.repo
+-rw-r--r--   0        0        0     1342 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/centos7.repo
+-rw-r--r--   0        0        0     1809 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/eln.repo
+-rw-r--r--   0        0        0     2158 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/epel.repo
+-rw-r--r--   0        0        0    14146 2023-06-26 23:03:24.132349 fedrq-0.9.0/src/fedrq/data/repos/fedora-eln.repo
+-rw-r--r--   0        0        0     2402 2023-06-26 23:03:24.133349 fedrq-0.9.0/src/fedrq/data/repos/fedora-rawhide.repo
+-rw-r--r--   0        0        0     1480 2023-06-26 23:03:24.133349 fedrq-0.9.0/src/fedrq/data/repos/fedora-updates-testing.repo
+-rw-r--r--   0        0        0     1422 2023-06-29 16:45:13.311775 fedrq-0.9.0/src/fedrq/data/repos/fedora-updates.repo
+-rw-r--r--   0        0        0     1375 2023-06-29 16:45:05.106801 fedrq-0.9.0/src/fedrq/data/repos/fedora.repo
+-rw-r--r--   0        0        0     1374 2023-06-28 02:09:36.446265 fedrq-0.9.0/src/fedrq/data/repos/oraclelinux-8.repo
+-rw-r--r--   0        0        0     1374 2023-06-29 16:45:34.108708 fedrq-0.9.0/src/fedrq/data/repos/oraclelinux-9.repo
+-rw-r--r--   0        0        0      425 2023-06-26 23:03:24.133349 fedrq-0.9.0/src/fedrq/data/repos/rawhide-buildroot.repo
+-rw-r--r--   0        0        0     6475 2023-06-28 02:09:36.447265 fedrq-0.9.0/src/fedrq/data/repos/rocky.repo
+-rw-r--r--   0        0        0     3505 2023-06-28 02:09:36.447265 fedrq-0.9.0/src/fedrq/data/repos/ubi.repo
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.133349 fedrq-0.9.0/src/fedrq/py.typed
+-rw-r--r--   0        0        0     9225 2023-06-29 16:24:22.948766 fedrq-0.9.0/src/fedrq/release_repo.py
+-rw-r--r--   0        0        0      994 2023-06-26 23:03:24.134349 fedrq-0.9.0/src/fedrq/repoquery.py
+-rw-r--r--   0        0        0      154 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2948 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1775 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/integration/test_backends.py
+-rw-r--r--   0        0        0      416 2023-06-28 23:32:16.795800 fedrq-0.9.0/tests/integration/test_download.py
+-rw-r--r--   0        0        0      771 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/integration/test_pkgs.py
+-rw-r--r--   0        0        0     1292 2023-06-26 23:03:24.134349 fedrq-0.9.0/tests/integration/test_subpkgs.py
+-rw-r--r--   0        0        0     1761 2023-06-26 23:03:24.135349 fedrq-0.9.0/tests/integration/test_whatrequires.py
+-rw-r--r--   0        0        0     1370 2023-06-26 23:03:24.135349 fedrq-0.9.0/tests/integration/test_whatrequires_src.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.135349 fedrq-0.9.0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0      332 2023-06-26 23:03:24.135349 fedrq-0.9.0/tests/test_data/_template.spec
+-rwxr-xr-x   0        0        0     1449 2023-06-26 23:03:24.135349 fedrq-0.9.0/tests/test_data/build.sh
+-rw-r--r--   0        0        0     1130 2023-06-26 23:03:24.136349 fedrq-0.9.0/tests/test_data/repos/repo1/specs/e1/packageb.spec
+-rw-r--r--   0        0        0     1060 2023-06-26 23:03:24.136349 fedrq-0.9.0/tests/test_data/repos/repo1/specs/packagea.spec
+-rw-r--r--   0        0        0     1156 2023-06-26 23:03:24.136349 fedrq-0.9.0/tests/test_data/repos/repo1/specs/packageb.spec
+-rw-r--r--   0        0        0        0 2023-06-26 23:03:24.136349 fedrq-0.9.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1178 2023-06-29 01:21:42.132684 fedrq-0.9.0/tests/unit/test_archive.py
+-rw-r--r--   0        0        0     2128 2023-06-26 23:03:24.136349 fedrq-0.9.0/tests/unit/test_checkconfig.py
+-rw-r--r--   0        0        0     7163 2023-06-26 23:03:24.137349 fedrq-0.9.0/tests/unit/test_command.py
+-rw-r--r--   0        0        0     1351 2023-06-28 23:32:16.795800 fedrq-0.9.0/tests/unit/test_download.py
+-rw-r--r--   0        0        0     9077 2023-06-28 02:09:36.447265 fedrq-0.9.0/tests/unit/test_formatters.py
+-rw-r--r--   0        0        0     3361 2023-06-26 23:03:24.137349 fedrq-0.9.0/tests/unit/test_pkgs.py
+-rw-r--r--   0        0        0     1681 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_release.py
+-rw-r--r--   0        0        0      562 2023-06-29 16:24:22.948766 fedrq-0.9.0/tests/unit/test_release_repo.py
+-rw-r--r--   0        0        0      449 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_repo.py
+-rw-r--r--   0        0        0      640 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_repolist.py
+-rw-r--r--   0        0        0     1325 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_repoquery.py
+-rw-r--r--   0        0        0     2712 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_subbpkgs.py
+-rw-r--r--   0        0        0      428 2023-06-28 23:32:16.468802 fedrq-0.9.0/tests/unit/test_util.py
+-rw-r--r--   0        0        0     4088 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_whatrequires.py
+-rw-r--r--   0        0        0      689 2023-06-26 23:03:24.138349 fedrq-0.9.0/tests/unit/test_whatrequires_src.py
+-rw-r--r--   0        0        0    14835 1970-01-01 00:00:00.000000 fedrq-0.9.0/PKG-INFO
```

### Comparing `fedrq-0.8.0/.builds/epel9.yml` & `fedrq-0.9.0/.builds/epel9.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/.builds/main.yml` & `fedrq-0.9.0/.builds/main.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/.builds/mockbuild-37.yml` & `fedrq-0.9.0/.builds/mockbuild-37.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/.builds/mockbuild.yml` & `fedrq-0.9.0/.builds/mockbuild.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/CONTRIBUTING.md` & `fedrq-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/LICENSES/GPL-2.0-or-later.txt` & `fedrq-0.9.0/LICENSES/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/LICENSES/MIT.txt` & `fedrq-0.9.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/LICENSES/PSF-2.0.txt` & `fedrq-0.9.0/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/LICENSES/Unlicense.txt` & `fedrq-0.9.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/NEWS.md` & `fedrq-0.9.0/NEWS.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,44 @@
 NEWS
 =====
 
+## 0.9.0 - 2023-06-29 <a id='0.9.0'></a>
+
+### Added
+
+- add remote_location formatter
+- document CentOS 7 release configuration
+- add UBI release configuration
+- add Oracle Linux release configuration
+- add Rocky Linux release configuration
+- add experimental download and download-spec subcommands
+- add fedrq [container builds][container builds]
+- add @source-repos repo class
+- BaseMaker: add enable_source_repos() method
+- PackageCompat: add remote_location() method
+
+### Changed
+
+- Remove enabled=1 from built-in fedora repo defs.
+  We want all repo to have enabled=0. We control which repos are enabled and
+  disabled with repo groups configured in releases.toml.
+  This previously led to divergent behavior with the --repo and --enablerepo
+  options when querying Fedora releases on Fedora systems and non-Fedora
+  systems (e.g. CentOS).
+
+### Deprecated
+
+- deprecate support for libdnf5 < 5.0.10 and raise warnings
+
+### Fixed
+
+- backends libdnf5: don't call rpm.ts.closeDB()
+
+[container builds]: https://git.sr.ht/~gotmax23/fedrq#container-images
+
 ## 0.8.0 - 2023-06-21 <a id='0.8.0'></a>
 
 ### Added
 
 - add --version flag to CLI
 - improve repo loading error handling ([#31])
 - add CentOS 7 release configuration
```

### Comparing `fedrq-0.8.0/README.md` & `fedrq-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,27 @@
 Note that fedrq can only be installed for the system python interpreter.
 fedrq cannot be installed in a venv unless it has `--system-site-packages`,
 as it needs to find the aforementioned system bindings.
 
 `fedrq check-config --dump` requires `tomli-w`.
 The RPM package weakly depends on `python3-tomli-w`.
 
+## Container images
+
+fedrq now provides container images.
+- `quay.io/gotmax23/fedrq:latest` is built with
+  `registry.fedoraproject.org/fedora:latest`.
+- `quay.io/gotmax23/fedrq:ubi9` is built with the ubi9 image.
+  It includes a builtin `rhel9` repository configuration that can be used to
+  query the actual RHEL repositories when run on a system registered with
+  subscription-manager.
+
+Both of these images use the latest fedrq RPM packages from the
+[gotmax23/fedrq][link-copr] Copr repository.
+
 ## Versioning
 
 This project is in beta and its versioning scheme follows semver.
 
 See [NEWS.md](https://git.sr.ht/~gotmax23/fedrq/tree/main/NEWS.md).
 
 ## Python API
```

### Comparing `fedrq-0.8.0/contrib/add_frag.py` & `fedrq-0.9.0/contrib/add_frag.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/contrib/api_examples/a_noarch_bash.py` & `fedrq-0.9.0/contrib/api_examples/a_noarch_bash.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/contrib/api_examples/ftbfs_retirements.py` & `fedrq-0.9.0/contrib/api_examples/ftbfs_retirements.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/contrib/deploy-docsite/main.yaml` & `fedrq-0.9.0/contrib/deploy-docsite/main.yaml`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/contrib/deploy-docsite/roles/configure/tasks/main.yml` & `fedrq-0.9.0/contrib/deploy-docsite/roles/configure/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/contrib/fedoraify.py` & `fedrq-0.9.0/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/doc/API/Summary.md` & `fedrq-0.9.0/doc/API/Summary.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/doc/API/backends/libdnf5.md` & `fedrq-0.9.0/doc/API/backends/libdnf5.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/doc/dnf-repoquery-diff.md` & `fedrq-0.9.0/doc/dnf-repoquery-diff.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/doc/fedrq.1.scd` & `fedrq-0.9.0/doc/fedrq.1.scd`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,17 @@
 	*https://copr.fedoraproject.org* but may be configured in fedrq's
 	configuration. *copr_chroot_fmt* must be specifced in the selected
 	branch's release configuration for this repo class to work. This is
 	configured for the builtin releases.
 *@copr:[user/name@copr_baseurl]* or *@copr:[@group/name@copr_baseurl]*
 	The *@copr* repo class also accepts a custom Copr instance.
 	Append *@* and a url.
+*@source-repos*
+	Enable the corresponding -source repos of the currently enabled
+	repositories
 *@base* or *base* or other group
 	The default repoistories for a release specified in a ReleaseConfig's
 	*defs.base*. Any other repo group specified in a release's is accepted,
 	with or without the *@*. See SPECIAL REPOS for which repo groups are
 	available for each release.
 *@repo:[key]* or *key* (fallback)
 	Accepts any repoid available in the system configuration or a .repo file
@@ -243,14 +246,18 @@
 |  EPEL Next
 :  epelX-next
 :  *@base*, *@testing*, *@testing-only*, *@next-base*, *@next-testing*,
    *@next-testing-only*
 :  *@base*, *@testing*, and *@testing-only* are supersets of the _epelX_
    equivalent.
    *@next-base*, *@next-testing*, and *@next-testing-only* only contain epel-next.
+|  CentOS 7
+:  c7
+:  *@base*
+:  
 |  CentOS Stream
 :  cXs
 :  *@base*, *@epel*, *@no-crb*, *@compose-latest*
 :  *@epel* contains epel, epel-next, and crb.
    *@no-crb* contains base minus the crb repo.
 |  CentOS Stream 8 (legacy)
 :  c8s
@@ -263,14 +270,30 @@
 :  *@base* always includes crb. *@epel* contains *@base* along with the EPEL
    repository. *@no-crb* contains *@base* minus the crb repository.
 |  Almalinux 8 (Legacy)
 :  al8
 :  @*base*, *@epel*, *@no-powertools*
 :  *@base* always includes powertools. *@epel* contains *@base* along with the EPEL
    repository. *@no-powertools* contains *@base* minus the powertools repository.
+|  UBI
+:  ubiX
+:  *@base*, *@epel*, *@no-crb*
+:  
+|  Oracle Linux 8 and 9
+:  ol8 / ol9
+:  *@base*, *@epel*, *@no-crb*, *@extra*
+:  *@extra* contains the distro_builder and UEK repos
+|  Rocky Linux 8
+:  rl8
+:  *@base*, *@epel*, *@no-powertools*
+:  
+|  Rocky Linux 9+
+:  rl9
+:  *@base*, *@epel*, *@no-crb*
+:  
 |  Amazon Linux
 :  amazon2023
 :  *@base*
 : 
 |  Fedora ELN
 :  eln
 :  *@base*, *no-crb*
```

### Comparing `fedrq-0.8.0/doc/fedrq.5.scd` & `fedrq-0.9.0/doc/fedrq.5.scd`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/fedrq.spec` & `fedrq-0.9.0/fedrq.spec`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT.html
 
 %bcond libdnf5 %[0%{?fedora} >= 38]
 
 Name:           fedrq
-Version:        0.8.0
+Version:        0.9.0
 Release:        1%{?dist}
 Summary:        A tool to query the Fedora and EPEL repositories
 
 # - code is GPL-2.0-or-later
 # - the data and config files in fedrq/data are UNLICENSEed
 # - Embeded repo defs are MIT.
 # - PSF-2.0 code copied from Cpython 3.11 for older Python versions
@@ -95,14 +95,17 @@
 %{bash_completions_dir}/fedrq
 %{fish_completions_dir}/fedrq.fish
 %{_mandir}/man1/fedrq.1*
 %{_mandir}/man5/fedrq.5*
 
 
 %changelog
+* Thu Jun 29 2023 Maxwell G <maxwell@gtmx.me> - 0.9.0-1
+- Release 0.9.0.
+
 * Wed Jun 21 2023 Maxwell G <maxwell@gtmx.me> - 0.8.0-1
 - Release 0.8.0.
 
 * Wed May 31 2023 Maxwell G <maxwell@gtmx.me> - 0.7.1-1
 - Release 0.7.1.
 
 * Tue May 30 2023 Maxwell G <maxwell@gtmx.me> - 0.7.0-1
```

### Comparing `fedrq-0.8.0/mkdocs.yml` & `fedrq-0.9.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/noxfile.py` & `fedrq-0.9.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/pyproject.toml` & `fedrq-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -94,19 +94,20 @@
 
 [tool.flit.external-data]
 # Currently, this just contains share/licenses/fedrq to work around flit's lack
 # of proper support for including these files in dist-info.
 # To comply with the license, its must be included in the wheel.
 directory = ".data"
 
-# [tool.mypy]
+[tool.mypy]
+check_untyped_defs = true
 # plugins = ["pydantic.mypy"]
 
 [[tool.mypy.overrides]]
-module = ["dnf.*", "hawkey.*", "libdnf5.*", "rpm.*"]
+module = ["argcomplete.*", "dnf.*", "hawkey.*", "libdnf5.*", "rpm.*"]
 ignore_missing_imports = true
 
 
 
 [tool.pytest.ini_options]
 markers = ["no_rpm_mock: Tests that cannot be run in a mock chroot w/o networking"]
 addopts = [
```

### Comparing `fedrq-0.8.0/ruff.toml` & `fedrq-0.9.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/_compat.py` & `fedrq-0.9.0/src/fedrq/_compat.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/_utils.py` & `fedrq-0.9.0/src/fedrq/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 from __future__ import annotations
 
 import logging
 import typing as t
-from collections.abc import MutableMapping
+from collections.abc import Iterator, MutableMapping
 
 if t.TYPE_CHECKING:
     from fedrq.backends.base import PackageCompat, PackageQueryCompat
 
 logger = logging.getLogger(__name__)
 
 
@@ -35,7 +35,12 @@
             pass
         elif isinstance(value, MutableMapping) and isinstance(
             dest[key], MutableMapping
         ):
             merge_dict(value, dest[key])
             continue
         dest[key] = value
+
+
+def exhaust_it(it: Iterator[t.Any]) -> None:
+    for _ in it:
+        pass
```

### Comparing `fedrq-0.8.0/src/fedrq/backends/__init__.py` & `fedrq-0.9.0/src/fedrq/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/backends/base.py` & `fedrq-0.9.0/src/fedrq/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,20 @@
     def packager(self) -> str:
         ...
 
     @property
     def location(self) -> str:
         ...
 
+    @abc.abstractmethod
+    def remote_location(
+        self, schemes: Collection[str] | None = ("http", "ftp", "file", "https")
+    ) -> str | None:
+        ...
+
     def __hash__(self) -> int:
         ...
 
     def __lt__(self, other) -> bool:
         ...
 
     def __le__(self, other) -> bool:
@@ -368,14 +374,22 @@
     def backend(self) -> BackendMod:
         ...
 
     @abc.abstractmethod
     def repolist(self, enabled: bool | None = None) -> list[str]:
         ...
 
+    @abc.abstractmethod
+    def enable_source_repos(self) -> None:
+        """
+        Enable the corresponding -source repos of the currently enabled
+        repositories
+        """
+        ...
+
 
 class RepoqueryBase(abc.ABC):
     """
     Helpers to query a repository.
     Provides a unified repoquery interface for different backends.
     """
```

### Comparing `fedrq-0.8.0/src/fedrq/backends/dnf/__init__.py` & `fedrq-0.9.0/src/fedrq/backends/dnf/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/backends/dnf/backend.py` & `fedrq-0.9.0/src/fedrq/backends/dnf/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,17 @@
         return sys.modules[__name__]
 
     def repolist(self, enabled: bool | None = None) -> list[str]:
         if enabled is None:
             return list(self.base.repos)
         return [r.id for r in self.base.repos.values() if r.enabled is bool(enabled)]
 
+    def enable_source_repos(self) -> None:
+        self.base.repos.enable_source_repos()
+
 
 class Repoquery(RepoqueryBase):
     def __init__(self, base: dnf.Base) -> None:
         self.base: dnf.Base = base
 
     @property
     def base_arches(self) -> set[str]:
```

### Comparing `fedrq-0.8.0/src/fedrq/backends/libdnf5/__init__.py` & `fedrq-0.9.0/src/fedrq/backends/libdnf5/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/backends/libdnf5/backend.py` & `fedrq-0.9.0/src/fedrq/backends/libdnf5/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 from __future__ import annotations
 
 import functools
 import inspect
 import logging
 import sys
 import typing as t
+import warnings
 from collections.abc import Collection, Iterable
+from os.path import join as path_join
+from urllib.parse import urlparse
 
 from fedrq._utils import filter_latest
 from fedrq.backends import MissingBackendError
 from fedrq.backends.base import BackendMod, BaseMakerBase, RepoqueryBase
 from fedrq.backends.libdnf5 import BACKEND  # noqa: F401
 
 if t.TYPE_CHECKING:
@@ -33,14 +36,15 @@
     raise MissingBackendError(str(exc)) from None
 
 LOG = logging.getLogger(__name__)
 Priority_RUNTIME = libdnf5.conf.Option.Priority_RUNTIME
 StrIter = t.Union[list[str], tuple[str], str]
 IntIter = t.Union[list[int], tuple[int], int]
 CONVERT_TO_LIST = (str, int)
+MINIMUM_NOT_DEPRECATED_VERSION = "5.0.10"
 
 
 class _QueryFilterKwargs(t.TypedDict, total=False):
     name: t.Union[StrIter, libdnf5.rpm.PackageSet]
     name__eq: t.Union[StrIter, libdnf5.rpm.PackageSet]
     name__neq: t.Union[StrIter, libdnf5.rpm.PackageSet]
     name__glob: StrIter
@@ -161,14 +165,46 @@
     reponame__contains: StrIter
 
     pkg: Iterable[libdnf5.rpm.Package]
     pkg__eq: Iterable[libdnf5.rpm.Package]
     pkg__neq: Iterable[libdnf5.rpm.Package]
 
 
+@functools.cache
+def _deprecation_warn() -> None:  # pragma: no cover
+    """
+    Warn that libdnf5 versions < MINIMUM_NOT_DEPRECATED_VERSION are deprecated.
+    This is memoized so we only warn users once.
+    """
+    warnings.warn(
+        f"Support for libdnf5 versions < {MINIMUM_NOT_DEPRECATED_VERSION}"
+        " is deprecated.",
+        stacklevel=2,
+    )
+
+
+def _get_option(config: libdnf5.conf.Config, key: str) -> libdnf5.conf.Option:
+    """
+    Get an Option object from a libdnf5 Config object.
+    Maintains compatability with dnf5 versions before
+    https://github.com/rpm-software-management/dnf5/pull/327
+    """
+    LOG.debug("Getting option %s", key)
+    # dnf5 >= 5.0.8
+    if option := getattr(config, f"get_{key}_option", None):
+        LOG.debug(f"option = get_{key}_option")
+        return option()
+    # dnf5 <= 5.0.7
+    elif option := getattr(config, key, None):  # pragma: no cover
+        _deprecation_warn()
+        return option()
+    else:
+        raise ValueError(f"{key!r} is not a valid option.")
+
+
 class BaseMaker(BaseMakerBase):
     """
     Create a Base object and load repos
     """
 
     base: libdnf5.base.Base
 
@@ -298,25 +334,15 @@
 
     def _get_option(self, config: libdnf5.conf.Config, key: str) -> libdnf5.conf.Option:
         """
         Get an Option object from a libdnf5 Config object.
         Maintains compatability with dnf5 versions before
         https://github.com/rpm-software-management/dnf5/pull/327
         """
-        LOG.debug("Getting option %s", key)
-        # dnf5 > 5.0.7
-        if option := getattr(config, f"get_{key}_option", None):
-            LOG.debug(f"option = get_{key}_options")
-            return option()
-        # dnf5 <= 5.0.7
-        # TODO: Add warning and deprecate
-        elif option := getattr(config, key, None):
-            return option()
-        else:
-            raise ValueError(f"{key!r} is not a valid option.")
+        return _get_option(config, key)
 
     # This is private for now
     def _read_repofile_new(self, file: StrPath, ensure_enabled: bool = False) -> None:
         """
         Load repositories from a repo file if they're not already in the
         configuration.
         """
@@ -400,14 +426,17 @@
 
     def repolist(self, enabled: bool | None = None) -> list[str]:
         repoq = libdnf5.repo.RepoQuery(self.base)
         if enabled is not None:
             repoq.filter_enabled(enabled)
         return [r.get_id() for r in repoq]
 
+    def enable_source_repos(self) -> None:
+        self.rs.enable_source_repos()
+
 
 @functools.total_ordering
 class Package(libdnf5.rpm.Package):
     DEBUGINFO_SUFFIX = "-debuginfo"
     DEBUGSOURCE_SUFFIX = "-debugsource"
     """
     libdnf5.rpm.Package subclass with strong dnf.package.Package compatability
@@ -607,14 +636,36 @@
     def packager(self) -> str:
         return self.get_packager()
 
     @property
     def location(self) -> str:
         return self.get_location()
 
+    def remote_location(
+        self, schemes: Collection[str] | None = ("http", "ftp", "file", "https")
+    ) -> str | None:
+        location = self.location
+        if not location:  # pragma: no cover
+            return None
+        repo_obj: libdnf5.repo.RepoWeakPtr = self.get_repo()
+        mirrors = (
+            repo_obj.get_mirrors()
+            or _get_option(repo_obj.get_config(), "baseurl").get_value()
+        )
+        if not mirrors:  # pragma: no cover
+            return None
+
+        for url in mirrors:
+            if not schemes:
+                return path_join(url, location)
+            scheme = urlparse(url).scheme
+            if scheme in schemes:
+                return path_join(url, location)
+        return None
+
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}<{str(self)}>"
 
     def __str__(self) -> str:
         return self.get_nevra()
 
 
@@ -822,62 +873,61 @@
         "system-release",
         "distribution-release(releasever)",
         "distribution-release",
         "redhat-release",
         "suse-release",
     )
     ts = rpm.TransactionSet("/")
-    try:
-        ts.setVSFlags(~(rpm._RPMVSF_NOSIGNATURES | rpm._RPMVSF_NODIGESTS))
-        for distroverpkg in map(lambda p: p.encode("utf-8"), DISTROVERPKG):
-            idx = ts.dbMatch("provides", distroverpkg)
-            if not len(idx):
-                continue
-            try:
-                hdr = next(idx)
-            except StopIteration:
-                raise RuntimeError(
-                    "Error: rpmdb failed to list provides. Try: rpm --rebuilddb"
-                ) from None
-            releasever = hdr["version"]
+    ts.setVSFlags(~(rpm._RPMVSF_NOSIGNATURES | rpm._RPMVSF_NODIGESTS))
+    for distroverpkg in map(lambda p: p.encode("utf-8"), DISTROVERPKG):
+        idx = ts.dbMatch("provides", distroverpkg)
+        if not len(idx):
+            continue
+        try:
+            hdr = next(idx)
+        except StopIteration:
+            raise RuntimeError(
+                "Error: rpmdb failed to list provides. Try: rpm --rebuilddb"
+            ) from None
+        releasever = hdr["version"]
+        try:
             try:
-                try:
-                    # header returns bytes -> look for bytes
-                    # it may fail because rpm returns a decoded string since 10 Apr 2019
-                    off = hdr[rpm.RPMTAG_PROVIDENAME].index(distroverpkg)
-                except ValueError:
-                    # header returns a string -> look for a string
-                    off = hdr[rpm.RPMTAG_PROVIDENAME].index(distroverpkg.decode("utf8"))
-                flag = hdr[rpm.RPMTAG_PROVIDEFLAGS][off]
-                ver = hdr[rpm.RPMTAG_PROVIDEVERSION][off]
-                if flag == rpm.RPMSENSE_EQUAL and ver:
-                    if hdr["name"] not in (distroverpkg, distroverpkg.decode("utf8")):
-                        # override the package version
-                        releasever = ver
-            except (ValueError, KeyError, IndexError):
-                pass
-            if isinstance(releasever, bytes):
-                releasever = releasever.decode("utf-8")
-            return releasever
-        return ""
-    finally:
-        ts.closeDB()
+                # header returns bytes -> look for bytes
+                # it may fail because rpm returns a decoded string since 10 Apr 2019
+                off = hdr[rpm.RPMTAG_PROVIDENAME].index(distroverpkg)
+            except ValueError:
+                # header returns a string -> look for a string
+                off = hdr[rpm.RPMTAG_PROVIDENAME].index(distroverpkg.decode("utf8"))
+            flag = hdr[rpm.RPMTAG_PROVIDEFLAGS][off]
+            ver = hdr[rpm.RPMTAG_PROVIDEVERSION][off]
+            if flag == rpm.RPMSENSE_EQUAL and ver:
+                if hdr["name"] not in (distroverpkg, distroverpkg.decode("utf8")):
+                    # override the package version
+                    releasever = ver
+        except (ValueError, KeyError, IndexError):
+            pass
+        if isinstance(releasever, bytes):
+            releasever = releasever.decode("utf-8")
+        return releasever
+    return ""
 
 
 @functools.cache
 def get_releasever() -> str:
     """
     Return the system releasever
     """
-    # libdnf5 > 5.0.10
+    # libdnf5 >= 5.0.10
+    # https://github.com/rpm-software-management/dnf5/pull/448
     if hasattr(libdnf5.conf.Vars, "detect_release"):
         base = libdnf5.base.Base()
         return libdnf5.conf.Vars.detect_release(base.get_weak_ptr(), "/").get()
     # Fall back to our copy of dnf4's code
     else:  # pragma: no cover
+        _deprecation_warn()
         return _dnf_getreleasever()
 
 
 RepoError = RuntimeError
 
 __all__ = (
     "BACKEND",
```

### Comparing `fedrq-0.8.0/src/fedrq/cli/__init__.py` & `fedrq-0.9.0/src/fedrq/cli/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     import argcomplete
 except ImportError:
     HAS_ARGCOMPLETE = False
 else:
     HAS_ARGCOMPLETE = True
 
 from fedrq.cli.base import CheckConfig, Command
+from fedrq.cli.commands.download import DownloadCommand, DownloadSpecCommand
 from fedrq.cli.commands.pkgs import Pkgs
 from fedrq.cli.commands.repolist import Repolist
 from fedrq.cli.commands.subpkgs import Subpkgs
 from fedrq.cli.commands.whatrequires import (
     WhatCommand,
     Whatenhances,
     Whatobsoletes,
@@ -30,14 +31,16 @@
 )
 
 __all__ = (
     "Command",
     "Pkgs",
     "Repolist",
     "Subpkgs",
+    "DownloadCommand",
+    "DownloadSpecCommand",
     "WhatCommand",
     "Whatenhances",
     "Whatobsoletes",
     "Whatrecommends",
     "Whatrequires",
     "WhatrequiresSrc",
     "Whatsuggests",
@@ -66,14 +69,16 @@
         argcomplete.autocomplete(parser)
     args = parser.parse_args(argv)
     return COMMANDS[args.action](args).run()
 
 
 COMMANDS: dict[str, type[Command]] = {
     "check-config": CheckConfig,
+    "download": DownloadCommand,
+    "download-spec": DownloadSpecCommand,
     "pkgs": Pkgs,
     "subpkgs": Subpkgs,
     "repolist": Repolist,
     "whatenhances": Whatenhances,
     "whatobsoletes": Whatobsoletes,
     "whatrecommends": Whatrecommends,
     "whatrequires": Whatrequires,
```

### Comparing `fedrq-0.8.0/src/fedrq/cli/base.py` & `fedrq-0.9.0/src/fedrq/cli/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -199,14 +199,63 @@
             metavar="REPO",
             # PROVISIONAL
             help=argparse.SUPPRESS,
         )
         return parser
 
     @classmethod
+    def arch_parser(cls) -> argparse.ArgumentParser:
+        parser = argparse.ArgumentParser(add_help=False)
+        arch_group = parser.add_mutually_exclusive_group()
+        arch_group.add_argument(
+            "-A",
+            "--arch",
+            help="Only include packages that match ARCH",
+        )
+        arch_group.add_argument(
+            "-S",
+            "--notsrc",
+            dest="arch",
+            action="store_const",
+            const="notsrc",
+            help="This includes all binary RPMs. Multilib is excluded on x86_64. "
+            "Equivalent to --arch=notsrc",
+        )
+        arch_group.add_argument(
+            "-s",
+            "--src",
+            dest="arch",
+            action="store_const",
+            const="src",
+            help="Query for BuildRequires of NAME. "
+            "This is equivalent to --arch=src.",
+        )
+        return parser
+
+    @classmethod
+    def resolve_parser(cls) -> argparse.ArgumentParser:
+        parser = argparse.ArgumentParser(add_help=False)
+        parser.add_argument(
+            "-P",
+            "--resolve-packages",
+            action="store_true",
+            help="Resolve the correct Package when given a virtual Provide."
+            " For instance, /usr/bin/yt-dlp would resolve to yt-dlp",
+        )
+        return parser
+
+    @classmethod
+    def assume_parser(cls) -> argparse.ArgumentParser:
+        parser = argparse.ArgumentParser(add_help=False)
+        run_parser = parser.add_mutually_exclusive_group()
+        run_parser.add_argument("-y", "--assumeyes", action="store_true")
+        run_parser.add_argument("-n", "--dry-run", action="store_true")
+        return parser
+
+    @classmethod
     def parent_parser(cls) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser(
             add_help=False, parents=[cls.branch_repo_parser()]
         )
         parser.add_argument(  # type: ignore[attr-defined]
             "names", metavar="NAME", nargs="*", help="Mutually exclusive with --stdin"
         ).completer = lambda **_: ()
@@ -256,20 +305,31 @@
         )
         return parser
 
     @classmethod
     @abc.abstractmethod
     def make_parser(
         cls,
-        parser_func: cabc.Callable = argparse.ArgumentParser,
+        parser_func: cabc.Callable[
+            ..., argparse.ArgumentParser
+        ] = argparse.ArgumentParser,
         *,
         add_help: bool = False,
         **kwargs,
     ) -> argparse.ArgumentParser:
-        ...
+        kwargs = {
+            "description": cls.__doc__,
+            "help": cls.__doc__,
+            "parents": [cls.parent_parser()],
+        } | kwargs
+        if not add_help:
+            kwargs.pop("help", None)
+
+        parser = parser_func(**kwargs)
+        return parser
 
     @classmethod
     def standalone(cls, argv: list[str] | None = None) -> None:
         parser = cls.make_parser(add_help=False)
         return cls(args=parser.parse_args(argv)).run()
 
     def get_names(self) -> None:
```

### Comparing `fedrq-0.8.0/src/fedrq/cli/commands/pkgs.py` & `fedrq-0.9.0/src/fedrq/cli/commands/subpkgs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,80 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
+#
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 from __future__ import annotations
 
 import argparse
-from collections import abc as cabc
+from collections.abc import Callable
 
-from fedrq._utils import filter_latest, mklog
-from fedrq.cli import Command
+from fedrq.cli.base import Command, v_add_errors
 
 
-class Pkgs(Command):
+class Subpkgs(Command):
     """
-    Find the packages that match NAMES.
-    NAMES can be package package name globs or NEVRs.
+    For each SRPM name, list the subpackages that it provides
     """
 
     def __init__(self, args: argparse.Namespace) -> None:
         super().__init__(args)
         self.v_default()
 
     @classmethod
     def make_parser(
         cls,
-        parser_func: cabc.Callable = argparse.ArgumentParser,
+        parser_func: Callable = argparse.ArgumentParser,
         *,
         add_help: bool = False,
         **kwargs,
     ) -> argparse.ArgumentParser:
-        kwargs.update(dict(description=Pkgs.__doc__, parents=[cls.parent_parser()]))
-        if add_help:
-            kwargs["help"] = "Find the packages that match a list of package specs"
-        parser = parser_func(**kwargs)
-
+        parser = super().make_parser(
+            parser_func,
+            add_help=add_help,
+            help="Find the subpackages of a list of SRPM",
+            **kwargs,
+        )
         parser.add_argument(
-            "-P",
-            "--resolve-packages",
-            action="store_true",
-            help="Resolve the correct Package when given a virtual Provide."
-            " For instance, /usr/bin/yt-dlp would resolve to yt-dlp",
+            "-M",
+            "--match",
+            action="append",
+            help="Only show subpackages whose name matches this string."
+            " Glob patterns are permitted."
+            " When specified multiple times, _any_ match is included.",
         )
-
         arch_group = parser.add_mutually_exclusive_group()
         arch_group.add_argument(
-            "-A",
-            "--arch",
-            help="Only include packages that match ARCH",
+            "-A", "--arch", help="Only show subpackages with this arch"
         )
         arch_group.add_argument(
             "-S",
             "--notsrc",
             dest="arch",
             action="store_const",
             const="notsrc",
             help="This includes all binary RPMs. Multilib is excluded on x86_64. "
             "Equivalent to --arch=notsrc",
         )
-        arch_group.add_argument(
-            "-s",
-            "--src",
-            dest="arch",
-            action="store_const",
-            const="src",
-            help="Query for BuildRequires of NAME. "
-            "This is equivalent to --arch=src.",
-        )
         return parser
 
     def run(self) -> None:
-        flog = mklog(__name__, self.__class__.__name__, "run")
-        self.query = self.rq.query(empty=True)
-        # flog.debug("self.query = %s", tuple(self.query))
-
-        resolved_packages = self.rq.resolve_pkg_specs(
-            self.args.names, self.args.resolve_packages
+        srpms = self.rq.resolve_pkg_specs(self.args.names, latest=self.args.latest)
+        srpms.filterm(arch="src")
+        self.query = self.rq.get_subpackages(
+            srpms, latest=self.args.latest, arch=self.args.arch
         )
-        self._logq(resolved_packages, "resolved_packages")
-        self.query = self.query.union(resolved_packages)
-
-        glob_packages = self.rq.query(name__glob=self.args.names)
-        self._logq(glob_packages, "glob_packages")
-        self.query = self.query.union(glob_packages)
-
-        self.query = self.rq.arch_filter(self.query, self.args.arch)
-        filter_latest(self.query, self.args.latest)
-        flog.debug("self.query = %s", tuple(self.query))
-
+        if self.args.match:
+            self.query.filterm(name__glob=self.args.match)
         for p in self.format():
             print(p)
+
+    @v_add_errors
+    def v_arch(self) -> str | None:
+        if super().v_arch():
+            return None
+        if (
+            self.args.arch
+            and "src" in self.args.arch
+            and "notsrc" not in self.args.arch
+        ):
+            return "Illegal option '--arch=src': Subpackages are binary RPMs"
+        return None
```

### Comparing `fedrq-0.8.0/src/fedrq/cli/commands/repolist.py` & `fedrq-0.9.0/src/fedrq/cli/commands/repolist.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,20 +32,17 @@
     def make_parser(
         cls,
         parser_func: cabc.Callable = argparse.ArgumentParser,
         *,
         add_help: bool = False,
         **kwargs,
     ) -> argparse.ArgumentParser:
-        kwargs["description"] = cls.__doc__
-        kwargs["parents"] = [cls.branch_repo_parser()]
-        if add_help:
-            kwargs["help"] = cls.__doc__
-
-        parser: argparse.ArgumentParser = parser_func(**kwargs)
+        parser: argparse.ArgumentParser = super().make_parser(
+            parser_func, add_help=add_help, parents=[cls.branch_repo_parser()], **kwargs
+        )
         parser.add_argument("--debug", action="store_true")
         parser.add_argument("--all", action="store_true")
         return parser
 
     def run(self) -> None:
         bm = self.backend.BaseMaker()
         self.release.make_base(self.config, base_maker=bm, fill_sack=False)
```

### Comparing `fedrq-0.8.0/src/fedrq/cli/commands/whatrequires.py` & `fedrq-0.9.0/src/fedrq/cli/commands/whatrequires.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,18 +66,21 @@
     def make_parser(
         cls,
         parser_func: cabc.Callable = argparse.ArgumentParser,
         *,
         add_help: bool = False,
         **kwargs,
     ) -> argparse.ArgumentParser:
-        pargs = dict(description=cls.__doc__, parents=[cls.parent_parser()], **kwargs)
-        if add_help:
-            pargs["help"] = f"Find reverse {cls.operator.title()} of a list of packages"
-        parser = parser_func(**pargs)
+        parser = super().make_parser(
+            parser_func,
+            add_help=add_help,
+            help=f"Find reverse {cls.operator.title()} of a list of packages",
+            parents=[cls.parent_parser(), cls.arch_parser()],
+            **kwargs,
+        )
 
         _rp_help = f"""
         Resolve the correct Package when given a virtual Provide. For instance,
         /usr/bin/yt-dlp would resolve to yt-dlp, and then any package that
         {cls.operator} python3dist(yt-dlp) would also be included.
         """
         resolve_group = parser.add_mutually_exclusive_group()
@@ -88,39 +91,14 @@
             "-E",
             "--exact",
             action="store_true",
             help="This is the opposite extreme to --resolve-packages. "
             "E.g., yt-dlp would not match python3dist(yt-dlp) like it does by default.",
         )
 
-        arch_group = parser.add_mutually_exclusive_group()
-        arch_group.add_argument(
-            "-A",
-            "--arch",
-            help=f"After finding the packages that {cls._operator} NAMES, "
-            "filter out the resulting packages that don't match ARCH",
-        )
-        arch_group.add_argument(
-            "-S",
-            "--notsrc",
-            dest="arch",
-            action="store_const",
-            const="notsrc",
-            help="This includes all binary RPMs. Multilib is excluded on x86_64. "
-            "Equivalent to --arch=notsrc",
-        )
-        arch_group.add_argument(
-            "-s",
-            "--src",
-            dest="arch",
-            action="store_const",
-            const="src",
-            help="Query for BuildRequires of NAME. "
-            "This is equivalent to --arch=src.",
-        )
         if cls._exclude_subpackages_opt:
             parser.add_argument("-X", "--exclude-subpackages", action="store_true")
         return parser
 
     def exclude_subpackages(self, rpms: t.Optional[PackageQueryCompat]) -> None:
         import re
```

### Comparing `fedrq-0.8.0/src/fedrq/cli/formatters.py` & `fedrq-0.9.0/src/fedrq/cli/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,14 +411,18 @@
             else:
                 out += attr.format_line(package)
             if index != len(self.attrs) - 1:
                 out += self.divider
         return out
 
 
+def remote_location(_, package: PackageCompat) -> str:
+    return _stringify(package.remote_location())
+
+
 class _DefaultFormatters(Formatters):
     def __call__(self) -> Any:
         warnings.warn(
             "DEPRECATED since 0.4.0: DefaultFormatters no longer needs to be called."
             " It's already initialized."
             " Just call DefaultFormatters.get_formatter() directly."
         )
@@ -437,10 +441,11 @@
         full_nevra="{0.name}-{0.evr}.{0.arch}",
         nv="{0.name}-{0.version}",
         source=SourceFromatter,
         src=SourceFromatter,
         attr=AttrFormatter,
         json=JsonFormatter,
         line=SingleLineFormatter,
+        remote_location=remote_location,
     ),
     AttrFallbackFormatter,
 )
```

### Comparing `fedrq-0.8.0/src/fedrq/config.py` & `fedrq-0.9.0/src/fedrq/config.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/releases.toml` & `fedrq-0.9.0/src/fedrq/data/releases.toml`

 * *Files 26% similar despite different names*

```diff
@@ -233,14 +233,140 @@
 defs.no-powertools = [
     "almalinux-appstream",
     "almalinux-appstream-source",
     "almalinux-baseos",
     "almalinux-baseos-source",
 ]
 
+
+[releases.rocky]
+matcher = '^rl(9|1\d)$'
+copr_chroot_fmt = "epel-{version}"
+defpaths = [
+    "rocky.repo",
+    "epel.repo",
+]
+defs.no-crb = [
+    "rocky-appstream",
+    "rocky-appstream-source",
+    "rocky-baseos",
+    "rocky-baseos-source",
+]
+defs.base = [
+    "@no-crb",
+    "rocky-crb",
+    "rocky-crb-source",
+]
+defs.epel = [
+    "@base",
+    "@repo:epel",
+    "epel-source",
+]
+
+[releases.rocky8]
+matcher = '^rl(8)$'
+copr_chroot_fmt = "epel-{version}"
+defpaths = [
+    "rocky.repo",
+    "epel.repo",
+]
+defs.no-powertools = [
+    "rocky-appstream",
+    "rocky-appstream-source",
+    "rocky-baseos",
+    "rocky-baseos-source",
+]
+defs.base = [
+    "@no-powertools",
+    "rocky8-powertools",
+    "rocky8-powertools-source",
+]
+defs.epel = [
+    "@base",
+    "@repo:epel",
+    "epel-source",
+]
+
+[releases.ubi]
+matcher = '^ubi(\d+)$'
+copr_chroot_fmt = "epel-{version}"
+defpaths = [
+    "ubi.repo",
+    "epel.repo",
+]
+defs.no-crb = [
+    "ubi-baseos-rpms",
+    "ubi-baseos-source",
+    "ubi-appstream-rpms",
+    "ubi-appstream-source",
+]
+defs.base = [
+    "@no-crb",
+    "ubi-codeready-builder-rpms",
+    "ubi-codeready-builder-source",
+]
+defs.epel = [
+    "@base",
+    "@repo:epel",
+    "epel-source",
+]
+
+[releases.oracle8]
+matcher = "^ol(8)$"
+copr_chroot_fmt = "epel-{version}"
+defpaths = [
+    "oraclelinux-8.repo",
+    "epel.repo",
+]
+defs.no-crb = [
+    "ol8_baseos_latest",
+    "ol8_appstream",
+]
+defs.base = [
+    "@no-crb",
+    "ol8_codeready_builder",
+]
+defs.extra = [
+    "@base",
+    "ol8_distro_builder",
+    "ol8_UEKR6",
+]
+defs.epel = [
+    "@base",
+    "@repo:epel",
+    "epel-source",
+]
+
+[releases.oracle9]
+matcher = "^ol(9)$"
+copr_chroot_fmt = "epel-{version}"
+defpaths = [
+    "oraclelinux-9.repo",
+    "epel.repo",
+]
+defs.no-crb = [
+    "ol9_baseos_latest",
+    "ol9_appstream",
+]
+defs.base = [
+    "@no-crb",
+    "ol9_codeready_builder",
+]
+defs.extra = [
+    "@base",
+    "ol9_distro_builder",
+    "ol9_UEKR7",
+]
+defs.epel = [
+    "@base",
+    "@repo:epel",
+    "epel-source",
+]
+
+
 [releases.eln]
 matcher = "^(eln)$"
 defpaths = [
     "fedora-eln.repo",
 ]
 defs.no-crb = [
     "eln-baseos",
```

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/almalinux.repo` & `fedrq-0.9.0/src/fedrq/data/repos/almalinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/amazonlinux.repo` & `fedrq-0.9.0/src/fedrq/data/repos/amazonlinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/centos-stream-compose.repo` & `fedrq-0.9.0/src/fedrq/data/repos/centos-stream-compose.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/centos-stream.repo` & `fedrq-0.9.0/src/fedrq/data/repos/centos-stream.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/centos-stream8-compose.repo` & `fedrq-0.9.0/src/fedrq/data/repos/centos-stream8-compose.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/centos-stream8.repo` & `fedrq-0.9.0/src/fedrq/data/repos/centos-stream8.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/centos7.repo` & `fedrq-0.9.0/src/fedrq/data/repos/centos7.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/eln.repo` & `fedrq-0.9.0/src/fedrq/data/repos/eln.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/epel.repo` & `fedrq-0.9.0/src/fedrq/data/repos/epel.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/fedora-eln.repo` & `fedrq-0.9.0/src/fedrq/data/repos/fedora-eln.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/fedora-rawhide.repo` & `fedrq-0.9.0/src/fedrq/data/repos/fedora-rawhide.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/fedora-updates-testing.repo` & `fedrq-0.9.0/src/fedrq/data/repos/fedora-updates-testing.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/fedora-updates.repo` & `fedrq-0.9.0/src/fedrq/data/repos/fedora-updates.repo`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 [updates]
 name=Fedora $releasever - $basearch - Updates
 #baseurl=http://download.example/pub/fedora/linux/updates/$releasever/Everything/$basearch/
 metalink=https://mirrors.fedoraproject.org/metalink?repo=updates-released-f$releasever&arch=$basearch
-enabled=1
+enabled=0
 repo_gpgcheck=0
 type=rpm
 gpgcheck=1
 metadata_expire=6h
 gpgkey=file:///usr/share/distribution-gpg-keys/fedora/RPM-GPG-KEY-fedora-$releasever-primary
 skip_if_unavailable=False
```

### Comparing `fedrq-0.8.0/src/fedrq/data/repos/fedora.repo` & `fedrq-0.9.0/src/fedrq/data/repos/fedora.repo`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 [fedora]
 name=Fedora $releasever - $basearch
 #baseurl=http://download.example/pub/fedora/linux/releases/$releasever/Everything/$basearch/os/
 metalink=https://mirrors.fedoraproject.org/metalink?repo=fedora-$releasever&arch=$basearch
-enabled=1
+enabled=0
 metadata_expire=7d
 repo_gpgcheck=0
 type=rpm
 gpgcheck=1
 gpgkey=file:///usr/share/distribution-gpg-keys/fedora/RPM-GPG-KEY-fedora-$releasever-primary
 skip_if_unavailable=False
```

### Comparing `fedrq-0.8.0/src/fedrq/release_repo.py` & `fedrq-0.9.0/src/fedrq/release_repo.py`

 * *Files 7% similar despite different names*

```diff
@@ -110,21 +110,26 @@
     ) -> None:
         try:
             base_maker.enable_repo(self.args)
         except ValueError:
             self.err(f"No repo named {self.args}", None)
 
 
-class MultiNameG(RepoG):
+class _NoArgRepoG(RepoG):
+    def validate(self):
+        if self.args:
+            raise ConfigError("No arguments are accepted")
+
+
+class MultiNameG(_NoArgRepoG):
     repos: Sequence[str] = ()
     repogs: list[RepoG]
 
     def validate(self):
-        if self.args:
-            raise ConfigError("No arguments are accepted")
+        super().validate()
         self.repogs = [self.container.get_repo(repo) for repo in self.repos]
 
     def load(
         self, base_maker: BaseMakerBase, config: RQConfig, release: Release
     ) -> None:
         for repog in self.repogs:
             repog.load(base_maker, config, release)
@@ -222,14 +227,21 @@
 
 
 class MirrorlistRepoG(BaseurlRepoG):
     _ATTR = "mirrorlist"
     _COERCE_TO_LIST = False
 
 
+class SourceRepoG(_NoArgRepoG):
+    def load(
+        self, base_maker: BaseMakerBase, config: RQConfig, release: Release
+    ) -> None:
+        base_maker.enable_source_repos()
+
+
 class Repos(Mapping[str, type[RepoG]]):
     """
     Immutable mapping like class of RepoG types.
     Converts repo aliases (strings) and list of repos in RepoG objects.
     Allows merging and adding other Repos objects.
     """
 
@@ -296,15 +308,16 @@
         return self.__data.values()
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.__data!r})"
 
 
 DefaultRepoGs = Repos(
-    dict(
-        file=FileRepoG,
-        copr=CoprRepoG,
-        repo=SimpleRepoG,
-        baseurl=BaseurlRepoG,
-        mirrorlist=MirrorlistRepoG,
-    )
+    {
+        "file": FileRepoG,
+        "copr": CoprRepoG,
+        "repo": SimpleRepoG,
+        "baseurl": BaseurlRepoG,
+        "mirrorlist": MirrorlistRepoG,
+        "source-repos": SourceRepoG,
+    }
 )
```

### Comparing `fedrq-0.8.0/src/fedrq/repoquery.py` & `fedrq-0.9.0/src/fedrq/repoquery.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/conftest.py` & `fedrq-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/integration/test_backends.py` & `fedrq-0.9.0/tests/integration/test_backends.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/integration/test_pkgs.py` & `fedrq-0.9.0/tests/integration/test_pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/integration/test_subpkgs.py` & `fedrq-0.9.0/tests/integration/test_subpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/integration/test_whatrequires.py` & `fedrq-0.9.0/tests/integration/test_whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/integration/test_whatrequires_src.py` & `fedrq-0.9.0/tests/integration/test_whatrequires_src.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/test_data/build.sh` & `fedrq-0.9.0/tests/test_data/build.sh`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/test_data/repos/repo1/specs/e1/packageb.spec` & `fedrq-0.9.0/tests/test_data/repos/repo1/specs/e1/packageb.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/test_data/repos/repo1/specs/packagea.spec` & `fedrq-0.9.0/tests/test_data/repos/repo1/specs/packagea.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/test_data/repos/repo1/specs/packageb.spec` & `fedrq-0.9.0/tests/test_data/repos/repo1/specs/packageb.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/unit/test_checkconfig.py` & `fedrq-0.9.0/tests/unit/test_checkconfig.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/unit/test_command.py` & `fedrq-0.9.0/tests/unit/test_command.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/unit/test_formatters.py` & `fedrq-0.9.0/tests/unit/test_formatters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 from __future__ import annotations
 
 import json
+from collections.abc import Callable, Collection
 from functools import cache
+from pathlib import Path
 
 import pytest
 
 from fedrq import config as rqconfig
 from fedrq.cli import formatters
 
 
@@ -188,14 +190,64 @@
 def test_repo_files_formatter(patch_config_dirs):
     repo_test_rq = get_rq()
     query = repo_test_rq.query(name=["packagea", "packageb"], arch="notsrc", latest=1)
     result = formatter(query, "files", attr=True)
     assert result == ["/usr/share/packagea", "/usr/share/packageb"]
 
 
+@pytest.mark.parametrize(
+    "args, expected_call",
+    [
+        pytest.param([], lambda x: x),
+        pytest.param([None], lambda x: x),
+        pytest.param([{"file"}], lambda x: x),
+        pytest.param([{"ftp"}], lambda _: None),
+    ],
+)
+def test_remote_location(
+    patch_config_dirs,
+    data_path: Path,
+    args: list[Collection[str] | None],
+    expected_call: Callable[[str], str | None],
+):
+    path = (
+        data_path
+        / "repos"
+        / "repo1"
+        / "repo"
+        / "SRPMS"
+        / "specs"
+        / "packagea-1-1.fc36.src.rpm"
+    )
+    expected = expected_call(f"file://{path}")
+
+    repo_test_rq = get_rq()
+    package = repo_test_rq.get_package("packagea", "src")
+    result = package.remote_location(*args)
+    assert result == expected
+
+
+def test_formatter_remote_location(patch_config_dirs, data_path: Path):
+    path = (
+        data_path
+        / "repos"
+        / "repo1"
+        / "repo"
+        / "SRPMS"
+        / "specs"
+        / "packagea-1-1.fc36.src.rpm"
+    )
+    expected = f"file://{path}"
+
+    repo_test_rq = get_rq()
+    package = repo_test_rq.get_package("packagea", "src")
+    result = formatter([package], "remote_location")
+    assert result == [expected]
+
+
 @pytest.mark.parametrize("attr", formatters._ATTRS)
 def test_formatter_sanity(patch_config_dirs, attr):
     """
     Sanity test to ensure that supported formatters work at all
     """
     repo_test_rq = get_rq()
     query = repo_test_rq.query(
```

### Comparing `fedrq-0.8.0/tests/unit/test_pkgs.py` & `fedrq-0.9.0/tests/unit/test_pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/unit/test_release.py` & `fedrq-0.9.0/tests/unit/test_release.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/unit/test_repolist.py` & `fedrq-0.9.0/tests/unit/test_repolist.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/unit/test_repoquery.py` & `fedrq-0.9.0/tests/unit/test_repoquery.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/unit/test_subbpkgs.py` & `fedrq-0.9.0/tests/unit/test_subbpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/unit/test_whatrequires.py` & `fedrq-0.9.0/tests/unit/test_whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/tests/unit/test_whatrequires_src.py` & `fedrq-0.9.0/tests/unit/test_whatrequires_src.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.8.0/PKG-INFO` & `fedrq-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedrq
-Version: 0.8.0
+Version: 0.9.0
 Summary: fedrq is a tool to query the Fedora and EPEL repositories
 Author-email: Maxwell G <gotmax@e.email>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -118,14 +118,27 @@
 Note that fedrq can only be installed for the system python interpreter.
 fedrq cannot be installed in a venv unless it has `--system-site-packages`,
 as it needs to find the aforementioned system bindings.
 
 `fedrq check-config --dump` requires `tomli-w`.
 The RPM package weakly depends on `python3-tomli-w`.
 
+## Container images
+
+fedrq now provides container images.
+- `quay.io/gotmax23/fedrq:latest` is built with
+  `registry.fedoraproject.org/fedora:latest`.
+- `quay.io/gotmax23/fedrq:ubi9` is built with the ubi9 image.
+  It includes a builtin `rhel9` repository configuration that can be used to
+  query the actual RHEL repositories when run on a system registered with
+  subscription-manager.
+
+Both of these images use the latest fedrq RPM packages from the
+[gotmax23/fedrq][link-copr] Copr repository.
+
 ## Versioning
 
 This project is in beta and its versioning scheme follows semver.
 
 See [NEWS.md](https://git.sr.ht/~gotmax23/fedrq/tree/main/NEWS.md).
 
 ## Python API
```

