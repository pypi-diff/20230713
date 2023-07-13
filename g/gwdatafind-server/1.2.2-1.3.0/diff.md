# Comparing `tmp/gwdatafind-server-1.2.2.tar.gz` & `tmp/gwdatafind-server-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdatafind-server-1.2.2.tar", last modified: Fri May  5 16:41:57 2023, max compression
+gzip compressed data, was "gwdatafind-server-1.3.0.tar", last modified: Thu Jul 13 15:57:17 2023, max compression
```

## Comparing `gwdatafind-server-1.2.2.tar` & `gwdatafind-server-1.3.0.tar`

### file list

```diff
@@ -1,55 +1,85 @@
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    35149 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/LICENSE
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      175 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/MANIFEST.in
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1895 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/PKG-INFO
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      627 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/README.md
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.394240 gwdatafind-server-1.2.2/config/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      691 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/config/gunicorn.conf
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     6737 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/config/gunicorn.conf.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2174 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/config/gwdatafind-server.ini
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      386 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/config/gwdatafind-server.service
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      698 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/config/wsgi.conf
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.394240 gwdatafind-server-1.2.2/debian/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2294 2023-05-05 16:33:14.000000 gwdatafind-server-1.2.2/debian/changelog
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        2 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/compat
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1446 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/control
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1048 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/copyright
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       16 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/gwdatafind-server.docs
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      212 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/gwdatafind-server.install
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       16 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/python3-gwdatafind-server.docs
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       30 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/python3-gwdatafind-server.install
--rwxrwxr-x   0 duncan    (1001) duncan    (1001)       82 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/rules
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.394240 gwdatafind-server-1.2.2/debian/source/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       12 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/debian/source/format
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.394240 gwdatafind-server-1.2.2/gwdatafind_server/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      543 2023-05-05 16:33:14.000000 gwdatafind-server-1.2.2/gwdatafind_server/__init__.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/gwdatafind_server/api/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      200 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/api/__init__.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      669 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/api/base.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1914 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/api/utils.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)    10881 2023-05-05 16:10:07.000000 gwdatafind-server-1.2.2/gwdatafind_server/api/v1.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4223 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/app.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4894 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/authentication.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     8011 2023-04-06 20:05:11.000000 gwdatafind-server-1.2.2/gwdatafind_server/cache.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      974 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/gwdatafind_server/config.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1895 2023-05-05 16:41:57.000000 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/PKG-INFO
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1158 2023-05-05 16:41:57.000000 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/SOURCES.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)        1 2023-05-05 16:41:57.000000 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/dependency_links.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       77 2023-05-05 16:41:57.000000 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/requires.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       18 2023-05-05 16:41:57.000000 gwdatafind-server-1.2.2/gwdatafind_server.egg-info/top_level.txt
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      727 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/pyproject.toml
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     4955 2023-05-05 16:33:14.000000 gwdatafind-server-1.2.2/python-gwdatafind-server.spec
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1475 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/setup.cfg
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      196 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/setup.py
-drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-05-05 16:41:57.398239 gwdatafind-server-1.2.2/tests/
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      702 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/cache.dat
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      369 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/conftest.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)       77 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/grid-mapfile
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      546 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/gwdatafind-server.ini
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     5654 2023-05-05 16:10:07.000000 gwdatafind-server-1.2.2/tests/test_api_v1.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      335 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/test_app.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     2518 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/test_authentication_scitokens.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)     1505 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/test_authentication_x509.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      790 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/test_config.py
--rw-rw-r--   0 duncan    (1001) duncan    (1001)      480 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.2/tests/utils.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      221 2023-07-13 14:54:11.000000 gwdatafind-server-1.3.0/.gitignore
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.906592 gwdatafind-server-1.3.0/.gitlab/
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.906592 gwdatafind-server-1.3.0/.gitlab/ci/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1079 2023-07-06 17:18:28.000000 gwdatafind-server-1.3.0/.gitlab/ci/analysis.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      571 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/.gitlab/ci/coverage.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     3932 2023-07-13 14:54:11.000000 gwdatafind-server-1.3.0/.gitlab/ci/debian.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      636 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/.gitlab/ci/dist.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      942 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/.gitlab/ci/docker.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1392 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/.gitlab/ci/docs.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1341 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/.gitlab/ci/python.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     3561 2023-07-13 14:54:11.000000 gwdatafind-server-1.3.0/.gitlab/ci/rhel.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1075 2023-07-13 14:54:11.000000 gwdatafind-server-1.3.0/.gitlab/ci/test.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      777 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/.gitlab-ci.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      113 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/.gitmodules
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1345 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/Dockerfile
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)    35149 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/LICENSE
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      175 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/MANIFEST.in
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1895 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/PKG-INFO
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      627 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/README.md
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.906592 gwdatafind-server-1.3.0/config/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      691 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/config/gunicorn.conf
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     6737 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/config/gunicorn.conf.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     2701 2023-07-06 17:18:28.000000 gwdatafind-server-1.3.0/config/gwdatafind-server.ini
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      386 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/config/gwdatafind-server.service
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      698 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/config/wsgi.conf
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/debian/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     2503 2023-07-13 15:56:24.000000 gwdatafind-server-1.3.0/debian/changelog
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)        2 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/debian/compat
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1497 2023-07-13 14:54:11.000000 gwdatafind-server-1.3.0/debian/control
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1048 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/debian/copyright
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       16 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/debian/gwdatafind-server.docs
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      212 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/debian/gwdatafind-server.install
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1327 2023-07-06 17:18:28.000000 gwdatafind-server-1.3.0/debian/gwdatafind-server.postinst
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       16 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/debian/python3-gwdatafind-server.docs
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       30 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/debian/python3-gwdatafind-server.install
+-rwxrwxr-x   0 duncan    (1001) duncan    (1001)       82 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/debian/rules
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/debian/source/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       12 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/debian/source/format
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/docker/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)    21954 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/docker/httpd.conf
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      452 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/docker/supervisord.conf
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      752 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/docker-compose.yml
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/docs/
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/docs/api/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      742 2023-07-13 15:56:24.000000 gwdatafind-server-1.3.0/docs/api/index.md
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     8941 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/docs/api/v1.md
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1430 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/docs/configuration.md
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      849 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/docs/index.md
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      122 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/docs/requirements.txt
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/gwdatafind_server/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      647 2023-07-13 14:54:11.000000 gwdatafind-server-1.3.0/gwdatafind_server/__init__.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      160 2023-07-13 15:57:17.000000 gwdatafind-server-1.3.0/gwdatafind_server/_version.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/gwdatafind_server/api/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      200 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/gwdatafind_server/api/__init__.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      669 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/gwdatafind_server/api/base.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     2572 2023-07-06 17:18:28.000000 gwdatafind-server-1.3.0/gwdatafind_server/api/utils.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)    11132 2023-07-06 17:18:28.000000 gwdatafind-server-1.3.0/gwdatafind_server/api/v1.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     4223 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/gwdatafind_server/app.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     4894 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/gwdatafind_server/authentication.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     8011 2023-04-06 20:05:11.000000 gwdatafind-server-1.3.0/gwdatafind_server/cache.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      974 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/gwdatafind_server/config.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      436 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/gwdatafind_server/gwdatafind_server.wsgi
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/gwdatafind_server.egg-info/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1895 2023-07-13 15:57:17.000000 gwdatafind-server-1.3.0/gwdatafind_server.egg-info/PKG-INFO
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1669 2023-07-13 15:57:17.000000 gwdatafind-server-1.3.0/gwdatafind_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)        1 2023-07-13 15:57:17.000000 gwdatafind-server-1.3.0/gwdatafind_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       77 2023-07-13 15:57:17.000000 gwdatafind-server-1.3.0/gwdatafind_server.egg-info/requires.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       18 2023-07-13 15:57:17.000000 gwdatafind-server-1.3.0/gwdatafind_server.egg-info/top_level.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1272 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/mkdocs.yml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      826 2023-07-13 14:54:11.000000 gwdatafind-server-1.3.0/pyproject.toml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     5311 2023-07-13 15:56:24.000000 gwdatafind-server-1.3.0/python-gwdatafind-server.spec
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1475 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/setup.cfg
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      216 2023-07-13 14:54:11.000000 gwdatafind-server-1.3.0/setup.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-07-13 15:57:17.910592 gwdatafind-server-1.3.0/tests/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      824 2023-07-06 17:18:28.000000 gwdatafind-server-1.3.0/tests/cache.dat
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      369 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/tests/conftest.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       77 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/tests/grid-mapfile
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      629 2023-07-06 17:18:28.000000 gwdatafind-server-1.3.0/tests/gwdatafind-server.ini
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     6329 2023-07-06 17:18:28.000000 gwdatafind-server-1.3.0/tests/test_api_v1.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      335 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/tests/test_app.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     2518 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/tests/test_authentication_scitokens.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1505 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/tests/test_authentication_x509.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      790 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/tests/test_config.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      480 2023-03-19 17:06:06.000000 gwdatafind-server-1.3.0/tests/utils.py
```

### Comparing `gwdatafind-server-1.2.2/LICENSE` & `gwdatafind-server-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/PKG-INFO` & `gwdatafind-server-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdatafind-server
-Version: 1.2.2
+Version: 1.3.0
 Summary: The server library for the GWDataFind service
 Home-page: https://git.ligo.org/computing/gwdatafind/server
 Author: Duncan Meacher
 Author-email: duncan.meacher@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://git.ligo.org/computing/gwdatafind/server/-/issues
 Project-URL: Documentation, https://computing.docs.ligo.org/gwdatafind/server/
