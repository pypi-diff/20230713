# Comparing `tmp/vdk-jupyterlab-extension-0.1.0.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.929969845.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-jupyterlab-extension-0.1.0.tar", last modified: Tue Dec 13 16:35:00 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `vdk-jupyterlab-extension-0.1.0.tar` & `vdk_jupyterlab_extension-0.1.929969845.tar`

### file list

```diff
@@ -1,17 +1,81 @@
-drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2022-12-13 16:35:00.263854 vdk-jupyterlab-extension-0.1.0/
--rw-r--r--   0 aivanov    (502) staff       (20)     1814 2022-12-13 16:35:00.263439 vdk-jupyterlab-extension-0.1.0/PKG-INFO
--rw-r--r--   0 aivanov    (502) staff       (20)     1247 2022-12-13 16:34:53.000000 vdk-jupyterlab-extension-0.1.0/README.md
--rw-r--r--   0 aivanov    (502) staff       (20)       38 2022-12-13 16:35:00.263974 vdk-jupyterlab-extension-0.1.0/setup.cfg
--rw-r--r--   0 aivanov    (502) staff       (20)     1339 2022-12-13 16:34:53.000000 vdk-jupyterlab-extension-0.1.0/setup.py
-drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2022-12-13 16:35:00.256427 vdk-jupyterlab-extension-0.1.0/src/
-drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2022-12-13 16:35:00.255416 vdk-jupyterlab-extension-0.1.0/src/vdk/
-drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2022-12-13 16:35:00.255859 vdk-jupyterlab-extension-0.1.0/src/vdk/plugin/
-drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2022-12-13 16:35:00.258319 vdk-jupyterlab-extension-0.1.0/src/vdk/plugin/jupyterlab_extension/
--rw-r--r--   0 aivanov    (502) staff       (20)      867 2022-12-13 16:34:53.000000 vdk-jupyterlab-extension-0.1.0/src/vdk/plugin/jupyterlab_extension/plugin_entry.py
-drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2022-12-13 16:35:00.262744 vdk-jupyterlab-extension-0.1.0/src/vdk_jupyterlab_extension.egg-info/
--rw-r--r--   0 aivanov    (502) staff       (20)     1814 2022-12-13 16:35:00.000000 vdk-jupyterlab-extension-0.1.0/src/vdk_jupyterlab_extension.egg-info/PKG-INFO
--rw-r--r--   0 aivanov    (502) staff       (20)      384 2022-12-13 16:35:00.000000 vdk-jupyterlab-extension-0.1.0/src/vdk_jupyterlab_extension.egg-info/SOURCES.txt
--rw-r--r--   0 aivanov    (502) staff       (20)        1 2022-12-13 16:35:00.000000 vdk-jupyterlab-extension-0.1.0/src/vdk_jupyterlab_extension.egg-info/dependency_links.txt
--rw-r--r--   0 aivanov    (502) staff       (20)       85 2022-12-13 16:35:00.000000 vdk-jupyterlab-extension-0.1.0/src/vdk_jupyterlab_extension.egg-info/entry_points.txt
--rw-r--r--   0 aivanov    (502) staff       (20)        9 2022-12-13 16:35:00.000000 vdk-jupyterlab-extension-0.1.0/src/vdk_jupyterlab_extension.egg-info/requires.txt
--rw-r--r--   0 aivanov    (502) staff       (20)        4 2022-12-13 16:35:00.000000 vdk-jupyterlab-extension-0.1.0/src/vdk_jupyterlab_extension.egg-info/top_level.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/install.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/jest.config.js
+-rw-r--r--   0        0        0  1169752 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/package-lock.json
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/tsconfig.json
+-rw-r--r--   0        0        0   421787 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/schema/plugin.json
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/handler.ts
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/index.ts
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/jobData.ts
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/serverRequests.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/vdkTags.ts
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/delete-job-component.spec.ts
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/components/DeleteJob.tsx
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/components/props.tsx
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/style/index.js
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
+-rw-r--r--   0        0        0    16431 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/labextension/static/800.8ed62c07893a05a3a69b.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/labextension/static/remoteEntry.81ac755d1774a4840fbe.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/LICENSE
+-rw-r--r--   0        0        0     7017 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/README.md
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/pyproject.toml
+-rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.929969845/PKG-INFO
```

