# Comparing `tmp/threadpoolctl-3.1.0.tar.gz` & `tmp/threadpoolctl-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadpoolctl-3.1.0.tar", last modified: Mon Jan 31 16:31:25 2022, max compression
+gzip compressed data, was "threadpoolctl-3.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `threadpoolctl-3.1.0.tar` & `threadpoolctl-3.2.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     5536 2022-01-31 15:08:24.277708 threadpoolctl-3.1.0/.azure_pipeline.yml
--rw-r--r--   0        0        0       14 2019-04-03 14:59:03.684333 threadpoolctl-3.1.0/.codecov.yml
--rw-r--r--   0        0        0       28 2019-04-03 14:59:03.684333 threadpoolctl-3.1.0/.coveragerc
--rw-r--r--   0        0        0      255 2019-09-16 12:06:34.688814 threadpoolctl-3.1.0/.gitignore
--rw-r--r--   0        0        0     3792 2022-01-31 16:25:14.640525 threadpoolctl-3.1.0/CHANGES.md
--rw-r--r--   0        0        0     1507 2019-04-03 14:59:03.684333 threadpoolctl-3.1.0/LICENSE
--rw-r--r--   0        0        0     8505 2022-01-31 15:08:24.277708 threadpoolctl-3.1.0/README.md
--rw-r--r--   0        0        0      862 2021-09-28 09:58:55.838120 threadpoolctl-3.1.0/benchmarks/bench_context_manager_overhead.py
--rw-r--r--   0        0        0       47 2021-09-15 13:26:21.489843 threadpoolctl-3.1.0/conftest.py
--rwxr-xr-x   0        0        0      296 2019-06-26 09:41:29.299105 threadpoolctl-3.1.0/continuous_integration/build_test_ext.sh
--rw-r--r--   0        0        0     1351 2021-09-17 09:26:34.308249 threadpoolctl-3.1.0/continuous_integration/check_no_test_skipped.py
--rw-r--r--   0        0        0     1191 2022-01-20 17:05:26.048133 threadpoolctl-3.1.0/continuous_integration/install.cmd
--rwxr-xr-x   0        0        0     3060 2022-01-31 15:08:24.277708 threadpoolctl-3.1.0/continuous_integration/install.sh
--rwxr-xr-x   0        0        0     1393 2022-01-20 17:05:26.048133 threadpoolctl-3.1.0/continuous_integration/install_with_blis.sh
--rw-r--r--   0        0        0     1788 2021-09-24 08:58:15.330052 threadpoolctl-3.1.0/continuous_integration/posix.yml
--rw-r--r--   0        0        0      270 2022-01-20 17:05:26.048133 threadpoolctl-3.1.0/continuous_integration/test_script.cmd
--rwxr-xr-x   0        0        0      572 2022-01-20 17:05:26.048133 threadpoolctl-3.1.0/continuous_integration/test_script.sh
--rwxr-xr-x   0        0        0      303 2019-04-03 14:59:03.684333 threadpoolctl-3.1.0/continuous_integration/upload_codecov.sh
--rw-r--r--   0        0        0      928 2021-09-15 13:26:21.493843 threadpoolctl-3.1.0/continuous_integration/windows.yml
--rw-r--r--   0        0        0       39 2019-04-03 14:59:03.684333 threadpoolctl-3.1.0/dev-requirements.txt
--rw-r--r--   0        0        0     3788 2021-09-15 13:26:21.493843 threadpoolctl-3.1.0/multiple_openmp.md
--rw-r--r--   0        0        0      844 2022-01-31 15:08:24.277708 threadpoolctl-3.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2020-06-02 21:31:29.138258 threadpoolctl-3.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-09-15 13:26:21.493843 threadpoolctl-3.1.0/tests/_openmp_test_helper/__init__.py
--rw-r--r--   0        0        0      572 2021-09-24 08:18:13.956710 threadpoolctl-3.1.0/tests/_openmp_test_helper/build_utils.py
--rw-r--r--   0        0        0     2073 2021-09-29 16:23:34.090675 threadpoolctl-3.1.0/tests/_openmp_test_helper/nested_prange_blas.pyx
--rw-r--r--   0        0        0       38 2021-09-15 13:26:21.493843 threadpoolctl-3.1.0/tests/_openmp_test_helper/openmp_helpers_inner.pxd
--rw-r--r--   0        0        0      918 2021-12-31 16:52:30.808669 threadpoolctl-3.1.0/tests/_openmp_test_helper/openmp_helpers_inner.pyx
--rw-r--r--   0        0        0      724 2021-09-15 13:26:21.493843 threadpoolctl-3.1.0/tests/_openmp_test_helper/openmp_helpers_outer.pyx
--rw-r--r--   0        0        0     1122 2021-09-24 08:18:13.956710 threadpoolctl-3.1.0/tests/_openmp_test_helper/setup_inner.py
--rw-r--r--   0        0        0     1066 2021-09-24 08:18:13.956710 threadpoolctl-3.1.0/tests/_openmp_test_helper/setup_nested_prange_blas.py
--rw-r--r--   0        0        0     1122 2021-09-24 08:18:13.956710 threadpoolctl-3.1.0/tests/_openmp_test_helper/setup_outer.py
--rw-r--r--   0        0        0    24705 2022-01-31 15:08:24.277708 threadpoolctl-3.1.0/tests/test_threadpoolctl.py
--rw-r--r--   0        0        0     2247 2021-09-29 16:23:34.090675 threadpoolctl-3.1.0/tests/utils.py
--rw-r--r--   0        0        0    41112 2022-01-31 16:25:14.640525 threadpoolctl-3.1.0/threadpoolctl.py
--rw-r--r--   0        0        0     9204 1970-01-01 00:00:00.000000 threadpoolctl-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6173 2023-07-13 14:19:36.077411 threadpoolctl-3.2.0/.azure_pipeline.yml
+-rw-r--r--   0        0        0       14 2019-04-03 14:59:03.684333 threadpoolctl-3.2.0/.codecov.yml
+-rw-r--r--   0        0        0       28 2019-04-03 14:59:03.684333 threadpoolctl-3.2.0/.coveragerc
+-rw-r--r--   0        0        0      302 2023-07-12 08:17:49.739681 threadpoolctl-3.2.0/.gitignore
+-rw-r--r--   0        0        0     4443 2023-07-13 14:44:13.625080 threadpoolctl-3.2.0/CHANGES.md
+-rw-r--r--   0        0        0     1507 2019-04-03 14:59:03.684333 threadpoolctl-3.2.0/LICENSE
+-rw-r--r--   0        0        0     9266 2023-07-12 08:17:49.739681 threadpoolctl-3.2.0/README.md
+-rw-r--r--   0        0        0      862 2021-09-28 09:58:55.838120 threadpoolctl-3.2.0/benchmarks/bench_context_manager_overhead.py
+-rw-r--r--   0        0        0       47 2021-09-15 13:26:21.489843 threadpoolctl-3.2.0/conftest.py
+-rwxr-xr-x   0        0        0      521 2023-07-12 08:17:49.739681 threadpoolctl-3.2.0/continuous_integration/build_test_ext.sh
+-rw-r--r--   0        0        0     1769 2023-06-30 15:31:34.528461 threadpoolctl-3.2.0/continuous_integration/check_no_test_skipped.py
+-rw-r--r--   0        0        0     1191 2022-01-20 17:05:26.048133 threadpoolctl-3.2.0/continuous_integration/install.cmd
+-rwxr-xr-x   0        0        0     3060 2023-07-12 13:11:15.498224 threadpoolctl-3.2.0/continuous_integration/install.sh
+-rwxr-xr-x   0        0        0     1386 2023-07-12 13:09:55.561690 threadpoolctl-3.2.0/continuous_integration/install_with_blis.sh
+-rw-r--r--   0        0        0     1565 2023-07-13 14:19:36.077411 threadpoolctl-3.2.0/continuous_integration/posix.yml
+-rw-r--r--   0        0        0      270 2022-01-20 17:05:26.048133 threadpoolctl-3.2.0/continuous_integration/test_script.cmd
+-rwxr-xr-x   0        0        0      572 2022-01-20 17:05:26.048133 threadpoolctl-3.2.0/continuous_integration/test_script.sh
+-rwxr-xr-x   0        0        0      303 2019-04-03 14:59:03.684333 threadpoolctl-3.2.0/continuous_integration/upload_codecov.sh
+-rw-r--r--   0        0        0      928 2021-09-15 13:26:21.493843 threadpoolctl-3.2.0/continuous_integration/windows.yml
+-rw-r--r--   0        0        0       39 2019-04-03 14:59:03.684333 threadpoolctl-3.2.0/dev-requirements.txt
+-rw-r--r--   0        0        0     3924 2023-07-12 08:17:49.739681 threadpoolctl-3.2.0/multiple_openmp.md
+-rw-r--r--   0        0        0      825 2023-07-12 08:17:49.743681 threadpoolctl-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-06-02 21:31:29.138258 threadpoolctl-3.2.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-15 13:26:21.493843 threadpoolctl-3.2.0/tests/_openmp_test_helper/__init__.py
+-rw-r--r--   0        0        0      572 2021-09-24 08:18:13.956710 threadpoolctl-3.2.0/tests/_openmp_test_helper/build_utils.py
+-rw-r--r--   0        0        0     2073 2021-09-29 16:23:34.090675 threadpoolctl-3.2.0/tests/_openmp_test_helper/nested_prange_blas.pyx
+-rw-r--r--   0        0        0       38 2021-09-15 13:26:21.493843 threadpoolctl-3.2.0/tests/_openmp_test_helper/openmp_helpers_inner.pxd
+-rw-r--r--   0        0        0      918 2021-12-31 16:52:30.808669 threadpoolctl-3.2.0/tests/_openmp_test_helper/openmp_helpers_inner.pyx
+-rw-r--r--   0        0        0      724 2021-09-15 13:26:21.493843 threadpoolctl-3.2.0/tests/_openmp_test_helper/openmp_helpers_outer.pyx
+-rw-r--r--   0        0        0     1122 2021-09-24 08:18:13.956710 threadpoolctl-3.2.0/tests/_openmp_test_helper/setup_inner.py
+-rw-r--r--   0        0        0     1066 2021-09-24 08:18:13.956710 threadpoolctl-3.2.0/tests/_openmp_test_helper/setup_nested_prange_blas.py
+-rw-r--r--   0        0        0     1122 2021-09-24 08:18:13.956710 threadpoolctl-3.2.0/tests/_openmp_test_helper/setup_outer.py
+-rw-r--r--   0        0        0     1789 2023-07-12 08:17:49.743681 threadpoolctl-3.2.0/tests/_pyMylib/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-12 08:17:49.743681 threadpoolctl-3.2.0/tests/_pyMylib/my_threaded_lib.c
+-rw-r--r--   0        0        0    26145 2023-07-12 08:17:49.743681 threadpoolctl-3.2.0/tests/test_threadpoolctl.py
+-rw-r--r--   0        0        0     2247 2021-09-29 16:23:34.090675 threadpoolctl-3.2.0/tests/utils.py
+-rw-r--r--   0        0        0    41648 2023-07-13 14:44:13.629080 threadpoolctl-3.2.0/threadpoolctl.py
+-rw-r--r--   0        0        0     9967 1970-01-01 00:00:00.000000 threadpoolctl-3.2.0/PKG-INFO
```

### Comparing `threadpoolctl-3.1.0/.azure_pipeline.yml` & `threadpoolctl-3.2.0/.azure_pipeline.yml`

 * *Files 16% similar despite different names*

```diff
@@ -14,32 +14,47 @@
     - master
   always: true
 
 stages:
 - stage:
   jobs:
 
