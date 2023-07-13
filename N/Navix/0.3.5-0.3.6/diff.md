# Comparing `tmp/Navix-0.3.5.tar.gz` & `tmp/Navix-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Navix-0.3.5.tar", last modified: Sat Jul  1 07:54:26 2023, max compression
+gzip compressed data, was "Navix-0.3.6.tar", last modified: Thu Jul 13 08:33:06 2023, max compression
```

## Comparing `Navix-0.3.5.tar` & `Navix-0.3.6.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.787100 Navix-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.779101 Navix-0.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-01 07:54:16.000000 Navix-0.3.5/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-01 07:54:16.000000 Navix-0.3.5/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-01 07:54:16.000000 Navix-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-01 07:54:16.000000 Navix-0.3.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-01 07:54:16.000000 Navix-0.3.5/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-01 07:54:16.000000 Navix-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 07:54:16.000000 Navix-0.3.5/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/Navix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18431 2023-07-01 07:54:26.000000 Navix-0.3.5/Navix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 07:54:26.000000 Navix-0.3.5/Navix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:54:26.000000 Navix-0.3.5/Navix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-01 07:54:26.000000 Navix-0.3.5/Navix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 07:54:26.000000 Navix-0.3.5/Navix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18431 2023-07-01 07:54:26.783100 Navix-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-01 07:54:16.000000 Navix-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-01 07:54:16.000000 Navix-0.3.5/docs/design_notes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-01 07:54:16.000000 Navix-0.3.5/docs/performance.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/navix/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/navix/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/environments/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/environments/keydoor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/environments/room.py
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/terminations.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 07:54:17.000000 Navix-0.3.5/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-01 07:54:16.000000 Navix-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-01 07:54:16.000000 Navix-0.3.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-07-01 07:54:16.000000 Navix-0.3.5/scripts/release.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 07:54:26.787100 Navix-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/minigrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/minigrid_report.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/observations_keydoor_report.txt
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/observations_room_report.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_terminations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.464160 Navix-0.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.464160 Navix-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-13 08:32:52.000000 Navix-0.3.6/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-13 08:32:52.000000 Navix-0.3.6/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-13 08:32:52.000000 Navix-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 08:32:52.000000 Navix-0.3.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 08:32:52.000000 Navix-0.3.6/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-13 08:32:52.000000 Navix-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 08:32:52.000000 Navix-0.3.6/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.464160 Navix-0.3.6/Navix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-13 08:33:06.000000 Navix-0.3.6/Navix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-13 08:33:06.000000 Navix-0.3.6/Navix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:33:06.000000 Navix-0.3.6/Navix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 08:33:06.000000 Navix-0.3.6/Navix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 08:33:06.000000 Navix-0.3.6/Navix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-13 08:33:06.468160 Navix-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-13 08:32:52.000000 Navix-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.464160 Navix-0.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-13 08:32:52.000000 Navix-0.3.6/docs/design_notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-13 08:32:52.000000 Navix-0.3.6/docs/performance.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-13 08:32:52.000000 Navix-0.3.6/docs/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/navix/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/navix/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/environments/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/environments/keydoor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/environments/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/terminations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-13 08:32:52.000000 Navix-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-13 08:32:52.000000 Navix-0.3.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-07-13 08:32:52.000000 Navix-0.3.6/scripts/release.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:33:06.468160 Navix-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/minigrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/minigrid_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/observations_keydoor_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/observations_room_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_terminations.py
```

### Comparing `Navix-0.3.5/.github/workflows/CD.yml` & `Navix-0.3.6/.github/workflows/CD.yml`

 * *Files 10% similar despite different names*

```diff
@@ -15,37 +15,33 @@
           VERSION_FILE="$/navix/_version.py"
           NAVIX_VERSION="$(cat navix/_version.py | grep '__version__ = ' |  cut -d'=' -f2 | sed 's,\",,g' | sed "s,\',,g" | sed 's, ,,g')"
           echo "Current version is:"
           echo "$NAVIX_VERSION"
 
           echo "NAVIX_VERSION=$NAVIX_VERSION" >> $GITHUB_ENV
 
-      - name: Create and push tag
-        run: |
-          echo "Creating tag ${{ env.NAVIX_VERSION }}"
-          git tag ${{ env.NAVIX_VERSION }}
-          git push --tags
-
-      - name: Create changelog
+      - name: Create changelog and push tag
         id: changelog
         uses: TriPSs/conventional-changelog-action@v3
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
-          output-file: "false"
+          output-file: false
+          fallback-version: ${{ env.NAVIX_VERSION }}
+          skip-commit: true
 
       - name: Create Release
         uses: ncipollo/release-action@v1
         with:
           tag: ${{ env.NAVIX_VERSION }}
           name: "NAVIX release v${{ env.NAVIX_VERSION }}"
           body: ${{ steps.changelog.outputs.clean_changelog }}
 
       - uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python_version }}
+          python-version: '3.10'
 
       - name: Install pypa/build
         run: |
           python -m pip install build
 
       - name: Build wheel and sdist
         run: |
```

### Comparing `Navix-0.3.5/.github/workflows/CI.yml` & `Navix-0.3.6/.github/workflows/CI.yml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       matrix:
         os: ["ubuntu"]
     continue-on-error: false
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
-        python-version: 3.9
+        python-version: '3.10'
     - name: Setup navix
       run: |
         pip install . -v
     - name: Check code quality
       run: |
         pip install pylint
         MESSAGE=$(pylint -ry $(git ls-files '*.py') ||:)
```

### Comparing `Navix-0.3.5/.gitignore` & `Navix-0.3.6/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# setuptools_scm
-helx/version.py
-
 # developing
 playground.ipynb
 
 # vscode
 .vscode/
 wandb/
 .DS_Store
