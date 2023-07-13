# Comparing `tmp/jupyterlab_theme_solarized_dark-2.1.0.tar.gz` & `tmp/jupyterlab_theme_solarized_dark-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_theme_solarized_dark-2.1.0.tar", last modified: Wed Jun 22 11:43:37 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_theme_solarized_dark-2.1.0.tar` & `jupyterlab_theme_solarized_dark-3.0.0.tar`

### file list

```diff
@@ -1,46 +1,27 @@
-drwxr-xr-x   0 ac        (1000) ac        (1000)        0 2022-06-22 11:43:37.927661 jupyterlab_theme_solarized_dark-2.1.0/
--rw-r--r--   0 ac        (1000) ac        (1000)       86 2022-06-22 10:10:36.000000 jupyterlab_theme_solarized_dark-2.1.0/CHANGELOG.md
--rw-r--r--   0 ac        (1000) ac        (1000)     1519 2022-06-21 03:55:47.000000 jupyterlab_theme_solarized_dark-2.1.0/LICENSE
--rw-r--r--   0 ac        (1000) ac        (1000)      425 2022-06-21 03:55:47.000000 jupyterlab_theme_solarized_dark-2.1.0/MANIFEST.in
--rw-r--r--   0 ac        (1000) ac        (1000)     5322 2022-06-22 11:43:37.927661 jupyterlab_theme_solarized_dark-2.1.0/PKG-INFO
--rw-r--r--   0 ac        (1000) ac        (1000)     4184 2022-06-22 10:30:02.000000 jupyterlab_theme_solarized_dark-2.1.0/README.md
--rw-r--r--   0 ac        (1000) ac        (1000)     1913 2022-06-21 03:55:47.000000 jupyterlab_theme_solarized_dark-2.1.0/RELEASE.md
--rw-r--r--   0 ac        (1000) ac        (1000)      223 2022-06-21 03:55:47.000000 jupyterlab_theme_solarized_dark-2.1.0/install.json
-drwxr-xr-x   0 ac        (1000) ac        (1000)        0 2022-06-22 11:43:37.920994 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/
--rw-r--r--   0 ac        (1000) ac        (1000)      321 2022-06-21 03:55:47.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/__init__.py
--rw-r--r--   0 ac        (1000) ac        (1000)      625 2022-06-21 03:55:47.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/_version.py
-drwxr-xr-x   0 ac        (1000) ac        (1000)        0 2022-06-22 11:43:37.924327 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/
--rw-r--r--   0 ac        (1000) ac        (1000)    22250 2022-06-21 11:45:47.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/build_log.json
--rw-r--r--   0 ac        (1000) ac        (1000)     3482 2022-06-21 11:45:54.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/package.json
-drwxr-xr-x   0 ac        (1000) ac        (1000)        0 2022-06-22 11:43:37.927661 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/static/
--rw-r--r--   0 ac        (1000) ac        (1000)     1664 2022-06-21 11:45:54.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/static/lib_index_js.88cfd94f93ca3056743b.js
--rw-r--r--   0 ac        (1000) ac        (1000)     1000 2022-06-21 11:45:54.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/static/lib_index_js.88cfd94f93ca3056743b.js.map
--rw-r--r--   0 ac        (1000) ac        (1000)     1644 2022-06-21 11:45:48.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/static/lib_index_js.a9f045a011f6eaf91a60.js
--rw-r--r--   0 ac        (1000) ac        (1000)      985 2022-06-21 11:45:48.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/static/lib_index_js.a9f045a011f6eaf91a60.js.map
--rw-r--r--   0 ac        (1000) ac        (1000)    27096 2022-06-21 11:45:54.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/static/remoteEntry.457435b4c1229552ec51.js
--rw-r--r--   0 ac        (1000) ac        (1000)    26072 2022-06-21 11:45:54.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/static/remoteEntry.457435b4c1229552ec51.js.map
--rw-r--r--   0 ac        (1000) ac        (1000)    26072 2022-06-21 11:45:48.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/static/remoteEntry.ee43757e5b4e61b5e80a.js.map
--rw-r--r--   0 ac        (1000) ac        (1000)      118 2022-06-21 11:45:47.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/static/style.js
-drwxr-xr-x   0 ac        (1000) ac        (1000)        0 2022-06-22 11:43:37.917661 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/themes/
-drwxr-xr-x   0 ac        (1000) ac        (1000)        0 2022-06-22 11:43:37.927661 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/themes/jupyterlab-theme-solarized-dark/
--rw-r--r--   0 ac        (1000) ac        (1000)    17504 2022-06-21 12:07:41.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/themes/jupyterlab-theme-solarized-dark/index.css
--rw-r--r--   0 ac        (1000) ac        (1000)        0 2022-06-21 12:07:41.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/themes/jupyterlab-theme-solarized-dark/index.js
-drwxr-xr-x   0 ac        (1000) ac        (1000)        0 2022-06-22 11:43:37.924327 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark.egg-info/
--rw-r--r--   0 ac        (1000) ac        (1000)     5322 2022-06-22 11:43:37.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark.egg-info/PKG-INFO
--rw-r--r--   0 ac        (1000) ac        (1000)     1570 2022-06-22 11:43:37.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark.egg-info/SOURCES.txt
--rw-r--r--   0 ac        (1000) ac        (1000)        1 2022-06-22 11:43:37.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark.egg-info/dependency_links.txt
--rw-r--r--   0 ac        (1000) ac        (1000)        1 2022-06-21 03:33:28.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark.egg-info/not-zip-safe
--rw-r--r--   0 ac        (1000) ac        (1000)       32 2022-06-22 11:43:37.000000 jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark.egg-info/top_level.txt
--rw-r--r--   0 ac        (1000) ac        (1000)     3429 2022-06-22 10:30:14.000000 jupyterlab_theme_solarized_dark-2.1.0/package.json
--rw-r--r--   0 ac        (1000) ac        (1000)      659 2022-06-21 03:55:47.000000 jupyterlab_theme_solarized_dark-2.1.0/pyproject.toml
--rw-r--r--   0 ac        (1000) ac        (1000)       38 2022-06-22 11:43:37.927661 jupyterlab_theme_solarized_dark-2.1.0/setup.cfg
--rw-r--r--   0 ac        (1000) ac        (1000)     2925 2022-06-21 11:20:36.000000 jupyterlab_theme_solarized_dark-2.1.0/setup.py
-drwxr-xr-x   0 ac        (1000) ac        (1000)        0 2022-06-22 11:43:37.927661 jupyterlab_theme_solarized_dark-2.1.0/src/
--rw-r--r--   0 ac        (1000) ac        (1000)      737 2022-06-21 04:00:49.000000 jupyterlab_theme_solarized_dark-2.1.0/src/index.ts
-drwxr-xr-x   0 ac        (1000) ac        (1000)        0 2022-06-22 11:43:37.927661 jupyterlab_theme_solarized_dark-2.1.0/style/
--rw-r--r--   0 ac        (1000) ac        (1000)      799 2022-06-22 09:58:36.000000 jupyterlab_theme_solarized_dark-2.1.0/style/base.css
--rw-r--r--   0 ac        (1000) ac        (1000)       22 2022-06-21 03:57:09.000000 jupyterlab_theme_solarized_dark-2.1.0/style/index.css
--rw-r--r--   0 ac        (1000) ac        (1000)       21 2022-06-21 03:31:39.000000 jupyterlab_theme_solarized_dark-2.1.0/style/index.js
--rw-r--r--   0 ac        (1000) ac        (1000)    16703 2022-06-22 09:57:49.000000 jupyterlab_theme_solarized_dark-2.1.0/style/variables.css
--rw-r--r--   0 ac        (1000) ac        (1000)      554 2022-06-21 03:55:47.000000 jupyterlab_theme_solarized_dark-2.1.0/tsconfig.json
--rw-r--r--   0 ac        (1000) ac        (1000)   291627 2022-06-21 11:40:02.000000 jupyterlab_theme_solarized_dark-2.1.0/yarn.lock
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/.copier-answers.yml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/RELEASE.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/install.json
+-rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/tsconfig.json
+-rw-r--r--   0        0        0   213668 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/yarn.lock
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/jupyterlab_theme_solarized_dark/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/jupyterlab_theme_solarized_dark/_version.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/jupyterlab_theme_solarized_dark/labextension/package.json
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/jupyterlab_theme_solarized_dark/labextension/static/568.76dc9668e69d5d7e4a81.js
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/jupyterlab_theme_solarized_dark/labextension/static/remoteEntry.4e9357cc5aee17d940f5.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/jupyterlab_theme_solarized_dark/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/jupyterlab_theme_solarized_dark/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/jupyterlab_theme_solarized_dark/labextension/themes/jupyterlab-theme-solarized-dark/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/jupyterlab_theme_solarized_dark/labextension/themes/jupyterlab-theme-solarized-dark/index.js
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/src/index.ts
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/style/index.scss
+-rw-r--r--   0        0        0    18762 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/style/variables.scss
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/README.md
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 jupyterlab_theme_solarized_dark-3.0.0/PKG-INFO
```