+  - job: 'linting'
+    displayName: Linting
+    pool:
+      vmImage: ubuntu-latest
+    steps:
+      - task: UsePythonVersion@0
+        inputs:
+          versionSpec: '3.11'
+      - script: |
+          pip install black
+        displayName: install black
+      - script: |
+          black --check --diff .
+        displayName: Run black
+
   - template: continuous_integration/windows.yml
     parameters:
       name: Windows
       vmImage: windows-latest
       matrix:
         pylatest_conda_forge_mkl:
           VERSION_PYTHON: '*'
           PACKAGER: 'conda-forge'
           BLAS: 'mkl'
-        py39_conda_forge_openblas:
-          VERSION_PYTHON: '3.9'
+        py310_conda_forge_openblas:
+          VERSION_PYTHON: '3.10'
           PACKAGER: 'conda-forge'
           BLAS: 'openblas'
-        py37_conda:
-          VERSION_PYTHON: '3.7'
+        py39_conda:
+          VERSION_PYTHON: '3.9'
           PACKAGER: 'conda'
-        py36_pip:
-          VERSION_PYTHON: '3.6'
+        py38_pip:
+          VERSION_PYTHON: '3.8'
           PACKAGER: 'pip'
 
 
   - template: continuous_integration/posix.yml
     parameters:
       name: Linux
       vmImage: ubuntu-20.04
@@ -48,24 +63,24 @@
         # are correctly handled.
         py38_ubuntu_atlas_gcc_gcc:
           PACKAGER: 'ubuntu'
           APT_BLAS: 'libatlas3-base libatlas-base-dev'
           VERSION_PYTHON: '3.8'
           CC_OUTER_LOOP: 'gcc'
           CC_INNER_LOOP: 'gcc'
-        py36_ubuntu_openblas_gcc_gcc:
+        py38_ubuntu_openblas_gcc_gcc:
           PACKAGER: 'ubuntu'
           APT_BLAS: 'libopenblas-base libopenblas-dev'
           VERSION_PYTHON: '3.8'
           CC_OUTER_LOOP: 'gcc'
           CC_INNER_LOOP: 'gcc'
-        # Linux + Python 3.7 and homogeneous runtime nesting.
-        py37_conda_openblas_clang_clang:
+        # Linux + Python 3.9 and homogeneous runtime nesting.
+        py39_conda_openblas_clang_clang:
           PACKAGER: 'conda'
-          VERSION_PYTHON: '3.7'
+          VERSION_PYTHON: '3.9'
           BLAS: 'openblas'
           CC_OUTER_LOOP: 'clang-10'
           CC_INNER_LOOP: 'clang-10'
         # Linux environment with MKL and Clang (known to be unsafe for
         # threadpoolctl) to only test the warning from multiple OpenMP.
         pylatest_conda_mkl_clang_gcc:
           PACKAGER: 'conda'
@@ -93,15 +108,14 @@
         pylatest_conda_forge:
           PACKAGER: 'conda-forge'
           VERSION_PYTHON: '*'
           BLAS: 'openblas'
           OPENBLAS_THREADING_LAYER: 'openmp'
           CC_OUTER_LOOP: 'gcc'
           CC_INNER_LOOP: 'gcc'
-          LINT: 'true'
         # Linux environment with no numpy and heterogeneous OpenMP runtimes.
         pylatest_conda_nonumpy_gcc_clang:
           PACKAGER: 'conda'
           NO_NUMPY: 'true'
           VERSION_PYTHON: '*'
           CC_OUTER_LOOP: 'gcc'
           CC_INNER_LOOP: 'clang-10'
@@ -133,24 +147,32 @@
           CC_INNER_LOOP: 'gcc'
           BLIS_CC: 'gcc-8'
           BLIS_ENABLE_THREADING: 'no'
 
   - template: continuous_integration/posix.yml
     parameters:
       name: macOS
-      vmImage: macOS-10.15
+      vmImage: macOS-11
       matrix:
         # MacOS environment with OpenMP installed through homebrew
-        py36_conda_homebrew_libomp:
+        py38_conda_homebrew_libomp:
           PACKAGER: 'conda'
-          VERSION_PYTHON: '3.6'
+          VERSION_PYTHON: '3.8'
           BLAS: 'openblas'
           CC_OUTER_LOOP: 'clang'
           CC_INNER_LOOP: 'clang'
           INSTALL_LIBOMP: 'homebrew'
+        # MacOS env with OpenBLAS and OpenMP installed through conda-forge compilers
+        py39_conda_forge_clang_openblas:
+          PACKAGER: 'conda-forge'
+          VERSION_PYTHON: '*'
+          BLAS: 'openblas'
+          CC_OUTER_LOOP: 'clang'
+          CC_INNER_LOOP: 'clang'
+          INSTALL_LIBOMP: 'conda-forge'
         # MacOS environment with OpenMP installed through conda-forge compilers
         pylatest_conda_forge_clang:
           PACKAGER: 'conda-forge'
           VERSION_PYTHON: '*'
           BLAS: 'mkl'
           CC_OUTER_LOOP: 'clang'
           CC_INNER_LOOP: 'clang'
@@ -160,13 +182,13 @@
   jobs:
   # Meta-test to ensure that at least of the above CI configurations had
   # the necessary platform settings to execute each test without raising
   # skipping.
   - job: 'no_test_always_skipped'
     displayName: 'No test always skipped'
     pool:
-      vmImage: ubuntu-20.04
+      vmImage: ubuntu-latest
     steps:
       - download: current
       - script: |
           python continuous_integration/check_no_test_skipped.py $(Pipeline.Workspace)
         displayName: 'No test always skipped'
```

### Comparing `threadpoolctl-3.1.0/CHANGES.md` & `threadpoolctl-3.2.0/CHANGES.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+3.2.0 (2023-07-13)
+==================
+
+- Dropped support for Python 3.6 and 3.7.
+
+- Added support for custom library controllers. Custom controllers must inherit from
+  the `threadpoolctl.LibController` class and be registered to threadpoolctl using the
+  `threadpoolctl.register` function.
+  https://github.com/joblib/threadpoolctl/pull/138
+
+- A warning is raised on macOS when threadpoolctl finds both Intel OpenMP and LLVM
+  OpenMP runtimes loaded simultaneously by the same Python program. See details and
+  workarounds at https://github.com/joblib/threadpoolctl/blob/master/multiple_openmp.md.
+  https://github.com/joblib/threadpoolctl/pull/142
+
 3.1.0 (2022-01-31)
 ==================
 
 - Fixed a detection issue of the BLAS libraires packaged by conda-forge on Windows.
   https://github.com/joblib/threadpoolctl/pull/112
 
 - `threadpool_limits` and `ThreadpoolController.limit` now accept the string
```

### Comparing `threadpoolctl-3.1.0/LICENSE` & `threadpoolctl-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/README.md` & `threadpoolctl-3.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -188,18 +188,33 @@
 ...     # Inside this function, calls to blas implementation (like openblas or MKL)
 ...     # will be limited to use only one thread.
 ...     a = np.random.randn(1000, 1000)
 ...     a_squared = a @ a
 ...
 ```
 
+### Writing a custom library controller
+
+Currently, `threadpoolctl` has support for `OpenMP` and the main `BLAS` libraries.
+However it can also be used to control the threadpool of other native libraries,
+provided that they expose an API to get and set the limit on the number of threads.
+For that, one must implement a controller for this library and register it to
+`threadpoolctl`.
+
+A custom controller must be a subclass of the `LibController` class and implement
+the attributes and methods described in the docstring of `LibController`. Then this
+new controller class must be registered using the `threadpoolctl.register` function.
+An complete example can be found [here](
+  https://github.com/joblib/threadpoolctl/blob/master/tests/_pyMylib/__init__.py).
+
 ### Sequential BLAS within OpenMP parallel region
 
 When one wants to have sequential BLAS calls within an OpenMP parallel region, it's
-safer to set `limits="sequential_blas_under_openmp"` since setting `limits=1` and `user_api="blas"` might not lead to the expected behavior in some configurations
+safer to set `limits="sequential_blas_under_openmp"` since setting `limits=1` and
+`user_api="blas"` might not lead to the expected behavior in some configurations
 (e.g. OpenBLAS with the OpenMP threading layer
 https://github.com/xianyi/OpenBLAS/issues/2985).
 
 ### Known Limitations
 
 - `threadpool_limits` can fail to limit the number of inner threads when nesting
   parallel loops managed by distinct OpenMP runtime implementations (for instance
```

### Comparing `threadpoolctl-3.1.0/benchmarks/bench_context_manager_overhead.py` & `threadpoolctl-3.2.0/benchmarks/bench_context_manager_overhead.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/continuous_integration/check_no_test_skipped.py` & `threadpoolctl-3.2.0/continuous_integration/check_no_test_skipped.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,15 +29,24 @@
                 print("    -", test_name)
             if test_name in always_skipped:
                 always_skipped[test_name] &= skipped
             else:
                 always_skipped[test_name] = skipped
 
 print("\n------------------------------------------------------------------\n")
+
+# List of tests that we don't want to fail the CI if they are skipped in
+# every job. This is useful for tests that depend on specific versions of
+# numpy or scipy and we don't want to pin old versions of these libraries.
+SAFE_SKIPPED_TESTS = ["test_multiple_shipped_openblas"]
+
 fail = False
 for test, skipped in always_skipped.items():
     if skipped:
-        fail = True
-        print(test, "was skipped in every job")
+        if test in SAFE_SKIPPED_TESTS:
+            print(test, "was skipped in every job but it's fine to skip it")
+        else:
+            fail = True
+            print(test, "was skipped in every job")
 
 if fail:
     sys.exit(1)
```

### Comparing `threadpoolctl-3.1.0/continuous_integration/install.cmd` & `threadpoolctl-3.2.0/continuous_integration/install.cmd`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/continuous_integration/install.sh` & `threadpoolctl-3.2.0/continuous_integration/install.sh`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/continuous_integration/install_with_blis.sh` & `threadpoolctl-3.2.0/continuous_integration/install_with_blis.sh`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Install a recent version of clang and libomp
 wget https://apt.llvm.org/llvm.sh
 chmod +x llvm.sh
 sudo ./llvm.sh 10
 sudo apt-get install libomp-dev
 
 # create conda env
-conda create -n $VIRTUALENV -q --yes python=$VERSION_PYTHON pip cython
+conda create -n $VIRTUALENV -q --yes -c conda-forge python=$VERSION_PYTHON pip cython
 source activate $VIRTUALENV
 
 if [[ "$BLIS_CC" == "gcc-8" ]]; then
     sudo apt install gcc-8
 fi
 
 pushd ..
@@ -37,16 +37,15 @@
 pushd numpy
 git submodule update --init
 echo "[blis]
 libraries = blis
 library_dirs = $ABS_PATH/BLIS_install/lib
 include_dirs = $ABS_PATH/BLIS_install/include/blis
 runtime_library_dirs = $ABS_PATH/BLIS_install/lib" > site.cfg
-python setup.py build_ext -i
-pip install -e .
+python setup.py develop
 popd
 
 popd
 
 python -m pip install -q -r dev-requirements.txt
 CFLAGS=-I$ABS_PATH/BLIS_install/include/blis LDFLAGS=-L$ABS_PATH/BLIS_install/lib \
     bash ./continuous_integration/build_test_ext.sh
```

### Comparing `threadpoolctl-3.1.0/continuous_integration/posix.yml` & `threadpoolctl-3.2.0/continuous_integration/posix.yml`

 * *Files 15% similar despite different names*

```diff
@@ -17,21 +17,14 @@
       condition: or(startsWith(variables['PACKAGER'], 'conda'), eq(variables['PACKAGER'], 'pip'))
     - bash: sudo chown -R $USER $CONDA
       # On Hosted macOS, the agent user doesn't have ownership of Miniconda's installation directory/
       # We need to take ownership if we want to update conda or install packages globally
       displayName: Take ownership of conda installation
       condition: eq('${{ parameters.name }}', 'macOS')
     - script: |
-        conda create -n tmp -y -c conda-forge python black
-        source activate tmp
-        black --check .
-        conda deactivate
-      displayName: Lint
-      condition: eq(variables['LINT'], 'true')
-    - script: |
         continuous_integration/install.sh
       displayName: 'Install without BLIS'
       condition: ne(variables['INSTALL_BLIS'], 'true')
     - script: |
         continuous_integration/install_with_blis.sh
       displayName: 'Install with BLIS'
       condition: eq(variables['INSTALL_BLIS'], 'true')
```

### Comparing `threadpoolctl-3.1.0/continuous_integration/test_script.sh` & `threadpoolctl-3.2.0/continuous_integration/test_script.sh`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/continuous_integration/windows.yml` & `threadpoolctl-3.2.0/continuous_integration/windows.yml`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/multiple_openmp.md` & `threadpoolctl-3.2.0/multiple_openmp.md`

 * *Files 11% similar despite different names*

