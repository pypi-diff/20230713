# Comparing `tmp/Mesh-Client-2.0.1.tar.gz` & `tmp/Mesh-Client-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mesh-Client-2.0.1.tar", last modified: Tue Jul  4 19:33:03 2023, max compression
+gzip compressed data, was "Mesh-Client-2.1.1.tar", last modified: Wed Jul 12 13:45:14 2023, max compression
```

## Comparing `Mesh-Client-2.0.1.tar` & `Mesh-Client-2.1.1.tar`

### file list

```diff
@@ -1,75 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.864758 Mesh-Client-2.0.1/
--rw-rw-r--   0 runner    (1001) docker     (123)     2044 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.gitallowed
--rw-rw-r--   0 runner    (1001) docker     (123)     1080 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.gitdisallowed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.856757 Mesh-Client-2.0.1/.github/
--rw-rw-r--   0 runner    (1001) docker     (123)       48 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (123)      462 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/dependabot.yml
--rw-rw-r--   0 runner    (1001) docker     (123)      204 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.856757 Mesh-Client-2.0.1/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (123)     2683 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/workflows/merge-develop.yml
--rw-rw-r--   0 runner    (1001) docker     (123)     4054 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/workflows/merge-release.yml
--rw-rw-r--   0 runner    (1001) docker     (123)     7424 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.github/workflows/pull-request.yml
--rw-rw-r--   0 runner    (1001) docker     (123)      563 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (123)       56 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/.tool-versions
--rw-rw-r--   0 runner    (1001) docker     (123)     1696 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (123)     1078 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (123)     3030 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.856757 Mesh-Client-2.0.1/Mesh_Client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 19:33:03.000000 Mesh-Client-2.0.1/Mesh_Client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-04 19:33:03.864758 Mesh-Client-2.0.1/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (123)     1447 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/README.md
--rw-rw-r--   0 runner    (1001) docker     (123)     1347 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (123)      734 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/docker-compose.yml
--rwxrwxr-x   0 runner    (1001) docker     (123)    12983 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/git-secrets
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.860757 Mesh-Client-2.0.1/mesh_client/
--rw-rw-r--   0 runner    (1001) docker     (123)    26312 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     9982 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/io_helpers.py
--rw-rw-r--   0 runner    (1001) docker     (123)      260 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/key_helper.py
--rwxrwxr-x   0 runner    (1001) docker     (123)      831 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/mesh_auth.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-dep-ca-bundle.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     2615 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-dev-ca-bundle.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     4632 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-digicert-ca-bundle.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     2985 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-digicert-root-ca.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-ig-int-ca-bundle.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     2896 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-ig-live-ca-bundle.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-int-ca-bundle.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     1460 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-live-root-ca.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     2558 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-opt-ca-bundle.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/nhs-train-ca-bundle.pem
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/py.typed
--rw-rw-r--   0 runner    (1001) docker     (123)     1499 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/mesh_client/types.py
--rw-rw-r--   0 runner    (1001) docker     (123)    97932 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/poetry.lock
--rw-rw-r--   0 runner    (1001) docker     (123)       61 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/poetry.toml
--rw-rw-r--   0 runner    (1001) docker     (123)     3815 2023-07-04 19:32:59.000000 Mesh-Client-2.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.860757 Mesh-Client-2.0.1/scripts/
--rwxrwxr-x   0 runner    (1001) docker     (123)      532 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/scripts/check-secrets.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.860757 Mesh-Client-2.0.1/scripts/hooks/
--rwxrwxr-x   0 runner    (1001) docker     (123)      390 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/scripts/hooks/commit-msg.sh
--rwxrwxr-x   0 runner    (1001) docker     (123)      398 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/scripts/hooks/pre-commit.sh
--rwxrwxr-x   0 runner    (1001) docker     (123)     6225 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/scripts/sonar_tests.py
--rwxrwxr-x   0 runner    (1001) docker     (123)      325 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/scripts/wait-for-container.sh
--rw-rw-r--   0 runner    (1001) docker     (123)       67 2023-07-04 19:33:03.864758 Mesh-Client-2.0.1/setup.cfg
--rwxrwxr-x   0 runner    (1001) docker     (123)     1344 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/setup.py
--rw-rw-r--   0 runner    (1001) docker     (123)      425 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/sonar-project.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:33:03.864758 Mesh-Client-2.0.1/tests/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1923 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/ca.cert.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     3243 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/ca.key.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     1879 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/client.cert.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     3243 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/client.key.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     1414 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/helpers.py
--rw-rw-r--   0 runner    (1001) docker     (123)     9449 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/io_helpers_tests.py
--rw-rw-r--   0 runner    (1001) docker     (123)      424 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mailboxes.jsonl
--rw-rw-r--   0 runner    (1001) docker     (123)     3889 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mesh_chunk_retries_tests.py
--rw-rw-r--   0 runner    (1001) docker     (123)    10017 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mesh_client_tests.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1964 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mesh_endpoint_connectivity_tests.py
--rw-rw-r--   0 runner    (1001) docker     (123)     9792 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mesh_sandbox_tests.py
--rwxrwxr-x   0 runner    (1001) docker     (123)    17388 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/mock_server.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2053 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/server.cert.pem
--rw-rw-r--   0 runner    (1001) docker     (123)     3243 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/server.key.pem
--rw-rw-r--   0 runner    (1001) docker     (123)      176 2023-07-04 19:32:38.000000 Mesh-Client-2.0.1/tests/workflows.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:45:14.952626 Mesh-Client-2.1.1/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2044 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/.gitallowed
+-rw-rw-r--   0 runner    (1001) docker     (123)     1080 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/.gitdisallowed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:45:14.948626 Mesh-Client-2.1.1/.github/
+-rw-rw-r--   0 runner    (1001) docker     (123)       48 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (123)      462 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/.github/dependabot.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)      204 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:45:14.948626 Mesh-Client-2.1.1/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2683 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/.github/workflows/merge-develop.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     4054 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/.github/workflows/merge-release.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     7424 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/.github/workflows/pull-request.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)      563 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (123)       56 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/.tool-versions
+-rw-rw-r--   0 runner    (1001) docker     (123)     1696 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     1078 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (123)     3030 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:45:14.948626 Mesh-Client-2.1.1/Mesh_Client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-12 13:45:14.000000 Mesh-Client-2.1.1/Mesh_Client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-12 13:45:14.000000 Mesh-Client-2.1.1/Mesh_Client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:45:14.000000 Mesh-Client-2.1.1/Mesh_Client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-12 13:45:14.000000 Mesh-Client-2.1.1/Mesh_Client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 13:45:14.000000 Mesh-Client-2.1.1/Mesh_Client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 13:45:14.000000 Mesh-Client-2.1.1/Mesh_Client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-12 13:45:14.952626 Mesh-Client-2.1.1/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (123)     1447 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/README.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     1347 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:45:14.944626 Mesh-Client-2.1.1/docker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:45:14.948626 Mesh-Client-2.1.1/docker/squid/
+-rw-rw-r--   0 runner    (1001) docker     (123)      632 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/docker/squid/Dockerfile
+-rwxrwxr-x   0 runner    (1001) docker     (123)      215 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/docker/squid/entrypoint.sh
+-rw-rw-r--   0 runner    (1001) docker     (123)     2753 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/docker/squid/squid.conf
+-rw-rw-r--   0 runner    (1001) docker     (123)     1024 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/docker-compose.yml
+-rwxrwxr-x   0 runner    (1001) docker     (123)    12983 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/git-secrets
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:45:14.952626 Mesh-Client-2.1.1/mesh_client/
+-rw-rw-r--   0 runner    (1001) docker     (123)    27994 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9982 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/io_helpers.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      260 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/key_helper.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)      831 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/mesh_auth.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/nhs-dep-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2615 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/nhs-dev-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     4632 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/nhs-digicert-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2985 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/nhs-digicert-root-ca.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/nhs-ig-int-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2896 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/nhs-ig-live-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/nhs-int-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     1460 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/nhs-live-root-ca.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2558 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/nhs-opt-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     2562 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/nhs-train-ca-bundle.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (123)     1499 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/mesh_client/types.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    72976 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/poetry.lock
+-rw-rw-r--   0 runner    (1001) docker     (123)       61 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/poetry.toml
+-rw-rw-r--   0 runner    (1001) docker     (123)     3876 2023-07-12 13:45:10.000000 Mesh-Client-2.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:45:14.952626 Mesh-Client-2.1.1/scripts/
+-rwxrwxr-x   0 runner    (1001) docker     (123)      532 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/scripts/check-secrets.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:45:14.952626 Mesh-Client-2.1.1/scripts/hooks/
+-rwxrwxr-x   0 runner    (1001) docker     (123)      390 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/scripts/hooks/commit-msg.sh
+-rwxrwxr-x   0 runner    (1001) docker     (123)      398 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/scripts/hooks/pre-commit.sh
+-rwxrwxr-x   0 runner    (1001) docker     (123)     6225 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/scripts/sonar_tests.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)      325 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/scripts/wait-for-container.sh
+-rw-rw-r--   0 runner    (1001) docker     (123)       67 2023-07-12 13:45:14.956626 Mesh-Client-2.1.1/setup.cfg
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1344 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/setup.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      425 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:45:14.952626 Mesh-Client-2.1.1/tests/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1923 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/ca.cert.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     3243 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/ca.key.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     1879 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/client.cert.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     3243 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/client.key.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     1435 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/helpers.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9449 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/io_helpers_tests.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      424 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/mailboxes.jsonl
+-rw-rw-r--   0 runner    (1001) docker     (123)     3889 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/mesh_chunk_retries_tests.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    10017 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/mesh_client_tests.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    10177 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/mesh_endpoint_connectivity_tests.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9792 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/mesh_sandbox_tests.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)    17388 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/mock_server.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2053 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/server.cert.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)     3243 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/server.key.pem
+-rw-rw-r--   0 runner    (1001) docker     (123)      176 2023-07-12 13:44:52.000000 Mesh-Client-2.1.1/tests/workflows.jsonl
```

### Comparing `Mesh-Client-2.0.1/.gitallowed` & `Mesh-Client-2.1.1/.gitallowed`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/.gitdisallowed` & `Mesh-Client-2.1.1/.gitdisallowed`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/.github/workflows/merge-develop.yml` & `Mesh-Client-2.1.1/.github/workflows/merge-develop.yml`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/.github/workflows/merge-release.yml` & `Mesh-Client-2.1.1/.github/workflows/merge-release.yml`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/.github/workflows/pull-request.yml` & `Mesh-Client-2.1.1/.github/workflows/pull-request.yml`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/.gitignore` & `Mesh-Client-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/CONTRIBUTING.md` & `Mesh-Client-2.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/LICENSE` & `Mesh-Client-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/Makefile` & `Mesh-Client-2.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/Mesh_Client.egg-info/PKG-INFO` & `Mesh-Client-2.1.1/Mesh_Client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mesh-Client
-Version: 2.0.1
+Version: 2.1.1
 Summary: Client for NHS England's MESH messaging system
 Home-page: https://github.com/NHSDigital/mesh-client
 Author: spinecore
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Mesh-Client-2.0.1/Mesh_Client.egg-info/SOURCES.txt` & `Mesh-Client-2.1.1/Mesh_Client.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 .github/workflows/pull-request.yml
 Mesh_Client.egg-info/PKG-INFO
 Mesh_Client.egg-info/SOURCES.txt
 Mesh_Client.egg-info/dependency_links.txt
 Mesh_Client.egg-info/entry_points.txt
 Mesh_Client.egg-info/requires.txt
 Mesh_Client.egg-info/top_level.txt
+docker/squid/Dockerfile
+docker/squid/entrypoint.sh
+docker/squid/squid.conf
 mesh_client/__init__.py
 mesh_client/io_helpers.py
 mesh_client/key_helper.py
 mesh_client/mesh_auth.py
 mesh_client/nhs-dep-ca-bundle.pem
 mesh_client/nhs-dev-ca-bundle.pem
 mesh_client/nhs-digicert-ca-bundle.pem
```

