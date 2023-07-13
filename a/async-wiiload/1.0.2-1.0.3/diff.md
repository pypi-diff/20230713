# Comparing `tmp/async-wiiload-1.0.2.tar.gz` & `tmp/async-wiiload-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/async-wiiload/async-wiiload/dist/tmp0gx3sfw9/async-wiiload-1.0.2.tar", last modified: Tue May 31 16:19:02 2022, max compression
+gzip compressed data, was "async-wiiload-1.0.3.tar", last modified: Thu Jul 13 10:19:48 2023, max compression
```

## Comparing `async-wiiload-1.0.2.tar` & `async-wiiload-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/async_wiiload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/async_wiiload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/async_wiiload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/async_wiiload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/async_wiiload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/async_wiiload.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 16:19:00.000000 async-wiiload-1.0.2/async_wiiload.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/requirements-setuptools.txt
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/tests/test_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 16:19:02.000000 async-wiiload-1.0.2/wiiload/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/wiiload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/wiiload/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1843 2022-05-31 16:18:46.000000 async-wiiload-1.0.2/wiiload/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-31 16:19:01.000000 async-wiiload-1.0.2/wiiload/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/.github/workflows/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/requirements-setuptools.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.857669 async-wiiload-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/src/async_wiiload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/async_wiiload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/async_wiiload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/async_wiiload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/async_wiiload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/async_wiiload.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/src/wiiload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/src/wiiload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/src/wiiload/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/src/wiiload/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/wiiload/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/tests/test_upload.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `async-wiiload-1.0.2/.github/workflows/ci.yml` & `async-wiiload-1.0.3/.github/workflows/ci.yml`

 * *Files 27% similar despite different names*

```diff
@@ -10,68 +10,65 @@
     branches: [ main ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
+          submodules: 'recursive'
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.7"
+          python-version: "3.8"
 
       - name: Prepare Python
         run: python -m pip install build
 
       - name: Build Packages
-        run: python -m build
+        run: PYTHONWARNINGS=error python -m build
 
       - name: Store the packages
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: python-package-distributions
           path: dist
 
   test:
     needs:
       - build
     
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ "3.7", "3.8", "3.9", "3.10", "3.11.0-beta - 3.11.0" ]
+        python-version: [ "3.8", "3.9", "3.10", "3.11", "3.12.0-beta - 3.12.0" ]
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Download all the dists
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
-          
-      - name: Glob match
-        id: glob
-        run: echo ::set-output name=wheel::$(ls dist/*.whl)
-        shell: bash
 
       - name: Install built wheel
-        run: python -m pip install "${{ steps.glob.outputs.wheel }}[test]" -c requirements.txt
+        run: python -m pip install "$(ls dist/*.whl)[test]" -c requirements.txt
+        shell: bash
 
       - name: run pytest
         run: python -m pytest --cov
 
       - name: codecov
         uses: codecov/codecov-action@v3
         with:
@@ -80,24 +77,24 @@
   pypi:
     runs-on: 'ubuntu-latest'
     needs:
       - test
 
     steps:
       - name: Download all the dists
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
 
       - name: Publish 📦 to TestPyPI
         if: ${{ github.ref == 'refs/heads/main' }}
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.testpypi_password }}
           repository_url: https://test.pypi.org/legacy/
       
       - name: Publish 📦 to PyPI
         if: ${{ startsWith(github.ref, 'refs/tags/') }}
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.pypi_password }}
```

### Comparing `async-wiiload-1.0.2/.gitignore` & `async-wiiload-1.0.3/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -128,8 +128,8 @@
 # Pyre type checker
 .pyre/
 
 # PyCharm
 /.idea
 
 # Project files
-/wiiload/version.py
+/src/wiiload/version.py
```

### Comparing `async-wiiload-1.0.2/LICENSE` & `async-wiiload-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async-wiiload-1.0.2/tests/test_main.py` & `async-wiiload-1.0.3/tests/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-import pytest
-from mock import MagicMock, AsyncMock
+from __future__ import annotations
+
+from unittest.mock import AsyncMock, MagicMock
 
+import pytest
 from wiiload import __main__
 
 
 @pytest.mark.parametrize("from_env", [False, True])
 async def test_execute_args(mocker, monkeypatch, from_env):
-    mock_upload_bytes = mocker.patch("wiiload.upload.upload_file", new_callable=AsyncMock)
+    mock_upload_bytes = mocker.patch(
+        "wiiload.upload.upload_file", new_callable=AsyncMock
+    )
 
     args = MagicMock()
     args.dol = "foo_file"
     args.rest = ["foo"]
     if from_env:
         args.wii = None
         monkeypatch.setenv("WIILOAD", "tcp:wii_ip")
