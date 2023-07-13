# Comparing `tmp/aicrowd-repo2docker-0.9.0.tar.gz` & `tmp/aicrowd-repo2docker-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aicrowd-repo2docker-0.9.0.tar", last modified: Thu Jun 13 01:58:06 2019, max compression
+gzip compressed data, was "dist/aicrowd-repo2docker-0.9.1.tar", last modified: Thu Jun 13 22:50:25 2019, max compression
```

## Comparing `aicrowd-repo2docker-0.9.0.tar` & `aicrowd-repo2docker-0.9.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/
--rw-r--r--   0 skbly7     (501) staff       (20)     4898 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/PKG-INFO
--rw-r--r--   0 skbly7     (501) staff       (20)     1528 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.0/LICENSE
-drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/repo2docker/
-drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/repo2docker/contentproviders/
--rw-r--r--   0 skbly7     (501) staff       (20)     2614 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/contentproviders/git.py
--rw-r--r--   0 skbly7     (501) staff       (20)       45 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/contentproviders/__init__.py
--rw-r--r--   0 skbly7     (501) staff       (20)     2863 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/contentproviders/base.py
--rw-r--r--   0 skbly7     (501) staff       (20)      497 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/repo2docker/_version.py
--rw-r--r--   0 skbly7     (501) staff       (20)       92 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/__init__.py
-drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/
-drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/nix/
--rw-r--r--   0 skbly7     (501) staff       (20)      533 2019-06-13 01:36:43.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/nix/install-nix.bash
--rw-r--r--   0 skbly7     (501) staff       (20)     2710 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/nix/__init__.py
--rw-r--r--   0 skbly7     (501) staff       (20)     1281 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/nix/nix-shell-wrapper
--rw-r--r--   0 skbly7     (501) staff       (20)    11582 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/r.py
-drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/python/
--rw-r--r--   0 skbly7     (501) staff       (20)     3627 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/python/__init__.py
-drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/
--rw-r--r--   0 skbly7     (501) staff       (20)     2326 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.frozen.yml
--rwxr-xr-x   0 skbly7     (501) staff       (20)      427 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/activate-conda.sh
--rw-r--r--   0 skbly7     (501) staff       (20)     2299 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-3.6.frozen.yml
--rw-r--r--   0 skbly7     (501) staff       (20)       48 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-2.7.yml
--rw-r--r--   0 skbly7     (501) staff       (20)      183 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.yml
--rw-r--r--   0 skbly7     (501) staff       (20)     7097 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/__init__.py
--rw-r--r--   0 skbly7     (501) staff       (20)      107 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-3.5.yml
--rw-r--r--   0 skbly7     (501) staff       (20)      268 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-3.7.yml
--rw-r--r--   0 skbly7     (501) staff       (20)      268 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-3.6.yml
--rw-r--r--   0 skbly7     (501) staff       (20)     1510 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-2.7.frozen.yml
--rw-r--r--   0 skbly7     (501) staff       (20)     2326 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-3.7.frozen.yml
--rwxr-xr-x   0 skbly7     (501) staff       (20)     3761 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/freeze.py
--rw-r--r--   0 skbly7     (501) staff       (20)     2330 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-3.5.frozen.yml
--rwxr-xr-x   0 skbly7     (501) staff       (20)     2481 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/install-miniconda.bash
--rwxr-xr-x   0 skbly7     (501) staff       (20)      284 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/repo2docker-entrypoint
-drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/
--rw-r--r--   0 skbly7     (501) staff       (20)      100 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/apt-sources.list
--rw-r--r--   0 skbly7     (501) staff       (20)       68 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/python3.yml
--rw-r--r--   0 skbly7     (501) staff       (20)     4578 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/root.frozen.yml
--rw-r--r--   0 skbly7     (501) staff       (20)     4685 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/__init__.py
--rw-r--r--   0 skbly7     (501) staff       (20)       48 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/root.yml
--rw-r--r--   0 skbly7     (501) staff       (20)     4889 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/python3.frozen.yml
--rwxr-xr-x   0 skbly7     (501) staff       (20)     1847 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/freeze.py
--rw-r--r--   0 skbly7     (501) staff       (20)      335 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/__init__.py
--rw-r--r--   0 skbly7     (501) staff       (20)     1463 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/docker.py
-drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/julia/
--rw-r--r--   0 skbly7     (501) staff       (20)     5093 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/julia/semver.py
--rw-r--r--   0 skbly7     (501) staff       (20)     5306 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/julia/julia_project.py
--rw-r--r--   0 skbly7     (501) staff       (20)      102 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/julia/__init__.py
--rw-r--r--   0 skbly7     (501) staff       (20)     6661 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/julia/julia_require.py
--rw-r--r--   0 skbly7     (501) staff       (20)      979 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/julia/install-repo-dependencies.jl
--rw-r--r--   0 skbly7     (501) staff       (20)    22310 2019-06-13 01:53:31.000000 aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/base.py
--rw-r--r--   0 skbly7     (501) staff       (20)     8946 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/utils.py
--rw-r--r--   0 skbly7     (501) staff       (20)    22959 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/app.py
--rw-r--r--   0 skbly7     (501) staff       (20)     9718 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/repo2docker/__main__.py
--rw-r--r--   0 skbly7     (501) staff       (20)      144 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.0/MANIFEST.in
--rw-r--r--   0 skbly7     (501) staff       (20)     3217 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/README.md
-drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/aicrowd_repo2docker.egg-info/
--rw-r--r--   0 skbly7     (501) staff       (20)     4898 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/aicrowd_repo2docker.egg-info/PKG-INFO
--rw-r--r--   0 skbly7     (501) staff       (20)     2173 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/aicrowd_repo2docker.egg-info/SOURCES.txt
--rw-r--r--   0 skbly7     (501) staff       (20)       67 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/aicrowd_repo2docker.egg-info/entry_points.txt
--rw-r--r--   0 skbly7     (501) staff       (20)       82 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/aicrowd_repo2docker.egg-info/requires.txt
--rw-r--r--   0 skbly7     (501) staff       (20)       12 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/aicrowd_repo2docker.egg-info/top_level.txt
--rw-r--r--   0 skbly7     (501) staff       (20)        1 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/aicrowd_repo2docker.egg-info/dependency_links.txt
--rw-r--r--   0 skbly7     (501) staff       (20)     1826 2019-06-13 01:53:09.000000 aicrowd-repo2docker-0.9.0/setup.py
--rw-r--r--   0 skbly7     (501) staff       (20)      181 2019-06-13 01:36:43.000000 aicrowd-repo2docker-0.9.0/ROADMAP.md
--rw-r--r--   0 skbly7     (501) staff       (20)     2358 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 skbly7     (501) staff       (20)      270 2019-06-13 01:58:06.000000 aicrowd-repo2docker-0.9.0/setup.cfg
--rw-r--r--   0 skbly7     (501) staff       (20)    68611 2019-06-13 01:46:00.000000 aicrowd-repo2docker-0.9.0/versioneer.py
+drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/
+-rw-r--r--   0 skbly7     (501) staff       (20)     4898 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/PKG-INFO
+-rw-r--r--   0 skbly7     (501) staff       (20)     1528 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.1/LICENSE
+drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/repo2docker/
+drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/repo2docker/contentproviders/
+-rw-r--r--   0 skbly7     (501) staff       (20)     2614 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/contentproviders/git.py
+-rw-r--r--   0 skbly7     (501) staff       (20)       45 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/contentproviders/__init__.py
+-rw-r--r--   0 skbly7     (501) staff       (20)     2863 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/contentproviders/base.py
+-rw-r--r--   0 skbly7     (501) staff       (20)      497 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/repo2docker/_version.py
+-rw-r--r--   0 skbly7     (501) staff       (20)       92 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/__init__.py
+drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/
+drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/nix/
+-rw-r--r--   0 skbly7     (501) staff       (20)      533 2019-06-13 01:36:43.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/nix/install-nix.bash
+-rw-r--r--   0 skbly7     (501) staff       (20)     2710 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/nix/__init__.py
+-rw-r--r--   0 skbly7     (501) staff       (20)     1281 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/nix/nix-shell-wrapper
+-rw-r--r--   0 skbly7     (501) staff       (20)    11582 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/r.py
+drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/python/
+-rw-r--r--   0 skbly7     (501) staff       (20)     3627 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/python/__init__.py
+drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/
+-rw-r--r--   0 skbly7     (501) staff       (20)     2326 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.frozen.yml
+-rwxr-xr-x   0 skbly7     (501) staff       (20)      427 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/activate-conda.sh
+-rw-r--r--   0 skbly7     (501) staff       (20)     2299 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-3.6.frozen.yml
+-rw-r--r--   0 skbly7     (501) staff       (20)       48 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-2.7.yml
+-rw-r--r--   0 skbly7     (501) staff       (20)      183 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.yml
+-rw-r--r--   0 skbly7     (501) staff       (20)     7097 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/__init__.py
+-rw-r--r--   0 skbly7     (501) staff       (20)      107 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-3.5.yml
+-rw-r--r--   0 skbly7     (501) staff       (20)      268 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-3.7.yml
+-rw-r--r--   0 skbly7     (501) staff       (20)      268 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-3.6.yml
+-rw-r--r--   0 skbly7     (501) staff       (20)     1510 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-2.7.frozen.yml
+-rw-r--r--   0 skbly7     (501) staff       (20)     2326 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-3.7.frozen.yml
+-rwxr-xr-x   0 skbly7     (501) staff       (20)     3761 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/freeze.py
+-rw-r--r--   0 skbly7     (501) staff       (20)     2330 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-3.5.frozen.yml
+-rwxr-xr-x   0 skbly7     (501) staff       (20)     2481 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/install-miniconda.bash
+-rwxr-xr-x   0 skbly7     (501) staff       (20)      284 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/repo2docker-entrypoint
+drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/
+-rw-r--r--   0 skbly7     (501) staff       (20)      100 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/apt-sources.list
+-rw-r--r--   0 skbly7     (501) staff       (20)       68 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/python3.yml
+-rw-r--r--   0 skbly7     (501) staff       (20)     4578 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/root.frozen.yml
+-rw-r--r--   0 skbly7     (501) staff       (20)     4685 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/__init__.py
+-rw-r--r--   0 skbly7     (501) staff       (20)       48 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/root.yml
+-rw-r--r--   0 skbly7     (501) staff       (20)     4889 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/python3.frozen.yml
+-rwxr-xr-x   0 skbly7     (501) staff       (20)     1847 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/freeze.py
+-rw-r--r--   0 skbly7     (501) staff       (20)      335 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/__init__.py
+-rw-r--r--   0 skbly7     (501) staff       (20)     1463 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/docker.py
+drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/julia/
+-rw-r--r--   0 skbly7     (501) staff       (20)     5093 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/julia/semver.py
+-rw-r--r--   0 skbly7     (501) staff       (20)     5306 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/julia/julia_project.py
+-rw-r--r--   0 skbly7     (501) staff       (20)      102 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/julia/__init__.py
+-rw-r--r--   0 skbly7     (501) staff       (20)     6661 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/julia/julia_require.py
+-rw-r--r--   0 skbly7     (501) staff       (20)      979 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/julia/install-repo-dependencies.jl
+-rw-r--r--   0 skbly7     (501) staff       (20)    22310 2019-06-13 22:47:42.000000 aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/base.py
+-rw-r--r--   0 skbly7     (501) staff       (20)     8946 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/utils.py
+-rw-r--r--   0 skbly7     (501) staff       (20)    22959 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/app.py
+-rw-r--r--   0 skbly7     (501) staff       (20)     9718 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/repo2docker/__main__.py
+-rw-r--r--   0 skbly7     (501) staff       (20)      144 2019-06-13 01:34:40.000000 aicrowd-repo2docker-0.9.1/MANIFEST.in
+-rw-r--r--   0 skbly7     (501) staff       (20)     3217 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/README.md
+drwxr-xr-x   0 skbly7     (501) staff       (20)        0 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/aicrowd_repo2docker.egg-info/
+-rw-r--r--   0 skbly7     (501) staff       (20)     4898 2019-06-13 22:50:24.000000 aicrowd-repo2docker-0.9.1/aicrowd_repo2docker.egg-info/PKG-INFO
+-rw-r--r--   0 skbly7     (501) staff       (20)     2173 2019-06-13 22:50:24.000000 aicrowd-repo2docker-0.9.1/aicrowd_repo2docker.egg-info/SOURCES.txt
+-rw-r--r--   0 skbly7     (501) staff       (20)       67 2019-06-13 22:50:24.000000 aicrowd-repo2docker-0.9.1/aicrowd_repo2docker.egg-info/entry_points.txt
+-rw-r--r--   0 skbly7     (501) staff       (20)       82 2019-06-13 22:50:24.000000 aicrowd-repo2docker-0.9.1/aicrowd_repo2docker.egg-info/requires.txt
+-rw-r--r--   0 skbly7     (501) staff       (20)       12 2019-06-13 22:50:24.000000 aicrowd-repo2docker-0.9.1/aicrowd_repo2docker.egg-info/top_level.txt
+-rw-r--r--   0 skbly7     (501) staff       (20)        1 2019-06-13 22:50:24.000000 aicrowd-repo2docker-0.9.1/aicrowd_repo2docker.egg-info/dependency_links.txt
+-rw-r--r--   0 skbly7     (501) staff       (20)     1826 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/setup.py
+-rw-r--r--   0 skbly7     (501) staff       (20)      181 2019-06-13 01:36:43.000000 aicrowd-repo2docker-0.9.1/ROADMAP.md
+-rw-r--r--   0 skbly7     (501) staff       (20)     2358 2019-06-13 01:38:02.000000 aicrowd-repo2docker-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 skbly7     (501) staff       (20)      270 2019-06-13 22:50:25.000000 aicrowd-repo2docker-0.9.1/setup.cfg
+-rw-r--r--   0 skbly7     (501) staff       (20)    68611 2019-06-13 22:40:08.000000 aicrowd-repo2docker-0.9.1/versioneer.py
```

### Comparing `aicrowd-repo2docker-0.9.0/PKG-INFO` & `aicrowd-repo2docker-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicrowd-repo2docker
-Version: 0.9.0
+Version: 0.9.1
 Summary: Repo2docker: Turn code repositories into Jupyter enabled Docker Images
 Home-page: https://repo2docker.readthedocs.io/en/latest/
 Author: Project Jupyter Contributors
 Author-email: jupyter@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://repo2docker.readthedocs.io
 Project-URL: Funding, https://jupyter.org/about
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aicrowd-repo2docker Version: 0.9.0 Summary:
+Metadata-Version: 2.1 Name: aicrowd-repo2docker Version: 0.9.1 Summary:
 Repo2docker: Turn code repositories into Jupyter enabled Docker Images Home-
 page: https://repo2docker.readthedocs.io/en/latest/ Author: Project Jupyter
 Contributors Author-email: jupyter@googlegroups.com License: BSD Project-URL:
 Documentation, https://repo2docker.readthedocs.io Project-URL: Funding, https:/
 /jupyter.org/about Project-URL: Source, https://github.com/jupyter/repo2docker/
 Project-URL: Tracker, https://github.com/jupyter/repo2docker/issues
 Description: # [https://raw.githubusercontent.com/jupyter/repo2docker/