### Comparing `Mesh-Client-2.0.1/PKG-INFO` & `Mesh-Client-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mesh-Client
-Version: 2.0.1
+Version: 2.1.1
 Summary: Client for NHS England's MESH messaging system
 Home-page: https://github.com/NHSDigital/mesh-client
 Author: spinecore
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Mesh-Client-2.0.1/README.md` & `Mesh-Client-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/SECURITY.md` & `Mesh-Client-2.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/git-secrets` & `Mesh-Client-2.1.1/git-secrets`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/__init__.py` & `Mesh-Client-2.1.1/mesh_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 import warnings
 from dataclasses import dataclass
 from hashlib import sha256
 from io import BytesIO
 from itertools import chain
 from typing import Any, Dict, List, Optional, Tuple, TypeVar, Union, cast
 from urllib.parse import quote as q
+from urllib.parse import urlparse
 
 import requests
 from requests.adapters import HTTPAdapter
+from urllib3.util.ssl_ import create_urllib3_context
 
 from .io_helpers import (
     CombineStreams,
     GzipCompressStream,
     GzipDecompressStream,
     SplitStream,
 )
@@ -87,24 +89,44 @@
     "message_id": "Mex-MessageID",
     "version": "Mex-Version",
     "partner_id": "Mex-PartnerID",
 }
 _RECEIVE_HEADERS.update(_OPTIONAL_HEADERS)
 
 
-Endpoint = collections.namedtuple("Endpoint", ["url", "verify", "cert", "check_hostname"])
+Endpoint = collections.namedtuple(
+    "Endpoint", ["url", "verify", "cert", "check_hostname", "hostname_checks_common_name"]
+)
+
+NHS_INT_ENDPOINT = Endpoint("https://msg.int.spine2.ncrs.nhs.uk", INT_CA_CERT, None, True, True)
+NHS_DEV_ENDPOINT = Endpoint("https://msg.dev.spine2.ncrs.nhs.uk", DEV_CA_CERT, None, True, True)
+NHS_DEP_ENDPOINT = Endpoint("https://msg.dep.spine2.ncrs.nhs.uk", DEP_CA_CERT, None, True, True)
+NHS_TRAIN_ENDPOINT = Endpoint("https://msg.train.spine2.ncrs.nhs.uk", TRAIN_CA_CERT, None, True, True)
+NHS_LIVE_ENDPOINT = Endpoint("https://mesh-sync.national.ncrs.nhs.uk", LIVE_CA_CERT, None, True, True)
+NHS_OPENTEST_ENDPOINT = Endpoint("https://192.168.128.11", OPENTEST_CA_CERT, None, False, False)
+NHS_INTERNET_GATEWAY_ENDPOINT = Endpoint("https://mesh-sync.spineservices.nhs.uk", IG_LIVE_CA_CERT, None, True, True)
+NHS_INTERNET_GATEWAY_INT_ENDPOINT = Endpoint("https://msg.intspineservices.nhs.uk", IG_INT_CA_CERT, None, True, False)
+
+ENDPOINTS = [
+    (name, endpoint) for name, endpoint in locals().items() if name.endswith("_ENDPOINT") and name.startswith("NHS_")
+]
+
+
+_HOSTNAME_ENDPOINT_MAP = {urlparse(ep.url).hostname: ep for name, ep in ENDPOINTS if "_OPENTEST_" not in name}
+
+
+def try_get_endpoint_from_url(url: str) -> Optional[Endpoint]:
+    url_parsed = urlparse(url)
+    if not url_parsed.hostname:
+        return None
+    defaults = _HOSTNAME_ENDPOINT_MAP.get(url_parsed.hostname.lower())
+    if not defaults:
+        return None
 
-NHS_INT_ENDPOINT = Endpoint("https://msg.int.spine2.ncrs.nhs.uk", INT_CA_CERT, None, False)
-NHS_DEV_ENDPOINT = Endpoint("https://msg.dev.spine2.ncrs.nhs.uk", DEV_CA_CERT, None, False)
-NHS_DEP_ENDPOINT = Endpoint("https://msg.dep.spine2.ncrs.nhs.uk", DEP_CA_CERT, None, False)
-NHS_TRAIN_ENDPOINT = Endpoint("https://msg.train.spine2.ncrs.nhs.uk", TRAIN_CA_CERT, None, False)
-NHS_LIVE_ENDPOINT = Endpoint("https://mesh-sync.national.ncrs.nhs.uk", LIVE_CA_CERT, None, False)
-NHS_OPENTEST_ENDPOINT = Endpoint("https://192.168.128.11", OPENTEST_CA_CERT, None, False)
-NHS_INTERNET_GATEWAY_ENDPOINT = Endpoint("https://mesh-sync.spineservices.nhs.uk", IG_LIVE_CA_CERT, None, True)
-NHS_INTERNET_GATEWAY_INT_ENDPOINT = Endpoint("https://msg.intspineservices.nhs.uk", IG_INT_CA_CERT, None, True)
+    return Endpoint(url, *defaults[1:])
 
 
 def deprecated(reason=None):
     """This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
     when the function is used."""
 
@@ -126,58 +148,67 @@
 class MeshError(Exception):
     pass
 
 
 class SSLContextAdapter(HTTPAdapter):
     def __init__(
         self,
-        url: Union[str, Endpoint],
         cert: Optional[Union[Tuple[str], Tuple[str, str], Tuple[str, str, str]]] = None,
         verify: Optional[Union[str, bool]] = None,
         check_hostname: Optional[bool] = None,
+        hostname_checks_common_name: Optional[bool] = None,
     ):
-        self.url = url
         self.cert = cert
         self.verify = verify
         self.check_hostname = check_hostname
-        if check_hostname is None and hasattr(url, "check_hostname"):
-            self.check_hostname = url.check_hostname
-
-        if cert is None and hasattr(url, "cert"):
-            self.cert = url.cert
-
-        if verify is None and hasattr(url, "verify"):
-            self.verify = url.verify
+        self.hostname_checks_common_name = hostname_checks_common_name
 
         super().__init__()
 
-    def init_poolmanager(self, *args, **kwargs):
-        context = ssl.create_default_context()
+    def create_ssl_context(self) -> ssl.SSLContext:
+        context = cast(ssl.SSLContext, create_urllib3_context())
+
+        context.minimum_version = ssl.TLSVersion.TLSv1_2
 
         if self.cert and isinstance(self.cert, (tuple, list)):
             context.load_cert_chain(*self.cert)
 
         if self.verify:
             if isinstance(self.verify, (str, bytes)):
                 context.load_verify_locations(self.verify)
 
-            if context.check_hostname is not None:
+            if self.check_hostname is not None:
                 context.check_hostname = cast(bool, self.check_hostname)
 
             context.verify_mode = ssl.CERT_REQUIRED
-            if self.check_hostname is not False:
-                context.hostname_checks_common_name = True
+            if context.check_hostname is not False:
+                if self.hostname_checks_common_name is not None:
+                    context.hostname_checks_common_name = self.hostname_checks_common_name
 
         if self.verify is False:
             context.check_hostname = False
             context.verify_mode = ssl.CERT_NONE
 
+        return context
+
+    def init_poolmanager(self, *args, **kwargs):
+        context = self.create_ssl_context()
         kwargs["ssl_context"] = context
+        if context.check_hostname is False:
+            kwargs["assert_hostname"] = False
         return super(SSLContextAdapter, self).init_poolmanager(*args, **kwargs)
 
+    def proxy_manager_for(self, proxy, **proxy_kwargs):
+        context = self.create_ssl_context()
+        proxy_kwargs["ssl_context"] = context
+        if context.check_hostname is False:
+            proxy_kwargs["assert_hostname"] = False
+
+        return super().proxy_manager_for(proxy, **proxy_kwargs)
+
 
 class MeshClient(object):
     """
     A class representing a single MESH session, for a given user on a given
     endpoint. This class handles details such as chunking and compression
     transparently.
     """
@@ -187,14 +218,15 @@
         url: Union[str, Endpoint],
         mailbox: str,
         password: str,
         shared_key: Optional[bytes] = None,
         cert: Optional[Union[Tuple[str], Tuple[str, str], Tuple[str, str, str]]] = None,
         verify: Optional[Union[str, bool]] = None,
         check_hostname: Optional[bool] = None,
+        hostname_checks_common_name: Optional[bool] = None,
         max_chunk_size=75 * 1024 * 1024,
         proxies: Optional[Dict[str, str]] = None,
         transparent_compress: bool = False,
         max_chunk_retries: int = 0,
         timeout: Union[int, float] = 10 * 60,
     ):
         """
@@ -225,34 +257,46 @@
         and whether messages should be compressed, transparently, before
         sending.
         """
 
         shared_key = shared_key or get_shared_key_from_environ()
 
         self._session = requests.Session()
-        adapter = SSLContextAdapter(url, cert, verify, check_hostname)
-        self._session.mount("https://", adapter)
-        self._session.mount("http://", adapter)
+
+        if isinstance(url, str):
+            endpoint_config = try_get_endpoint_from_url(url)
+            if endpoint_config:
+                url = endpoint_config
+
+        self._url = url.url if hasattr(url, "url") else url
+
+        if verify is None and hasattr(url, "verify"):
+            verify = url.verify
+
+        if check_hostname is None and hasattr(url, "check_hostname"):
+            check_hostname = url.check_hostname
+
+        if hostname_checks_common_name is None and hasattr(url, "hostname_checks_common_name"):
+            hostname_checks_common_name = url.hostname_checks_common_name
+
+        if cert is None and hasattr(url, "cert"):
+            cert = url.cert
+
+        if verify is False:
+            self._session.verify = False
+
+        self._session.mount(self._url, SSLContextAdapter(cert, verify, check_hostname, hostname_checks_common_name))
         self._session.headers = {
             "User-Agent": (
                 f"mesh_client;{__version__};N/A;{platform.processor() or platform.machine()};"
                 f"{platform.system()};{platform.release()} {platform.version()}"
             ),
             "Accept-Encoding": "gzip",
         }
         self._session.auth = AuthTokenGenerator(shared_key, mailbox, password)
-        if hasattr(url, "url"):
-            self._url = url.url
-        else:
-            self._url = url
-
-        if verify is not None:
-            self._session.verify = verify
-        elif hasattr(url, "verify"):
-            self._session.verify = url.verify
 
         self._session.proxies = proxies or {}
         self._mailbox = mailbox
         self._max_chunk_size = max_chunk_size
         self._transparent_compress = transparent_compress
         self._max_chunk_retries = max_chunk_retries
         self._timeout = timeout
```