```diff
@@ -25,43 +25,45 @@
 `prange`), LightGBM and XGBoost (via pragmas in the C++ source code).
 
 From our experience, **most OpenMP libraries can seamlessly coexist in a same
 program**. For instance, on Linux, we never observed any issue between
 `libgomp` and `libiomp`, which is the most common mix (NumPy with MKL + a
 package compiled with GCC, the most widely used C compiler on that platform).
 
-## Incompatibility between Intel OpenMP and LLVM OpenMP under Linux
+## Incompatibility between Intel OpenMP and LLVM OpenMP
 
 The only unrecoverable incompatibility we encountered happens when loading a
 mix of compiled extensions linked with **`libomp` (LLVM/Clang) and `libiomp`
-(ICC), on Linux**, manifested by crashes or deadlocks. It can happen even with
-the simplest OpenMP calls like getting the maximum number of threads that will
-be used in a subsequent parallel region. A possible explanation is that
+(ICC), on Linux and macOS**, manifested by crashes or deadlocks. It can happen
+even with the simplest OpenMP calls like getting the maximum number of threads
+that will be used in a subsequent parallel region. A possible explanation is that
 `libomp` is actually a fork of `libiomp` causing name colliding for instance.
 Using `threadpoolctl` may crash your program in such a setting.
 
 **Fortunately this problem is very rare**: at the time of writing, all major
 binary distributions of Python packages for Linux use either GCC or ICC to
 build the Python scientific packages. Therefore this problem would only happen
 if some packagers decide to start shipping Python packages built with
-LLVM/Clang instead of GCC.
-
-Surprisingly, we never encountered this kind of issue on macOS, where this mix
-is the most frequent (Clang being the default C compiler on macOS).
+LLVM/Clang instead of GCC (this is the case for instance with conda's default channel).
 
 ## Workarounds for Intel OpenMP and LLVM OpenMP case
 
 As far as we know, the only workaround consists in making sure only of one of
 the two incompatible OpenMP libraries is loaded. For example:
 
-- Tell MKL (used by NumPy) to use the GNU OpenMP runtime instead of the Intel
-  OpenMP runtime by setting the following environment variable:
+- Tell MKL (used by NumPy) to use another threading implementation instead of the Intel
+  OpenMP runtime. It can be the GNU OpenMP runtime on Linux or TBB on Linux and MacOS
+  for instance. This is done by setting the following environment variable:
 
       export MKL_THREADING_LAYER=GNU
 
+  or, if TBB is installed:
+
+      export MKL_THREADING_LAYER=TBB
+
 - Install a build of NumPy and SciPy linked against OpenBLAS instead of MKL.
   This can be done for instance by installing NumPy and SciPy from PyPI:
 
       pip install numpy scipy
 
   from the conda-forge conda channel:
 
@@ -78,8 +80,8 @@
 ## References
 
 The above incompatibility has been reported upstream to the LLVM and Intel
 developers on the following public issue trackers/forums along with a minimal
 reproducer written in C:
 
 - https://bugs.llvm.org/show_bug.cgi?id=43565
-- https://software.intel.com/en-us/forums/intel-c-compiler/topic/827607
+- https://community.intel.com/t5/Intel-C-Compiler/Cannot-call-OpenMP-functions-from-libiomp-after-calling-from/m-p/1176406
```

### Comparing `threadpoolctl-3.1.0/pyproject.toml` & `threadpoolctl-3.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 [tool.flit.metadata]
 module = "threadpoolctl"
 author = "Thomas Moreau"
 author-email = "thomas.moreau.2010@gmail.com"
 home-page = "https://github.com/joblib/threadpoolctl"
 description-file = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 license = "BSD-3-Clause"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.black]
 line-length = 88
-target_version = ['py36', 'py37', 'py38', 'py39']
-experimental_string_processing = true
+target_version = ['py38', 'py39', 'py310', 'py311']
+preview = true
```

### Comparing `threadpoolctl-3.1.0/tests/_openmp_test_helper/build_utils.py` & `threadpoolctl-3.2.0/tests/_openmp_test_helper/build_utils.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/tests/_openmp_test_helper/nested_prange_blas.pyx` & `threadpoolctl-3.2.0/tests/_openmp_test_helper/nested_prange_blas.pyx`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/tests/_openmp_test_helper/openmp_helpers_inner.pyx` & `threadpoolctl-3.2.0/tests/_openmp_test_helper/openmp_helpers_inner.pyx`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/tests/_openmp_test_helper/openmp_helpers_outer.pyx` & `threadpoolctl-3.2.0/tests/_openmp_test_helper/openmp_helpers_outer.pyx`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/tests/_openmp_test_helper/setup_inner.py` & `threadpoolctl-3.2.0/tests/_openmp_test_helper/setup_inner.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/tests/_openmp_test_helper/setup_nested_prange_blas.py` & `threadpoolctl-3.2.0/tests/_openmp_test_helper/setup_nested_prange_blas.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/tests/_openmp_test_helper/setup_outer.py` & `threadpoolctl-3.2.0/tests/_openmp_test_helper/setup_outer.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/tests/test_threadpoolctl.py` & `threadpoolctl-3.2.0/tests/test_threadpoolctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,29 @@
 
 def is_old_openblas(lib_controller):
     # Possible bug in getting maximum number of threads with OpenBLAS < 0.2.16
     # and OpenBLAS does not expose its version before 0.3.4.
     return lib_controller.internal_api == "openblas" and lib_controller.version is None
 
 
+def skip_if_openblas_openmp():
+    """Helper to skip tests with side effects when OpenBLAS has the OpenMP
+    threading layer.
+    """
+    if any(
+        lib_controller.internal_api == "openblas"
+        and lib_controller.threading_layer == "openmp"
+        for lib_controller in ThreadpoolController().lib_controllers
+    ):
+        pytest.skip(
+            "Setting a limit on OpenBLAS when using the OpenMP threading layer also "
+            "impact the OpenMP library. They can't be controlled independently."
+        )
+
+
 def effective_num_threads(nthreads, max_threads):
     if nthreads is None or nthreads > max_threads:
         return max_threads
     return nthreads
 
 
 def test_threadpool_info():
@@ -192,34 +207,32 @@
 
     assert ThreadpoolController().info() == original_info
 
 
 def test_threadpool_controller_limit():
     # Check that using the limit method of ThreadpoolController only impact its
     # library controllers.
+
+    # This is not True for OpenBLAS with the OpenMP threading layer.
+    skip_if_openblas_openmp()
+
     blas_controller = ThreadpoolController().select(user_api="blas")
     original_openmp_info = ThreadpoolController().select(user_api="openmp").info()
 
     with blas_controller.limit(limits=1):
         blas_controller = ThreadpoolController().select(user_api="blas")
         openmp_info = ThreadpoolController().select(user_api="openmp").info()
 
         assert all(
             lib_controller.num_threads == 1
             for lib_controller in blas_controller.lib_controllers
         )
         # original_blas_controller contains only blas libraries so no opemp library
-        # should be impacted. This is not True for OpenBLAS with the OpenMP threading
-        # layer.
-        if not any(
-            lib_controller.internal_api == "openblas"
-            and lib_controller.threading_layer == "openmp"
-            for lib_controller in blas_controller.lib_controllers
-        ):
-            assert openmp_info == original_openmp_info
+        # should be impacted.
+        assert openmp_info == original_openmp_info
 
 
 def test_get_params_for_sequential_blas_under_openmp():
     # Test for the behavior of get_params_for_sequential_blas_under_openmp.
     controller = ThreadpoolController()
     original_info = controller.info()
 
@@ -403,14 +416,16 @@
     # threads requested by the context manager when nested in an outer OpenMP
     # loop.
     import numpy as np
     import tests._openmp_test_helper.nested_prange_blas as prange_blas
 
     check_nested_prange_blas = prange_blas.check_nested_prange_blas
 
+    skip_if_openblas_openmp()
+
     original_info = ThreadpoolController().info()
 
     blas_controller = ThreadpoolController().select(user_api="blas")
     blis_controller = ThreadpoolController().select(internal_api="blis")
 
     # skip if the BLAS used by numpy is an old openblas. OpenBLAS 0.3.3 and
     # older are known to cause an unrecoverable deadlock at process shutdown
@@ -441,15 +456,15 @@
     assert all(lib_info["num_threads"] == 1 for lib_info in nested_blas_info)
 
     assert ThreadpoolController().info() == original_info
 
 
 # the method `get_original_num_threads` raises a UserWarning due to different
 # num_threads from libraries with the same `user_api`. It will be raised only
-# in the CI job with 2 openblas (py37_pip_openblas_gcc_clang). It is expected
+# in the CI job with 2 openblas (py38_pip_openblas_gcc_clang). It is expected
 # so we can safely filter it.
 @pytest.mark.filterwarnings("ignore::UserWarning")
 @pytest.mark.parametrize("limit", [1, None])
 def test_get_original_num_threads(limit):
     # Tests the method get_original_num_threads of the context manager
     with threadpool_limits(limits=2, user_api="blas") as ctx:
         # set different blas num threads to start with (when multiple openblas)
@@ -653,7 +668,37 @@
     @controller.wrap(limits=2, user_api="blas")
     def inner_func():
         check_blas_num_threads(expected_num_threads=2)
 
     outer_func()
 
     assert ThreadpoolController().info() == original_info
+
+
+def test_custom_controller():
+    # Check that a custom controller can be used to change the number of threads
+    # used by a library.
+    try:
+        import tests._pyMylib  # noqa
+    except:
+        pytest.skip("requires my_thread_lib to be compiled")
+
+    controller = ThreadpoolController()
+    original_info = controller.info()
+
+    mylib_controller = controller.select(user_api="my_threaded_lib")
+
+    # my_threaded_lib has been found and there's 1 matching shared library
+    assert len(mylib_controller.lib_controllers) == 1
+    mylib_controller = mylib_controller.lib_controllers[0]
+
+    # we linked against my_threaded_lib v2.0 and by default it uses 42 thread
+    assert mylib_controller.version == "2.0"
+    assert mylib_controller.num_threads == 42
+
+    # my_threaded_lib exposes an additional info "some_attr":
+    assert mylib_controller.info()["some_attr"] == "some_value"
+
+    with controller.limit(limits=1, user_api="my_threaded_lib"):
+        assert mylib_controller.num_threads == 1
+
+    assert ThreadpoolController().info() == original_info
```