```

### Comparing `gwdatafind-server-1.2.2/README.md` & `gwdatafind-server-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/config/gunicorn.conf` & `gwdatafind-server-1.3.0/config/gunicorn.conf`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/config/gunicorn.conf.py` & `gwdatafind-server-1.3.0/config/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/config/wsgi.conf` & `gwdatafind-server-1.3.0/config/wsgi.conf`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/debian/changelog` & `gwdatafind-server-1.3.0/debian/changelog`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+gwdatafind-server (1.3.0-1) stable; urgency=low
+
+  * Improved/cleaned up build and CI testing scripts
+  * Added OSDF URL support
+
+ -- Duncan Meacher <duncan.meacher@ligo.org>  Thu, 13 Jul 2023 00:00:00 +0100
+
 gwdatafind-server (1.2.2-1) stable; urgency=low
 
   * Fixed bug in single file queries
   * Fixed bug in search for fractional GPS times
 
  -- Duncan Meacher <duncan.meacher@ligo.org>  Fri, 05 May 2023 00:00:00 +0100
```

### Comparing `gwdatafind-server-1.2.2/debian/control` & `gwdatafind-server-1.3.0/debian/control`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 Standards-Version: 3.9.1
 X-Python3-Version: >= 3.6
 Build-Depends:
  debhelper (>= 9),
  debhelper (>= 9.20160709~) | dh-systemd,
  dh-python,
  python3-all,