### Comparing `Mesh-Client-2.0.1/mesh_client/io_helpers.py` & `Mesh-Client-2.1.1/mesh_client/io_helpers.py`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/mesh_auth.py` & `Mesh-Client-2.1.1/mesh_client/mesh_auth.py`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/nhs-dep-ca-bundle.pem` & `Mesh-Client-2.1.1/mesh_client/nhs-dep-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/nhs-dev-ca-bundle.pem` & `Mesh-Client-2.1.1/mesh_client/nhs-dev-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/nhs-digicert-ca-bundle.pem` & `Mesh-Client-2.1.1/mesh_client/nhs-digicert-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/nhs-digicert-root-ca.pem` & `Mesh-Client-2.1.1/mesh_client/nhs-digicert-root-ca.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/nhs-ig-int-ca-bundle.pem` & `Mesh-Client-2.1.1/mesh_client/nhs-ig-int-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/nhs-ig-live-ca-bundle.pem` & `Mesh-Client-2.1.1/mesh_client/nhs-ig-live-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/nhs-int-ca-bundle.pem` & `Mesh-Client-2.1.1/mesh_client/nhs-int-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/nhs-live-root-ca.pem` & `Mesh-Client-2.1.1/mesh_client/nhs-live-root-ca.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/nhs-opt-ca-bundle.pem` & `Mesh-Client-2.1.1/mesh_client/nhs-opt-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/nhs-train-ca-bundle.pem` & `Mesh-Client-2.1.1/mesh_client/nhs-train-ca-bundle.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/mesh_client/types.py` & `Mesh-Client-2.1.1/mesh_client/types.py`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/poetry.lock` & `Mesh-Client-2.1.1/poetry.lock`

 * *Files 16% similar despite different names*

