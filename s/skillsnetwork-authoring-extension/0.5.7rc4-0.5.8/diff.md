# Comparing `tmp/skillsnetwork-authoring-extension-0.5.7rc4.tar.gz` & `tmp/skillsnetwork-authoring-extension-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillsnetwork-authoring-extension-0.5.7rc4.tar", last modified: Wed Jul 12 17:55:36 2023, max compression
+gzip compressed data, was "skillsnetwork-authoring-extension-0.5.8.tar", last modified: Thu Jul 13 18:53:33 2023, max compression
```

## Comparing `skillsnetwork-authoring-extension-0.5.7rc4.tar` & `skillsnetwork-authoring-extension-0.5.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.246301 skillsnetwork-authoring-extension-0.5.7rc4/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/jupyter-config/server-config/skillsnetwork_authoring_extension.json
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-12 17:54:03.000000 skillsnetwork-authoring-extension-0.5.7rc4/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/568.51d4a727ea85f89ce2e1.js
--rw-r--r--   0 runner    (1001) docker     (123)    19770 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/remoteEntry.9e7c06ac94a6b92bf5ef.js
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 17:55:33.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-12 17:55:35.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.250301 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-12 17:55:36.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-12 17:55:36.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:55:36.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:54:45.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 17:55:36.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 17:55:36.000000 skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/src/button/
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/button/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/button/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/config.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/dialog.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/handler.ts
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/src/menu/
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/menu/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/sn-file-library.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/src/tools.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:55:36.254301 skillsnetwork-authoring-extension-0.5.7rc4/style/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-12 17:54:01.000000 skillsnetwork-authoring-extension-0.5.7rc4/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)   219982 2023-07-12 17:55:19.000000 skillsnetwork-authoring-extension-0.5.7rc4/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.877274 skillsnetwork-authoring-extension-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-13 18:53:33.877274 skillsnetwork-authoring-extension-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.869273 skillsnetwork-authoring-extension-0.5.8/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.873274 skillsnetwork-authoring-extension-0.5.8/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.873274 skillsnetwork-authoring-extension-0.5.8/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/jupyter-config/server-config/skillsnetwork_authoring_extension.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:53:33.877274 skillsnetwork-authoring-extension-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.873274 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.873274 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.877274 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/568.efb2fec05e051487a4bb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19770 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/remoteEntry.b040bf3f9a425509fc14.js
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 18:53:31.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.877274 skillsnetwork-authoring-extension-0.5.8/skillsnetwork_authoring_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork_authoring_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:52:46.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork_authoring_extension.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork_authoring_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 18:53:33.000000 skillsnetwork-authoring-extension-0.5.8/skillsnetwork_authoring_extension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.877274 skillsnetwork-authoring-extension-0.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.877274 skillsnetwork-authoring-extension-0.5.8/src/button/
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/src/button/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/src/button/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/src/config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/src/dialog.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/src/handler.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.877274 skillsnetwork-authoring-extension-0.5.8/src/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/src/menu/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/src/sn-file-library.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/src/tools.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:53:33.877274 skillsnetwork-authoring-extension-0.5.8/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-13 18:52:09.000000 skillsnetwork-authoring-extension-0.5.8/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)   220494 2023-07-13 18:53:17.000000 skillsnetwork-authoring-extension-0.5.8/yarn.lock
```

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/LICENSE` & `skillsnetwork-authoring-extension-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/PKG-INFO` & `skillsnetwork-authoring-extension-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.5.7rc4
+Version: 0.5.8
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
 Author: Jenny Cao
 Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/README.md` & `skillsnetwork-authoring-extension-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/RELEASE.md` & `skillsnetwork-authoring-extension-0.5.8/RELEASE.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/package.json` & `skillsnetwork-authoring-extension-0.5.8/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.5.8'"}*

```diff
@@ -107,9 +107,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.7-rc4"
+    "version": "0.5.8"
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/pyproject.toml` & `skillsnetwork-authoring-extension-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/setup.py` & `skillsnetwork-authoring-extension-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/__init__.py` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/__init__.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/_version.py` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/_version.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/handlers.py` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/handlers.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/package.json` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9767992424242423%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b040bf3f9a425509fc14.js'}}",*

 * * "'version'": "'0.5.8'"}*