- python3-setuptools,
  python3-configobj,
  python3-flask (>= 1.0.0),
  python3-ligo-segments,
  python3-scitokens,
+ python3-setuptools,
+ python3-setuptools-scm,
+ python3-wheel,
 
 # -- python3-gwdatafind-server ------------------
 
 Package: python3-gwdatafind-server
 Architecture: all
 Depends:
  ${misc:Depends},
@@ -38,14 +40,15 @@
 
 Package: gwdatafind-server
 Architecture: all
 Depends:
  ${shlibs:Depends},
  ${misc:Depends},
  ${python3:Depends},
+ adduser,
  python3-gwdatafind-server (= ${binary:Version}),
  python3-gunicorn,
 Description: Server app for the GWDataFind service
  The GWDataFind service allows users to query for the location of
  files containing data from the current
  gravitational-wave detectors.
  This package provides the HTTP app configuration for a GWDataFind
```

### Comparing `gwdatafind-server-1.2.2/debian/copyright` & `gwdatafind-server-1.3.0/debian/copyright`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/gwdatafind_server/api/base.py` & `gwdatafind-server-1.3.0/gwdatafind_server/api/base.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/gwdatafind_server/api/utils.py` & `gwdatafind-server-1.3.0/gwdatafind_server/api/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -74,7 +74,29 @@
     >>> _gsiftp_url('/data/X-TEST-0-1.gwf')
     'gsiftp://datahost.example.com:15000/data/X-TEST-0-1.gwf'
     """
     config = current_app.config
     host = config.get('gsiftphost', _DEFAULT_GSIFTP_HOST)
     port = config.get('gsiftpport', _DEFAULT_GSIFTP_PORT)
     return f'gsiftp://{host}:{port}{path}'
+
+
+def _osdf_url(path):
+    """Format a POSIX ``path`` as an ``osdf://`` URL
+
+    Examples
+    --------
+    >>> _osdf_url('/cvmfs/x.storage.igwn.org/data/X-TEST-0-1.gwf')
+    'osdf:///data/X-TEST-0-1.gwf'
+    """
+    config = current_app.config
+    base = None
+    for section in filter(lambda x: x.startswith("osdf "), config):
+        prefix = config[section].get("posix_prefix", f"/cvmfs/{section}")
+        if path.startswith(prefix):
+            base = config[section].get("osdf_base_path", "")
+            break
+
+    if base is None:  # nothing found, just return the original path
+        return None
+
+    return f"osdf://{path.replace(prefix, base)}"
```