```diff
@@ -86,32 +86,14 @@
 [package.extras]
 colorama = ["colorama (>=0.4.3)"]
 d = ["aiohttp (>=3.7.4)"]
 jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
 uvloop = ["uvloop (>=0.15.2)"]
 
 [[package]]
-name = "bleach"
-version = "6.0.0"
-description = "An easy safelist-based HTML-sanitizing tool."
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "bleach-6.0.0-py3-none-any.whl", hash = "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"},
-    {file = "bleach-6.0.0.tar.gz", hash = "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414"},
-]
-
-[package.dependencies]
-six = ">=1.9.0"
-webencodings = "*"
-
-[package.extras]
-css = ["tinycss2 (>=1.1.0,<1.2)"]
-
-[[package]]
 name = "build"
 version = "0.10.0"
 description = "A simple, correct Python build frontend"
 optional = false
 python-versions = ">= 3.7"
 files = [
     {file = "build-0.10.0-py3-none-any.whl", hash = "sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171"},
@@ -150,193 +132,117 @@
 python-versions = ">=3.6"
 files = [
     {file = "certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
     {file = "certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
 ]
 
 [[package]]
-name = "cffi"
-version = "1.15.1"
-description = "Foreign Function Interface for Python calling C code."
-optional = false
-python-versions = "*"
-files = [
-    {file = "cffi-1.15.1-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2"},
-    {file = "cffi-1.15.1-cp27-cp27m-manylinux1_i686.whl", hash = "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2"},
-    {file = "cffi-1.15.1-cp27-cp27m-manylinux1_x86_64.whl", hash = "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914"},
-    {file = "cffi-1.15.1-cp27-cp27m-win32.whl", hash = "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3"},
-    {file = "cffi-1.15.1-cp27-cp27m-win_amd64.whl", hash = "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e"},
-    {file = "cffi-1.15.1-cp27-cp27mu-manylinux1_i686.whl", hash = "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162"},
-    {file = "cffi-1.15.1-cp27-cp27mu-manylinux1_x86_64.whl", hash = "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b"},
-    {file = "cffi-1.15.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21"},
-    {file = "cffi-1.15.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185"},
-    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd"},
-    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc"},
-    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f"},
-    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e"},
-    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4"},
-    {file = "cffi-1.15.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01"},
-    {file = "cffi-1.15.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e"},
-    {file = "cffi-1.15.1-cp310-cp310-win32.whl", hash = "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2"},
-    {file = "cffi-1.15.1-cp310-cp310-win_amd64.whl", hash = "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d"},
-    {file = "cffi-1.15.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac"},
-    {file = "cffi-1.15.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83"},
-    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9"},
-    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c"},
-    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325"},
-    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c"},
-    {file = "cffi-1.15.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef"},
-    {file = "cffi-1.15.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8"},
-    {file = "cffi-1.15.1-cp311-cp311-win32.whl", hash = "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d"},
-    {file = "cffi-1.15.1-cp311-cp311-win_amd64.whl", hash = "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104"},
-    {file = "cffi-1.15.1-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7"},
-    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6"},
-    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d"},
-    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a"},
-    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405"},
-    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e"},
-    {file = "cffi-1.15.1-cp36-cp36m-win32.whl", hash = "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf"},
-    {file = "cffi-1.15.1-cp36-cp36m-win_amd64.whl", hash = "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497"},
-    {file = "cffi-1.15.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375"},
-    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e"},
-    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82"},
-    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b"},
-    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c"},
-    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426"},
-    {file = "cffi-1.15.1-cp37-cp37m-win32.whl", hash = "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9"},
-    {file = "cffi-1.15.1-cp37-cp37m-win_amd64.whl", hash = "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045"},
-    {file = "cffi-1.15.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3"},
-    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a"},
-    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5"},
-    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca"},
-    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02"},
-    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192"},
-    {file = "cffi-1.15.1-cp38-cp38-win32.whl", hash = "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314"},
-    {file = "cffi-1.15.1-cp38-cp38-win_amd64.whl", hash = "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5"},
-    {file = "cffi-1.15.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585"},
-    {file = "cffi-1.15.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"},
-    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415"},
-    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d"},
-    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984"},
-    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35"},
-    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27"},
-    {file = "cffi-1.15.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76"},
-    {file = "cffi-1.15.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3"},
-    {file = "cffi-1.15.1-cp39-cp39-win32.whl", hash = "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee"},
-    {file = "cffi-1.15.1-cp39-cp39-win_amd64.whl", hash = "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c"},
-    {file = "cffi-1.15.1.tar.gz", hash = "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9"},
-]
-
-[package.dependencies]
-pycparser = "*"
-
-[[package]]
 name = "chardet"
 version = "5.1.0"
 description = "Universal encoding detector for Python 3"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "chardet-5.1.0-py3-none-any.whl", hash = "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"},
     {file = "chardet-5.1.0.tar.gz", hash = "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5"},
 ]
 
 [[package]]
 name = "charset-normalizer"
-version = "3.1.0"
+version = "3.2.0"
 description = "The Real First Universal Charset Detector. Open, modern and actively maintained alternative to Chardet."
 optional = false
 python-versions = ">=3.7.0"
 files = [
-    {file = "charset-normalizer-3.1.0.tar.gz", hash = "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-win32.whl", hash = "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-win_amd64.whl", hash = "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-win32.whl", hash = "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-win_amd64.whl", hash = "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-musllinux_1_1_ppc64le.whl", hash = "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-win32.whl", hash = "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-win_amd64.whl", hash = "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-win32.whl", hash = "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-win_amd64.whl", hash = "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-win32.whl", hash = "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-win_amd64.whl", hash = "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b"},
-    {file = "charset_normalizer-3.1.0-py3-none-any.whl", hash = "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d"},
+    {file = "charset-normalizer-3.2.0.tar.gz", hash = "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-win32.whl", hash = "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-win_amd64.whl", hash = "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-win32.whl", hash = "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-win_amd64.whl", hash = "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_ppc64le.whl", hash = "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-win32.whl", hash = "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-win_amd64.whl", hash = "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-win32.whl", hash = "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-win_amd64.whl", hash = "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-win32.whl", hash = "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-win_amd64.whl", hash = "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80"},
+    {file = "charset_normalizer-3.2.0-py3-none-any.whl", hash = "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6"},
 ]
 
 [[package]]
 name = "click"
-version = "8.1.3"
+version = "8.1.4"
 description = "Composable command line interface toolkit"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
-    {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
+    {file = "click-8.1.4-py3-none-any.whl", hash = "sha256:2739815aaa5d2c986a88f1e9230c55e17f0caad3d958a5e13ad0797c166db9e3"},
+    {file = "click-8.1.4.tar.gz", hash = "sha256:b97d0c74955da062a7d4ef92fadb583806a585b2ea81958a81bd72726cbb8e37"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
 importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
 
 [[package]]
@@ -419,55 +325,14 @@
     {file = "coverage-7.2.7.tar.gz", hash = "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59"},
 ]
 
 [package.extras]
 toml = ["tomli"]
 
 [[package]]
-name = "cryptography"
-version = "41.0.1"
-description = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "cryptography-41.0.1-cp37-abi3-macosx_10_12_universal2.whl", hash = "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"},
-    {file = "cryptography-41.0.1-cp37-abi3-macosx_10_12_x86_64.whl", hash = "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a"},
-    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca"},
-    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43"},
-    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_28_aarch64.whl", hash = "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b"},
-    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_28_x86_64.whl", hash = "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3"},
-    {file = "cryptography-41.0.1-cp37-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db"},
-    {file = "cryptography-41.0.1-cp37-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31"},
-    {file = "cryptography-41.0.1-cp37-abi3-win32.whl", hash = "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5"},
-    {file = "cryptography-41.0.1-cp37-abi3-win_amd64.whl", hash = "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c"},
-    {file = "cryptography-41.0.1-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb"},
-    {file = "cryptography-41.0.1-pp38-pypy38_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3"},
-    {file = "cryptography-41.0.1-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039"},
-    {file = "cryptography-41.0.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc"},
-    {file = "cryptography-41.0.1-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485"},
-    {file = "cryptography-41.0.1-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c"},
-    {file = "cryptography-41.0.1-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a"},
-    {file = "cryptography-41.0.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5"},
-    {file = "cryptography-41.0.1.tar.gz", hash = "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006"},
-]
-
-[package.dependencies]
-cffi = ">=1.12"
-
-[package.extras]
-docs = ["sphinx (>=5.3.0)", "sphinx-rtd-theme (>=1.1.1)"]
-docstest = ["pyenchant (>=1.6.11)", "sphinxcontrib-spelling (>=4.0.1)", "twine (>=1.12.0)"]
-nox = ["nox"]
-pep8test = ["black", "check-sdist", "mypy", "ruff"]
-sdist = ["build"]
-ssh = ["bcrypt (>=3.1.5)"]
-test = ["pretend", "pytest (>=6.2.0)", "pytest-benchmark", "pytest-cov", "pytest-xdist"]
-test-randomorder = ["pytest-randomly"]
-
-[[package]]
 name = "decorator"
 version = "5.1.1"
 description = "Decorators for Humans"
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "decorator-5.1.1-py3-none-any.whl", hash = "sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186"},
@@ -482,33 +347,22 @@
 python-versions = "*"
 files = [
     {file = "distlib-0.3.6-py2.py3-none-any.whl", hash = "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"},
     {file = "distlib-0.3.6.tar.gz", hash = "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46"},
 ]
 
 [[package]]
-name = "docutils"
-version = "0.20.1"
-description = "Docutils -- Python Documentation Utilities"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "docutils-0.20.1-py3-none-any.whl", hash = "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6"},
-    {file = "docutils-0.20.1.tar.gz", hash = "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"},
-]
-
-[[package]]
 name = "exceptiongroup"
-version = "1.1.1"
+version = "1.1.2"
 description = "Backport of PEP 654 (exception groups)"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
-    {file = "exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
+    {file = "exceptiongroup-1.1.2-py3-none-any.whl", hash = "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"},
+    {file = "exceptiongroup-1.1.2.tar.gz", hash = "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5"},
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "executing"
@@ -619,32 +473,14 @@
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 perf = ["ipython"]
 testing = ["flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)", "pytest-ruff"]
 
 [[package]]
-name = "importlib-resources"
-version = "5.12.0"
-description = "Read resources from Python packages"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "importlib_resources-5.12.0-py3-none-any.whl", hash = "sha256:7b1deeebbf351c7578e09bf2f63fa2ce8b5ffec296e0d349139d43cca061a81a"},
-    {file = "importlib_resources-5.12.0.tar.gz", hash = "sha256:4be82589bf5c1d7999aedf2a45159d10cb3ca4f19b2271f8792bc8e6da7b22f6"},
-]
-
-[package.dependencies]
-zipp = {version = ">=3.1.0", markers = "python_version < \"3.10\""}
-
-[package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
-testing = ["flake8 (<5)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
-
-[[package]]
 name = "iniconfig"
 version = "2.0.0"
 description = "brain-dead simple config-ini parsing"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
@@ -704,32 +540,14 @@
 [package.extras]
 colors = ["colorama (>=0.4.3)"]
 pipfile-deprecated-finder = ["pip-shims (>=0.5.2)", "pipreqs", "requirementslib"]
 plugins = ["setuptools"]
 requirements-deprecated-finder = ["pip-api", "pipreqs"]
 
 [[package]]
-name = "jaraco-classes"
-version = "3.2.3"
-description = "Utility functions for Python class constructs"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "jaraco.classes-3.2.3-py3-none-any.whl", hash = "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158"},
-    {file = "jaraco.classes-3.2.3.tar.gz", hash = "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"},
-]
-
-[package.dependencies]
-more-itertools = "*"
-
-[package.extras]
-docs = ["jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)"]
-testing = ["flake8 (<5)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
-
-[[package]]
 name = "jedi"
 version = "0.18.2"
 description = "An autocompletion tool for Python that can be used for text editors."
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "jedi-0.18.2-py2.py3-none-any.whl", hash = "sha256:203c1fd9d969ab8f2119ec0a3342e0b49910045abe6af0a3ae83a5764d54639e"},
@@ -741,78 +559,14 @@
 
 [package.extras]
 docs = ["Jinja2 (==2.11.3)", "MarkupSafe (==1.1.1)", "Pygments (==2.8.1)", "alabaster (==0.7.12)", "babel (==2.9.1)", "chardet (==4.0.0)", "commonmark (==0.8.1)", "docutils (==0.17.1)", "future (==0.18.2)", "idna (==2.10)", "imagesize (==1.2.0)", "mock (==1.0.1)", "packaging (==20.9)", "pyparsing (==2.4.7)", "pytz (==2021.1)", "readthedocs-sphinx-ext (==2.1.4)", "recommonmark (==0.5.0)", "requests (==2.25.1)", "six (==1.15.0)", "snowballstemmer (==2.1.0)", "sphinx (==1.8.5)", "sphinx-rtd-theme (==0.4.3)", "sphinxcontrib-serializinghtml (==1.1.4)", "sphinxcontrib-websupport (==1.2.4)", "urllib3 (==1.26.4)"]
 qa = ["flake8 (==3.8.3)", "mypy (==0.782)"]
 testing = ["Django (<3.1)", "attrs", "colorama", "docopt", "pytest (<7.0.0)"]
 
 [[package]]
-name = "jeepney"
-version = "0.8.0"
-description = "Low-level, pure Python DBus protocol wrapper."
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "jeepney-0.8.0-py3-none-any.whl", hash = "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"},
-    {file = "jeepney-0.8.0.tar.gz", hash = "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806"},
-]
-
-[package.extras]
-test = ["async-timeout", "pytest", "pytest-asyncio (>=0.17)", "pytest-trio", "testpath", "trio"]
-trio = ["async_generator", "trio"]
-
-[[package]]
-name = "keyring"
-version = "24.1.1"
-description = "Store and access your passwords safely."
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "keyring-24.1.1-py3-none-any.whl", hash = "sha256:bc402c5e501053098bcbd149c4ddbf8e36c6809e572c2d098d4961e88d4c270d"},
-    {file = "keyring-24.1.1.tar.gz", hash = "sha256:3d44a48fa9a254f6c72879d7c88604831ebdaac6ecb0b214308b02953502c510"},
-]
-
-[package.dependencies]
-importlib-metadata = {version = ">=4.11.4", markers = "python_version < \"3.12\""}
-importlib-resources = {version = "*", markers = "python_version < \"3.9\""}
-"jaraco.classes" = "*"
-jeepney = {version = ">=0.4.2", markers = "sys_platform == \"linux\""}
-pywin32-ctypes = {version = ">=0.2.0", markers = "sys_platform == \"win32\""}
-SecretStorage = {version = ">=3.2", markers = "sys_platform == \"linux\""}
-
-[package.extras]
-completion = ["shtab"]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
-testing = ["pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-ruff"]
-
-[[package]]
-name = "markdown-it-py"
-version = "2.2.0"
-description = "Python port of markdown-it. Markdown parsing, done right!"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "markdown-it-py-2.2.0.tar.gz", hash = "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"},
-    {file = "markdown_it_py-2.2.0-py3-none-any.whl", hash = "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30"},
-]
-
-[package.dependencies]
-mdurl = ">=0.1,<1.0"
-typing_extensions = {version = ">=3.7.4", markers = "python_version < \"3.8\""}
-
-[package.extras]
-benchmarking = ["psutil", "pytest", "pytest-benchmark"]
-code-style = ["pre-commit (>=3.0,<4.0)"]
-compare = ["commonmark (>=0.9,<1.0)", "markdown (>=3.4,<4.0)", "mistletoe (>=1.0,<2.0)", "mistune (>=2.0,<3.0)", "panflute (>=2.3,<3.0)"]
-linkify = ["linkify-it-py (>=1,<3)"]
-plugins = ["mdit-py-plugins"]
-profiling = ["gprof2dot"]
-rtd = ["attrs", "myst-parser", "pyyaml", "sphinx", "sphinx-copybutton", "sphinx-design", "sphinx_book_theme"]
-testing = ["coverage", "pytest", "pytest-cov", "pytest-regressions"]
-
-[[package]]
 name = "matplotlib-inline"
 version = "0.1.6"
 description = "Inline Matplotlib backend for Jupyter"
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "matplotlib-inline-0.1.6.tar.gz", hash = "sha256:f887e5f10ba98e8d2b150ddcf4702c1e5f8b3a20005eb0f74bfdbd360ee6f304"},
@@ -830,52 +584,30 @@
 python-versions = ">=3.6"
 files = [
     {file = "mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {file = "mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
 
 [[package]]
-name = "mdurl"
-version = "0.1.2"
-description = "Markdown URL utilities"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
-    {file = "mdurl-0.1.2.tar.gz", hash = "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"},
-]
-
-[[package]]
 name = "mock"
-version = "5.0.2"
+version = "5.1.0"
 description = "Rolling backport of unittest.mock for all Pythons"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "mock-5.0.2-py3-none-any.whl", hash = "sha256:0e0bc5ba78b8db3667ad636d964eb963dc97a59f04c6f6214c5f0e4a8f726c56"},
-    {file = "mock-5.0.2.tar.gz", hash = "sha256:06f18d7d65b44428202b145a9a36e99c2ee00d1eb992df0caf881d4664377891"},
+    {file = "mock-5.1.0-py3-none-any.whl", hash = "sha256:18c694e5ae8a208cdb3d2c20a993ca1a7b0efa258c247a1e565150f477f83744"},
+    {file = "mock-5.1.0.tar.gz", hash = "sha256:5e96aad5ccda4718e0a229ed94b2024df75cc2d55575ba5762d31f5767b8767d"},
 ]
 
 [package.extras]
 build = ["blurb", "twine", "wheel"]
 docs = ["sphinx"]
 test = ["pytest", "pytest-cov"]
 
 [[package]]
-name = "more-itertools"
-version = "9.1.0"
-description = "More routines for operating on iterables, beyond itertools"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "more-itertools-9.1.0.tar.gz", hash = "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d"},
-    {file = "more_itertools-9.1.0-py3-none-any.whl", hash = "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"},
-]
-
-[[package]]
 name = "mypy"
 version = "1.4.1"
 description = "Optional static typing for Python"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "mypy-1.4.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8"},
@@ -988,36 +720,22 @@
 python-versions = "*"
 files = [
     {file = "pickleshare-0.7.5-py2.py3-none-any.whl", hash = "sha256:9649af414d74d4df115d5d718f82acb59c9d418196b7b4290ed47a12ce62df56"},
     {file = "pickleshare-0.7.5.tar.gz", hash = "sha256:87683d47965c1da65cdacaf31c8441d12b8044cdec9aca500cd78fc2c683afca"},
 ]
 
 [[package]]
-name = "pkginfo"
-version = "1.9.6"
-description = "Query metadata from sdists / bdists / installed packages."
-optional = false
-python-versions = ">=3.6"
-files = [
-    {file = "pkginfo-1.9.6-py3-none-any.whl", hash = "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546"},
-    {file = "pkginfo-1.9.6.tar.gz", hash = "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"},
-]
-
-[package.extras]
-testing = ["pytest", "pytest-cov"]
-
-[[package]]
 name = "platformdirs"
-version = "3.8.0"
+version = "3.8.1"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-3.8.0-py3-none-any.whl", hash = "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"},
-    {file = "platformdirs-3.8.0.tar.gz", hash = "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc"},
+    {file = "platformdirs-3.8.1-py3-none-any.whl", hash = "sha256:cec7b889196b9144d088e4c57d9ceef7374f6c39694ad1577a0aab50d27ea28c"},
+    {file = "platformdirs-3.8.1.tar.gz", hash = "sha256:f87ca4fcff7d2b0f81c6a748a77973d7af0f4d526f98f308477c3c436c74d528"},
 ]
 
 [package.dependencies]
 typing-extensions = {version = ">=4.6.3", markers = "python_version < \"3.8\""}
 
 [package.extras]
 docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
@@ -1039,21 +757,21 @@
 
 [package.extras]
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
 name = "prompt-toolkit"
-version = "3.0.38"
+version = "3.0.39"
 description = "Library for building powerful interactive command lines in Python"
 optional = false
 python-versions = ">=3.7.0"
 files = [
-    {file = "prompt_toolkit-3.0.38-py3-none-any.whl", hash = "sha256:45ea77a2f7c60418850331366c81cf6b5b9cf4c7fd34616f733c5427e6abbb1f"},
-    {file = "prompt_toolkit-3.0.38.tar.gz", hash = "sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b"},
+    {file = "prompt_toolkit-3.0.39-py3-none-any.whl", hash = "sha256:9dffbe1d8acf91e3de75f3b544e4842382fc06c6babe903ac9acb74dc6e08d88"},
+    {file = "prompt_toolkit-3.0.39.tar.gz", hash = "sha256:04505ade687dc26dc4284b1ad19a83be2f2afe83e7a828ace0c72f3a1df72aac"},
 ]
 
 [package.dependencies]
 wcwidth = "*"
 
 [[package]]
 name = "ptyprocess"
@@ -1088,25 +806,14 @@
 python-versions = ">=3.6"
 files = [
     {file = "pycodestyle-2.10.0-py2.py3-none-any.whl", hash = "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"},
     {file = "pycodestyle-2.10.0.tar.gz", hash = "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053"},
 ]
 
 [[package]]
-name = "pycparser"
-version = "2.21"
-description = "C parser in Python"
-optional = false
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
-files = [
-    {file = "pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
-    {file = "pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
-]
-
-[[package]]
 name = "pyflakes"
 version = "3.0.1"
 description = "passive checker of Python programs"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "pyflakes-3.0.1-py2.py3-none-any.whl", hash = "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf"},
@@ -1125,21 +832,21 @@
 ]
 
 [package.extras]
 plugins = ["importlib-metadata"]
 
 [[package]]
 name = "pyproject-api"
-version = "1.5.2"
+version = "1.5.3"
 description = "API to interact with the python pyproject.toml based projects"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pyproject_api-1.5.2-py3-none-any.whl", hash = "sha256:9cffcbfb64190f207444d7579d315f3278f2c04ba46d685fad93197b5326d348"},
-    {file = "pyproject_api-1.5.2.tar.gz", hash = "sha256:999f58fa3c92b23ebd31a6bad5d1f87d456744d75e05391be7f5c729015d3d91"},
+    {file = "pyproject_api-1.5.3-py3-none-any.whl", hash = "sha256:14cf09828670c7b08842249c1f28c8ee6581b872e893f81b62d5465bec41502f"},
+    {file = "pyproject_api-1.5.3.tar.gz", hash = "sha256:ffb5b2d7cad43f5b2688ab490de7c4d3f6f15e0b819cb588c4b771567c9729eb"},
 ]
 
 [package.dependencies]
 packaging = ">=23.1"
 tomli = {version = ">=2.0.1", markers = "python_version < \"3.11\""}
 
 [package.extras]
@@ -1180,44 +887,14 @@
 pluggy = ">=0.12,<2.0"
 tomli = {version = ">=1.0.0", markers = "python_version < \"3.11\""}
 
 [package.extras]
 testing = ["argcomplete", "attrs (>=19.2.0)", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
 
 [[package]]
-name = "pywin32-ctypes"
-version = "0.2.2"
-description = "A (partial) reimplementation of pywin32 using ctypes/cffi"
-optional = false
-python-versions = ">=3.6"
-files = [
-    {file = "pywin32-ctypes-0.2.2.tar.gz", hash = "sha256:3426e063bdd5fd4df74a14fa3cf80a0b42845a87e1d1e81f6549f9daec593a60"},
-    {file = "pywin32_ctypes-0.2.2-py3-none-any.whl", hash = "sha256:bf490a1a709baf35d688fe0ecf980ed4de11d2b3e37b51e5442587a75d9957e7"},
-]
-
-[[package]]
-name = "readme-renderer"
-version = "37.3"
-description = "readme_renderer is a library for rendering \"readme\" descriptions for Warehouse"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "readme_renderer-37.3-py3-none-any.whl", hash = "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"},
-    {file = "readme_renderer-37.3.tar.gz", hash = "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273"},
-]
-
-[package.dependencies]
-bleach = ">=2.1.0"
-docutils = ">=0.13.1"
-Pygments = ">=2.5.1"
-
-[package.extras]
-md = ["cmarkgfm (>=0.8.0)"]
-
-[[package]]
 name = "requests"
 version = "2.31.0"
 description = "Python HTTP for Humans."
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "requests-2.31.0-py3-none-any.whl", hash = "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f"},
@@ -1231,114 +908,14 @@
 urllib3 = ">=1.21.1,<3"
 
 [package.extras]
 socks = ["PySocks (>=1.5.6,!=1.5.7)"]
 use-chardet-on-py3 = ["chardet (>=3.0.2,<6)"]
 
 [[package]]
-name = "requests-toolbelt"
-version = "1.0.0"
-description = "A utility belt for advanced users of python-requests"
-optional = false
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
-files = [
-    {file = "requests-toolbelt-1.0.0.tar.gz", hash = "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6"},
-    {file = "requests_toolbelt-1.0.0-py2.py3-none-any.whl", hash = "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"},
-]
-
-[package.dependencies]
-requests = ">=2.0.1,<3.0.0"
-
-[[package]]
-name = "rfc3986"
-version = "2.0.0"
-description = "Validating URI References per RFC 3986"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "rfc3986-2.0.0-py2.py3-none-any.whl", hash = "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd"},
-    {file = "rfc3986-2.0.0.tar.gz", hash = "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"},
-]
-
-[package.extras]
-idna2008 = ["idna"]
-
-[[package]]
-name = "rich"
-version = "13.4.2"
-description = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
-optional = false
-python-versions = ">=3.7.0"
-files = [
-    {file = "rich-13.4.2-py3-none-any.whl", hash = "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec"},
-    {file = "rich-13.4.2.tar.gz", hash = "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"},
-]
-
-[package.dependencies]
-markdown-it-py = ">=2.2.0"
-pygments = ">=2.13.0,<3.0.0"
-typing-extensions = {version = ">=4.0.0,<5.0", markers = "python_version < \"3.9\""}
-
-[package.extras]
-jupyter = ["ipywidgets (>=7.5.1,<9)"]
-
-[[package]]
-name = "secretstorage"
-version = "3.3.3"
-description = "Python bindings to FreeDesktop.org Secret Service API"
-optional = false
-python-versions = ">=3.6"
-files = [
-    {file = "SecretStorage-3.3.3-py3-none-any.whl", hash = "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"},
-    {file = "SecretStorage-3.3.3.tar.gz", hash = "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77"},
-]
-
-[package.dependencies]
-cryptography = ">=2.0"
-jeepney = ">=0.6"
-
-[[package]]
-name = "setuptools"
-version = "68.0.0"
-description = "Easily download, build, install, upgrade, and uninstall Python packages"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "setuptools-68.0.0-py3-none-any.whl", hash = "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f"},
-    {file = "setuptools-68.0.0.tar.gz", hash = "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"},
-]
-
-[package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-hoverxref (<2)", "sphinx-inline-tabs", "sphinx-lint", "sphinx-notfound-page (==0.8.3)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
-testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-ruff", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
-testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
-
-[[package]]
-name = "setuptools-scm"
-version = "7.1.0"
-description = "the blessed package to manage your versions by scm tags"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "setuptools_scm-7.1.0-py3-none-any.whl", hash = "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"},
-    {file = "setuptools_scm-7.1.0.tar.gz", hash = "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27"},
-]
-
-[package.dependencies]
-importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
-packaging = ">=20.0"
-setuptools = "*"
-tomli = {version = ">=1.0.0", markers = "python_version < \"3.11\""}
-typing-extensions = "*"
-
-[package.extras]
-test = ["pytest (>=6.2)", "virtualenv (>20)"]
-toml = ["setuptools (>=42)"]
-
-[[package]]
 name = "six"
 version = "1.16.0"
 description = "Python 2 and 3 compatibility utilities"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 files = [
     {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
@@ -1384,40 +961,40 @@
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tox"
-version = "4.6.3"
+version = "4.6.4"
 description = "tox is a generic virtualenv management and test command line tool"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "tox-4.6.3-py3-none-any.whl", hash = "sha256:2946a0bb38924c3a9f9575c7fb4ca1f4c11a7c69c61592f176778892155cb50c"},
-    {file = "tox-4.6.3.tar.gz", hash = "sha256:9e2c5091a117d03b583c57c4c40aecd068099c17d40520e7b165e85c19334534"},
+    {file = "tox-4.6.4-py3-none-any.whl", hash = "sha256:1b8f8ae08d6a5475cad9d508236c51ea060620126fd7c3c513d0f5c7f29cc776"},
+    {file = "tox-4.6.4.tar.gz", hash = "sha256:5e2ad8845764706170d3dcaac171704513cc8a725655219acb62fe4380bdadda"},
 ]
 
 [package.dependencies]
 cachetools = ">=5.3.1"
 chardet = ">=5.1"
 colorama = ">=0.4.6"
 filelock = ">=3.12.2"
-importlib-metadata = {version = ">=6.6", markers = "python_version < \"3.8\""}
+importlib-metadata = {version = ">=6.7", markers = "python_version < \"3.8\""}
 packaging = ">=23.1"
-platformdirs = ">=3.5.3"
-pluggy = ">=1"
+platformdirs = ">=3.8"
+pluggy = ">=1.2"
 pyproject-api = ">=1.5.2"
 tomli = {version = ">=2.0.1", markers = "python_version < \"3.11\""}
 typing-extensions = {version = ">=4.6.3", markers = "python_version < \"3.8\""}
 virtualenv = ">=20.23.1"
 
 [package.extras]
-docs = ["furo (>=2023.5.20)", "sphinx (>=7.0.1)", "sphinx-argparse-cli (>=1.11.1)", "sphinx-autodoc-typehints (>=1.23.2,!=1.23.4)", "sphinx-copybutton (>=0.5.2)", "sphinx-inline-tabs (>=2023.4.21)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
-testing = ["build[virtualenv] (>=0.10)", "covdefaults (>=2.3)", "detect-test-pollution (>=1.1.1)", "devpi-process (>=0.3.1)", "diff-cover (>=7.6)", "distlib (>=0.3.6)", "flaky (>=3.7)", "hatch-vcs (>=0.3)", "hatchling (>=1.17.1)", "psutil (>=5.9.5)", "pytest (>=7.3.2)", "pytest-cov (>=4.1)", "pytest-mock (>=3.11.1)", "pytest-xdist (>=3.3.1)", "re-assert (>=1.1)", "time-machine (>=2.10)", "wheel (>=0.40)"]
+docs = ["furo (>=2023.5.20)", "sphinx (>=7.0.1)", "sphinx-argparse-cli (>=1.11.1)", "sphinx-autodoc-typehints (>=1.23.3,!=1.23.4)", "sphinx-copybutton (>=0.5.2)", "sphinx-inline-tabs (>=2023.4.21)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
+testing = ["build[virtualenv] (>=0.10)", "covdefaults (>=2.3)", "detect-test-pollution (>=1.1.1)", "devpi-process (>=0.3.1)", "diff-cover (>=7.6)", "distlib (>=0.3.6)", "flaky (>=3.7)", "hatch-vcs (>=0.3)", "hatchling (>=1.17.1)", "psutil (>=5.9.5)", "pytest (>=7.4)", "pytest-cov (>=4.1)", "pytest-mock (>=3.11.1)", "pytest-xdist (>=3.3.1)", "re-assert (>=1.1)", "time-machine (>=2.10)", "wheel (>=0.40)"]
 
 [[package]]
 name = "traitlets"
 version = "5.9.0"
 description = "Traitlets Python configuration system"
 optional = false
 python-versions = ">=3.7"
@@ -1427,66 +1004,61 @@
 ]
 
 [package.extras]
 docs = ["myst-parser", "pydata-sphinx-theme", "sphinx"]
 test = ["argcomplete (>=2.0)", "pre-commit", "pytest", "pytest-mock"]
 
 [[package]]
-name = "twine"
-version = "4.0.2"
-description = "Collection of utilities for publishing packages on PyPI"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "twine-4.0.2-py3-none-any.whl", hash = "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8"},
-    {file = "twine-4.0.2.tar.gz", hash = "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"},
-]
-
-[package.dependencies]
-importlib-metadata = ">=3.6"
-keyring = ">=15.1"
-pkginfo = ">=1.8.1"
-readme-renderer = ">=35.0"
-requests = ">=2.20"
-requests-toolbelt = ">=0.8.0,<0.9.0 || >0.9.0"
-rfc3986 = ">=1.4.0"
-rich = ">=12.0.0"
-urllib3 = ">=1.26.0"
-
-[[package]]
 name = "typed-ast"
-version = "1.5.4"
+version = "1.5.5"
 description = "a fork of Python 2 and 3 ast modules with type comment support"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "typed_ast-1.5.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:669dd0c4167f6f2cd9f57041e03c3c2ebf9063d0757dc89f79ba1daa2bfca9d4"},
-    {file = "typed_ast-1.5.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:211260621ab1cd7324e0798d6be953d00b74e0428382991adfddb352252f1d62"},
-    {file = "typed_ast-1.5.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:267e3f78697a6c00c689c03db4876dd1efdfea2f251a5ad6555e82a26847b4ac"},
-    {file = "typed_ast-1.5.4-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:c542eeda69212fa10a7ada75e668876fdec5f856cd3d06829e6aa64ad17c8dfe"},
-    {file = "typed_ast-1.5.4-cp310-cp310-win_amd64.whl", hash = "sha256:a9916d2bb8865f973824fb47436fa45e1ebf2efd920f2b9f99342cb7fab93f72"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:79b1e0869db7c830ba6a981d58711c88b6677506e648496b1f64ac7d15633aec"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a94d55d142c9265f4ea46fab70977a1944ecae359ae867397757d836ea5a3f47"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:183afdf0ec5b1b211724dfef3d2cad2d767cbefac291f24d69b00546c1837fb6"},
-    {file = "typed_ast-1.5.4-cp36-cp36m-win_amd64.whl", hash = "sha256:639c5f0b21776605dd6c9dbe592d5228f021404dafd377e2b7ac046b0349b1a1"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:cf4afcfac006ece570e32d6fa90ab74a17245b83dfd6655a6f68568098345ff6"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ed855bbe3eb3715fca349c80174cfcfd699c2f9de574d40527b8429acae23a66"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:6778e1b2f81dfc7bc58e4b259363b83d2e509a65198e85d5700dfae4c6c8ff1c"},
-    {file = "typed_ast-1.5.4-cp37-cp37m-win_amd64.whl", hash = "sha256:0261195c2062caf107831e92a76764c81227dae162c4f75192c0d489faf751a2"},
-    {file = "typed_ast-1.5.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2efae9db7a8c05ad5547d522e7dbe62c83d838d3906a3716d1478b6c1d61388d"},
-    {file = "typed_ast-1.5.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:7d5d014b7daa8b0bf2eaef684295acae12b036d79f54178b92a2b6a56f92278f"},
-    {file = "typed_ast-1.5.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:370788a63915e82fd6f212865a596a0fefcbb7d408bbbb13dea723d971ed8bdc"},
-    {file = "typed_ast-1.5.4-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:4e964b4ff86550a7a7d56345c7864b18f403f5bd7380edf44a3c1fb4ee7ac6c6"},
-    {file = "typed_ast-1.5.4-cp38-cp38-win_amd64.whl", hash = "sha256:683407d92dc953c8a7347119596f0b0e6c55eb98ebebd9b23437501b28dcbb8e"},
-    {file = "typed_ast-1.5.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4879da6c9b73443f97e731b617184a596ac1235fe91f98d279a7af36c796da35"},
-    {file = "typed_ast-1.5.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3e123d878ba170397916557d31c8f589951e353cc95fb7f24f6bb69adc1a8a97"},
-    {file = "typed_ast-1.5.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ebd9d7f80ccf7a82ac5f88c521115cc55d84e35bf8b446fcd7836eb6b98929a3"},
-    {file = "typed_ast-1.5.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:98f80dee3c03455e92796b58b98ff6ca0b2a6f652120c263efdba4d6c5e58f72"},
-    {file = "typed_ast-1.5.4-cp39-cp39-win_amd64.whl", hash = "sha256:0fdbcf2fef0ca421a3f5912555804296f0b0960f0418c440f5d6d3abb549f3e1"},
-    {file = "typed_ast-1.5.4.tar.gz", hash = "sha256:39e21ceb7388e4bb37f4c679d72707ed46c2fbf2a5609b8b8ebc4b067d977df2"},
+    {file = "typed_ast-1.5.5-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:4bc1efe0ce3ffb74784e06460f01a223ac1f6ab31c6bc0376a21184bf5aabe3b"},
+    {file = "typed_ast-1.5.5-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:5f7a8c46a8b333f71abd61d7ab9255440d4a588f34a21f126bbfc95f6049e686"},
+    {file = "typed_ast-1.5.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:597fc66b4162f959ee6a96b978c0435bd63791e31e4f410622d19f1686d5e769"},
+    {file = "typed_ast-1.5.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d41b7a686ce653e06c2609075d397ebd5b969d821b9797d029fccd71fdec8e04"},
+    {file = "typed_ast-1.5.5-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:5fe83a9a44c4ce67c796a1b466c270c1272e176603d5e06f6afbc101a572859d"},
+    {file = "typed_ast-1.5.5-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d5c0c112a74c0e5db2c75882a0adf3133adedcdbfd8cf7c9d6ed77365ab90a1d"},
+    {file = "typed_ast-1.5.5-cp310-cp310-win_amd64.whl", hash = "sha256:e1a976ed4cc2d71bb073e1b2a250892a6e968ff02aa14c1f40eba4f365ffec02"},
+    {file = "typed_ast-1.5.5-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:c631da9710271cb67b08bd3f3813b7af7f4c69c319b75475436fcab8c3d21bee"},
+    {file = "typed_ast-1.5.5-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b445c2abfecab89a932b20bd8261488d574591173d07827c1eda32c457358b18"},
+    {file = "typed_ast-1.5.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cc95ffaaab2be3b25eb938779e43f513e0e538a84dd14a5d844b8f2932593d88"},
+    {file = "typed_ast-1.5.5-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:61443214d9b4c660dcf4b5307f15c12cb30bdfe9588ce6158f4a005baeb167b2"},
+    {file = "typed_ast-1.5.5-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:6eb936d107e4d474940469e8ec5b380c9b329b5f08b78282d46baeebd3692dc9"},
+    {file = "typed_ast-1.5.5-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e48bf27022897577d8479eaed64701ecaf0467182448bd95759883300ca818c8"},
+    {file = "typed_ast-1.5.5-cp311-cp311-win_amd64.whl", hash = "sha256:83509f9324011c9a39faaef0922c6f720f9623afe3fe220b6d0b15638247206b"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:44f214394fc1af23ca6d4e9e744804d890045d1643dd7e8229951e0ef39429b5"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:118c1ce46ce58fda78503eae14b7664163aa735b620b64b5b725453696f2a35c"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:be4919b808efa61101456e87f2d4c75b228f4e52618621c77f1ddcaae15904fa"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:fc2b8c4e1bc5cd96c1a823a885e6b158f8451cf6f5530e1829390b4d27d0807f"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:16f7313e0a08c7de57f2998c85e2a69a642e97cb32f87eb65fbfe88381a5e44d"},
+    {file = "typed_ast-1.5.5-cp36-cp36m-win_amd64.whl", hash = "sha256:2b946ef8c04f77230489f75b4b5a4a6f24c078be4aed241cfabe9cbf4156e7e5"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:2188bc33d85951ea4ddad55d2b35598b2709d122c11c75cffd529fbc9965508e"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0635900d16ae133cab3b26c607586131269f88266954eb04ec31535c9a12ef1e"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:57bfc3cf35a0f2fdf0a88a3044aafaec1d2f24d8ae8cd87c4f58d615fb5b6311"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:fe58ef6a764de7b4b36edfc8592641f56e69b7163bba9f9c8089838ee596bfb2"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d09d930c2d1d621f717bb217bf1fe2584616febb5138d9b3e8cdd26506c3f6d4"},
+    {file = "typed_ast-1.5.5-cp37-cp37m-win_amd64.whl", hash = "sha256:d40c10326893ecab8a80a53039164a224984339b2c32a6baf55ecbd5b1df6431"},
+    {file = "typed_ast-1.5.5-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:fd946abf3c31fb50eee07451a6aedbfff912fcd13cf357363f5b4e834cc5e71a"},
+    {file = "typed_ast-1.5.5-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:ed4a1a42df8a3dfb6b40c3d2de109e935949f2f66b19703eafade03173f8f437"},
+    {file = "typed_ast-1.5.5-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:045f9930a1550d9352464e5149710d56a2aed23a2ffe78946478f7b5416f1ede"},
+    {file = "typed_ast-1.5.5-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:381eed9c95484ceef5ced626355fdc0765ab51d8553fec08661dce654a935db4"},
+    {file = "typed_ast-1.5.5-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:bfd39a41c0ef6f31684daff53befddae608f9daf6957140228a08e51f312d7e6"},
+    {file = "typed_ast-1.5.5-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:8c524eb3024edcc04e288db9541fe1f438f82d281e591c548903d5b77ad1ddd4"},
+    {file = "typed_ast-1.5.5-cp38-cp38-win_amd64.whl", hash = "sha256:7f58fabdde8dcbe764cef5e1a7fcb440f2463c1bbbec1cf2a86ca7bc1f95184b"},
+    {file = "typed_ast-1.5.5-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:042eb665ff6bf020dd2243307d11ed626306b82812aba21836096d229fdc6a10"},
+    {file = "typed_ast-1.5.5-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:622e4a006472b05cf6ef7f9f2636edc51bda670b7bbffa18d26b255269d3d814"},
+    {file = "typed_ast-1.5.5-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1efebbbf4604ad1283e963e8915daa240cb4bf5067053cf2f0baadc4d4fb51b8"},
+    {file = "typed_ast-1.5.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f0aefdd66f1784c58f65b502b6cf8b121544680456d1cebbd300c2c813899274"},
+    {file = "typed_ast-1.5.5-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:48074261a842acf825af1968cd912f6f21357316080ebaca5f19abbb11690c8a"},
+    {file = "typed_ast-1.5.5-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:429ae404f69dc94b9361bb62291885894b7c6fb4640d561179548c849f8492ba"},
+    {file = "typed_ast-1.5.5-cp39-cp39-win_amd64.whl", hash = "sha256:335f22ccb244da2b5c296e6f96b06ee9bed46526db0de38d2f0e5a6597b81155"},
+    {file = "typed_ast-1.5.5.tar.gz", hash = "sha256:94282f7a354f36ef5dbce0ef3467ebf6a258e370ab33d5b40c249fa996e590dd"},
 ]
 
 [[package]]
 name = "types-mock"
 version = "5.0.0.7"
 description = "Typing stubs for mock"
 optional = false
@@ -1541,21 +1113,21 @@
 files = [
     {file = "types-urllib3-1.26.25.13.tar.gz", hash = "sha256:3300538c9dc11dad32eae4827ac313f5d986b8b21494801f1bf97a1ac6c03ae5"},
     {file = "types_urllib3-1.26.25.13-py3-none-any.whl", hash = "sha256:5dbd1d2bef14efee43f5318b5d36d805a489f6600252bb53626d4bfafd95e27c"},
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.7.0"
+version = "4.7.1"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "typing_extensions-4.7.0-py3-none-any.whl", hash = "sha256:5d8c9dac95c27d20df12fb1d97b9793ab8b2af8a3a525e68c80e21060c161771"},
-    {file = "typing_extensions-4.7.0.tar.gz", hash = "sha256:935ccf31549830cda708b42289d44b6f74084d616a00be651601a4f968e77c82"},
+    {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
+    {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
 ]
 
 [[package]]
 name = "urllib3"
 version = "2.0.3"
 description = "HTTP library with thread-safe connection pooling, file post, and more."
 optional = false
@@ -1600,25 +1172,14 @@
 python-versions = "*"
 files = [
     {file = "wcwidth-0.2.6-py2.py3-none-any.whl", hash = "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e"},
     {file = "wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
 
 [[package]]
-name = "webencodings"
-version = "0.5.1"
-description = "Character encoding aliases for legacy web content"
-optional = false
-python-versions = "*"
-files = [
-    {file = "webencodings-0.5.1-py2.py3-none-any.whl", hash = "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78"},
-    {file = "webencodings-0.5.1.tar.gz", hash = "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"},
-]
-
-[[package]]
 name = "zipp"
 version = "3.15.0"
 description = "Backport of pathlib-compatible object wrapper for zip files"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
@@ -1628,8 +1189,8 @@
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = ">=3.7"
-content-hash = "d7e825986463a9d73dc264129fadb8959ba469a4015f1108b33dd93d87e17357"
+content-hash = "47a384a5974b39eb336182b7e87f6aca86e7646db966446d16f5578816b588ec"
```