```diff
@@ -55,15 +55,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9e7c06ac94a6b92bf5ef.js",
+            "load": "static/remoteEntry.b040bf3f9a425509fc14.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "skillsnetwork-authoring-extension/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
@@ -112,9 +112,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.7-rc4"
+    "version": "0.5.8"
 }
```

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/568.51d4a727ea85f89ce2e1.js` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/568.efb2fec05e051487a4bb.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -282,15 +282,15 @@
                             }
                         }),
                         w = async (t, e) => {
                             try {
                                 const o = u()(e),
                                     n = o.version_id,
                                     a = o.lab_id,
-                                    l = await t.get(`api/v1/labs/${a}`).then((t => `${t.data.name}.ipynb`)),
+                                    l = `${o.lab_name}.ipynb`,
                                     s = await t.get(`api/v1/labs/${a}/lab_versions/${n}/download`).then((t => t.data));
                                 return i.Dialog.flush(), {
                                     labFilename: l,
                                     body: s
                                 }
                             } catch (t) {
                                 throw console.log(t), "Failed to fetch notebook"
```

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/remoteEntry.9e7c06ac94a6b92bf5ef.js` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/remoteEntry.b040bf3f9a425509fc14.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -84,20 +84,20 @@
     }, j.d = (e, r) => {
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         245: "74d5f0c3fbdb9413b03b",
-        568: "51d4a727ea85f89ce2e1",
+        568: "efb2fec05e051487a4bb",
         669: "d32869c9490cd02b1382",
         747: "1af575e10eb228bf3434"
     } [e] + ".js?v=" + {
         245: "74d5f0c3fbdb9413b03b",
-        568: "51d4a727ea85f89ce2e1",
+        568: "efb2fec05e051487a4bb",
         669: "d32869c9490cd02b1382",
         747: "1af575e10eb228bf3434"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -151,15 +151,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("axios", "0.21.4", (() => j.e(669).then((() => () => j(9669))))), u("jwt-decode", "3.1.2", (() => j.e(245).then((() => () => j(6245))))), u("skillsnetwork-authoring-extension", "0.5.7-rc4", (() => j.e(568).then((() => () => j(1568)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("axios", "0.21.4", (() => j.e(669).then((() => () => j(9669))))), u("jwt-decode", "3.1.2", (() => j.e(245).then((() => () => j(6245))))), u("skillsnetwork-authoring-extension", "0.5.8", (() => j.e(568).then((() => () => j(1568)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/PKG-INFO` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork_authoring_extension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.5.7rc4
+Version: 0.5.8
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
 Author: Jenny Cao
 Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/skillsnetwork_authoring_extension.egg-info/SOURCES.txt` & `skillsnetwork-authoring-extension-0.5.8/skillsnetwork_authoring_extension.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 jupyter-config/nb-config/skillsnetwork_authoring_extension.json
 jupyter-config/server-config/skillsnetwork_authoring_extension.json
 skillsnetwork-authoring-extension/__init__.py
 skillsnetwork-authoring-extension/_version.py
 skillsnetwork-authoring-extension/handlers.py
 skillsnetwork-authoring-extension/labextension/package.json
 skillsnetwork-authoring-extension/labextension/static/245.74d5f0c3fbdb9413b03b.js
-skillsnetwork-authoring-extension/labextension/static/568.51d4a727ea85f89ce2e1.js
+skillsnetwork-authoring-extension/labextension/static/568.efb2fec05e051487a4bb.js
 skillsnetwork-authoring-extension/labextension/static/669.d32869c9490cd02b1382.js
 skillsnetwork-authoring-extension/labextension/static/747.1af575e10eb228bf3434.js
-skillsnetwork-authoring-extension/labextension/static/remoteEntry.9e7c06ac94a6b92bf5ef.js
+skillsnetwork-authoring-extension/labextension/static/remoteEntry.b040bf3f9a425509fc14.js
 skillsnetwork-authoring-extension/labextension/static/style.js
 skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
 skillsnetwork_authoring_extension.egg-info/PKG-INFO
 skillsnetwork_authoring_extension.egg-info/SOURCES.txt
 skillsnetwork_authoring_extension.egg-info/dependency_links.txt
 skillsnetwork_authoring_extension.egg-info/not-zip-safe
 skillsnetwork_authoring_extension.egg-info/requires.txt