### Comparing `gwdatafind-server-1.2.2/gwdatafind_server/api/v1.py` & `gwdatafind-server-1.3.0/gwdatafind_server/api/v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from .. import authentication
 from .utils import (
     as_json,
     error_as_json,
     _file_url,
     _gsiftp_url,
+    _osdf_url,
 )
 
 blueprint = Blueprint(
     "api/v1",
     __name__,
     url_prefix="/services/data/v1",
 )
@@ -247,25 +248,39 @@
         urltype=urltype,
         latest=True,
     ))
 
 
 # -- URL matcher --------------------------------------------------------------
 
+URL_TRANSFORM = {
+    "file": _file_url,
+    "gsiftp": _gsiftp_url,
+    "osdf": _osdf_url,
+}
+
 
 def _get_latest_segment(seglist, duration):
     """Get segment for latest file of the given duration in a segment list
     """
     end = seglist[-1][1]
     return segment(end-duration, end)
 
 
-def _find_urls(ext, site, tag, start, end, urltype=None, match=None,
-               latest=False):
-    """Find all URLs for the given GPS interval
+def _find_urls(
+    ext,
+    site,
+    tag,
+    start,
+    end,
+    urltype=None,
+    match=None,
+    latest=False,
+):
+    """Find all URLs for the given GPS interval.
     """
     cache = get_dataset_cache(ext, site, tag)
 
     # parse file paths
     search = segment(float(start), float(end))
     lfns = defaultdict(list)
     maxgps = -1e9  # something absurdly old
@@ -291,28 +306,32 @@
             while gps < seg[1]:
                 if segment(gps, gps+cdur).intersects(search):
                     lfn = f'{site}-{tag}-{gps}-{cdur}.{ext}'
                     lfns[lfn].append(f'{path}/{lfn}')
                 gps += cdur
 
     # convert paths to URLs for various schemes
+    urltypes = set(URL_TRANSFORM.keys())
+    if urltype:
+        urltypes &= {urltype}
     allurls = {}
     for lfn in lfns:
         allurls[lfn] = []
         for path in lfns[lfn]:
-            # build file:// and gsiftp:// URL for each LFN
-            allurls[lfn].extend((
-                _file_url(path),
-                _gsiftp_url(path),
+            # build URL for each urltype (ignoring None)
+            allurls[lfn].extend(filter(
+                None,
+                (URL_TRANSFORM[_urlt](path) for _urlt in sorted(urltypes))
             ))
 
     # filter URLs for each LFN and return
     urls = []
     for lfn in allurls:
         urls.extend(_filter_urls(allurls[lfn], urltype=urltype, regex=match))
+
     return urls
 
 
 # -- URL filtering ------------------------------------------------------------
 
 def _filter_urls(urls, urltype=None, regex=None):
     """Filter a list of URLs that all represent the same LFN.
```

### Comparing `gwdatafind-server-1.2.2/gwdatafind_server/app.py` & `gwdatafind-server-1.3.0/gwdatafind_server/app.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/gwdatafind_server/authentication.py` & `gwdatafind-server-1.3.0/gwdatafind_server/authentication.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/gwdatafind_server/cache.py` & `gwdatafind-server-1.3.0/gwdatafind_server/cache.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/gwdatafind_server/config.py` & `gwdatafind-server-1.3.0/gwdatafind_server/config.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/gwdatafind_server.egg-info/PKG-INFO` & `gwdatafind-server-1.3.0/gwdatafind_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdatafind-server
-Version: 1.2.2
+Version: 1.3.0
 Summary: The server library for the GWDataFind service
 Home-page: https://git.ligo.org/computing/gwdatafind/server
 Author: Duncan Meacher
 Author-email: duncan.meacher@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://git.ligo.org/computing/gwdatafind/server/-/issues
 Project-URL: Documentation, https://computing.docs.ligo.org/gwdatafind/server/