### Comparing `threadpoolctl-3.1.0/tests/utils.py` & `threadpoolctl-3.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.1.0/threadpoolctl.py` & `threadpoolctl-3.2.0/threadpoolctl.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,29 @@
 # https://github.com/IntelPython/smp (Copyright (c) 2017, Intel Corporation)
 # and also published under the BSD 3-Clause license
 import os
 import re
 import sys
 import ctypes
 import textwrap
+from typing import final
 import warnings
 from ctypes.util import find_library
 from abc import ABC, abstractmethod
 from functools import lru_cache
 from contextlib import ContextDecorator
 
-__version__ = "3.1.0"
-__all__ = ["threadpool_limits", "threadpool_info", "ThreadpoolController"]
+__version__ = "3.2.0"
+__all__ = [
+    "threadpool_limits",
+    "threadpool_info",
+    "ThreadpoolController",
+    "LibController",
+    "register",
+]
 
 
 # One can get runtime errors or even segfaults due to multiple OpenMP libraries
 # loaded simultaneously which can happen easily in Python when importing and
 # using compiled extensions built with different compilers and therefore
 # different OpenMP runtimes in the same program. In particular libiomp (used by
 # Intel ICC) and libomp used by clang/llvm tend to crash. This can happen for
@@ -36,16 +43,16 @@
 # performance issues, in sections of the code where nested OpenMP loops can
 # happen, by dynamically reconfiguring the inner OpenMP runtime to temporarily
 # disable it while under the scope of the outer OpenMP parallel section.
 os.environ.setdefault("KMP_DUPLICATE_LIB_OK", "True")
 
 # Structure to cast the info on dynamically loaded library. See
 # https://linux.die.net/man/3/dl_iterate_phdr for more details.