```

### Comparing `aicrowd-repo2docker-0.9.0/LICENSE` & `aicrowd-repo2docker-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/contentproviders/git.py` & `aicrowd-repo2docker-0.9.1/repo2docker/contentproviders/git.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/contentproviders/base.py` & `aicrowd-repo2docker-0.9.1/repo2docker/contentproviders/base.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/nix/install-nix.bash` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/nix/install-nix.bash`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/nix/__init__.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/nix/__init__.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/nix/nix-shell-wrapper` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/nix/nix-shell-wrapper`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/r.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/r.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/python/__init__.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/python/__init__.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.frozen.yml` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.frozen.yml`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-3.6.frozen.yml` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-3.6.frozen.yml`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/__init__.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-2.7.frozen.yml` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-2.7.frozen.yml`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-3.7.frozen.yml` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-3.7.frozen.yml`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/freeze.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/freeze.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/environment.py-3.5.frozen.yml` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/environment.py-3.5.frozen.yml`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/conda/install-miniconda.bash` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/conda/install-miniconda.bash`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/root.frozen.yml` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/root.frozen.yml`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/__init__.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/python3.frozen.yml` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/python3.frozen.yml`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/legacy/freeze.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/legacy/freeze.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/docker.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/docker.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/julia/semver.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/julia/semver.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/julia/julia_project.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/julia/julia_project.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/julia/julia_require.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/julia/julia_require.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/julia/install-repo-dependencies.jl` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/julia/install-repo-dependencies.jl`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/buildpacks/base.py` & `aicrowd-repo2docker-0.9.1/repo2docker/buildpacks/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import docker
 import sys
 import xml.etree.ElementTree as ET
 
 from traitlets import Dict
 
 TEMPLATE = r"""
-FROM nvidia/cuda:10.1-cudnn7-runtime-ubuntu18.04
+FROM nvidia/cuda:10.0-cudnn7-runtime-ubuntu18.04
 
 # avoid prompts from apt
 ENV DEBIAN_FRONTEND=noninteractive
 
 # Set up locales properly
 RUN apt-get -qq update && \
     apt-get -qq install --yes --no-install-recommends locales wget bzip2 > /dev/null && \
```

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/utils.py` & `aicrowd-repo2docker-0.9.1/repo2docker/utils.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/app.py` & `aicrowd-repo2docker-0.9.1/repo2docker/app.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/repo2docker/__main__.py` & `aicrowd-repo2docker-0.9.1/repo2docker/__main__.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/README.md` & `aicrowd-repo2docker-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/aicrowd_repo2docker.egg-info/PKG-INFO` & `aicrowd-repo2docker-0.9.1/aicrowd_repo2docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicrowd-repo2docker
-Version: 0.9.0
+Version: 0.9.1
 Summary: Repo2docker: Turn code repositories into Jupyter enabled Docker Images
 Home-page: https://repo2docker.readthedocs.io/en/latest/
 Author: Project Jupyter Contributors
 Author-email: jupyter@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://repo2docker.readthedocs.io
 Project-URL: Funding, https://jupyter.org/about
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aicrowd-repo2docker Version: 0.9.0 Summary:
+Metadata-Version: 2.1 Name: aicrowd-repo2docker Version: 0.9.1 Summary:
 Repo2docker: Turn code repositories into Jupyter enabled Docker Images Home-
 page: https://repo2docker.readthedocs.io/en/latest/ Author: Project Jupyter
 Contributors Author-email: jupyter@googlegroups.com License: BSD Project-URL:
 Documentation, https://repo2docker.readthedocs.io Project-URL: Funding, https:/
 /jupyter.org/about Project-URL: Source, https://github.com/jupyter/repo2docker/
 Project-URL: Tracker, https://github.com/jupyter/repo2docker/issues
 Description: # [https://raw.githubusercontent.com/jupyter/repo2docker/
```

### Comparing `aicrowd-repo2docker-0.9.0/aicrowd_repo2docker.egg-info/SOURCES.txt` & `aicrowd-repo2docker-0.9.1/aicrowd_repo2docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/setup.py` & `aicrowd-repo2docker-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/CONTRIBUTING.md` & `aicrowd-repo2docker-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aicrowd-repo2docker-0.9.0/versioneer.py` & `aicrowd-repo2docker-0.9.1/versioneer.py`

 * *Files identical despite different names*