### Comparing `Mesh-Client-2.0.1/pyproject.toml` & `Mesh-Client-2.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Mesh-Client"
-version = "2.0.1"
+version = "2.1.1"
 description = "Client for NHS England's MESH messaging system"
 repository = "https://github.com/NHSDigital/mesh-client"
 authors = ["spinecore"]
 license = "MIT"
 packages = [
     { include = "mesh_client" },
 ]
@@ -23,36 +23,36 @@
 #    "py.typed",
 #    "*.pem"
 #]
 
 [tool.poetry.dependencies]
 # core dependencies
 python = ">=3.7"
-requests = ">=2.9.0"
+requests = ">=2.26.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = {version = "^5.12.0", python = ">=3.8"}
 mypy = "^1.4.1"
 flake8 = {version = "^6.0.0", python = ">=3.8.1"}
 flake8-pyproject = "^1.2.3"
 flake8-black = "^0.3.6"
 types-six = "^1.16.21.8"
 types-requests = "^2.31.0.1"
 types-mock = "^5.0.0.7"
 mock = "^5.0.2"
 build = "^0.10.0"
-twine = "^4.0.2"
 toml = "^0.10.2"
-setuptools-scm = "^7.1.0"
 tox = "^4.6.3"
 types-pkg-resources = "^0.1.3"
 coverage = "^7.2.7"
 pytest = "^7.4.0"