```

### Comparing `gwdatafind-server-1.2.2/gwdatafind_server.egg-info/SOURCES.txt` & `gwdatafind-server-1.3.0/gwdatafind_server.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,59 @@
+.gitignore
+.gitlab-ci.yml
+.gitmodules
+Dockerfile
 LICENSE
 MANIFEST.in
 README.md
+docker-compose.yml
+mkdocs.yml
 pyproject.toml
 python-gwdatafind-server.spec
 setup.cfg
 setup.py
+.gitlab/ci/analysis.yml
+.gitlab/ci/coverage.yml
+.gitlab/ci/debian.yml
+.gitlab/ci/dist.yml
+.gitlab/ci/docker.yml
+.gitlab/ci/docs.yml
+.gitlab/ci/python.yml
+.gitlab/ci/rhel.yml
+.gitlab/ci/test.yml
 config/gunicorn.conf
 config/gunicorn.conf.py
 config/gwdatafind-server.ini
 config/gwdatafind-server.service
 config/wsgi.conf
 debian/changelog
 debian/compat
 debian/control
 debian/copyright
 debian/gwdatafind-server.docs
 debian/gwdatafind-server.install
+debian/gwdatafind-server.postinst
 debian/python3-gwdatafind-server.docs
 debian/python3-gwdatafind-server.install
 debian/rules
 debian/source/format
+docker/httpd.conf
+docker/supervisord.conf
+docs/configuration.md
+docs/index.md
+docs/requirements.txt
+docs/api/index.md
+docs/api/v1.md
 gwdatafind_server/__init__.py
+gwdatafind_server/_version.py
 gwdatafind_server/app.py
 gwdatafind_server/authentication.py
 gwdatafind_server/cache.py
 gwdatafind_server/config.py
+gwdatafind_server/gwdatafind_server.wsgi
 gwdatafind_server.egg-info/PKG-INFO
 gwdatafind_server.egg-info/SOURCES.txt
 gwdatafind_server.egg-info/dependency_links.txt
 gwdatafind_server.egg-info/requires.txt
 gwdatafind_server.egg-info/top_level.txt
 gwdatafind_server/api/__init__.py
 gwdatafind_server/api/base.py
```

### Comparing `gwdatafind-server-1.2.2/python-gwdatafind-server.spec` & `gwdatafind-server-1.3.0/python-gwdatafind-server.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 %define srcname gwdatafind-server
-%define version 1.2.2
+%define version 1.3.0
 %define release 1
 
 Name:      python-%{srcname}
 Version:   %{version}
 Release:   %{release}%{?dist}
 Summary:   The server app for the GWDataFind service
 License:   GPLv3+
@@ -14,15 +14,18 @@
 
 BuildArch: noarch
 
 # build dependencies
 BuildRequires: python-srpm-macros
 BuildRequires: python-rpm-macros
 BuildRequires: python3-rpm-macros
+BuildRequires: %__python3
 BuildRequires: python%{python3_pkgversion}-setuptools
+BuildRequires: python%{python3_pkgversion}-setuptools_scm
+BuildRequires: python%{python3_pkgversion}-wheel
 BuildRequires: systemd
 
 # these are needed for setuptools to parse the version number
 # out of gwdatafind_server/__init__.py, but only because setuptools
 # is so old on rhel (< 46.4.0, https://github.com/pypa/setuptools/pull/1753)
 %if 0%{?rhel} > 0 && 0%{?rhel} < 9
 BuildRequires: python%{python3_pkgversion}-configobj
@@ -90,19 +93,24 @@
 %__mkdir -pv %{buildroot}%{_sysconfdir}/
 %__install -m 644 -p -v config/gwdatafind-server.ini %{buildroot}%{_sysconfdir}/%{srcname}.ini
 
 # systemd
 %__mkdir -pv %{buildroot}%{_unitdir}/
 %__install -m 644 -p -v config/gwdatafind-server.service %{buildroot}%{_unitdir}/%{srcname}.service
 
-%pre
+%pre -n %{srcname}
 getent group gwdatafind >/dev/null || groupadd -r gwdatafind
 getent passwd gwdatafind >/dev/null || \
-    useradd -r -g gwdatafind -d %{_sharedstatedir} -s /sbin/nologin \
-    -c "Dedicated gwdatafind service account" gwdatafind
+useradd \
+    --system \
+    --gid gwdatafind \
+    --home-dir %{_sharedstatedir}/gwdatafind \
+    --shell /sbin/nologin \
+    --comment "Dedicated gwdatafind service account" \
+    gwdatafind
 exit 0
 
 %post -n %{srcname}
 %systemd_post %{srcname}.service
 
 %preun -n %{srcname}
 %systemd_preun %{srcname}.service