### Comparing `jupyterlab_theme_solarized_dark-2.1.0/LICENSE` & `jupyterlab_theme_solarized_dark-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_theme_solarized_dark-2.1.0/README.md` & `jupyterlab_theme_solarized_dark-3.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,44 @@
-# jupyterlab-theme-solarized-dark
+# JupyterLab Theme Solarized Dark
 
 ![Github Actions Status](https://github.com/AllanChain/jupyterlab-theme-solarized-dark/workflows/Build/badge.svg)
 ![License](https://img.shields.io/github/license/AllanChain/jupyterlab-theme-solarized-dark.svg)
 ![GitHub last commit](https://img.shields.io/github/last-commit/AllanChain/jupyterlab-theme-solarized-dark)
 ![GitHub stars](https://img.shields.io/github/stars/AllanChain/jupyterlab-theme-solarized-dark)
 
-[![NPM Version](https://img.shields.io/npm/v/jupyterlab-theme-solarized-dark.svg)](https://npmjs.org/package/jupyterlab-theme-solarized-dark)
-![Monthly Downloads](https://img.shields.io/npm/dm/jupyterlab-theme-solarized-dark.svg?label=npm%20downloads)
+[![NPM Version](<https://img.shields.io/npm/v/jupyterlab-theme-solarized-dark.svg?logo=npm&label=npm%20(deprecated)>)](https://npmjs.org/package/jupyterlab-theme-solarized-dark)
+![Monthly Downloads](https://img.shields.io/npm/dm/jupyterlab-theme-solarized-dark.svg?logo=npm&label=npm%20downloads)
 
-[![PyPI](https://img.shields.io/pypi/v/jupyterlab_theme_solarized_dark)](https://pypi.org/project/jupyterlab-theme-solarized-dark/)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/jupyterlab_theme_solarized_dark?label=pypi%20downloads)
+[![PyPI](https://img.shields.io/pypi/v/jupyterlab_theme_solarized_dark?logo=pypi&label=PyPi)](https://pypi.org/project/jupyterlab-theme-solarized-dark/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/jupyterlab_theme_solarized_dark?logo=pypi&label=PyPi%20downloads)
 
-JupyterLab 2.x / 3.x Solarized Dark extension.
-
-The theme is originally created by [Jae Hee Lee](https://github.com/dschaehi) in this [gist](https://gist.github.com/dschaehi/ff6d30e6779a683053a1f078af178cdb)
+The theme was originally created by [Joses W. Ho](https://github.com/josesho) and [Jae Hee Lee](https://github.com/dschaehi) in this [gist](https://gist.github.com/dschaehi/ff6d30e6779a683053a1f078af178cdb).
 
 ## Screenshot
 
-![Screenshot](https://user-images.githubusercontent.com/36528777/79721723-6927f680-8315-11ea-8a5b-e2c298eeed09.png)
-
-## Prerequisites
-
-- JupyterLab
-
-## Version
-
-- `v0.2.x` is mainly based on Jae Hee Lee's original theme
-- `v1.x` aims to provide a smoother looking.
-- Starting from `v2.x`, Jupyterlab `v3.x` support is added.
+<img width="960" alt="Screenshot" src="https://github.com/AllanChain/jupyterlab-theme-solarized-dark/assets/36528777/de6dd210-d92b-4015-9da9-92dd07a4a9a9">
 
 ## Requirements
 
-- JupyterLab >= 2.0 or JupyterLab >= 3.0
+- JupyterLab >= 4.0.0
 
 ## Install
 
-To install it as a prebuilt extension (requires JupyterLab >= 3.0):
+To install the extension, execute:
 
 ```bash
 pip install jupyterlab_theme_solarized_dark
 ```
 
-Or install it as a source extension:
+## Uninstall
+
+To remove the extension, execute:
 
 ```bash
-jupyter labextension install jupyterlab-theme-solarized-dark
+pip uninstall jupyterlab_theme_solarized_dark
 ```
 
 Apply the theme by checking `Settings -> Jupyterlab Theme -> Jupyterlab Solarized Dark`
 
 To enable theme scrollbars, in JupyterLab, either
 
 - navigate to `Settings -> Advanced Settings Editor -> Theme`, and add `"theme-scrollbars": true` to `User Preferences`
@@ -64,15 +54,15 @@
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
 # Change directory to the jupyterlab_theme_solarized_dark directory
 # Install package in development mode
-pip install -e .
+pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
@@ -94,20 +84,14 @@
 
 ### Development uninstall
 
 ```bash
 pip uninstall jupyterlab_theme_solarized_dark
 ```
 
-Or
-
-```bash
-jupyter labextension uninstall jupyterlab-theme-solarized-dark
-```
-
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `jupyterlab-theme-solarized-dark` within that folder.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
```

### Comparing `jupyterlab_theme_solarized_dark-2.1.0/jupyterlab_theme_solarized_dark/labextension/themes/jupyterlab-theme-solarized-dark/index.css` & `jupyterlab_theme_solarized_dark-3.0.0/style/variables.scss`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-/*-----------------------------------------------------------------------------
+/* -----------------------------------------------------------------------------
 | Copyright (c) Jupyter Development Team.
 | Distributed under the terms of the Modified BSD License.
-|----------------------------------------------------------------------------*/
+|---------------------------------------------------------------------------- */
 
 /*
 The following CSS variables define the main, public API for styling JupyterLab.
 These variables should be used by all plugins wherever possible. In other
 words, plugins should not define custom colors, sizes, etc unless absolutely
 necessary. This enables users to change the visual theme of JupyterLab
 by changing these variables.
@@ -20,45 +20,41 @@
 * 3: tertiary, next most important under normal situations
 
 Throughout JupyterLab, we are mostly following principles from Google's
 Material Design when selecting colors. We are not, however, following
 all of MD as it is not optimized for dense, information rich UIs.
 */
 
-:root {
-
-  /* Create the solarized dark palette.
-   * The bases run in increasing brightness.
-   */
-
-  --solarized-base03: #002b36;
-  --solarized-base02: #073642;
-  /* Non-standard color between base02 and base01.
-   * Because base01 and base02 are so different.
-   * Note base015 is not exactly at the half. It's just a name.
-   */
-  --solarized-base015: #1b444f;
-  --solarized-base01: #586e75;
-  --solarized-base00: #657b83;
-
-  --solarized-base0: #839496;
-  --solarized-base1: #93a1a1;
-  --solarized-base2: #eee8d5;
-  --solarized-base3: #fdf6e3;
-
-  --solarized-yellow: #b58900;
-  --solarized-orange: #cb4b16;
-  --solarized-red: #dc322f;
-  --solarized-magenta: #d33682;
-  --solarized-violet: #6c71c4;
-  --solarized-blue: #268bd2;
-  --solarized-cyan: #2aa198;
-  --solarized-green: #859900;
-
+/* Create the solarized dark palette.
+ * The bases run in increasing brightness.
+ */
+@use 'sass:color';
+
+$solarized-base03: #002b36;
+$solarized-base02: #073642;
+
+// $solarized-base015: #1b444f;
+$solarized-base01: #586e75;
+$solarized-base00: #657b83;
+$solarized-base0: #839496;
+$solarized-base1: #93a1a1;
+$solarized-base2: #eee8d5;
+$solarized-base3: #fdf6e3;
+$solarized-yellow: #b58900;
+$solarized-orange: #cb4b16;
+$solarized-red: #dc322f;
+$solarized-magenta: #d33682;
+$solarized-violet: #6c71c4;
+$solarized-blue: #268bd2;
+$solarized-cyan: #2aa198;
+$solarized-green: #859900;
+$solarized-base015: color.mix($solarized-base02, $solarized-base01, 80%);
+$solarized-base025: color.mix($solarized-base03, $solarized-base02, 50%);
 
+:root {
   /* Elevation
    *
    * We style box-shadows using Material Design's idea of elevation. These particular numbers are taken from here:
    *
    * https://github.com/material-components/material-components-web
    * https://material-components-web.appspot.com/elevation.html
    */
@@ -81,141 +77,137 @@
   --jp-shadow-ambient-color: rgba(
     var(--jp-shadow-base-lightness),
     var(--jp-shadow-base-lightness),
     var(--jp-shadow-base-lightness),
     0.12
   );
   --jp-elevation-z0: none;
-  --jp-elevation-z1: 0px 2px 1px -1px var(--jp-shadow-umbra-color),
-    0px 1px 1px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 3px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z2: 0px 3px 1px -2px var(--jp-shadow-umbra-color),
-    0px 2px 2px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 5px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z4: 0px 2px 4px -1px var(--jp-shadow-umbra-color),
-    0px 4px 5px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 10px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z6: 0px 3px 5px -1px var(--jp-shadow-umbra-color),
-    0px 6px 10px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 18px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z8: 0px 5px 5px -3px var(--jp-shadow-umbra-color),
-    0px 8px 10px 1px var(--jp-shadow-penumbra-color),
-    0px 3px 14px 2px var(--jp-shadow-ambient-color);
-  --jp-elevation-z12: 0px 7px 8px -4px var(--jp-shadow-umbra-color),
-    0px 12px 17px 2px var(--jp-shadow-penumbra-color),
-    0px 5px 22px 4px var(--jp-shadow-ambient-color);
-  --jp-elevation-z16: 0px 8px 10px -5px var(--jp-shadow-umbra-color),
-    0px 16px 24px 2px var(--jp-shadow-penumbra-color),
-    0px 6px 30px 5px var(--jp-shadow-ambient-color);
-  --jp-elevation-z20: 0px 10px 13px -6px var(--jp-shadow-umbra-color),
-    0px 20px 31px 3px var(--jp-shadow-penumbra-color),
-    0px 8px 38px 7px var(--jp-shadow-ambient-color);
-  --jp-elevation-z24: 0px 11px 15px -7px var(--jp-shadow-umbra-color),
-    0px 24px 38px 3px var(--jp-shadow-penumbra-color),
-    0px 9px 46px 8px var(--jp-shadow-ambient-color);
+  --jp-elevation-z1: 0 2px 1px -1px var(--jp-shadow-umbra-color),
+    0 1px 1px 0 var(--jp-shadow-penumbra-color),
+    0 1px 3px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z2: 0 3px 1px -2px var(--jp-shadow-umbra-color),
+    0 2px 2px 0 var(--jp-shadow-penumbra-color),
+    0 1px 5px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z4: 0 2px 4px -1px var(--jp-shadow-umbra-color),
+    0 4px 5px 0 var(--jp-shadow-penumbra-color),
+    0 1px 10px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z6: 0 3px 5px -1px var(--jp-shadow-umbra-color),
+    0 6px 10px 0 var(--jp-shadow-penumbra-color),
+    0 1px 18px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z8: 0 5px 5px -3px var(--jp-shadow-umbra-color),
+    0 8px 10px 1px var(--jp-shadow-penumbra-color),
+    0 3px 14px 2px var(--jp-shadow-ambient-color);
+  --jp-elevation-z12: 0 7px 8px -4px var(--jp-shadow-umbra-color),
+    0 12px 17px 2px var(--jp-shadow-penumbra-color),
+    0 5px 22px 4px var(--jp-shadow-ambient-color);
+  --jp-elevation-z16: 0 8px 10px -5px var(--jp-shadow-umbra-color),
+    0 16px 24px 2px var(--jp-shadow-penumbra-color),
+    0 6px 30px 5px var(--jp-shadow-ambient-color);
+  --jp-elevation-z20: 0 10px 13px -6px var(--jp-shadow-umbra-color),
+    0 20px 31px 3px var(--jp-shadow-penumbra-color),
+    0 8px 38px 7px var(--jp-shadow-ambient-color);
+  --jp-elevation-z24: 0 11px 15px -7px var(--jp-shadow-umbra-color),
+    0 24px 38px 3px var(--jp-shadow-penumbra-color),
+    0 9px 46px 8px var(--jp-shadow-ambient-color);
 
   /* Borders
    *
    * The following variables, specify the visual styling of borders in JupyterLab.
    */
 
   --jp-border-width: 1px;
-  --jp-border-color0: var(--solarized-base015);
-  --jp-border-color1: var(--solarized-base015);
-  --jp-border-color2: var(--solarized-base01);
-  --jp-border-color3: var(--solarized-base00);
+  --jp-border-color0: #{$solarized-base015};
+  --jp-border-color1: #{$solarized-base015};
+  --jp-border-color2: #{color.mix($solarized-base02, $solarized-base01, 50%)};
+  --jp-border-color3: #{$solarized-base01};
   --jp-border-radius: 2px;
 
   /* UI Fonts
    *
    * The UI font CSS variables are used for the typography all of the JupyterLab
    * user interface elements that are not directly user generated content.
    *
    * The font sizing here is done assuming that the body font size of --jp-ui-font-size1
    * is applied to a parent element. When children elements, such as headings, are sized
    * in em all things will be computed relative to that body size.
    */
 
   --jp-ui-font-scale-factor: 1.2;
-  --jp-ui-font-size0: 0.83333em;
+  --jp-ui-font-size0: 0.8333em;
   --jp-ui-font-size1: 13px; /* Base font size */
   --jp-ui-font-size2: 1.2em;
   --jp-ui-font-size3: 1.44em;
-
-  --jp-ui-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica,
-  Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
+  --jp-ui-font-family: -apple-system, blinkmacsystemfont, 'Segoe UI', helvetica,
+    arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
 
   /*
    * Use these font colors against the corresponding main layout colors.
    * In a light theme, these go from dark to light.
    */
 
-  --jp-ui-font-color0: var(--solarized-base1);
-  --jp-ui-font-color1: var(--solarized-base1);
-  --jp-ui-font-color2: var(--solarized-base00);
+  --jp-ui-font-color0: #{$solarized-base1};
+  --jp-ui-font-color1: #{$solarized-base1};
+  --jp-ui-font-color2: #{$solarized-base00};
+
   /* Disabled item */
-  --jp-ui-font-color3: var(--solarized-base01);
+  --jp-ui-font-color3: #{$solarized-base01};
 
   /*
    * Use these against the brand/accent/warn/error colors.
    * These will typically go from light to darker, in both a dark and light theme.
    */
 
-  --jp-ui-inverse-font-color0: var(--solarized-base03);
-  --jp-ui-inverse-font-color1: var(--solarized-base02);
-  --jp-ui-inverse-font-color2: var(--solarized-base015);
-  --jp-ui-inverse-font-color3: var(--solarized-base015);
+  --jp-ui-inverse-font-color0: #{$solarized-base03};
+  --jp-ui-inverse-font-color1: #{$solarized-base02};
+  --jp-ui-inverse-font-color2: #{$solarized-base015};
+  --jp-ui-inverse-font-color3: #{$solarized-base015};
 
   /* Content Fonts
    *
    * Content font variables are used for typography of user generated content.
    *
    * The font sizing here is done assuming that the body font size of --jp-content-font-size1
    * is applied to a parent element. When children elements, such as headings, are sized
    * in em all things will be computed relative to that body size.
    */
 
   --jp-content-line-height: 1.6;
   --jp-content-font-scale-factor: 1.2;
-  --jp-content-font-size0: 0.83333em;
+  --jp-content-font-size0: 0.8333em;
   --jp-content-font-size1: 14px; /* Base font size */
   --jp-content-font-size2: 1.2em;
   --jp-content-font-size3: 1.44em;
   --jp-content-font-size4: 1.728em;
   --jp-content-font-size5: 2.0736em;
 
   /* This gives a magnification of about 125% in presentation mode over normal. */
   --jp-content-presentation-font-size1: 17px;
-
   --jp-content-heading-line-height: 1;
   --jp-content-heading-margin-top: 1.2em;
   --jp-content-heading-margin-bottom: 0.8em;
   --jp-content-heading-font-weight: 500;
-
-  --jp-content-font-color0: var(--solarized-base2);
-  --jp-content-font-color1: var(--solarized-base1);
-  --jp-content-font-color2: var(--solarized-base0);
-  --jp-content-font-color3: var(--solarized-base00);
-
-  --jp-content-link-color: var(--solarized-blue);
-
-  --jp-content-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI',
-    Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
+  --jp-content-font-color0: #{$solarized-base2};
+  --jp-content-font-color1: #{$solarized-base1};
+  --jp-content-font-color2: #{$solarized-base0};
+  --jp-content-font-color3: #{$solarized-base00};
+  --jp-content-link-color: #{$solarized-blue};
+  --jp-content-font-family: -apple-system, blinkmacsystemfont, 'Segoe UI',
+    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
     'Segoe UI Symbol';
 
   /*
    * Code Fonts
    *
    * Code font variables are used for typography of code and other monospaces content.
    */
 
   --jp-code-font-size: 13px;
   --jp-code-line-height: 1.3077; /* 17px for 13px base */
   --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
-  --jp-code-font-family-default: Menlo, Consolas, 'DejaVu Sans Mono', monospace;
+  --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
   --jp-code-font-family: var(--jp-code-font-family-default);
 
   /* This gives a magnification of about 125% in presentation mode over normal. */
   --jp-code-presentation-font-size: 16px;
 
   /* may need to tweak cursor width if you change font size */
   --jp-code-cursor-width0: 1.4px;
@@ -224,241 +216,259 @@
 
   /* Layout
    *
    * The following are the main layout colors use in JupyterLab. In a light
    * theme these would go from light to dark.
    */
 
-  --jp-layout-color0: var(--solarized-base03);
-  --jp-layout-color1: var(--solarized-base03);
+  --jp-layout-color0: #{$solarized-base03};
+  --jp-layout-color1: #{$solarized-base025};
+
   /* Note the separator of menu items uses --jp-layout-color2 */
-  --jp-layout-color2: var(--solarized-base02);
-  --jp-layout-color3: var(--solarized-base015);
-  --jp-layout-color4: var(--solarized-base00);
+  --jp-layout-color2: #{$solarized-base02};
+  --jp-layout-color3: #{$solarized-base015};
+  --jp-layout-color4: #{$solarized-base00};
 
   /* Inverse Layout
    *
    * The following are the inverse layout colors use in JupyterLab. In a light
    * theme these would go from dark to light.
    */
 
-  --jp-inverse-layout-color0: var(--solarized-base3);
-  --jp-inverse-layout-color1: var(--solarized-base3);
-  --jp-inverse-layout-color2: var(--solarized-base2);
-  --jp-inverse-layout-color3: var(--solarized-base1);
-  --jp-inverse-layout-color4: var(--solorized-base0);
+  --jp-inverse-layout-color0: #{$solarized-base3};
+  --jp-inverse-layout-color1: #{$solarized-base2};
+  --jp-inverse-layout-color2: #{color.mix(
+      $solarized-base2,
+      $solarized-base1,
+      50%
+    )};
+  --jp-inverse-layout-color3: #{$solarized-base1};
+  --jp-inverse-layout-color4: #{$solarized-base0};
 
   /* Brand/accent */
 
-  --jp-brand-color0: var(--solarized-blue);
-  --jp-brand-color1: var(--solarized-blue);
-  --jp-brand-color2: var(--md-blue-300);
-  --jp-brand-color3: var(--md-blue-100);
-
-  --jp-accent-color0: var(--solarized-green);
-  --jp-accent-color1: var(--solarized-green);
-  --jp-accent-color2: var(--md-green-300);
-  --jp-accent-color3: var(--md-green-100);
+  --jp-brand-color0: #{$solarized-blue};
+  --jp-brand-color1: #{color.mix($solarized-blue, $solarized-base02, 80%)};
+  --jp-brand-color2: #{color.mix($solarized-blue, $solarized-base02, 60%)};
+  --jp-brand-color3: #{color.mix($solarized-blue, $solarized-base02, 40%)};
+  --jp-accent-color0: #{$solarized-green};
+  --jp-accent-color1: #{color.mix($solarized-green, $solarized-base02, 80%)};
+  --jp-accent-color2: #{color.mix($solarized-green, $solarized-base02, 60%)};
+  --jp-accent-color3: #{color.mix($solarized-green, $solarized-base02, 40%)};
 
   /* State colors (warn, error, success, info) */
-
-  --jp-warn-color0: var(--solarized-orange);
-  --jp-warn-color1: var(--solarized-orange);
-  --jp-warn-color2: var(--md-orange-300);
-  --jp-warn-color3: var(--md-orange-100);
-
-  --jp-error-color0: var(--solarized-red);
-  --jp-error-color1: var(--solarized-red);
-  --jp-error-color2: var(--md-red-300);
-  --jp-error-color3: var(--md-red-100);
-
-  --jp-success-color0: var(--solarized-green);
-  --jp-success-color1: var(--solarized-green);
-  --jp-success-color2: var(--md-green-300);
-  --jp-success-color3: var(--md-green-100);
-
-  --jp-info-color0: var(--solarized-cyan);
-  --jp-info-color1: var(--solarized-cyan);
-  --jp-info-color2: var(--md-cyan-300);
-  --jp-info-color3: var(--md-cyan-100);
+  --jp-warn-color0: #{$solarized-orange};
+  --jp-warn-color1: #{color.mix($solarized-orange, $solarized-base02, 80%)};
+  --jp-warn-color2: #{color.mix($solarized-orange, $solarized-base02, 60%)};
+  --jp-warn-color3: #{color.mix($solarized-orange, $solarized-base02, 40%)};
+  --jp-error-color0: #{$solarized-red};
+  --jp-error-color1: #{color.mix($solarized-red, $solarized-base02, 80%)};
+  --jp-error-color2: #{color.mix($solarized-red, $solarized-base02, 60%)};
+  --jp-error-color3: #{color.mix($solarized-red, $solarized-base02, 40%)};
+  --jp-success-color0: #{$solarized-green};
+  --jp-success-color1: #{color.mix($solarized-green, $solarized-base02, 80%)};
+  --jp-success-color2: #{color.mix($solarized-green, $solarized-base02, 60%)};
+  --jp-success-color3: #{color.mix($solarized-green, $solarized-base02, 40%)};
+  --jp-info-color0: #{$solarized-cyan};
+  --jp-info-color1: #{color.mix($solarized-cyan, $solarized-base02, 80%)};
+  --jp-info-color2: #{color.mix($solarized-cyan, $solarized-base02, 60%)};
+  --jp-info-color3: #{color.mix($solarized-cyan, $solarized-base02, 40%)};
 
   /* Cell specific styles */
 
   --jp-cell-padding: 5px;
-
   --jp-cell-collapser-width: 8px;
   --jp-cell-collapser-min-height: 20px;
   --jp-cell-collapser-not-active-hover-opacity: 0.6;
-
-  --jp-cell-editor-background: var(--jp-layout-color0);
-  /* --jp-cell-editor-border-color: #93a1a1; /\* base1 *\/ */
-  --jp-cell-editor-border-color: var(--solarized-base01); /* base1 */
-  --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
-  --jp-cell-editor-active-background: var(--jp-layout-color1);
-  --jp-cell-editor-active-border-color: var(--jp-brand-color2);
-
+  --jp-cell-editor-border-color: #{$solarized-base015};
+  --jp-cell-editor-background: var(--jp-layout-color1);
+  --jp-cell-editor-active-background: #{color.mix(
+      $solarized-base03,
+      $solarized-base02,
+      70%
+    )};
+  --jp-cell-editor-active-border-color: var(--jp-input-active-border-color);
   --jp-cell-prompt-width: 64px;
   --jp-cell-prompt-font-family: 'Source Code Pro', monospace;
-  --jp-cell-prompt-letter-spacing: 0px;
+  --jp-cell-prompt-letter-spacing: 0;
   --jp-cell-prompt-opacity: 1;
   --jp-cell-prompt-not-active-opacity: 1;
-  /* --jp-cell-prompt-not-active-font-color: var(--md-grey-300); */
-  /* --jp-cell-inprompt-font-color: var(--md-grey-50); */
-  /* --jp-cell-outprompt-font-color: var(--md-grey-50); */
-  --jp-cell-prompt-not-active-font-color: var(--solarized-base0);
-  --jp-cell-inprompt-font-color: var(--solarized-base0);
-  --jp-cell-outprompt-font-color: var(--solarized-base0);
+  --jp-cell-prompt-not-active-font-color: #{$solarized-base0};
+  --jp-cell-inprompt-font-color: #{$solarized-blue};
+  --jp-cell-outprompt-font-color: #{$solarized-orange};
 
   /* Notebook specific styles */
 
   --jp-notebook-padding: 10px;
-  /* --jp-notebook-select-background is not seen in jupyterlab codebase*/
+
+  /* --jp-notebook-select-background is not seen in jupyterlab codebase */
   --jp-notebook-select-background: var(--jp-layout-color1);
   --jp-notebook-multiselected-color: #268bd230;
 
   /* The scroll padding is calculated to fill enough space at the bottom of the
   notebook to show one single-line cell (with appropriate padding) at the top
   when the notebook is scrolled all the way to the bottom. We also subtract one
   pixel so that no scrollbar appears if we have just one single-line cell in the
   notebook. This padding is to enable a 'scroll past end' feature in a notebook.
   */
+  /* stylelint-disable scss/operator-no-newline-after */
   --jp-notebook-scroll-padding: calc(
     100% - var(--jp-code-font-size) * var(--jp-code-line-height) -
       var(--jp-code-padding) - var(--jp-cell-padding) - 1px
   );
+  /* stylelint-enable scss/operator-no-newline-after */
 
   /* Rendermime styles */
 
   --jp-rendermime-error-background: #dc322f38;
   --jp-rendermime-table-row-background: var(--jp-layout-color2);
   --jp-rendermime-table-row-hover-background: rgba(3, 169, 244, 0.2);
 
   /* Dialog specific styles */
+
   /* Dialog overlay background color */
   --jp-dialog-background: rgba(0, 0, 0, 0.6);
 
   /* Console specific styles */
 
   --jp-console-padding: 10px;
 
   /* Toolbar specific styles */
 
   --jp-toolbar-border-color: var(--jp-layout-color3);
   --jp-toolbar-micro-height: 8px;
   --jp-toolbar-background: var(--jp-layout-color0);
-  --jp-toolbar-box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.8);
-  --jp-toolbar-header-margin: 4px 4px 0px 4px;
+  --jp-toolbar-box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.8);
+  --jp-toolbar-header-margin: 4px 4px 0 4px;
   --jp-toolbar-active-background: var(--jp-layout-color0);
 
   /* Statusbar specific styles */
 
   --jp-statusbar-height: 24px;
 
   /* Input field styles */
 
-  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
   --jp-input-active-background: var(--jp-layout-color0);
   --jp-input-hover-background: var(--jp-layout-color2);
   --jp-input-background: var(--jp-layout-color3);
-  --jp-input-border-color: var(--jp-border-color1);
-  --jp-input-active-border-color: var(--jp-brand-color1);
+  --jp-input-border-color: var(--jp-border-color2);
+  --jp-input-active-border-color: #{color.mix(
+      $solarized-blue,
+      $solarized-base03,
+      80%
+    )};
   --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);
 
   /* General editor styles */
 
   --jp-editor-selected-background: var(--jp-layout-color0);
   --jp-editor-selected-focused-background: rgba(33, 150, 243, 0.24);
   --jp-editor-cursor-color: var(--jp-ui-font-color0);
 
   /* Code mirror specific styles */
 
-  --jp-mirror-editor-keyword-color: var(--solarized-green);
-  --jp-mirror-editor-atom-color: var(--solarized-blue);
-  --jp-mirror-editor-number-color: var(--solarized-magenta);
-  --jp-mirror-editor-def-color: var(--solarized-red);
-  --jp-mirror-editor-variable-color: var(--solarized-base0);
-  --jp-mirror-editor-variable-2-color: var(--solarized-base00);
-  --jp-mirror-editor-variable-3-color: var(--solarized-base01);
-  --jp-mirror-editor-punctuation-color: var(--solarized-base0);
-  --jp-mirror-editor-property-color: var(--solarized-blue);
-  --jp-mirror-editor-operator-color: var(--solarized-base0);
-  --jp-mirror-editor-comment-color: var(--solarized-base01);
-  --jp-mirror-editor-string-color: var(--solarized-cyan);
-  --jp-mirror-editor-string-2-color: #f50;
-  --jp-mirror-editor-meta-color: #aa22ff;
+  --jp-mirror-editor-keyword-color: #{$solarized-green};
+  --jp-mirror-editor-atom-color: #{$solarized-blue};
+  --jp-mirror-editor-number-color: #{$solarized-magenta};
+  --jp-mirror-editor-def-color: #{$solarized-blue};
+  --jp-mirror-editor-variable-color: #{$solarized-base0};
+  --jp-mirror-editor-variable-2-color: #{$solarized-base00};
+  --jp-mirror-editor-variable-3-color: #{$solarized-base01};
+  --jp-mirror-editor-punctuation-color: #{$solarized-base0};
+  --jp-mirror-editor-property-color: #{$solarized-blue};
+  --jp-mirror-editor-operator-color: #{$solarized-base0};
+  --jp-mirror-editor-comment-color: #{$solarized-base01};
+  --jp-mirror-editor-string-color: #{$solarized-cyan};
+  --jp-mirror-editor-string-2-color: #{$solarized-orange};
+  --jp-mirror-editor-meta-color: #{$solarized-magenta};
   --jp-mirror-editor-qualifier-color: #555;
-  --jp-mirror-editor-builtin-color: var(--md-green-600);
+  --jp-mirror-editor-builtin-color: #{$solarized-green};
   --jp-mirror-editor-bracket-color: #997;
-  --jp-mirror-editor-tag-color: var(--md-green-700);
-  --jp-mirror-editor-attribute-color: var(--md-blue-700);
-  --jp-mirror-editor-header-color: var(--md-blue-500);
-  --jp-mirror-editor-quote-color: var(--md-green-300);
-  --jp-mirror-editor-link-color: var(--md-blue-700);
-  --jp-mirror-editor-error-color: #f00;
+  --jp-mirror-editor-tag-color: #{$solarized-green};
+  --jp-mirror-editor-attribute-color: #{$solarized-blue};
+  --jp-mirror-editor-header-color: #{color.mix(
+      $solarized-blue,
+      $solarized-base2,
+      90%
+    )};
+  --jp-mirror-editor-quote-color: #{$solarized-cyan};
+  --jp-mirror-editor-link-color: #{$solarized-blue};
+  --jp-mirror-editor-error-color: #{$solarized-red};
   --jp-mirror-editor-hr-color: #999;
 
+  /* User colors */
+
+  --jp-collaborator-color1: #ad4a00;
+  --jp-collaborator-color2: #7b6a00;
+  --jp-collaborator-color3: #007e00;
+  --jp-collaborator-color4: #008772;
+  --jp-collaborator-color5: #0079b9;
+  --jp-collaborator-color6: #8b45c6;
+  --jp-collaborator-color7: #be208b;
+
+  /* File or activity icons and switch semantic variables */
+
+  --jp-jupyter-icon-color: var(--md-orange-900);
+  --jp-notebook-icon-color: var(--md-orange-700);
+  --jp-json-icon-color: #{$solarized-orange};
+  --jp-console-icon-background-color: #{$solarized-blue};
+  --jp-console-icon-color: #{$solarized-base3};
+  --jp-terminal-icon-background-color: var(--jp-inverse-layout-color2);
+  --jp-terminal-icon-color: #{$solarized-base02};
+  --jp-text-editor-icon-color: #{$solarized-base2};
+  --jp-inspector-icon-color: #{$solarized-base2};
+  --jp-switch-color: #{$solarized-base1};
+  --jp-switch-true-position-color: #{$solarized-green};
+  --jp-switch-cursor-color: rgba(0, 0, 0, 0.8);
+
   /* Vega extension styles */
 
-  --jp-vega-background: var(--solarized-base0);
+  --jp-vega-background: #{$solarized-base0};
 
   /* Sidebar-related styles */
 
   --jp-sidebar-min-width: 180px;
 
   /* Search-related styles */
 
   --jp-search-toggle-off-opacity: 0.4;
   --jp-search-toggle-hover-opacity: 0.7;
   --jp-search-toggle-on-opacity: 1;
-  --jp-search-selected-match-background-color: var(--solarized-yellow);
-  --jp-search-selected-match-color: var(--solarized-base02);
+  --jp-search-selected-match-background-color: #{$solarized-yellow};
+  --jp-search-selected-match-color: #{$solarized-base02};
   --jp-search-unselected-match-background-color: var(
     --jp-inverse-layout-color0
   );
   --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);
 
   /* scrollbar related styles. Supports every browser except Edge. */
 
-  --jp-scrollbar-background-color: var(--solarized-base03);
+  --jp-scrollbar-background-color: #{$solarized-base03};
   --jp-scrollbar-thumb-color: 21, 102, 103; /* need to specify thumb color as an RGB triplet */
-
   --jp-scrollbar-endpad: 3px; /* the minimum gap between the thumb and the ends of a scrollbar */
 
   /* hacks for setting the thumb shape. These do nothing in Firefox */
 
   --jp-scrollbar-thumb-margin: 3.5px; /* the space in between the sides of the thumb and the track */
   --jp-scrollbar-thumb-radius: 9px; /* set to a large-ish value for rounded endcaps on the thumb */
 
   /* Icon colors that work well with light or dark backgrounds */
-  --jp-icon-contrast-color0: var(--md-purple-600);
-  --jp-icon-contrast-color1: var(--md-green-600);
-  --jp-icon-contrast-color2: var(--md-pink-600);
-  --jp-icon-contrast-color3: var(--md-blue-600);
+  --jp-icon-contrast-color0: #{$solarized-violet};
+  --jp-icon-contrast-color1: #{$solarized-green};
+  --jp-icon-contrast-color2: #{$solarized-magenta};
+  --jp-icon-contrast-color3: #{$solarized-blue};
+
+  /* Button colors */
+  --jp-accept-color-normal: #{$solarized-blue};
+  --jp-accept-color-hover: #{color.mix($solarized-blue, $solarized-base02, 80%)};
+  --jp-accept-color-active: #{color.mix($solarized-blue, $solarized-base02, 60%)};
+  --jp-warn-color-normal: #{$solarized-red};
+  --jp-warn-color-hover: #{color.mix($solarized-red, $solarized-base02, 80%)};
+  --jp-warn-color-active: #{color.mix($solarized-red, $solarized-base02, 60%)};
+  --jp-reject-color-normal: #{$solarized-base0};
+  --jp-reject-color-hover: #{$solarized-base01};
+  --jp-reject-color-active: #{color.mix(
+      $solarized-base01,
+      $solarized-base02,
+      70%
+    )};
 }
-
-/*-----------------------------------------------------------------------------
-| Copyright (c) Jupyter Development Team.
-| Distributed under the terms of the Modified BSD License.
-|----------------------------------------------------------------------------*/
-
-/* Set the default typography for monospace elements */
-tt,
-code,
-kbd,
-samp,
-pre {
-  font-family: var(--jp-code-font-family);
-  font-size: var(--jp-code-font-size);
-  line-height: var(--jp-code-line-height);
-}
-
-/* Disable code mirror text-shadow when searching for readability */
-.cm-searching {
-  text-shadow: none;
-}
-
-.jp-RenderedText.jp-OutputArea-output[data-mime-type="application/vnd.jupyter.stderr"] pre{
-  color: var(--solarized-base2);
-}
-
-
-
```

### Comparing `jupyterlab_theme_solarized_dark-2.1.0/src/index.ts` & `jupyterlab_theme_solarized_dark-3.0.0/src/index.ts`

 * *Files 21% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 import { IThemeManager } from '@jupyterlab/apputils';
 
 /**
  * Initialization data for the jupyterlab-theme-solarized-dark extension.
  */
 const plugin: JupyterFrontEndPlugin<void> = {
   id: 'jupyterlab-theme-solarized-dark:plugin',
+  description: 'Solarized dark theme for JupyterLab.',
   autoStart: true,
   requires: [IThemeManager],
   activate: (app: JupyterFrontEnd, manager: IThemeManager) => {
+    console.log(
+      'JupyterLab extension jupyterlab-theme-solarized-dark is activated!'
+    );
     const style = 'jupyterlab-theme-solarized-dark/index.css';
 
     manager.register({
       name: 'JupyterLab Solarized Dark',
       isLight: false,
       themeScrollbars: true,
       load: () => manager.loadCSS(style),
```

### Comparing `jupyterlab_theme_solarized_dark-2.1.0/style/base.css` & `jupyterlab_theme_solarized_dark-3.0.0/style/index.scss`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-/* -----------------------------------------------------------------------------
-| Copyright (c) Jupyter Development Team.
-| Distributed under the terms of the Modified BSD License.
-|---------------------------------------------------------------------------- */
-
-@import './variables.css';
+@use './variables.scss';
 
 /* Set the default typography for monospace elements */
 tt,
 code,
 kbd,
 samp,
 pre {
```

### Comparing `jupyterlab_theme_solarized_dark-2.1.0/tsconfig.json` & `jupyterlab_theme_solarized_dark-3.0.0/tsconfig.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'compilerOptions'": "{'target': 'ES2018'}"}*

```diff
@@ -13,14 +13,14 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
+        "target": "ES2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