+importlib-metadata = {version = ">=4.11.4", python = "<3.12"}
+#importlib-resources = {version = "*", python = "<3.9"}
 
 [tool.poetry.group.local.dependencies]
 ipython = {version = "^8.14.0", python = ">=3.9,<4.0"}
 
 
 [tool.pytest.ini_options]
 #asyncio_mode = "auto"
@@ -110,16 +110,15 @@
     RELEASE_VERSION=1.2.3
 
 [testenv]
 wheel_build_env = .pkg
 use_develop = true
 package = wheel
 deps =
-    requests>=2.9.0
-    six>=1.10.0
+    requests>=2.26.0
     mock
     pytest
 commands =
     python -m pytest
 
 """
```

### Comparing `Mesh-Client-2.0.1/scripts/check-secrets.sh` & `Mesh-Client-2.1.1/scripts/check-secrets.sh`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/scripts/sonar_tests.py` & `Mesh-Client-2.1.1/scripts/sonar_tests.py`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/setup.py` & `Mesh-Client-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/ca.cert.pem` & `Mesh-Client-2.1.1/tests/ca.cert.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/ca.key.pem` & `Mesh-Client-2.1.1/tests/ca.key.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/client.cert.pem` & `Mesh-Client-2.1.1/tests/client.cert.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/client.key.pem` & `Mesh-Client-2.1.1/tests/client.key.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/helpers.py` & `Mesh-Client-2.1.1/tests/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 Usable default values for verify and cert, providing certificates and keys
 which should work with mock_server. Note that these certs will not work with
 any NHS Digital test environments - such certs must be obtained from
 NHS Digital.
 """
 default_ssl_opts = MOCK_SSL_OPTS
 