@@ -124,14 +132,17 @@
 %license LICENSE
 %{_datadir}/%{srcname}/
 %{_unitdir}/%{srcname}.service
 
 # -- changelog
 
 %changelog
+* Fri Jul 13 2023 Duncan Meacher <duncan.meacher@ligo.org> 1.3.0-1
+- Improved/cleaned up build and CI testing scripts
+- Added OSDF URL support
 * Fri May 05 2023 Duncan Meacher <duncan.meacher@ligo.org> 1.2.2-1
 - Fixed bug in single file queries
 - Fixed bug in search for fractional GPS times
 * Fri Apr 07 2023 Duncan Meacher <duncan.meacher@ligo.org> 1.2.1-1
 - Added comment handling in cache file
 - Updated default SciToken issue and scope
 - Added ability to search for fractional GPS times
```

### Comparing `gwdatafind-server-1.2.2/setup.cfg` & `gwdatafind-server-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/tests/cache.dat` & `gwdatafind-server-1.3.0/tests/cache.dat`

 * *Files 23% similar despite different names*

```diff
@@ -4,7 +4,9 @@
 /test/path2,L,L1_TEST_1,1,4,gwf 1556913881 2 {1000000012 1000000020}
 /test/path,L,L1_TEST_1,1,4,gwf 1556913881 2 {1000000000 1000000008}
 /test/path,L,L1_TEST_1,1,4,h5 1556913881 2 {1000000000 1000000008}
 /test/path,L,L1_TEST_2,1,8,gwf 1556913881 1 {1000000000 1000000008}
 /test/path,L,L1_TEST_IGNORE,1,8,gwf 1556913881 1 {1000000000 1000000008}
 /test/path,X,X1_TEST_2,1,8,gwf 1556913881 1 {1000000000 1000000008}
 /test/path,Y,Y1_EXCLUDE_1,1,8,gwf 1556913881 1 {1000000000 1000000008}
+# test CVMFS OSDF transforms
+/cvmfs/h.storage.igwn.org/igwn/test,H,H1_TEST_1,1,4,gwf 1556913881 1 {1000000008 1000000016}
```

### Comparing `gwdatafind-server-1.2.2/tests/test_api_v1.py` & `gwdatafind-server-1.3.0/tests/test_api_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,37 @@
         "file://localhost/test/path2/L-L1_TEST_1-1000000012-4.gwf",
         "gsiftp://testhost:15000/test/path/L-L1_TEST_1-1000000000-4.gwf",
         "gsiftp://testhost:15000/test/path/L-L1_TEST_1-1000000004-4.gwf",
         "gsiftp://testhost:15000/test/path2/L-L1_TEST_1-1000000012-4.gwf",
     ]
 
 
+def test_find_urls_osdf(client):
+    """Check that paths get transformed into OSDF URLs appropriately.
+    """
+    resp = client.get(
+        "/services/data/v1"
+        "/gwf/H/H1_TEST_1/1000000000,1000000012/osdf.json",
+    )
+    assert resp.status_code == 200
+    assert sorted(resp.json) == [
+        "osdf:///export/igwn/test/H-H1_TEST_1-1000000008-4.gwf",
+    ]
+
+
+def test_find_urls_osdf_empty(client):
+    """Check that URLS that don't support OSDF return empty.
+    """
+    resp = client.get(
+        "/services/data/v1/gwf/L/L1_TEST_1/1000000004,1000000016/osdf.json",
+    )
+    assert resp.status_code == 200
+    assert not resp.json  # no hits that support OSDF
+
+
 @mock.patch.object(api_utils, "_DEFAULT_GSIFTP_HOST", new="testhost")
 def test_find_latest(client):
     """Test the `find_latest` view
     """
     resp = client.get(
         "/services/data/v1/gwf/L/L1_TEST_1/latest.json",
     )
```

### Comparing `gwdatafind-server-1.2.2/tests/test_authentication_scitokens.py` & `gwdatafind-server-1.3.0/tests/test_authentication_scitokens.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/tests/test_authentication_x509.py` & `gwdatafind-server-1.3.0/tests/test_authentication_x509.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.2/tests/test_config.py` & `gwdatafind-server-1.3.0/tests/test_config.py`

 * *Files identical despite different names*