```

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/src/button/index.ts` & `skillsnetwork-authoring-extension-0.5.8/src/button/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/src/button/sample.json` & `skillsnetwork-authoring-extension-0.5.8/src/button/sample.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/src/config.ts` & `skillsnetwork-authoring-extension-0.5.8/src/config.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/src/dialog.ts` & `skillsnetwork-authoring-extension-0.5.8/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/src/handler.ts` & `skillsnetwork-authoring-extension-0.5.8/src/handler.ts`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,15 @@
  */
 export const getIndependentLabModel = async (awbAxiosHandler: AxiosInstance, lab_token: string) => {
   try {
     const token_info = jwt_decode(lab_token) as { [key: string]: any };
     const version_id = token_info.version_id
     const lab_id = token_info.lab_id
 
-    const labFilename = await awbAxiosHandler.get(`api/v1/labs/${lab_id}`).then(result => {
-      const labData = result.data as { [key: string]: any };
-      return `${labData["name"]}.ipynb`
-    });
+    const labFilename = `${token_info.lab_name}.ipynb`
     const instructions = await awbAxiosHandler.get(`api/v1/labs/${lab_id}/lab_versions/${version_id}/download`).then(result => { return result.data })
 
     Dialog.flush();
     return {labFilename, body: instructions};
 
     // handle the decoded token here
   } catch (error) {
```

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/src/menu/index.ts` & `skillsnetwork-authoring-extension-0.5.8/src/menu/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/src/sn-file-library.ts` & `skillsnetwork-authoring-extension-0.5.8/src/sn-file-library.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/src/tools.ts` & `skillsnetwork-authoring-extension-0.5.8/src/tools.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/tsconfig.json` & `skillsnetwork-authoring-extension-0.5.8/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork-authoring-extension-0.5.7rc4/yarn.lock` & `skillsnetwork-authoring-extension-0.5.8/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -494,17 +494,17 @@
     "@jupyterlab/ui-components" "^3.6.5"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/widgets" "^1.37.2"
 
 "@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15":
-  version "4.0.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-4.0.2.tgz#a735304dfcd3ac5214bc6e471cd24f7e198a01b3"
-  integrity sha512-K83wDb1iUViTk4mj228SR4E0GPASiykXcD/tVYAOvxWv8TsaZ2UK/dcX4ZtBEZpVqI5enRrq8Z7xISMR+3CRBg==
+  version "4.0.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-4.0.3.tgz#02f005a7dccf34d70c99d935d92459927ec9c489"
+  integrity sha512-wpOktEi5XLPrAvTH+xkimeDghOz+oj1lPUHLeRTzcYBZfMybHQxV9XKfroXllcypkyqSBI5Ppfv6/GYeQQzmHQ==
   dependencies:
     "@lumino/coreutils" "^2.1.1"
 
 "@jupyterlab/nbformat@^3.3.3", "@jupyterlab/nbformat@^3.6.5":
   version "3.6.5"
   resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.5.tgz#dfb957d1297b2f319690df326e2ecc1eee99edfa"
   integrity sha512-yyyNniuzxycsF+kHvjpAIjZ+qrt3G/HEViZN+FJA3vFpg6e2n/nqa7BgzlxINS5SH4FnBG6rM/u45bwih38VkA==
@@ -569,17 +569,17 @@
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
     resize-observer-polyfill "^1.5.1"
 
 "@jupyterlab/rendermime-interfaces@^3.6.5":
-  version "3.8.2"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.8.2.tgz#115d70f1dd064784cd5816785c94b7c36e605fd5"
-  integrity sha512-IOnzA/ccfwXGO/RaWysYn74ojJ7PaH5igTnS0sjo4qIprFZ6tCORTrKF594BA7Qz6PpW2+GpdUVMUnnYdU5R9Q==
+  version "3.8.3"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.8.3.tgz#ecf0a6dcfdaa9187a4666f1b80e165969f21f549"
+  integrity sha512-XG0Wp/WMXcWdAILej766VpeXUAN31XYSAW9mMTw5Y+SQFfBAmHBekLMp+/+aG8n3ngqXcALeYIwBR3eF4QsKcA==
   dependencies:
     "@lumino/coreutils" "^1.11.0 || ^2.1.1"
     "@lumino/widgets" "^1.37.2 || ^2.1.1"
 
 "@jupyterlab/rendermime@^3.6.5":
   version "3.6.5"
   resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.5.tgz#95e49172914118ea5ca2d5037659ee2baf1c132a"
@@ -931,17 +931,17 @@
 
 "@types/minimist@^1.2.0":
   version "1.2.2"
   resolved "https://registry.yarnpkg.com/@types/minimist/-/minimist-1.2.2.tgz#ee771e2ba4b3dc5b372935d549fd9617bf345b8c"
   integrity sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==
 
 "@types/node@*":
-  version "20.4.1"
-  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.4.1.tgz#a6033a8718653c50ac4962977e14d0f984d9527d"
-  integrity sha512-JIzsAvJeA/5iY6Y/OxZbv1lUcc8dNSE77lb2gnBH+/PJ3lFR1Ccvgwl5JWnHAkNHcRsT0TbpVOsiMKZ1F/yyJg==
+  version "20.4.2"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.4.2.tgz#129cc9ae69f93824f92fac653eebfb4812ab4af9"
+  integrity sha512-Dd0BYtWgnWJKwO1jkmTrzofjK2QXXcai0dmtzvIBhcA+RsG5h8R3xlyta0kGOZRNfL9GuRtb1knmPEhQrePCEw==
 
 "@types/node@^17.0.29":
   version "17.0.45"
   resolved "https://registry.yarnpkg.com/@types/node/-/node-17.0.45.tgz#2c0fafd78705e7a18b7906b5201a522719dc5190"
   integrity sha512-w+tIMs3rq2afQdsPJlODhoUEKzFP1ayaoyl1CcnwtIlsVe7K7bA1NGm4s3PraqTLlXnbIN84zuBlxBWo1u9BLw==
 
 "@types/normalize-package-data@^2.4.0":
@@ -1826,17 +1826,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.431:
-  version "1.4.457"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.457.tgz#3fdc7b4f97d628ac6b51e8b4b385befb362fe343"
-  integrity sha512-/g3UyNDmDd6ebeWapmAoiyy+Sy2HyJ+/X8KyvNeHfKRFfHaA2W8oF5fxD5F3tjBDcjpwo0iek6YNgxNXDBoEtA==
+  version "1.4.460"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.460.tgz#f360a5059c039c4a5fb4dfa99680ad8129dd9f84"
+  integrity sha512-kKiHnbrHME7z8E6AYaw0ehyxY5+hdaRmeUbjBO22LZMdqTYCO29EvF0T1cQ3pJ1RN5fyMcHl1Lmcsdt9WWJpJQ==
 
 emoji-regex@^8.0.0:
   version "8.0.0"
   resolved "https://registry.yarnpkg.com/emoji-regex/-/emoji-regex-8.0.0.tgz#e818fd69ce5ccfcb404594f842963bf53164cc37"
   integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
 
 emojis-list@^3.0.0:
@@ -1890,25 +1890,25 @@
   version "1.3.2"
   resolved "https://registry.yarnpkg.com/error-ex/-/error-ex-1.3.2.tgz#b4ac40648107fdcdcfae242f428bea8a14d4f1bf"
   integrity sha512-7dFHNmqeFSEt2ZBsCriorKnn3Z2pj+fd9kmI6QoWw4//DL+icEBfc0U7qJCisqrTsKTjw4fNFy2pW9OqStD84g==
   dependencies:
     is-arrayish "^0.2.1"
 
 es-abstract@^1.19.0, es-abstract@^1.20.4:
-  version "1.21.2"
-  resolved "https://registry.yarnpkg.com/es-abstract/-/es-abstract-1.21.2.tgz#a56b9695322c8a185dc25975aa3b8ec31d0e7eff"
-  integrity sha512-y/B5POM2iBnIxCiernH1G7rC9qQoM77lLIMQLuob0zhp8C56Po81+2Nj0WFKnd0pNReDTnkYryc+zhOzpEIROg==
+  version "1.21.3"
+  resolved "https://registry.yarnpkg.com/es-abstract/-/es-abstract-1.21.3.tgz#8aaa0ffc080e8a6fef6ace72631dc1ec5d47bf94"
+  integrity sha512-ZU4miiY1j3sGPFLJ34VJXEqhpmL+HGByCinGHv4HC+Fxl2fI2Z4yR6tl0mORnDr6PA8eihWo4LmSWDbvhALckg==
   dependencies:
     array-buffer-byte-length "^1.0.0"
     available-typed-arrays "^1.0.5"
     call-bind "^1.0.2"
     es-set-tostringtag "^2.0.1"
     es-to-primitive "^1.2.1"
     function.prototype.name "^1.1.5"
-    get-intrinsic "^1.2.0"
+    get-intrinsic "^1.2.1"
     get-symbol-description "^1.0.0"
     globalthis "^1.0.3"
     gopd "^1.0.1"
     has "^1.0.3"
     has-property-descriptors "^1.0.0"
     has-proto "^1.0.1"
     has-symbols "^1.0.3"
@@ -1920,22 +1920,23 @@
     is-shared-array-buffer "^1.0.2"
     is-string "^1.0.7"
     is-typed-array "^1.1.10"
     is-weakref "^1.0.2"
     object-inspect "^1.12.3"
     object-keys "^1.1.1"
     object.assign "^4.1.4"
-    regexp.prototype.flags "^1.4.3"
+    regexp.prototype.flags "^1.5.0"
     safe-regex-test "^1.0.0"
     string.prototype.trim "^1.2.7"
     string.prototype.trimend "^1.0.6"
     string.prototype.trimstart "^1.0.6"
+    typed-array-byte-offset "^1.0.0"
     typed-array-length "^1.0.4"
     unbox-primitive "^1.0.2"
-    which-typed-array "^1.1.9"
+    which-typed-array "^1.1.10"
 
 es-module-lexer@^1.2.1:
   version "1.3.0"
   resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-1.3.0.tgz#6be9c9e0b4543a60cd166ff6f8b4e9dae0b0c16f"
   integrity sha512-vZK7T0N2CBmBOixhmjdqx2gWVbFZ4DXZ/NyRMZVlJXPa7CyFS+/a4QQsDGDQy9ZfEzxFuNEsMLeQJnKP2p5/JA==
 
 es-set-tostringtag@^2.0.1:
@@ -2271,15 +2272,15 @@
   integrity sha512-dsKNQNdj6xA3T+QlADDA7mOSlX0qiMINjn0cgr+eGHGsbSHzTabcIogz2+p/iqP1Xs6EP/sS2SbqH+brGTbq0g==
 
 functions-have-names@^1.2.2, functions-have-names@^1.2.3:
   version "1.2.3"
   resolved "https://registry.yarnpkg.com/functions-have-names/-/functions-have-names-1.2.3.tgz#0404fe4ee2ba2f607f0e0ec3c80bae994133b834"
   integrity sha512-xckBUXyTIqT97tq2x2AMb+g163b5JFysYk0x4qxNFwbfQkmNZoiRHb6sPzI9/QV33WeuvVYBUIiD4NzNIyqaRQ==
 
-get-intrinsic@^1.0.2, get-intrinsic@^1.1.1, get-intrinsic@^1.1.3, get-intrinsic@^1.2.0:
+get-intrinsic@^1.0.2, get-intrinsic@^1.1.1, get-intrinsic@^1.1.3, get-intrinsic@^1.2.0, get-intrinsic@^1.2.1:
   version "1.2.1"
   resolved "https://registry.yarnpkg.com/get-intrinsic/-/get-intrinsic-1.2.1.tgz#d295644fed4505fc9cde952c37ee12b477a83d82"
   integrity sha512-2DcsyfABl+gVHEfCOaTrWgyt+tb6MSEGmKq+kI5HwLbIYgjgmMcV8KQ41uaKz1xxUcn9tJtgFbQUEVcEbd0FYw==
   dependencies:
     function-bind "^1.1.1"
     has "^1.0.3"
     has-proto "^1.0.1"
@@ -3760,15 +3761,15 @@
     strip-indent "^3.0.0"
 
 regenerator-runtime@^0.13.11:
   version "0.13.11"
   resolved "https://registry.yarnpkg.com/regenerator-runtime/-/regenerator-runtime-0.13.11.tgz#f6dca3e7ceec20590d07ada785636a90cdca17f9"
   integrity sha512-kY1AZVr2Ra+t+piVaJ4gxaFaReZVH40AKNo7UCX6W+dEwBo/2oZJzqfuN1qLq1oL45o56cPaTXELwrTh8Fpggg==
 
-regexp.prototype.flags@^1.2.0, regexp.prototype.flags@^1.4.3:
+regexp.prototype.flags@^1.2.0, regexp.prototype.flags@^1.5.0:
   version "1.5.0"
   resolved "https://registry.yarnpkg.com/regexp.prototype.flags/-/regexp.prototype.flags-1.5.0.tgz#fe7ce25e7e4cca8db37b6634c8a2c7009199b9cb"
   integrity sha512-0SutC3pNudRKgquxGoRGIz946MZVHqbNfPjBdxeOhBrdgDKlRoXmYLQN9xRbrR09ZXWeGAdPuif7egofn6v5LA==
   dependencies:
     call-bind "^1.0.2"
     define-properties "^1.2.0"
     functions-have-names "^1.2.3"
@@ -4411,14 +4412,25 @@
   integrity sha512-q+MB8nYR1KDLrgr4G5yemftpMC7/QLqVndBmEEdqzmNj5dcFOO4Oo8qlwZE3ULT3+Zim1F8Kq4cBnikNhlCMlg==
 
 type-fest@^0.8.1:
   version "0.8.1"
   resolved "https://registry.yarnpkg.com/type-fest/-/type-fest-0.8.1.tgz#09e249ebde851d3b1e48d27c105444667f17b83d"
   integrity sha512-4dbzIzqvjtgiM5rw1k5rEHtBANKmdudhGyBEajN01fEyhaAIhsoKNy6y7+IN93IfpFtwY9iqi7kD+xwKhQsNJA==
 
+typed-array-byte-offset@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.yarnpkg.com/typed-array-byte-offset/-/typed-array-byte-offset-1.0.0.tgz#cbbe89b51fdef9cd6aaf07ad4707340abbc4ea0b"
+  integrity sha512-RD97prjEt9EL8YgAgpOkf3O4IF9lhJFr9g0htQkm0rchFp/Vx7LW5Q8fSXXub7BXAODyUQohRMyOc3faCPd0hg==
+  dependencies:
+    available-typed-arrays "^1.0.5"
+    call-bind "^1.0.2"
+    for-each "^0.3.3"
+    has-proto "^1.0.1"
+    is-typed-array "^1.1.10"
+
 typed-array-length@^1.0.4:
   version "1.0.4"
   resolved "https://registry.yarnpkg.com/typed-array-length/-/typed-array-length-1.0.4.tgz#89d83785e5c4098bec72e08b319651f0eac9c1bb"
   integrity sha512-KjZypGq+I/H7HI5HlOoGHkWUUGq+Q0TPhQurLbyrVrvnKTBgzLhIJ7j6J/XTQOi0d1RjyZ0wdas8bKs2p0x3Ng==
   dependencies:
     call-bind "^1.0.2"
     for-each "^0.3.3"
@@ -4682,15 +4694,15 @@
   dependencies:
     is-bigint "^1.0.1"
     is-boolean-object "^1.1.0"
     is-number-object "^1.0.4"
     is-string "^1.0.5"
     is-symbol "^1.0.3"
 
-which-typed-array@^1.1.9:
+which-typed-array@^1.1.10:
   version "1.1.10"
   resolved "https://registry.yarnpkg.com/which-typed-array/-/which-typed-array-1.1.10.tgz#74baa2789991905c2076abb317103b866c64e69e"
   integrity sha512-uxoA5vLUfRPdjCuJ1h5LlYdmTLbYfums398v3WLkM+i/Wltl2/XyZpQWKbN++ck5L64SR/grOHqtXCUKmlZPNA==
   dependencies:
     available-typed-arrays "^1.0.5"
     call-bind "^1.0.2"
     for-each "^0.3.3"
```