-LOCAL_MOCK_ENDPOINT = Endpoint("https://localhost:8000", MOCK_CA_CERT, (MOCK_CERT, MOCK_KEY), False)
-LOCAL_FAKE_ENDPOINT = Endpoint("https://localhost:8829", MOCK_CA_CERT, (MOCK_CERT, MOCK_KEY), False)
-SANDBOX_ENDPOINT = Endpoint("https://localhost:8701", MOCK_CA_CERT, (MOCK_CERT, MOCK_KEY), False)
+LOCAL_MOCK_ENDPOINT = Endpoint("https://localhost:8000", MOCK_CA_CERT, (MOCK_CERT, MOCK_KEY), False, False)
+LOCAL_FAKE_ENDPOINT = Endpoint("https://localhost:8829", MOCK_CA_CERT, (MOCK_CERT, MOCK_KEY), False, False)
+SANDBOX_ENDPOINT = Endpoint("https://localhost:8701", MOCK_CA_CERT, (MOCK_CERT, MOCK_KEY), False, False)
 
 
 @contextlib.contextmanager
 def temp_env_vars(**kwargs):
     """
     Temporarily set the process environment variables.
     >>> with temp_env_vars(PLUGINS_DIR=u'test/plugins'):
```

### Comparing `Mesh-Client-2.0.1/tests/io_helpers_tests.py` & `Mesh-Client-2.1.1/tests/io_helpers_tests.py`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/mesh_chunk_retries_tests.py` & `Mesh-Client-2.1.1/tests/mesh_chunk_retries_tests.py`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/mesh_client_tests.py` & `Mesh-Client-2.1.1/tests/mesh_client_tests.py`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/mesh_sandbox_tests.py` & `Mesh-Client-2.1.1/tests/mesh_sandbox_tests.py`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/mock_server.py` & `Mesh-Client-2.1.1/tests/mock_server.py`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/server.cert.pem` & `Mesh-Client-2.1.1/tests/server.cert.pem`

 * *Files identical despite different names*

### Comparing `Mesh-Client-2.0.1/tests/server.key.pem` & `Mesh-Client-2.1.1/tests/server.key.pem`

 * *Files identical despite different names*