@@ -24,15 +28,17 @@
     # Assert
     mock_upload_bytes.assert_awaited_once_with("foo_file", ["foo"], "wii_ip")
 
 
 @pytest.mark.parametrize("missing", [False, True])
 def test_get_wii_from_env_fail(monkeypatch, missing):
     if missing:
-        expected_msg = '--wii not specified, and WIILOAD environment variable is missing'
+        expected_msg = (
+            "--wii not specified, and WIILOAD environment variable is missing"
+        )
         monkeypatch.delenv("WIILOAD", raising=False)
     else:
         expected_msg = "does not start with"
         monkeypatch.setenv("WIILOAD", "wrong env")
 
     with pytest.raises(RuntimeError, match=expected_msg):
         __main__.get_wii_from_env()
```

### Comparing `async-wiiload-1.0.2/wiiload/__main__.py` & `async-wiiload-1.0.3/src/wiiload/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,51 @@
+from __future__ import annotations
+
 import argparse
 import asyncio
 import os
 from pathlib import Path
 
 from wiiload import upload
 
 
 def create_parser():
     parser = argparse.ArgumentParser("wiiload")
-    parser.add_argument("--wii", help="The hostname of the Wii to upload to. "
-                                      "Defaults to using the WIILOAD environment variable.")
+    parser.add_argument(
+        "--wii",
+        help="The hostname of the Wii to upload to. "
+        "Defaults to using the WIILOAD environment variable.",
+    )
     parser.add_argument("dol", type=Path, help="Path to the dol to upload.")
     parser.add_argument("rest", nargs=argparse.REMAINDER)
     return parser
 
 
 def get_wii_from_env():
     wiiload_env = os.getenv("WIILOAD")
     if wiiload_env is None:
-        raise RuntimeError("--wii not specified, and WIILOAD environment variable is missing")
+        raise RuntimeError(
+            "--wii not specified, and WIILOAD environment variable is missing"
+        )
 
     if wiiload_env.startswith("tcp:"):
         return wiiload_env[4:]
     else:
-        raise RuntimeError(f"WIILOAD environment variable ({wiiload_env}) does not start with `tcp:`")
+        raise RuntimeError(
+            f"WIILOAD environment variable ({wiiload_env}) does not start with `tcp:`"
+        )
 
 
 async def execute_args(args):
     wii = args.wii
     if wii is None:
         wii = get_wii_from_env()
     await upload.upload_file(args.dol, args.rest, wii)
 
 
 async def main():
     args = create_parser().parse_args()
     await execute_args(args)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `async-wiiload-1.0.2/wiiload/upload.py` & `async-wiiload-1.0.3/src/wiiload/upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+from __future__ import annotations
+
 import asyncio
-import os
 import struct
 import zlib
-from os import PathLike
-from typing import List
+from pathlib import Path
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from os import PathLike
 
 WIILOAD_VERSION_MAJOR = 0
 WIILOAD_VERSION_MINOR = 5
 
 
-async def upload_bytes(dol: bytes, argv: List[str], host: str, port: int = 4299):
+async def upload_bytes(dol: bytes, argv: list[str], host: str, port: int = 4299):
     """
     Uploads a file it to a Wii.
     :param dol: The bytes of a file to upload to wii.
     :param argv: Arguments to send to wii. The first value is usually the name of the file.
     :param host: The Wii's hostname/ip
     :param port: The port that Homebrew Channel is listening at.
     :return:
@@ -35,24 +39,24 @@
     writer.write(c_data)
     writer.write(args)
     await writer.drain()
     writer.close()
     await writer.wait_closed()
 
 
-async def upload_file(path: PathLike, argv: List[str], host: str, port: int = 4299):
+async def upload_file(path: PathLike, argv: list[str], host: str, port: int = 4299):
     """
     Reads a file from disk and uploads it to a Wii.
     :param path: Path to a file to be uploaded.
     :param argv: Extra arguments to send to wii, after the name of the file.
     :param host: The Wii's hostname/ip
     :param port: The port that Homebrew Channel is listening at.
     :return:
     """
 
-    with open(path, "rb") as f:
-        dol = f.read()
+    path = Path(path)
+    dol = path.read_bytes()
 
-    args = [os.path.basename(path)]
+    args = [path.name]
     args.extend(argv)
 
     return await upload_bytes(dol, args, host, port)
```