```

### Comparing `Navix-0.3.5/COPYRIGHT` & `Navix-0.3.6/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `Navix-0.3.5/LICENSE` & `Navix-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.3.5/Navix.egg-info/PKG-INFO` & `Navix-0.3.6/Navix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.3.5
+Version: 0.3.6
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -234,32 +234,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 License-File: AUTHORS
 
-# NAVIX
+# NAVIX: minigrid in JAX
 
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
+![PyPI version](https://img.shields.io/pypi/v/navix?label=PyPI&color=%230099ab)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
 NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
-You can see a superficial performance comparison [here](docs/profiling.ipynb).
+You can see a superficial performance comparison [here](docs/performance.ipynb).
 
 The library is in active development, and we are working on adding more environments and features.
 If you want join the development and contribute, please [open a discussion](https://github.com/epignatelli/navix/discussions/new?category=general) and let's have a chat!
 
 
 ## Installation
 We currently support the OSs supported by JAX.
@@ -315,15 +315,15 @@
 
 Another use case it to backpropagate through the environment transition function, for example to learn a world model.
 
 TODO(epignatelli): add example.
 
 
 ## Cite
-If you use `helx` please consider citing it as:
+If you use `navix` please consider citing it as:
 
 ```bibtex
 @misc{pignatelli2023navix,
   author = {Pignatelli, Eduardo},
   title = {Navix: Accelerated gridworld navigation with JAX},
   year = {2023},
   publisher = {GitHub},
```

### Comparing `Navix-0.3.5/Navix.egg-info/SOURCES.txt` & `Navix-0.3.6/Navix.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 .gitignore
 AUTHORS
 COPYRIGHT
 LICENSE
 NOTICE
 README.md
-package.json
 pyproject.toml
 requirements.txt
 ./requirements.txt
 .github/workflows/CD.yml
 .github/workflows/CI.yml
 Navix.egg-info/PKG-INFO
 Navix.egg-info/SOURCES.txt
 Navix.egg-info/dependency_links.txt
 Navix.egg-info/requires.txt
 Navix.egg-info/top_level.txt
 docs/design_notes.md
 docs/performance.ipynb
+docs/performance.py
 navix/__init__.py
 navix/_version.py
 navix/actions.py
 navix/components.py
+navix/config.py
 navix/entities.py
 navix/graphics.py
 navix/grid.py
 navix/observations.py
 navix/tasks.py
 navix/terminations.py
 navix/environments/__init__.py
```

### Comparing `Navix-0.3.5/PKG-INFO` & `Navix-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.3.5
+Version: 0.3.6
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -234,32 +234,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 License-File: AUTHORS
 
-# NAVIX
+# NAVIX: minigrid in JAX
 
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
+![PyPI version](https://img.shields.io/pypi/v/navix?label=PyPI&color=%230099ab)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
 NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
-You can see a superficial performance comparison [here](docs/profiling.ipynb).
+You can see a superficial performance comparison [here](docs/performance.ipynb).
 
 The library is in active development, and we are working on adding more environments and features.
 If you want join the development and contribute, please [open a discussion](https://github.com/epignatelli/navix/discussions/new?category=general) and let's have a chat!
 
 
 ## Installation
 We currently support the OSs supported by JAX.
@@ -315,15 +315,15 @@
 
 Another use case it to backpropagate through the environment transition function, for example to learn a world model.
 
 TODO(epignatelli): add example.
 
 
 ## Cite
-If you use `helx` please consider citing it as:
+If you use `navix` please consider citing it as:
 
 ```bibtex
 @misc{pignatelli2023navix,
   author = {Pignatelli, Eduardo},
   title = {Navix: Accelerated gridworld navigation with JAX},
   year = {2023},
   publisher = {GitHub},
```

### Comparing `Navix-0.3.5/README.md` & `Navix-0.3.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# NAVIX
+# NAVIX: minigrid in JAX
 
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
+![PyPI version](https://img.shields.io/pypi/v/navix?label=PyPI&color=%230099ab)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
 NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
-You can see a superficial performance comparison [here](docs/profiling.ipynb).
+You can see a superficial performance comparison [here](docs/performance.ipynb).
 
 The library is in active development, and we are working on adding more environments and features.
 If you want join the development and contribute, please [open a discussion](https://github.com/epignatelli/navix/discussions/new?category=general) and let's have a chat!
 
 
 ## Installation
 We currently support the OSs supported by JAX.
@@ -69,15 +69,15 @@
 
 Another use case it to backpropagate through the environment transition function, for example to learn a world model.
 
 TODO(epignatelli): add example.
 
 
 ## Cite
-If you use `helx` please consider citing it as:
+If you use `navix` please consider citing it as:
 
 ```bibtex
 @misc{pignatelli2023navix,
   author = {Pignatelli, Eduardo},
   title = {Navix: Accelerated gridworld navigation with JAX},
   year = {2023},
   publisher = {GitHub},
```

### Comparing `Navix-0.3.5/docs/design_notes.md` & `Navix-0.3.6/docs/design_notes.md`

 * *Files identical despite different names*

### Comparing `Navix-0.3.5/docs/performance.ipynb` & `Navix-0.3.6/docs/performance.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953226461038961%*

 * *Differences: {"'cells'": "{0: {'source': ['<a "*

 * *            'href="https://colab.research.google.com/github/epignatelli/navix/blob/master/docs/performance.ipynb" '*

 * *            'target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" '*

 * *            'alt="Open In Colab"/></a>\']}, 2: {\'source\': {insert: [(13, \'N_TIMESTEPS = '*

 * *            "1_000\\n'), (14, 'N_SEEDS = 10_000\\n'), (18, '    env = nx.environments.Room(16, 16, "*

 * *            "8)\\n'), (23, '    timestep, _ = jax.lax.while_loop(\\ […]*

```diff
@@ -4,15 +4,15 @@
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "colab_type": "text",
                 "id": "view-in-github"
             },
             "source": [
-                "<a href=\"https://colab.research.google.com/gist/epignatelli/da5c0f63b8c4a189ae261232121ae446/navix_profiling.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
+                "<a href=\"https://colab.research.google.com/github/epignatelli/navix/blob/master/docs/performance.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "colab": {
@@ -43,26 +43,29 @@
                 "import random\n",
                 "import time\n",
                 "\n",
                 "from timeit import timeit\n",
                 "\n",
                 "\n",
                 "N_TIMEIT_LOOPS = 5\n",
-                "N_TIMESTEPS = 100\n",
-                "N_SEEDS = 10\n",
+                "N_TIMESTEPS = 1_000\n",
+                "N_SEEDS = 10_000\n",
                 "\n",
                 "\n",
                 "def profile_navix(seed):\n",
-                "    env = nx.environments.Room(16, 16, 8, observation_fn=nx.observations.rgb)\n",
+                "    env = nx.environments.Room(16, 16, 8)\n",
                 "    key = jax.random.PRNGKey(seed)\n",
                 "    timestep = env.reset(key)\n",
                 "    actions = jax.random.randint(key, (N_TIMESTEPS,), 0, 6)\n",
                 "\n",
-                "    for i in range(N_TIMESTEPS):\n",
-                "        timestep = env.step(timestep, actions[i])\n",
+                "    timestep, _ = jax.lax.while_loop(\n",
+                "        lambda x: x[1] < N_TIMESTEPS,\n",
+                "        lambda x: (env.step(x[0], actions[x[1]]), x[1] + 1),\n",
+                "        (timestep, jnp.asarray(0)),\n",
+                "    )\n",
                 "\n",
                 "    return timestep\n",
                 "\n",
                 "\n",
                 "def profile_minigrid(seed):\n",
                 "    env = gym.make(\"MiniGrid-Empty-16x16-v0\", render_mode=None)\n",
                 "    observation, info = env.reset(seed=42)\n",
@@ -81,15 +84,19 @@
                 "    print(\n",
                 "        \"Profiling navix, N_SEEDS = {}, N_TIMESTEPS = {}\".format(N_SEEDS, N_TIMESTEPS)\n",
                 "    )\n",
                 "    seeds = jnp.arange(N_SEEDS)\n",
                 "\n",
                 "    print(\"\\tCompiling...\")\n",
                 "    start = time.time()\n",
-                "    f = jax.jit(jax.vmap(profile_navix)).lower(seeds).compile()\n",
+                "    n_devices = jax.local_device_count()\n",
+                "    seeds = seeds.reshape(n_devices, N_SEEDS // n_devices)\n",
+                "    f = jax.vmap(profile_navix, axis_name=\"batch\")\n",
+                "    f = jax.pmap(f, axis_name=\"device\")\n",
+                "    f = f.lower(seeds).compile()\n",
                 "    print(\"\\tCompiled in {:.2f}s\".format(time.time() - start))\n",
                 "\n",
                 "    print(\"\\tRunning ...\")\n",
                 "    res_navix = timeit(\n",
                 "        lambda: f(seeds).state.grid.block_until_ready(), number=N_TIMEIT_LOOPS\n",
                 "    )\n",
                 "    print(res_navix)\n",
```

### Comparing `Navix-0.3.5/navix/__init__.py` & `Navix-0.3.6/navix/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,9 @@
     entities,
     graphics,
     grid,
     observations,
     tasks,
     environments,
     terminations,
+    config,
 )
```

### Comparing `Navix-0.3.5/navix/_version.py` & `Navix-0.3.6/navix/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `Navix-0.3.5/navix/actions.py` & `Navix-0.3.6/navix/actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,55 +14,73 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from __future__ import annotations
-from typing import Tuple
 
 import jax
 import jax.numpy as jnp
 from jax import Array
 
-from .entities import Door, Key, State
+from .entities import Entities, State
 from .components import DISCARD_PILE_COORDS
 from .grid import translate, rotate, positions_equal
+from jax_enums import Enumerable as Enum
 
 
-DIRECTIONS = {0: "east", 1: "south", 2: "west", 3: "north"}
+class Directions(Enum):
+    EAST = 0
+    SOUTH = 1
+    WEST = 2
+    NORTH = 3
 
 
 def _rotate(state: State, spin: int) -> State:
-    direction = rotate(state.players.direction, spin)
-    player = state.players.replace(direction=direction)
-    return state.replace(players=player)
+    if "player" not in state.entities:
+        return state
+
+    player = state.get_player(idx=0)
+
+    # update player's direction
+    direction = rotate(player.direction, spin)
+
+    # update sprite representation
+    player = player.replace(direction=direction)
+
+    state = state.set_player(player)
+
+    return state
 
 
 def _walkable(state: State, position: Array) -> Array:
     # according to the grid
     walkable = jnp.equal(state.grid[tuple(position)], 0)
 
-    # and not occupied by another non-walkable entity
-    occupied_keys = positions_equal(position, state.keys.position)
-    # occupied by a door, and door is not open
-    occupied_doors = positions_equal(position, state.doors.position)
-    occupied_doors = occupied_doors & ~state.doors.open
-
-    occupied = jnp.any(jnp.logical_or(occupied_keys, occupied_doors))
-    # return: if walkable and not occupied
-    return jnp.logical_and(walkable, jnp.logical_not(occupied))
+    for k in state.entities:
+        obstructs = jnp.logical_and(
+            jnp.logical_not(state.entities[k].walkable),
+            positions_equal(state.entities[k].position, position),
+        )
+        walkable = jnp.logical_and(walkable, jnp.any(jnp.logical_not(obstructs)))
+    return jnp.asarray(walkable, dtype=jnp.bool_)
 
 
 def _move(state: State, direction: Array) -> State:
-    new_position = translate(state.players.position, direction)
+    if "player" not in state.entities:
+        return state
+
+    player = state.get_player(idx=0)
+    new_position = translate(player.position, direction)
     can_move = _walkable(state, new_position)
-    new_position = jnp.where(can_move, new_position, state.players.position)
-    player = state.players.replace(position=new_position)
-    return state.replace(players=player)
+    new_position = jnp.where(can_move, new_position, player.position)
+    player = player.replace(position=new_position)
+    state = state.set_player(player)
+    return state
 
 
 def undefined(state: State) -> State:
     # this is problematic because jax.lax.switch evaluates
     # all *python* branches (no XLA computation is performed)
     # even though only one is selected
     # one option is the following, but this breaks type checking
@@ -81,68 +99,94 @@
 
 
 def rotate_ccw(state: State) -> State:
     return _rotate(state, -1)
 
 
 def forward(state: State) -> State:
-    return _move(state, state.players.direction)
+    player = state.get_player(idx=0)
+    return _move(state, player.direction)
 
 
 def right(state: State) -> State:
-    return _move(state, state.players.direction + 1)
+    player = state.get_player(idx=0)
+    return _move(state, player.direction + 1)
 
 
 def backward(state: State) -> State:
-    return _move(state, state.players.direction + 2)
+    player = state.get_player(idx=0)
+    return _move(state, player.direction + 2)
 
 
 def left(state: State) -> State:
-    return _move(state, state.players.direction + 3)
+    player = state.get_player(idx=0)
+    return _move(state, player.direction + 3)
 
 
 def pickup(state: State) -> State:
-    position_in_front = translate(state.players.position, state.players.direction)
+    if Entities.KEY.value not in state.entities:
+        return state
 
-    key_found = positions_equal(position_in_front, state.keys.position)
+    player = state.get_player(idx=0)
+    keys = state.get_keys()
+
+    position_in_front = translate(player.position, player.direction)
+
+    key_found = positions_equal(position_in_front, keys.position)
 
     # update keys
-    positions = jnp.where(key_found, DISCARD_PILE_COORDS, state.keys.position)
-    keys = state.keys.replace(position=positions)
+    positions = jnp.where(key_found, DISCARD_PILE_COORDS, keys.position)
+    keys = keys.replace(position=positions)
 
     # update player's pocket, if the pocket has something else, we overwrite it
-    key = jnp.sum(state.keys.id * key_found, dtype=jnp.int32)
-    player = jax.lax.cond(jnp.any(key_found), lambda: state.players.replace(pocket=key), lambda: state.players)
+    key = jnp.sum(keys.id * key_found, dtype=jnp.int32)
+    player = jax.lax.cond(
+        jnp.any(key_found), lambda: player.replace(pocket=key), lambda: player
+    )
 
-    return state.replace(players=player, keys=keys)
+    state = state.set_player(player)
+    state = state.set_keys(keys)
+    return state
 
 
 def open(state: State) -> State:
     """Unlocks and opens an openable object (like a door) if possible"""
+
+    if "door" not in state.entities:
+        return state
+
     # get the tile in front of the player
-    position_in_front = translate(state.players.position, state.players.direction)
+    player = state.get_player(idx=0)
+    doors = state.get_doors()
+
+    position_in_front = translate(player.position, player.direction)
 
     # check if there is a door in front of the player
-    door_found = positions_equal(position_in_front, state.doors.position)
+    door_found = positions_equal(position_in_front, doors.position)
 
     # and that, if so, either it does not require a key or the player has the key
-    requires_key = state.doors.requires != -1
-    key_match = state.players.pocket == state.doors.requires
-    can_open = door_found & (key_match | ~requires_key )
+    requires_key = doors.requires != -1
+    key_match = player.pocket == doors.requires
+    can_open = door_found & (key_match | ~requires_key)
 
     # update doors if closed and can_open
-    do_open = (~state.doors.open & can_open)
-    open = jnp.where(do_open, True, state.doors.open)
-    doors = state.doors.replace(open=open)
+    do_open = ~doors.open & can_open
+    open = jnp.where(do_open, True, doors.open)
+    doors = doors.replace(open=open)
 
     # remove key from player's pocket
-    pocket = jnp.asarray(state.players.pocket * jnp.any(can_open), dtype=jnp.int32)
-    player = jax.lax.cond(jnp.any(can_open), lambda: state.players.replace(pocket=pocket), lambda: state.players)
+    pocket = jnp.asarray(player.pocket * jnp.any(can_open), dtype=jnp.int32)
+    player = jax.lax.cond(
+        jnp.any(can_open), lambda: player.replace(pocket=pocket), lambda: player
+    )
 
-    return state.replace(players=player, doors=doors)
+    state = state.set_player(player)
+    state = state.set_doors(doors)
+
+    return state
 
 
 # TODO(epignatelli): a mutable dictionary here is dangerous
 ACTIONS = {
     # -1: undefined,
     0: noop,
     1: rotate_cw,
```

### Comparing `Navix-0.3.5/navix/components.py` & `Navix-0.3.6/navix/components.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,80 +15,75 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
-from enum import IntEnum
+from typing import Tuple
+
 
 from jax import Array
 from flax import struct
 import jax.numpy as jnp
+import dataclasses
 
 
 DISCARD_PILE_COORDS = jnp.asarray((0, -1), dtype=jnp.int32)
 DISCARD_PILE_IDX = jnp.asarray(-1, dtype=jnp.int32)
 EMPTY_POCKET_ID = jnp.asarray(-1, dtype=jnp.int32)
 UNSET_DIRECTION = jnp.asarray(-1, dtype=jnp.int32)
 UNSET_CONSUMED = jnp.asarray(-1, dtype=jnp.int32)
 
 
-class EntityType(IntEnum):
-    WALL = 0
-    FLOOR = 1
-    PLAYER = 2
-    GOAL = 3
-    KEY = 4
-    DOOR = 5
+def field(shape: Tuple[int, ...], **kwargs):
+    return dataclasses.field(metadata={"shape": shape}, **kwargs)
 
 
 class Component(struct.PyTreeNode):
-    entity_type: Array = jnp.asarray(0, dtype=jnp.int32)
-    """The type of the entity, 0 = player, 1 = goal, 2 = key, 3 = door"""
-
-    def get_sprite(self, registry: Array) -> Array:
-        raise NotImplementedError()
+    def check_ndim(self, batched: bool = False) -> None:
+        return
 
-    @property
-    def walkable(self) -> Array:
-        raise NotImplementedError()
 
-    def is_transparent(self) -> Array:
-        raise NotImplementedError()
-
-
-class Positionable(struct.PyTreeNode):
-    position: Array = DISCARD_PILE_COORDS
+class Positionable(Component):
+    position: Array = field(shape=(2,))
     """The (row, column) position of the entity in the grid, defaults to the discard pile (-1, -1)"""
 
 
-class Directional(struct.PyTreeNode):
-    direction: Array = jnp.asarray(0, dtype=jnp.int32)
+class Directional(Component):
+    direction: Array = field(shape=())
     """The direction the entity: 0 = east, 1 = south, 2 = west, 3 = north"""
 
 
-class HasTag(struct.PyTreeNode):
-    tag: Array = jnp.asarray(0, dtype=jnp.int32)
-    """The tag of the component, used to identify the type of the component in `oobservations.categorical`"""
-
-
-class Stochastic(struct.PyTreeNode):
-    probability: Array = jnp.asarray(1.0, dtype=jnp.float32)
+class Stochastic(Component):
+    probability: Array = field(shape=())
     """The probability of receiving the reward, if reached."""
 
 
-class Openable(struct.PyTreeNode):
-    requires: Array = EMPTY_POCKET_ID
+class Openable(Component):
+    requires: Array = field(shape=())
     """The id of the item required to consume this item. If set, it must be >= 1."""
-    open: Array = jnp.asarray(False, dtype=jnp.bool_)
+    open: Array = field(shape=())
     """Whether the item is open or not."""
 
 
-class Pickable(struct.PyTreeNode):
-    id: Array = jnp.asarray(1, dtype=jnp.int32)
+class Pickable(Component):
+    id: Array = field(shape=())
     """The id of the item. If set, it must be >= 1."""
 
 
-class Holder(struct.PyTreeNode):
-    pocket: Array = EMPTY_POCKET_ID
+class Holder(Component):
+    pocket: Array = field(shape=())
     """The id of the item in the pocket (0 if empty)"""
+
+
+class HasTag(Component):
+    @property
+    def tag(self) -> Array:
+        """The tag of the component, used to identify the type of the component in `observations.categorical`"""
+        raise NotImplementedError()
+
+
+class HasSprite(Component):
+    @property
+    def sprite(self) -> Array:
+        raise NotImplementedError()
```

### Comparing `Navix-0.3.5/navix/environments/__init__.py` & `Navix-0.3.6/navix/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.5/navix/environments/environment.py` & `Navix-0.3.6/navix/environments/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import jax.numpy as jnp
 from jax.random import KeyArray
 from jax import Array
 from flax import struct
 
 
 from .. import tasks, terminations, observations
+from ..graphics import RenderingCache
 from ..entities import State
 from ..actions import ACTIONS
 
 
 class StepType(IntEnum):
     TRANSITION = 0
     """discount > 0, episode continues"""
@@ -73,15 +74,15 @@
         pytree_node=False, default=tasks.navigation
     )
     termination_fn: Callable[[State, Array, State], Array] = struct.field(
         pytree_node=False, default=terminations.on_navigation_completion
     )
 
     @abc.abstractmethod
-    def reset(self, key: KeyArray) -> Timestep:
+    def reset(self, key: KeyArray, cache: RenderingCache | None = None) -> Timestep:
         raise NotImplementedError()
 
     def _step(self, timestep: Timestep, action: Array, actions_set=ACTIONS) -> Timestep:
         # update agents
         state = jax.lax.switch(action, actions_set.values(), timestep.state)
 
         # build timestep
@@ -95,15 +96,15 @@
         )
 
     def step(self, timestep: Timestep, action: Array, actions_set=ACTIONS) -> Timestep:
         # autoreset if necessary: 0 = transition, 1 = truncation, 2 = termination
         should_reset = timestep.step_type > 0
         return jax.lax.cond(
             should_reset,
-            lambda timestep: self.reset(timestep.state.key),
+            lambda timestep: self.reset(timestep.state.key, timestep.state.cache),
             lambda timestep: self._step(timestep, action, actions_set),
             timestep,
         )
 
     def observation(self, state: State):
         return self.observation_fn(state)
```

### Comparing `Navix-0.3.5/navix/graphics.py` & `Navix-0.3.6/navix/graphics.py`

 * *Files 13% similar despite different names*

```diff
@@ -115,15 +115,18 @@
             ],
             axis=0,
         )
         return cls(patches=patches)
 
 
 def colorise_tile(tile: Array, colour: Array, background: Array = WHITE) -> Array:
-    assert tile.shape == (TILE_SIZE, TILE_SIZE), "Tile must be of size TILE_SIZE, TILE_SIZE, 3, got {}".format(tile.shape)
+    assert tile.shape == (
+        TILE_SIZE,
+        TILE_SIZE,
+    ), "Tile must be of size TILE_SIZE, TILE_SIZE, 3, got {}".format(tile.shape)
     tile = jnp.stack([tile] * colour.shape[0], axis=-1)
     tile = jnp.where(tile, colour, background)
     return tile
 
 
 def render_rectangle(size: int = TILE_SIZE, colour: Array = BLACK) -> Array:
     rectangle = jnp.ones((size - 2, size - 2), dtype=jnp.int32)
@@ -257,92 +260,102 @@
 
 
 def tile_grid(grid: Array, tile: Array) -> Array:
     tiled = jnp.tile(tile, (*grid.shape, 1))
     return jnp.asarray(tiled, dtype=jnp.uint8)
 
 
-def build_sprites_registry() -> Array:
+@jax.jit
+def build_sprites_registry() -> Dict[str, Any]:
+    registry = {}
+
     wall = render_wall()
     floor = render_floor()
     player = render_triangle_east()
     goal = render_diamond()
     key = render_key()
     door_closed = render_door_closed()
-    door_locked = render_door_locked()
     door_open = render_door_open()
 
-    # index by [entity_type, direction, open/closed, y, x, channel]
-    sprites = jnp.zeros((6, 4, 2, TILE_SIZE, TILE_SIZE, 3), dtype=jnp.uint8)
-
     # 0: set wall sprites
-    sprites = sprites.at[0].set(jnp.tile(wall, (4, 2, 1, 1, 1)))
+    registry["wall"] = wall
 
     # 1: set floor sprites
-    sprites = sprites.at[1].set(jnp.tile(floor, (4, 2, 1, 1, 1)))
+    registry["floor"] = floor
 
     # 2: set player sprites
-    player_sprites = jnp.stack([
-        player,
-        jnp.rot90(player, k=3),
-        jnp.rot90(player, k=2),
-        jnp.rot90(player, k=1),
-    ])
-    player_sprites = jnp.stack([player_sprites] * 2, axis=1)
-    sprites = sprites.at[2].set(player_sprites)
+    registry["player"] = jnp.stack(
+        [
+            player,
+            jnp.rot90(player, k=3),
+            jnp.rot90(player, k=2),
+            jnp.rot90(player, k=1),
+        ]
+    )
 
     # 3: set goal sprites
-    sprites = sprites.at[3].set(jnp.tile(goal, (4, 2, 1, 1, 1)))
+    registry["goal"] = goal
 
     # 4: set key sprites
-    sprites = sprites.at[4].set(jnp.tile(key, (4, 2, 1, 1, 1)))
+    registry["key"] = key
 
     # 5: set door sprites
-    door_closed =jnp.stack([
-        jnp.rot90(door_closed, k=1),
-        door_closed,
-        jnp.rot90(door_closed, k=3),
-        jnp.rot90(door_closed, k=2),
-    ])
-    sprites = sprites.at[5, :, 0].set(door_closed)
-    door_open = jnp.stack([
-        door_open,
-        jnp.rot90(door_open, k=1),
-        jnp.rot90(door_open, k=2),
-        jnp.rot90(door_open, k=3),
-    ])
-    sprites = sprites.at[5, :, 1].set(door_open)
+    door = jnp.zeros((4, 2, TILE_SIZE, TILE_SIZE, 3), dtype=jnp.uint8)
 
-    return sprites
+    door_closed_by_direction = jnp.stack(
+        [
+            jnp.rot90(door_closed, k=1),
+            door_closed,
+            jnp.rot90(door_closed, k=3),
+            jnp.rot90(door_closed, k=2),
+        ]
+    )
+    door = door.at[:, 0].set(door_closed_by_direction)
 
+    door_open_by_direction = jnp.stack(
+        [
+            door_open,
+            jnp.rot90(door_open, k=1),
+            jnp.rot90(door_open, k=2),
+            jnp.rot90(door_open, k=3),
+        ]
+    )
+    door = door.at[:, 1].set(door_open_by_direction)
 
-SPRITES_REGISTRY: Array = build_sprites_registry()
+    registry["door"] = door
+
+    return registry
+
+
+SPRITES_REGISTRY: Dict[str, Any] = build_sprites_registry()
 
 
 def render_background(
-    grid: Array, sprites_registry: Array = SPRITES_REGISTRY
+    grid: Array, sprites_registry: Dict[str, Any] = SPRITES_REGISTRY
 ) -> Array:
     image_width = grid.shape[0] * TILE_SIZE
     image_height = grid.shape[1] * TILE_SIZE
     n_channels = 3
 
     background = jnp.zeros((image_height, image_width, n_channels), dtype=jnp.uint8)
     grid_resized = jax.image.resize(
         grid, (grid.shape[0] * TILE_SIZE, grid.shape[1] * TILE_SIZE), method="nearest"
     )
 
     mask = jnp.asarray(grid_resized, dtype=bool)  # 0 = floor, 1 = wall
     # index by [entity_type, direction, open/closed, y, x, channel]
-    wall_tile = tile_grid(grid, sprites_registry[0, 0, 0])
-    floor_tile = tile_grid(grid, sprites_registry[1, 0, 0])
+    wall_tile = tile_grid(grid, sprites_registry["wall"])
+    floor_tile = tile_grid(grid, sprites_registry["floor"])
     background = jnp.where(mask[..., None], wall_tile, floor_tile)
     return background
 
 
-def flatten_patches(image: Array, patch_size: Tuple[int, int] = (TILE_SIZE, TILE_SIZE)) -> Array:
+def flatten_patches(
+    image: Array, patch_size: Tuple[int, int] = (TILE_SIZE, TILE_SIZE)
+) -> Array:
     height = image.shape[0] // patch_size[0]
     width = image.shape[1] // patch_size[1]
     n_channels = image.shape[2]
 
     grid = image.reshape(height, patch_size[0], width, patch_size[1], n_channels)
 
     # Swap the first and second axes of the grid to revert the stacking order
@@ -358,15 +371,21 @@
     image_height = image_size[0]
     image_width = image_size[1]
     patch_height = patches.shape[1]
     patch_width = patches.shape[2]
     n_channels = patches.shape[3]
 
     # Reshape the list of tiles into a 2D grid
-    grid = patches.reshape(image_height // patch_height, image_width // patch_width, patch_height, patch_width, n_channels)
+    grid = patches.reshape(
+        image_height // patch_height,
+        image_width // patch_width,
+        patch_height,
+        patch_width,
+        n_channels,
+    )
 
     # Swap the first and second axes of the grid to change the order of stacking
     grid = jnp.swapaxes(grid, 1, 2)
 
     # Reshape and stack the grid tiles horizontally and vertically to form the final image
     image = grid.reshape(image_height, image_width, n_channels)
```

### Comparing `Navix-0.3.5/navix/grid.py` & `Navix-0.3.6/navix/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
-from functools import partial
 
 
-from typing import Callable, Dict, Tuple, Sequence
+from typing import Callable, Dict, Tuple
 import jax
 import jax.numpy as jnp
 from jax.random import KeyArray
 from jax import Array
-from jax._src.util import canonicalize_axis
 
 
 Coordinates = Tuple[Array, Array]
 
 
 def coordinates(grid: Array) -> Coordinates:
     return tuple(jnp.mgrid[0 : grid.shape[0], 0 : grid.shape[1]])
@@ -135,15 +133,15 @@
     is_equal = jnp.all(jnp.equal(a, b), axis=-1)
     assert is_equal.shape == (max(b.shape[0], a.shape[0]),)
     return is_equal
 
 
 def room(height: int, width: int):
     """A grid of ids of size `width` x `height`"""
-    grid = jnp.zeros((height, width), dtype=jnp.int32)
+    grid = jnp.zeros((height - 2, width - 2), dtype=jnp.int32)
     return jnp.pad(grid, 1, mode="constant", constant_values=-1)
 
 
 def two_rooms(height: int, width: int, key: KeyArray) -> Tuple[Array, Array]:
     """Two rooms separated by a vertical wall at `width // 2`"""
     # create room
     grid = jnp.zeros((height - 2, width - 2), dtype=jnp.int32)
@@ -173,27 +171,36 @@
     origin = origin + jnp.asarray((padding[0][0] - radius, padding[1][0] - radius))
     height, width = (padded.shape[0] - radius * 2, padded.shape[1] - radius * 2)
 
     # rotate
     rotated, centre = jax.lax.switch(
         direction,
         (
-            lambda x: (jnp.rot90(x, 1), (width - 1 - origin[1], origin[0])),  # 0 = transpose, 1 = flip
-            lambda x: (jnp.rot90(x, 2), (height - 1 - origin[0], width - 1 - origin[1])),  # 0 = flip, 1 = flip
-            lambda x: (jnp.rot90(x, 3), (origin[1], height - 1 - origin[0])),  # 0 = flip, 1 = transpose
-            lambda x: (x, (origin[0], origin[1]))
+            lambda x: (
+                jnp.rot90(x, 1),
+                (width - 1 - origin[1], origin[0]),
+            ),  # 0 = transpose, 1 = flip
+            lambda x: (
+                jnp.rot90(x, 2),
+                (height - 1 - origin[0], width - 1 - origin[1]),
+            ),  # 0 = flip, 1 = flip
+            lambda x: (
+                jnp.rot90(x, 3),
+                (origin[1], height - 1 - origin[0]),
+            ),  # 0 = flip, 1 = transpose
+            lambda x: (x, (origin[0], origin[1])),
         ),
-        padded
+        padded,
     )
 
     # translate
     translated = jnp.roll(rotated, -jnp.asarray(centre), axis=(0, 1))
 
     # crop
-    cropped = translated[:radius + 1, :2 * radius + 1]
+    cropped = translated[: radius + 1, : 2 * radius + 1]
 
     return jnp.asarray(cropped, dtype=grid.dtype)
 
 
 def view_cone(transparency_map: Array, origin: Array, radius: int) -> Array:
     # transparency_map is a boolean map of transparent (1) and opaque (0) tiles
```

### Comparing `Navix-0.3.5/navix/observations.py` & `Navix-0.3.6/navix/observations.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,116 +28,113 @@
 from .components import DISCARD_PILE_IDX
 from .entities import State
 from .grid import align, idx_from_coordinates, crop, view_cone
 
 
 def none(
     state: State,
-    sprites_registry: Array = graphics.SPRITES_REGISTRY,
 ) -> Array:
     return jnp.asarray(())
 
 
 def categorical(
     state: State,
-    sprites_registry: Array = graphics.SPRITES_REGISTRY,
 ) -> Array:
     # get idx of entity on the set of patches
-    indices = idx_from_coordinates(state.grid, state.get_positions(axis=0))
+    indices = idx_from_coordinates(state.grid, state.get_positions())
     # get tags corresponding to the entities
-    tags = state.get_tags(axis=0)
+    tags = state.get_tags()
     # set tags on the flat set of patches
     shape = state.grid.shape
     grid = state.grid.reshape(-1).at[indices].set(tags)
     # unflatten patches to reconstruct the grid
     return grid.reshape(shape)
 
 
 def categorical_first_person(
     state: State,
-    sprites_registry: Array = graphics.SPRITES_REGISTRY,
     radius: int = 3,
 ) -> Array:
     # get transparency map
     transparency_map = jnp.where(state.grid == 0, 1, 0)
-    positions = state.get_positions(axis=0)
-    transparent = state.get_transparents(axis=0)
+    positions = state.get_positions()
+    transparent = state.get_transparency()
     transparency_map = transparency_map.at[tuple(positions.T)].set(~transparent)
 
     # apply view mask
-    view = view_cone(transparency_map, state.players.position, radius)
+    player = state.get_player()
+    view = view_cone(transparency_map, player.position, radius)
 
     # get categorical representation
-    tags = state.get_tags(axis=0)
+    tags = state.get_tags()
     obs = state.grid.at[tuple(positions.T)].set(tags) * view
 
     # crop grid to agent's view
-    obs = crop(obs, state.players.position, state.players.direction, radius)
+    obs = crop(obs, player.position, player.direction, radius)
 
     return obs
 
 
 def rgb(
     state: State,
-    sprites_registry: Array = graphics.SPRITES_REGISTRY,
 ) -> Array:
     # for 1-d vs 2-d indexing benchamarks
     # see https://github.com/epignatelli/navix/tree/observation/2dindexing
 
     # get idx of entity on the flat set of patches
-    indices = idx_from_coordinates(state.grid, state.get_positions(axis=0))
+    indices = idx_from_coordinates(state.grid, state.get_positions())
     # get tiles corresponding to the entities
-    tiles = state.get_sprites(sprites_registry, axis=0)
+    tiles = state.get_sprites()
     # set tiles on the flat set of patches
     patches = state.cache.patches.at[indices].set(tiles)
     # remove discard pile
     patches = patches[:DISCARD_PILE_IDX]
     # unflatten patches to reconstruct the image
     image_size = (
         state.grid.shape[0] * graphics.TILE_SIZE,
         state.grid.shape[1] * graphics.TILE_SIZE,
     )
     image = graphics.unflatten_patches(patches, image_size)
     return image
 
 
 def rgb_first_person(
-        state: State,
-        sprites_registry: Array = graphics.SPRITES_REGISTRY,
-        radius: int = 3,
+    state: State,
+    radius: int = 3,
 ) -> Array:
-    transparency_map = jnp.where(state.grid == 0, 1, 0)
-    positions = state.get_positions(axis=0)
-    transparent = state.get_transparents(axis=0)
-    transparency_map = transparency_map.at[tuple(positions.T)].set(~transparent)
-
+    # calculate final image size
     image_size = (
         state.grid.shape[0] * graphics.TILE_SIZE,
         state.grid.shape[1] * graphics.TILE_SIZE,
     )
-    # apply view mask
-    view = view_cone(transparency_map, state.players.position, radius)
+
+    # get agent's view
+    transparency_map = jnp.where(state.grid == 0, 1, 0)
+    positions = state.get_positions()
+    transparent = state.get_transparency()
+    transparency_map = transparency_map.at[tuple(positions.T)].set(~transparent)
+    player = state.get_player()
+    view = view_cone(transparency_map, player.position, radius)
     view = jax.image.resize(view, image_size, method="nearest")
     view = jnp.tile(view[..., None], (1, 1, 3))
 
-    # get rgb representation
-    indices = idx_from_coordinates(state.grid, state.get_positions(axis=0))
-    tiles = state.get_sprites(sprites_registry, axis=0)
-    patches = state.cache.patches.at[indices].set(tiles)
-
-    # remove discard pile
-    patches = patches[:DISCARD_PILE_IDX]
+    # get sprites aligned to player's direction
+    sprites = state.get_sprites()
+    sprites = jax.vmap(lambda x: align(x, jnp.asarray(0), player.direction))(sprites)
 
     # align sprites to player's direction
-    patches = jax.vmap(lambda x: align(x, jnp.asarray(0), state.players.direction))(patches)
+    indices = idx_from_coordinates(state.grid, state.get_positions())
+    patches = state.cache.patches.at[indices].set(sprites)
 
+    # remove discard pile
+    patches = patches[:DISCARD_PILE_IDX]
     # rearrange the sprites in a grid
     patchwork = patches.reshape(*state.grid.shape, *patches.shape[1:])
 
     # crop grid to agent's view
-    patchwork = crop(patchwork, state.players.position, state.players.direction, radius)
+    patchwork = crop(patchwork, player.position, player.direction, radius)
 
     # reconstruct image
     obs = jnp.swapaxes(patchwork, 1, 2)
     shape = obs.shape
     obs = obs.reshape(shape[0] * shape[1], shape[2] * shape[3], *shape[4:])
     return obs
```

### Comparing `Navix-0.3.5/navix/tasks.py` & `Navix-0.3.6/navix/tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,21 +40,24 @@
 
 
 def free(state: State) -> Array:
     return jnp.asarray(0.0)
 
 
 def navigation(prev_state: State, action: Array, state: State) -> Array:
+    player = state.get_player()
+    goals = state.get_goals()
+
     reached = jax.vmap(jnp.array_equal, in_axes=(None, 0))(
-        state.players.position, state.goals.position
+        player.position, goals.position
     )
     any_reached = jnp.sum(reached)
 
     draw = jax.random.uniform(state.key, ())
-    reward = any_reached * jnp.greater_equal(draw, state.goals.probability)
+    reward = any_reached * jnp.greater_equal(draw, goals.probability)
     reward = jnp.asarray(reward, jnp.float32).squeeze()
 
     # make sure that reward is a scalar
     assert reward.shape == (), f"Reward must be a scalar but got shape {reward.shape}"
     return reward
 
 
@@ -71,12 +74,15 @@
     # time always has a cost
     return -jnp.asarray(cost)
 
 
 def wall_hit_cost(
     prev_state: State, action: Array, state: State, cost: float = 0.01
 ) -> Array:
+    prev_player = prev_state.get_player()
+    player = state.get_player()
+
     # if state is unchanged, maybe the wall was hit
-    didnt_move = jnp.array_equal(prev_state.players.position, state.players.position)
+    didnt_move = jnp.array_equal(prev_player.position, player.position)
     but_wanted_to = jnp.less_equal(3, action) * jnp.less_equal(action, 6)
     hit = jnp.logical_and(didnt_move, but_wanted_to)
     return -jnp.asarray(cost) * hit
```

### Comparing `Navix-0.3.5/navix/terminations.py` & `Navix-0.3.6/navix/terminations.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
 
 from jax import Array
-import jax
 import jax.numpy as jnp
 from .entities import State
 from .grid import positions_equal
 
 
 def check_truncation(terminated: Array, truncated: Array) -> Array:
     result = jnp.asarray(truncated + 2 * terminated, dtype=jnp.int32)
     return jnp.clip(result, 0, 2)
 
 
 def on_navigation_completion(prev_state: State, action: Array, state: State) -> Array:
-    reached = positions_equal(state.players.position, state.goals.position)
+    player = state.get_player()
+    goals = state.get_goals()
+
+    reached = positions_equal(player.position, goals.position)
     return jnp.any(reached)
```

### Comparing `Navix-0.3.5/pyproject.toml` & `Navix-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 requires = ["setuptools >= 50", "setuptools-scm[toml]>=6.2", "wheel"]
 
 [project]
 name = "Navix"
 dynamic = ["version", "dependencies"]
 description = "Accelerated gridworld navigation with JAX for deep reinforcement learning"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 readme = "README.md"
 license = {file = "LICENSE", name = "Apache-2.0"}
 authors = [
   {name = "Eduardo Pignatelli", email = "edu.pignatelli@gmail.com"},
 ]
 maintainers = [
   {name = "Eduardo Pignatelli", email = "edu.pignatelli@gmail.com"},
```

### Comparing `Navix-0.3.5/scripts/release.sh` & `Navix-0.3.6/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `Navix-0.3.5/tests/performance/grid.py` & `Navix-0.3.6/tests/performance/grid.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,19 +21,15 @@
         timestep = env.reset(key)
 
         actions = jax.random.randint(key, (100,), 0, 6)
         timestep = jax.lax.scan(lambda c, x: (env.step(c, x), ()), timestep, actions)[0]
         return timestep
 
     # profile navix scanned
-    print(
-        "Profiling, N_SEEDS = {}, N_TIMESTEPS = {}".format(
-            N_SEEDS, N_TIMESTEPS
-        )
-    )
+    print("Profiling, N_SEEDS = {}, N_TIMESTEPS = {}".format(N_SEEDS, N_TIMESTEPS))
 
     seeds = jnp.arange(N_SEEDS)
 
     print(f"\tCompiling {test}...")
     start = time.time()
     test_jit = jax.jit(jax.vmap(test)).lower(seeds).compile()
     print("\tCompiled in {:.2f}s".format(time.time() - start))
```

### Comparing `Navix-0.3.5/tests/performance/minigrid.py` & `Navix-0.3.6/tests/performance/minigrid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.5/tests/performance/observations.py` & `Navix-0.3.6/tests/performance/observations.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,53 +4,71 @@
 import jax
 import jax.numpy as jnp
 import navix as nx
 
 
 N_TIMEIT_LOOPS = 10
 N_REPEAT = 30
-N_TIMESTEPS = 1000
-N_SEEDS = 1000
+N_TIMESTEPS = 10
+N_SEEDS = 10000
 
 
 def test_observation(observation_fn):
     def test(seed):
-        env = nx.environments.KeyDoor(
+        env = nx.environments.Room(
             height=5, width=10, max_steps=100, gamma=1.0, observation_fn=observation_fn
         )
         key = jax.random.PRNGKey(seed)
         timestep = env.reset(key)
 
+        # option 1
+        # actions = jax.random.randint(key, (100,), 0, 6)
+        # timestep = jax.lax.scan(lambda c, x: (env.step(c, x), ()), timestep, actions)[0]
+
+        # option 2
+        # for i in range(N_TIMESTEPS):
+        #     action = jax.random.randint(key, (), 0, 6)
+        #     timestep = env.step(timestep, jnp.asarray(action))
+
+        # option 3
         actions = jax.random.randint(key, (100,), 0, 6)
-        timestep = jax.lax.scan(lambda c, x: (env.step(c, x), ()), timestep, actions)[0]
+        jax.lax.while_loop(
+            lambda x: x[1] < N_TIMESTEPS,
+            lambda x: (env.step(x[0], actions[x[1]]), x[1] + 1),
+            (timestep, jnp.asarray(0)),
+        )
+
         return timestep
 
     # profile navix scanned
     print(
         "Profiling observation {}, N_SEEDS = {}, N_TIMESTEPS = {}".format(
             observation_fn, N_SEEDS, N_TIMESTEPS
         )
     )
 
     seeds = jnp.arange(N_SEEDS)
 
     print(f"\tCompiling {observation_fn}...")
     start = time.time()
-    test_jit = jax.jit(jax.vmap(test)).lower(seeds).compile()
+    test_jit = jax.vmap(test)
+    test_jit = jax.jit(test_jit)
+    test_jit = test_jit.lower(seeds)
+    test_jit = test_jit.compile()
     print("\tCompiled in {:.2f}s".format(time.time() - start))
 
     print(f"\tRunning {observation_fn}...")
     res = repeat(
         lambda: test_jit(seeds).observation.block_until_ready(),
         number=N_TIMEIT_LOOPS,
         repeat=N_REPEAT,
     )
     res = jnp.asarray(res)
     print(f"\t {jnp.mean(res)} ± {jnp.std(res)}")
 
 
 if __name__ == "__main__":
-    # test_observation(nx.observations.none)
-    # test_observation(nx.observations.categorical)
-    # test_observation(nx.observations.rgb)
-    # test_observation(nx.observations.categorical_first_person)
+    test_observation(nx.observations.none)
+    test_observation(nx.observations.categorical)
+    test_observation(nx.observations.categorical_first_person)
+    test_observation(nx.observations.rgb)
     test_observation(nx.observations.rgb_first_person)
```

### Comparing `Navix-0.3.5/tests/performance/observations_keydoor_report.txt` & `Navix-0.3.6/tests/performance/observations_keydoor_report.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.3.5/tests/performance/observations_room_report.txt` & `Navix-0.3.6/tests/performance/observations_room_report.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.3.5/tests/test_environments.py` & `Navix-0.3.6/tests/test_environments.py`

 * *Files 25% similar despite different names*

```diff
@@ -67,10 +67,20 @@
             print(timestep)
         return timestep
 
     f()
     jax.jit(f)()
 
 
+def test_keydoor2():
+    env = nx.environments.KeyDoor(5, 7, 100, observation_fn=nx.observations.rgb)
+
+    key = jax.random.PRNGKey(1)
+    timestep = env.reset(key)
+    return
+
+
 if __name__ == "__main__":
-    test_room()
-    test_keydoor()
+    # test_room()
+    # jax.jit(test_room)()
+    # test_keydoor()
+    test_keydoor2()
```

### Comparing `Navix-0.3.5/tests/test_grid.py` & `Navix-0.3.6/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.5/tests/test_observations.py` & `Navix-0.3.6/tests/test_observations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,131 @@
 import jax
 import jax.numpy as jnp
 
 import navix as nx
-from navix.entities import Player, Goal, Key, Door
+from navix.entities import Entities, Player, Goal, Key, Door
+from navix.components import EMPTY_POCKET_ID
 
 
 def test_rgb():
     height = 10
     width = 10
     grid = jnp.zeros((height - 2, width - 2), dtype=jnp.int32)
     grid = jnp.pad(grid, 1, mode="constant", constant_values=-1)
 
+    players = Player(
+        position=jnp.asarray((1, 1)), direction=jnp.asarray(0), pocket=EMPTY_POCKET_ID
+    )
+    goals = Goal(position=jnp.asarray((4, 4)), probability=jnp.asarray(1.0))
+    keys = Key(position=jnp.asarray((2, 2)), id=jnp.asarray(0))
+    doors = Door(
+        position=jnp.asarray([(1, 5), (1, 6)]),
+        direction=jnp.asarray((0, 2)),
+        requires=jnp.asarray((0, 0)),
+        open=jnp.asarray((False, True)),
+    )
+
+    entities = {
+        Entities.PLAYER.value: players[None],
+        Entities.GOAL.value: goals[None],
+        Entities.KEY.value: keys[None],
+        Entities.DOOR.value: doors,
+    }
+
     state = nx.entities.State(
         key=jax.random.PRNGKey(0),
         grid=grid,
-        players=Player.create(position=jnp.asarray((1, 1)), direction=jnp.asarray(0)),
-        goals=Goal.create(position=jnp.asarray((4, 4)), probability=jnp.asarray(1.0)),
-        keys=Key.create(position=jnp.asarray((2, 2)), id=jnp.asarray(0)),
-        doors=Door.create(position=jnp.asarray([(1, 5), (1, 6)]), direction=jnp.asarray((0, 2)), requires=jnp.asarray((0, 0))),
         cache=nx.graphics.RenderingCache.init(grid),
+        entities=entities,
     )
     sprites_registry = nx.graphics.SPRITES_REGISTRY
 
-    doors = state.doors.replace(open=jnp.asarray((False, True)))
-    state = state.replace(doors=doors)
-
-    obs = nx.observations.rgb(state, sprites_registry=sprites_registry)
-    expected_obs_shape = (height * nx.graphics.TILE_SIZE, width * nx.graphics.TILE_SIZE, 3)
-    assert obs.shape == expected_obs_shape, (
-        f"Expected observation {expected_obs_shape}, got {obs.shape} instead"
+    doors = state.get_doors()
+    doors = doors.replace(open=jnp.asarray((False, True)))
+    state.entities[Entities.DOOR.value] = doors
+
+    obs = nx.observations.rgb(state)
+    expected_obs_shape = (
+        height * nx.graphics.TILE_SIZE,
+        width * nx.graphics.TILE_SIZE,
+        3,
     )
+    assert (
+        obs.shape == expected_obs_shape
+    ), f"Expected observation {expected_obs_shape}, got {obs.shape} instead"
 
     def get_tile(position):
         x = position[0] * nx.graphics.TILE_SIZE
         y = position[1] * nx.graphics.TILE_SIZE
-        return obs[x:x + nx.graphics.TILE_SIZE, y:y + nx.graphics.TILE_SIZE, :]
-
-    player_tile = get_tile(state.players.position)
-    assert jnp.array_equal(player_tile, sprites_registry[2][0][0]), player_tile
-
-    goal_tile = get_tile(state.goals.position[0])
-    assert jnp.array_equal(goal_tile, sprites_registry[3][0][0]), goal_tile
+        return obs[x : x + nx.graphics.TILE_SIZE, y : y + nx.graphics.TILE_SIZE, :]
 
-    key_tile = get_tile(state.keys.position[0])
-    assert jnp.array_equal(key_tile, sprites_registry[4][0][0]), key_tile
-
-    door_tile = get_tile(state.doors.position[0])
-    assert jnp.array_equal(door_tile, sprites_registry[5][0][0]), door_tile
-
-    door_tile = get_tile(state.doors.position[1])
-    assert jnp.array_equal(door_tile, sprites_registry[5][2][1]), door_tile
+    player = state.get_player()
+    player_tile = get_tile(player.position)
+    assert jnp.array_equal(
+        player_tile, sprites_registry[Entities.PLAYER.value][player.direction]
+    ), player_tile
+
+    goals = state.get_goals()
+    goal_tile = get_tile(goals.position[0])
+    assert jnp.array_equal(goal_tile, sprites_registry[Entities.GOAL.value]), goal_tile
+
+    keys = state.get_keys()
+    key_tile = get_tile(keys.position[0])
+    assert jnp.array_equal(key_tile, sprites_registry[Entities.KEY.value]), key_tile
+
+    doors = state.get_doors()
+    door_tile = get_tile(doors.position[0])
+    direction = doors.direction[0]
+    open = jnp.asarray(doors.open[0], dtype=jnp.int32)
+    assert jnp.array_equal(
+        door_tile, sprites_registry[Entities.DOOR.value][direction, open]
+    ), door_tile
+
+    door_tile = get_tile(doors.position[1])
+    direction = doors.direction[1]
+    open = jnp.asarray(doors.open[1], dtype=jnp.int32)
+    assert jnp.array_equal(
+        door_tile, sprites_registry[Entities.DOOR.value][direction, open]
+    ), door_tile
 
     return
 
 
 def test_categorical_first_person():
     height = 10
     width = 10
     grid = jnp.zeros((height - 2, width - 2), dtype=jnp.int32)
     grid = jnp.pad(grid, 1, mode="constant", constant_values=-1)
 
+    players = Player(
+        position=jnp.asarray((1, 1)), direction=jnp.asarray(0), pocket=EMPTY_POCKET_ID
+    )
+    goals = Goal(position=jnp.asarray((4, 4)), probability=jnp.asarray(1.0))
+    keys = Key(position=jnp.asarray((2, 2)), id=jnp.asarray(0))
+    doors = Door(
+        position=jnp.asarray([(1, 5), (1, 6)]),
+        direction=jnp.asarray((0, 2)),
+        requires=jnp.asarray((0, 0)),
+        open=jnp.asarray((False, True)),
+    )
+    entities = {
+        Entities.PLAYER.value: players[None],
+        Entities.GOAL.value: goals[None],
+        Entities.KEY.value: keys[None],
+        Entities.DOOR.value: doors,
+    }
+
     state = nx.entities.State(
         key=jax.random.PRNGKey(0),
         grid=grid,
-        players=Player.create(position=jnp.asarray((1, 1)), direction=jnp.asarray(0)),
-        goals=Goal.create(position=jnp.asarray((4, 4)), probability=jnp.asarray(1.0)),
-        keys=Key.create(position=jnp.asarray((2, 2)), id=jnp.asarray(0)),
-        doors=Door.create(position=jnp.asarray([(1, 5), (1, 6)]), direction=jnp.asarray((0, 2)), requires=jnp.asarray((0, 0))),
         cache=nx.graphics.RenderingCache.init(grid),
+        entities=entities,
     )
 
     obs = nx.observations.categorical_first_person(state)
     print(obs)
 
+
 if __name__ == "__main__":
-    # test_rgb()
+    test_rgb()
     test_categorical_first_person()
-    jax.jit(test_categorical_first_person)()
+    # jax.jit(test_categorical_first_person)()
```

### Comparing `Navix-0.3.5/tests/test_tasks.py` & `Navix-0.3.6/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.5/tests/test_terminations.py` & `Navix-0.3.6/tests/test_terminations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,68 @@
 import jax
 import jax.numpy as jnp
 
 import navix as nx
+from navix.components import EMPTY_POCKET_ID
 
 
 def test_on_navigation_completion():
     grid = jnp.zeros((5, 5), dtype=jnp.int32)
+
+    players = nx.entities.Player(
+        position=jnp.asarray((1, 1)), direction=jnp.asarray(0), pocket=EMPTY_POCKET_ID
+    )
+    goals = nx.entities.Goal(position=jnp.asarray((3, 3)), probability=jnp.asarray(1))
+    entities = {
+        nx.entities.Entities.PLAYER.value: players[None],
+        nx.entities.Entities.GOAL.value: goals[None],
+    }
+
     state = nx.entities.State(
         key=jax.random.PRNGKey(0),
         grid=grid,
         cache=nx.entities.RenderingCache.init(grid),
-        players=nx.entities.Player.create(jnp.asarray((1, 1)), jnp.asarray(0)),
-        goals=nx.entities.Goal.create(jnp.asarray((3, 3)), jnp.asarray(1)),
+        entities=entities,
     )
     # shpuld not terminate
     termination = nx.terminations.on_navigation_completion(state, jnp.asarray(0), state)
     assert not termination, f"Should not terminate, got {termination} instead"
 
     # artificially put agent on goal
-    new_state = state.replace(players=state.players.replace(position=state.goals.position))
-    termination = nx.terminations.on_navigation_completion(state, jnp.asarray(0), new_state)
+    player = state.get_player()
+    goals = state.get_goals()
+    new_state = state.set_player(player.replace(position=goals.position[0]))
+    termination = nx.terminations.on_navigation_completion(
+        state, jnp.asarray(0), new_state
+    )
     assert termination, f"Should terminate, got {termination} instead"
 
 
 def test_check_truncation():
     terminated = jnp.asarray(False)
     truncated = jnp.asarray(False)
-    assert nx.terminations.check_truncation(terminated, truncated) == jnp.asarray(0, dtype=jnp.int32)
+    assert nx.terminations.check_truncation(terminated, truncated) == jnp.asarray(
+        0, dtype=jnp.int32
+    )
 
     terminated = jnp.asarray(True)
     truncated = jnp.asarray(False)
-    assert nx.terminations.check_truncation(terminated, truncated) == jnp.asarray(2, dtype=jnp.int32)
+    assert nx.terminations.check_truncation(terminated, truncated) == jnp.asarray(
+        2, dtype=jnp.int32
+    )
 
     terminated = jnp.asarray(False)
     truncated = jnp.asarray(True)
-    assert nx.terminations.check_truncation(terminated, truncated) == jnp.asarray(1, dtype=jnp.int32)
+    assert nx.terminations.check_truncation(terminated, truncated) == jnp.asarray(
+        1, dtype=jnp.int32
+    )
 
     terminated = jnp.asarray(True)
     truncated = jnp.asarray(True)
-    assert nx.terminations.check_truncation(terminated, truncated) == jnp.asarray(2, dtype=jnp.int32)
+    assert nx.terminations.check_truncation(terminated, truncated) == jnp.asarray(
+        2, dtype=jnp.int32
+    )
 
 
 if __name__ == "__main__":
     test_on_navigation_completion()
     test_check_truncation()
```