-_SYSTEM_UINT = ctypes.c_uint64 if sys.maxsize > 2 ** 32 else ctypes.c_uint32
-_SYSTEM_UINT_HALF = ctypes.c_uint32 if sys.maxsize > 2 ** 32 else ctypes.c_uint16
+_SYSTEM_UINT = ctypes.c_uint64 if sys.maxsize > 2**32 else ctypes.c_uint32
+_SYSTEM_UINT_HALF = ctypes.c_uint32 if sys.maxsize > 2**32 else ctypes.c_uint16
 
 
 class _dl_phdr_info(ctypes.Structure):
     _fields_ = [
         ("dlpi_addr", _SYSTEM_UINT),  # Base address of object
         ("dlpi_name", ctypes.c_char_p),  # path to the library
         ("dlpi_phdr", ctypes.c_void_p),  # pointer on dlpi_headers
@@ -56,64 +63,326 @@
 # The RTLD_NOLOAD flag for loading shared libraries is not defined on Windows.
 try:
     _RTLD_NOLOAD = os.RTLD_NOLOAD
 except AttributeError:
     _RTLD_NOLOAD = ctypes.DEFAULT_MODE
 
 
-# List of the supported libraries. The items are indexed by the name of the
-# class to instantiate to create the library controller objects. The items hold
-# the possible prefixes of loaded shared objects, the name of the internal_api
-# to call, the name of the user_api and potentially some symbols that the library is
-# expected to have (this is necessary to distinguish between the blas implementations
-# when they are all renamed "libblas.dll" on conda-forge on windows).
-_SUPPORTED_LIBRARIES = {
-    "OpenMPController": {
-        "user_api": "openmp",
-        "internal_api": "openmp",
-        "filename_prefixes": ("libiomp", "libgomp", "libomp", "vcomp"),
-    },
-    "OpenBLASController": {
-        "user_api": "blas",
-        "internal_api": "openblas",
-        "filename_prefixes": ("libopenblas", "libblas"),
-        "check_symbols": ("openblas_get_num_threads", "openblas_get_num_threads64_"),
-    },
-    "MKLController": {
-        "user_api": "blas",
-        "internal_api": "mkl",
-        "filename_prefixes": ("libmkl_rt", "mkl_rt", "libblas"),
-        "check_symbols": ("MKL_Get_Max_Threads",),
-    },
-    "BLISController": {
-        "user_api": "blas",
-        "internal_api": "blis",
-        "filename_prefixes": ("libblis", "libblas"),
-        "check_symbols": ("bli_thread_get_num_threads",),
-    },
-}
+class LibController(ABC):
+    """Abstract base class for the individual library controllers
+
+    A library controller must expose the following class attributes:
+        - user_api : str
+            Usually the name of the library or generic specification the library
+            implements, e.g. "blas" is a specification with different implementations.
+        - internal_api : str
+            Usually the name of the library or concrete implementation of some
+            specification, e.g. "openblas" is an implementation of the "blas"
+            specification.
+        - filename_prefixes : tuple
+            Possible prefixes of the shared library's filename that allow to
+            identify the library. e.g. "libopenblas" for libopenblas.so.
+
+    and implement the following methods: `get_num_threads`, `set_num_threads` and
+    `get_version`.
+
+    Threadpoolctl loops through all the loaded shared libraries and tries to match
+    the filename of each library with the `filename_prefixes`. If a match is found, a
+    controller is instantiated and a handler to the library is stored in the `dynlib`
+    attribute as a `ctypes.CDLL` object. It can be used to access the necessary symbols
+    of the shared library to implement the above methods.
+
+    The following information will be exposed in the info dictionary:
+      - user_api : standardized API, if any, or a copy of internal_api.
+      - internal_api : implementation-specific API.
+      - num_threads : the current thread limit.
+      - prefix : prefix of the shared library's filename.
+      - filepath : path to the loaded shared library.
+      - version : version of the library (if available).
+
+    In addition, each library controller may expose internal API specific entries. They
+    must be set as attributes in the `set_additional_attributes` method.
+    """
+
+    @final
+    def __init__(self, *, filepath=None, prefix=None):
+        """This is not meant to be overriden by subclasses."""
+        self.prefix = prefix
+        self.filepath = filepath
+        self.dynlib = ctypes.CDLL(filepath, mode=_RTLD_NOLOAD)
+        self.version = self.get_version()
+        self.set_additional_attributes()
+
+    @final
+    def info(self):
+        """Return relevant info wrapped in a dict
+
+        This is not meant to be overriden by subclasses.
+        """
+        exposed_attrs = {
+            "user_api": self.user_api,
+            "internal_api": self.internal_api,
+            "num_threads": self.num_threads,
+            **vars(self),
+        }
+        exposed_attrs.pop("dynlib")
+        return exposed_attrs
+
+    def set_additional_attributes(self):
+        """Set additional attributes meant to be exposed in the info dict"""
+
+    @property
+    def num_threads(self):
+        """Exposes the current thread limit as a dynamic property
+
+        This is not meant to be used or overriden by subclasses.
+        """
+        return self.get_num_threads()
+
+    @abstractmethod
+    def get_num_threads(self):
+        """Return the maximum number of threads available to use"""
+
+    @abstractmethod
+    def set_num_threads(self, num_threads):
+        """Set the maximum number of threads to use"""
+
+    @abstractmethod
+    def get_version(self):
+        """Return the version of the shared library"""
+
+
+class OpenBLASController(LibController):
+    """Controller class for OpenBLAS"""
+
+    user_api = "blas"
+    internal_api = "openblas"
+    filename_prefixes = ("libopenblas", "libblas")
+    check_symbols = ("openblas_get_num_threads", "openblas_get_num_threads64_")
+
+    def set_additional_attributes(self):
+        self.threading_layer = self._get_threading_layer()
+        self.architecture = self._get_architecture()
+
+    def get_num_threads(self):
+        get_func = getattr(
+            self.dynlib,
+            "openblas_get_num_threads",
+            # Symbols differ when built for 64bit integers in Fortran
+            getattr(self.dynlib, "openblas_get_num_threads64_", lambda: None),
+        )
+
+        return get_func()
+
+    def set_num_threads(self, num_threads):
+        set_func = getattr(
+            self.dynlib,
+            "openblas_set_num_threads",
+            # Symbols differ when built for 64bit integers in Fortran
+            getattr(
+                self.dynlib, "openblas_set_num_threads64_", lambda num_threads: None
+            ),
+        )
+        return set_func(num_threads)
+
+    def get_version(self):
+        # None means OpenBLAS is not loaded or version < 0.3.4, since OpenBLAS
+        # did not expose its version before that.
+        get_config = getattr(
+            self.dynlib,
+            "openblas_get_config",
+            getattr(self.dynlib, "openblas_get_config64_", None),
+        )
+        if get_config is None:
+            return None
+
+        get_config.restype = ctypes.c_char_p
+        config = get_config().split()
+        if config[0] == b"OpenBLAS":
+            return config[1].decode("utf-8")
+        return None
+
+    def _get_threading_layer(self):
+        """Return the threading layer of OpenBLAS"""
+        openblas_get_parallel = getattr(
+            self.dynlib,
+            "openblas_get_parallel",
+            getattr(self.dynlib, "openblas_get_parallel64_", None),
+        )
+        if openblas_get_parallel is None:
+            return "unknown"
+        threading_layer = openblas_get_parallel()
+        if threading_layer == 2:
+            return "openmp"
+        elif threading_layer == 1:
+            return "pthreads"
+        return "disabled"
+
+    def _get_architecture(self):
+        """Return the architecture detected by OpenBLAS"""
+        get_corename = getattr(
+            self.dynlib,
+            "openblas_get_corename",
+            getattr(self.dynlib, "openblas_get_corename64_", None),
+        )
+        if get_corename is None:
+            return None
+
+        get_corename.restype = ctypes.c_char_p
+        return get_corename().decode("utf-8")
+
+
+class BLISController(LibController):
+    """Controller class for BLIS"""
+
+    user_api = "blas"
+    internal_api = "blis"
+    filename_prefixes = ("libblis", "libblas")
+    check_symbols = ("bli_thread_get_num_threads",)
+
+    def set_additional_attributes(self):
+        self.threading_layer = self._get_threading_layer()
+        self.architecture = self._get_architecture()
+
+    def get_num_threads(self):
+        get_func = getattr(self.dynlib, "bli_thread_get_num_threads", lambda: None)
+        num_threads = get_func()
+        # by default BLIS is single-threaded and get_num_threads
+        # returns -1. We map it to 1 for consistency with other libraries.
+        return 1 if num_threads == -1 else num_threads
+
+    def set_num_threads(self, num_threads):
+        set_func = getattr(
+            self.dynlib, "bli_thread_set_num_threads", lambda num_threads: None
+        )
+        return set_func(num_threads)
+
+    def get_version(self):
+        get_version_ = getattr(self.dynlib, "bli_info_get_version_str", None)
+        if get_version_ is None:
+            return None
+
+        get_version_.restype = ctypes.c_char_p
+        return get_version_().decode("utf-8")
+
+    def _get_threading_layer(self):
+        """Return the threading layer of BLIS"""
+        if self.dynlib.bli_info_get_enable_openmp():
+            return "openmp"
+        elif self.dynlib.bli_info_get_enable_pthreads():
+            return "pthreads"
+        return "disabled"
+
+    def _get_architecture(self):
+        """Return the architecture detected by BLIS"""
+        bli_arch_query_id = getattr(self.dynlib, "bli_arch_query_id", None)
+        bli_arch_string = getattr(self.dynlib, "bli_arch_string", None)
+        if bli_arch_query_id is None or bli_arch_string is None:
+            return None
+
+        # the true restype should be BLIS' arch_t (enum) but int should work
+        # for us:
+        bli_arch_query_id.restype = ctypes.c_int
+        bli_arch_string.restype = ctypes.c_char_p
+        return bli_arch_string(bli_arch_query_id()).decode("utf-8")
+
+
+class MKLController(LibController):
+    """Controller class for MKL"""
+
+    user_api = "blas"
+    internal_api = "mkl"
+    filename_prefixes = ("libmkl_rt", "mkl_rt", "libblas")
+    check_symbols = ("MKL_Get_Max_Threads",)
+
+    def set_additional_attributes(self):
+        self.threading_layer = self._get_threading_layer()
+
+    def get_num_threads(self):
+        get_func = getattr(self.dynlib, "MKL_Get_Max_Threads", lambda: None)
+        return get_func()
+
+    def set_num_threads(self, num_threads):
+        set_func = getattr(self.dynlib, "MKL_Set_Num_Threads", lambda num_threads: None)
+        return set_func(num_threads)
+
+    def get_version(self):
+        if not hasattr(self.dynlib, "MKL_Get_Version_String"):
+            return None
+
+        res = ctypes.create_string_buffer(200)
+        self.dynlib.MKL_Get_Version_String(res, 200)
+
+        version = res.value.decode("utf-8")
+        group = re.search(r"Version ([^ ]+) ", version)
+        if group is not None:
+            version = group.groups()[0]
+        return version.strip()
+
+    def _get_threading_layer(self):
+        """Return the threading layer of MKL"""
+        # The function mkl_set_threading_layer returns the current threading
+        # layer. Calling it with an invalid threading layer allows us to safely
+        # get the threading layer
+        set_threading_layer = getattr(
+            self.dynlib, "MKL_Set_Threading_Layer", lambda layer: -1
+        )
+        layer_map = {
+            0: "intel",
+            1: "sequential",
+            2: "pgi",
+            3: "gnu",
+            4: "tbb",
+            -1: "not specified",
+        }
+        return layer_map[set_threading_layer(-1)]
+
+
+class OpenMPController(LibController):
+    """Controller class for OpenMP"""
+
+    user_api = "openmp"
+    internal_api = "openmp"
+    filename_prefixes = ("libiomp", "libgomp", "libomp", "vcomp")
+
+    def get_num_threads(self):
+        get_func = getattr(self.dynlib, "omp_get_max_threads", lambda: None)
+        return get_func()
+
+    def set_num_threads(self, num_threads):
+        set_func = getattr(self.dynlib, "omp_set_num_threads", lambda num_threads: None)
+        return set_func(num_threads)
+
+    def get_version(self):
+        # There is no way to get the version number programmatically in OpenMP.
+        return None
+
+
+# Controllers for the libraries that we'll look for in the loaded libraries.
+# Third party libraries can register their own controllers.
+_ALL_CONTROLLERS = [OpenBLASController, BLISController, MKLController, OpenMPController]
 
 # Helpers for the doc and test names
-_ALL_USER_APIS = list(set(lib["user_api"] for lib in _SUPPORTED_LIBRARIES.values()))
-_ALL_INTERNAL_APIS = [lib["internal_api"] for lib in _SUPPORTED_LIBRARIES.values()]
+_ALL_USER_APIS = list(set(lib.user_api for lib in _ALL_CONTROLLERS))
+_ALL_INTERNAL_APIS = [lib.internal_api for lib in _ALL_CONTROLLERS]
 _ALL_PREFIXES = list(
-    set(
-        prefix
-        for lib in _SUPPORTED_LIBRARIES.values()
-        for prefix in lib["filename_prefixes"]
-    )
+    set(prefix for lib in _ALL_CONTROLLERS for prefix in lib.filename_prefixes)
 )
 _ALL_BLAS_LIBRARIES = [
-    lib["internal_api"]
-    for lib in _SUPPORTED_LIBRARIES.values()
-    if lib["user_api"] == "blas"
+    lib.internal_api for lib in _ALL_CONTROLLERS if lib.user_api == "blas"
 ]
-_ALL_OPENMP_LIBRARIES = list(
-    _SUPPORTED_LIBRARIES["OpenMPController"]["filename_prefixes"]
-)
+_ALL_OPENMP_LIBRARIES = OpenMPController.filename_prefixes
+
+
+def register(controller):
+    """Register a new controller"""
+    _ALL_CONTROLLERS.append(controller)
+    _ALL_USER_APIS.append(controller.user_api)
+    _ALL_INTERNAL_APIS.append(controller.internal_api)
+    _ALL_PREFIXES.extend(controller.filename_prefixes)
 
 
 def _format_docstring(*args, **kwargs):
     def decorator(o):
         if o.__doc__ is not None:
             o.__doc__ = o.__doc__.format(*args, **kwargs)
         return o
@@ -373,20 +642,14 @@
         super().__init__(ThreadpoolController(), limits=limits, user_api=user_api)
 
     @classmethod
     def wrap(cls, limits=None, user_api=None):
         return super().wrap(ThreadpoolController(), limits=limits, user_api=user_api)
 
 
-@_format_docstring(
-    PREFIXES=", ".join(f'"{prefix}"' for prefix in _ALL_PREFIXES),
-    USER_APIS=", ".join(f'"{api}"' for api in _ALL_USER_APIS),
-    BLAS_LIBS=", ".join(_ALL_BLAS_LIBRARIES),
-    OPENMP_LIBS=", ".join(_ALL_OPENMP_LIBRARIES),
-)
 class ThreadpoolController:
     """Collection of LibController objects for all loaded supported libraries
 
     Attributes
     ----------
     lib_controllers : list of `LibController` objects
         The list of library controllers of all loaded supported libraries.
@@ -660,15 +923,14 @@
             count = needed.value // (buf_size // buf_count)
             h_modules = map(HMODULE, buf[:count])
 
             # Loop through all the module headers and get the library path
             buf = ctypes.create_unicode_buffer(MAX_PATH)
             n_size = DWORD()
             for h_module in h_modules:
-
                 # Get the path of the current module
                 if not ps_api.GetModuleFileNameExW(
                     h_process, h_module, ctypes.byref(buf), ctypes.byref(n_size)
                 ):
                     raise OSError("GetModuleFileNameEx failed")
                 filepath = buf.value
 
@@ -683,17 +945,17 @@
         filepath = _realpath(filepath)
         # `lower` required to take account of OpenMP dll case on Windows
         # (vcomp, VCOMP, Vcomp, ...)
         filename = os.path.basename(filepath).lower()
 
         # Loop through supported libraries to find if this filename corresponds
         # to a supported one.
-        for controller_class, candidate_lib in _SUPPORTED_LIBRARIES.items():
+        for controller_class in _ALL_CONTROLLERS:
             # check if filename matches a supported prefix
-            prefix = self._check_prefix(filename, candidate_lib["filename_prefixes"])
+            prefix = self._check_prefix(filename, controller_class.filename_prefixes)
 
             # filename does not match any of the prefixes of the candidate
             # library. move to next library.
             if prefix is None:
                 continue
 
             # workaround for BLAS libraries packaged by conda-forge on windows, which
@@ -701,77 +963,69 @@
             # implementation it actually corresponds looking for implementation
             # specific symbols.
             if prefix == "libblas":
                 if filename.endswith(".dll"):
                     libblas = ctypes.CDLL(filepath, _RTLD_NOLOAD)
                     if not any(
                         hasattr(libblas, func)
-                        for func in candidate_lib["check_symbols"]
+                        for func in controller_class.check_symbols
                     ):
                         continue
                 else:
                     # We ignore libblas on other platforms than windows because there
                     # might be a libblas dso comming with openblas for instance that
                     # can't be used to instantiate a pertinent LibController (many
                     # symbols are missing) and would create confusion by making a
                     # duplicate entry in threadpool_info.
                     continue
 
             # filename matches a prefix. Create and store the library
             # controller.
-            user_api = candidate_lib["user_api"]
-            internal_api = candidate_lib["internal_api"]
 
-            lib_controller_class = globals()[controller_class]
-            lib_controller = lib_controller_class(
-                filepath=filepath,
-                prefix=prefix,
-                user_api=user_api,
-                internal_api=internal_api,
-            )
+            lib_controller = controller_class(filepath=filepath, prefix=prefix)
             self.lib_controllers.append(lib_controller)
 
     def _check_prefix(self, library_basename, filename_prefixes):
         """Return the prefix library_basename starts with
 
         Return None if none matches.
         """
         for prefix in filename_prefixes:
             if library_basename.startswith(prefix):
                 return prefix
         return None
 
     def _warn_if_incompatible_openmp(self):
         """Raise a warning if llvm-OpenMP and intel-OpenMP are both loaded"""
-        if sys.platform != "linux":
-            # Only raise the warning on linux
-            return
-
         prefixes = [lib_controller.prefix for lib_controller in self.lib_controllers]
-        msg = textwrap.dedent(
-            """
+        msg = textwrap.dedent("""
             Found Intel OpenMP ('libiomp') and LLVM OpenMP ('libomp') loaded at
             the same time. Both libraries are known to be incompatible and this
             can cause random crashes or deadlocks on Linux when loaded in the
             same Python program.
             Using threadpoolctl may cause crashes or deadlocks. For more
             information and possible workarounds, please see
                 https://github.com/joblib/threadpoolctl/blob/master/multiple_openmp.md
-            """
-        )
+            """)
         if "libomp" in prefixes and "libiomp" in prefixes:
             warnings.warn(msg, RuntimeWarning)
 
     @classmethod
     def _get_libc(cls):
         """Load the lib-C for unix systems."""
         libc = cls._system_libraries.get("libc")
         if libc is None:
             libc_name = find_library("c")
             if libc_name is None:  # pragma: no cover
+                warnings.warn(
+                    "libc not found. The ctypes module in Python"
+                    f" {sys.version_info.major}.{sys.version_info.minor} is maybe"
+                    " too old for this OS.",
+                    RuntimeWarning,
+                )
                 return None
             libc = ctypes.CDLL(libc_name, mode=_RTLD_NOLOAD)
             cls._system_libraries["libc"] = libc
         return libc
 
     @classmethod
     def _get_windll(cls, dll_name):
@@ -779,260 +1033,14 @@
         dll = cls._system_libraries.get(dll_name)
         if dll is None:
             dll = ctypes.WinDLL(f"{dll_name}.dll")
             cls._system_libraries[dll_name] = dll
         return dll
 
 
-@_format_docstring(
-    USER_APIS=", ".join('"{}"'.format(api) for api in _ALL_USER_APIS),
-    INTERNAL_APIS=", ".join('"{}"'.format(api) for api in _ALL_INTERNAL_APIS),
-)
-class LibController(ABC):
-    """Abstract base class for the individual library controllers
-
-    A library controller is represented by the following information:
-      - "user_api" : user API. Possible values are {USER_APIS}.
-      - "internal_api" : internal API. Possible values are {INTERNAL_APIS}.
-      - "prefix" : prefix of the shared library's name.
-      - "filepath" : path to the loaded library.
-      - "version" : version of the library (if available).
-      - "num_threads" : the current thread limit.
-
-    In addition, each library controller may contain internal_api specific
-    entries.
-    """
-
-    def __init__(self, *, filepath=None, prefix=None, user_api=None, internal_api=None):
-        self.user_api = user_api
-        self.internal_api = internal_api
-        self.prefix = prefix
-        self.filepath = filepath
-        self._dynlib = ctypes.CDLL(filepath, mode=_RTLD_NOLOAD)
-        self.version = self.get_version()
-
-    def info(self):
-        """Return relevant info wrapped in a dict"""
-        all_attrs = dict(vars(self), **{"num_threads": self.num_threads})
-        return {k: v for k, v in all_attrs.items() if not k.startswith("_")}
-
-    @property
-    def num_threads(self):
-        return self.get_num_threads()
-
-    @abstractmethod
-    def get_num_threads(self):
-        """Return the maximum number of threads available to use"""
-        pass  # pragma: no cover
-
-    @abstractmethod
-    def set_num_threads(self, num_threads):
-        """Set the maximum number of threads to use"""
-        pass  # pragma: no cover
-
-    @abstractmethod
-    def get_version(self):
-        """Return the version of the shared library"""
-        pass  # pragma: no cover
-
-
-class OpenBLASController(LibController):
-    """Controller class for OpenBLAS"""
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.threading_layer = self._get_threading_layer()
-        self.architecture = self._get_architecture()
-
-    def get_num_threads(self):
-        get_func = getattr(
-            self._dynlib,
-            "openblas_get_num_threads",
-            # Symbols differ when built for 64bit integers in Fortran
-            getattr(self._dynlib, "openblas_get_num_threads64_", lambda: None),
-        )
-
-        return get_func()
-
-    def set_num_threads(self, num_threads):
-        set_func = getattr(
-            self._dynlib,
-            "openblas_set_num_threads",
-            # Symbols differ when built for 64bit integers in Fortran
-            getattr(
-                self._dynlib, "openblas_set_num_threads64_", lambda num_threads: None
-            ),
-        )
-        return set_func(num_threads)
-
-    def get_version(self):
-        # None means OpenBLAS is not loaded or version < 0.3.4, since OpenBLAS
-        # did not expose its version before that.
-        get_config = getattr(
-            self._dynlib,
-            "openblas_get_config",
-            getattr(self._dynlib, "openblas_get_config64_", None),
-        )
-        if get_config is None:
-            return None
-
-        get_config.restype = ctypes.c_char_p
-        config = get_config().split()
-        if config[0] == b"OpenBLAS":
-            return config[1].decode("utf-8")
-        return None
-
-    def _get_threading_layer(self):
-        """Return the threading layer of OpenBLAS"""
-        openblas_get_parallel = getattr(
-            self._dynlib,
-            "openblas_get_parallel",
-            getattr(self._dynlib, "openblas_get_parallel64_", None),
-        )
-        if openblas_get_parallel is None:
-            return "unknown"
-        threading_layer = openblas_get_parallel()
-        if threading_layer == 2:
-            return "openmp"
-        elif threading_layer == 1:
-            return "pthreads"
-        return "disabled"
-
-    def _get_architecture(self):
-        """Return the architecture detected by OpenBLAS"""
-        get_corename = getattr(
-            self._dynlib,
-            "openblas_get_corename",
-            getattr(self._dynlib, "openblas_get_corename64_", None),
-        )
-        if get_corename is None:
-            return None
-
-        get_corename.restype = ctypes.c_char_p
-        return get_corename().decode("utf-8")
-
-
-class BLISController(LibController):
-    """Controller class for BLIS"""
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.threading_layer = self._get_threading_layer()
-        self.architecture = self._get_architecture()
-
-    def get_num_threads(self):
-        get_func = getattr(self._dynlib, "bli_thread_get_num_threads", lambda: None)
-        num_threads = get_func()
-        # by default BLIS is single-threaded and get_num_threads
-        # returns -1. We map it to 1 for consistency with other libraries.
-        return 1 if num_threads == -1 else num_threads
-
-    def set_num_threads(self, num_threads):
-        set_func = getattr(
-            self._dynlib, "bli_thread_set_num_threads", lambda num_threads: None
-        )
-        return set_func(num_threads)
-
-    def get_version(self):
-        get_version_ = getattr(self._dynlib, "bli_info_get_version_str", None)
-        if get_version_ is None:
-            return None
-
-        get_version_.restype = ctypes.c_char_p
-        return get_version_().decode("utf-8")
-
-    def _get_threading_layer(self):
-        """Return the threading layer of BLIS"""
-        if self._dynlib.bli_info_get_enable_openmp():
-            return "openmp"
-        elif self._dynlib.bli_info_get_enable_pthreads():
-            return "pthreads"
-        return "disabled"
-
-    def _get_architecture(self):
-        """Return the architecture detected by BLIS"""
-        bli_arch_query_id = getattr(self._dynlib, "bli_arch_query_id", None)
-        bli_arch_string = getattr(self._dynlib, "bli_arch_string", None)
-        if bli_arch_query_id is None or bli_arch_string is None:
-            return None
-
-        # the true restype should be BLIS' arch_t (enum) but int should work
-        # for us:
-        bli_arch_query_id.restype = ctypes.c_int
-        bli_arch_string.restype = ctypes.c_char_p
-        return bli_arch_string(bli_arch_query_id()).decode("utf-8")
-
-
-class MKLController(LibController):
-    """Controller class for MKL"""
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.threading_layer = self._get_threading_layer()
-
-    def get_num_threads(self):
-        get_func = getattr(self._dynlib, "MKL_Get_Max_Threads", lambda: None)
-        return get_func()
-
-    def set_num_threads(self, num_threads):
-        set_func = getattr(
-            self._dynlib, "MKL_Set_Num_Threads", lambda num_threads: None
-        )
-        return set_func(num_threads)
-
-    def get_version(self):
-        if not hasattr(self._dynlib, "MKL_Get_Version_String"):
-            return None
-
-        res = ctypes.create_string_buffer(200)
-        self._dynlib.MKL_Get_Version_String(res, 200)
-
-        version = res.value.decode("utf-8")
-        group = re.search(r"Version ([^ ]+) ", version)
-        if group is not None:
-            version = group.groups()[0]
-        return version.strip()
-
-    def _get_threading_layer(self):
-        """Return the threading layer of MKL"""
-        # The function mkl_set_threading_layer returns the current threading
-        # layer. Calling it with an invalid threading layer allows us to safely
-        # get the threading layer
-        set_threading_layer = getattr(
-            self._dynlib, "MKL_Set_Threading_Layer", lambda layer: -1
-        )
-        layer_map = {
-            0: "intel",
-            1: "sequential",
-            2: "pgi",
-            3: "gnu",
-            4: "tbb",
-            -1: "not specified",
-        }
-        return layer_map[set_threading_layer(-1)]
-
-
-class OpenMPController(LibController):
-    """Controller class for OpenMP"""
-
-    def get_num_threads(self):
-        get_func = getattr(self._dynlib, "omp_get_max_threads", lambda: None)
-        return get_func()
-
-    def set_num_threads(self, num_threads):
-        set_func = getattr(
-            self._dynlib, "omp_set_num_threads", lambda num_threads: None
-        )
-        return set_func(num_threads)
-
-    def get_version(self):
-        # There is no way to get the version number programmatically in OpenMP.
-        return None
-
-
 def _main():
     """Commandline interface to display thread-pool information and exit."""
     import argparse
     import importlib
     import json
     import sys
```

### Comparing `threadpoolctl-3.1.0/PKG-INFO` & `threadpoolctl-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: threadpoolctl
-Version: 3.1.0
+Version: 3.2.0
 Summary: threadpoolctl
 Home-page: https://github.com/joblib/threadpoolctl
 License: BSD-3-Clause
 Author: Thomas Moreau
 Author-email: thomas.moreau.2010@gmail.com
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 
 # Thread-pool Controls [![Build Status](https://dev.azure.com/joblib/threadpoolctl/_apis/build/status/joblib.threadpoolctl?branchName=master)](https://dev.azure.com/joblib/threadpoolctl/_build/latest?definitionId=1&branchName=master) [![codecov](https://codecov.io/gh/joblib/threadpoolctl/branch/master/graph/badge.svg)](https://codecov.io/gh/joblib/threadpoolctl)
 
 Python helpers to limit the number of threads used in the
 threadpool-backed of common native libraries used for scientific
 computing and data science (e.g. BLAS and OpenMP).
@@ -207,18 +207,33 @@
 ...     # Inside this function, calls to blas implementation (like openblas or MKL)
 ...     # will be limited to use only one thread.
 ...     a = np.random.randn(1000, 1000)
 ...     a_squared = a @ a
 ...
 ```
 
+### Writing a custom library controller
+
+Currently, `threadpoolctl` has support for `OpenMP` and the main `BLAS` libraries.
+However it can also be used to control the threadpool of other native libraries,
+provided that they expose an API to get and set the limit on the number of threads.
+For that, one must implement a controller for this library and register it to
+`threadpoolctl`.
+
+A custom controller must be a subclass of the `LibController` class and implement
+the attributes and methods described in the docstring of `LibController`. Then this
+new controller class must be registered using the `threadpoolctl.register` function.
+An complete example can be found [here](
+  https://github.com/joblib/threadpoolctl/blob/master/tests/_pyMylib/__init__.py).
+
 ### Sequential BLAS within OpenMP parallel region
 
 When one wants to have sequential BLAS calls within an OpenMP parallel region, it's
-safer to set `limits="sequential_blas_under_openmp"` since setting `limits=1` and `user_api="blas"` might not lead to the expected behavior in some configurations
+safer to set `limits="sequential_blas_under_openmp"` since setting `limits=1` and
+`user_api="blas"` might not lead to the expected behavior in some configurations
 (e.g. OpenBLAS with the OpenMP threading layer
 https://github.com/xianyi/OpenBLAS/issues/2985).
 
 ### Known Limitations
 
 - `threadpool_limits` can fail to limit the number of inner threads when nesting
   parallel loops managed by distinct OpenMP runtime implementations (for instance
```

