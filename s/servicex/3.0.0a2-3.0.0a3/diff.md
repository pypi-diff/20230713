# Comparing `tmp/servicex-3.0.0a2.tar.gz` & `tmp/servicex-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex-3.0.0a2.tar", max compression
+gzip compressed data, was "servicex-3.0.0a3.tar", max compression
```

## Comparing `servicex-3.0.0a2.tar` & `servicex-3.0.0a3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1499 2023-06-19 14:46:52.495569 servicex-3.0.0a2/LICENSE
--rw-r--r--   0        0        0     4890 2023-06-19 14:46:52.495569 servicex-3.0.0a2/README.md
--rw-r--r--   0        0        0     1187 2023-06-19 14:47:30.391655 servicex-3.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     1535 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/__init__.py
--rw-r--r--   0        0        0       96 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/_version.py
--rw-r--r--   0        0        0     1535 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/app/__init__.py
--rw-r--r--   0        0        0     3157 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/app/cache.py
--rw-r--r--   0        0        0     1776 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/app/cli_options.py
--rw-r--r--   0        0        0     2643 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/app/main.py
--rw-r--r--   0        0        0     5414 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/app/transforms.py
--rw-r--r--   0        0        0     3721 2023-06-19 14:46:52.495569 servicex-3.0.0a2/servicex_client/configuration.py
--rw-r--r--   0        0        0    17500 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/dataset.py
--rw-r--r--   0        0        0     2674 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/dataset_group.py
--rw-r--r--   0        0        0     3410 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/dataset_identifier.py
--rw-r--r--   0        0        0     1535 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/func_adl/__init__.py
--rw-r--r--   0        0        0     4013 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/func_adl/util.py
--rw-r--r--   0        0        0    11894 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/func_adl_dataset.py
--rw-r--r--   0        0        0     4184 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/minio_adpater.py
--rw-r--r--   0        0        0     5130 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/models.py
--rw-r--r--   0        0        0     3111 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/python_dataset.py
--rw-r--r--   0        0        0     4405 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/query_cache.py
--rw-r--r--   0        0        0     5424 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/servicex_adapter.py
--rw-r--r--   0        0        0     8042 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/servicex_client.py
--rw-r--r--   0        0        0     1692 2023-06-19 14:46:52.499569 servicex-3.0.0a2/servicex_client/types.py
--rw-r--r--   0        0        0     6278 1970-01-01 00:00:00.000000 servicex-3.0.0a2/setup.py
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 servicex-3.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1499 2023-07-13 21:15:11.933733 servicex-3.0.0a3/LICENSE
+-rw-r--r--   0        0        0     4890 2023-07-13 21:15:11.933733 servicex-3.0.0a3/README.md
+-rw-r--r--   0        0        0     1246 2023-07-13 21:16:36.119434 servicex-3.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     2212 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/__init__.py
+-rw-r--r--   0        0        0       96 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/_version.py
+-rw-r--r--   0        0        0     1535 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/app/__init__.py
+-rw-r--r--   0        0        0     3181 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/app/cache.py
+-rw-r--r--   0        0        0     1776 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/app/cli_options.py
+-rw-r--r--   0        0        0     2608 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/app/main.py
+-rw-r--r--   0        0        0     5221 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/app/transforms.py
+-rw-r--r--   0        0        0     3760 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/configuration.py
+-rw-r--r--   0        0        0    17443 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/dataset.py
+-rw-r--r--   0        0        0     2396 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/dataset_group.py
+-rw-r--r--   0        0        0     3403 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/dataset_identifier.py
+-rw-r--r--   0        0        0     1535 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/func_adl/__init__.py
+-rw-r--r--   0        0        0     4013 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/func_adl/util.py
+-rw-r--r--   0        0        0    12140 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/func_adl_dataset.py
+-rw-r--r--   0        0        0     4563 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/minio_adapter.py
+-rw-r--r--   0        0        0     5268 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/models.py
+-rw-r--r--   0        0        0     3069 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/python_dataset.py
+-rw-r--r--   0        0        0     4391 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/query_cache.py
+-rw-r--r--   0        0        0     5542 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/servicex_adapter.py
+-rw-r--r--   0        0        0     7598 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/servicex_client.py
+-rw-r--r--   0        0        0     1685 2023-07-13 21:15:11.937733 servicex-3.0.0a3/servicex/types.py
+-rw-r--r--   0        0        0     6314 1970-01-01 00:00:00.000000 servicex-3.0.0a3/setup.py
+-rw-r--r--   0        0        0     6194 1970-01-01 00:00:00.000000 servicex-3.0.0a3/PKG-INFO
```

### Comparing `servicex-3.0.0a2/LICENSE` & `servicex-3.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a2/README.md` & `servicex-3.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a2/pyproject.toml` & `servicex-3.0.0a3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 [tool.poetry]
 name = "servicex"
-version = "3.0.0-alpha.2"
+version = "3.0.0-alpha.3"
 description = ""
-authors = ["Ben Galewsky <bengal1@illinois.edu>", "Gordon Watts <gwatts@uw.edu>"]
+authors = [
+    "Ben Galewsky <bengal1@illinois.edu>",
+    "Gordon Watts <gwatts@uw.edu>",
+]
 readme = "README.md"
-packages = [{include = "servicex_client"}]
+packages = [{ include = "servicex" }]
 
 [tool.poetry.scripts]
-servicex = "servicex_client.app.main:app"
+servicex = "servicex.app.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.8, < 3.12"
 qastle = "^0.16"
-func_adl = "3.2.5"
+func_adl = "^3.2.6"
 requests = "^2.31"
 pydantic = "^1.10"
 httpx = "^0.24"
 miniopy-async = "^1.15"
 tinydb = "^4.7"
 google-auth = "^2.17"
 typer = { extras = ["all"], version = "^0.9.0" }
 PyYAML = "^6.0"
 types-PyYAML = "^6.0"
+make_it_sync = "^1.0.0"
 
-pandas = {version = "^2.0.2", optional = true}
-pyarrow = {version = "^12.0.0", optional = true}
-fastparquet = {version="^2023.4.0", optional = true}
-
-sphinx = {version="^7.0.1", optional = true}
-furo = {version="^2023.5.20", optional = true}
+pandas = { version = "^2.0.2", optional = true }
+pyarrow = { version = "^12.0.0", optional = true }
+fastparquet = { version = "^2023.4.0", optional = true }
+
+sphinx = { version = "^7.0.1", optional = true }
+furo = { version = "^2023.5.20", optional = true }
+jupyter = "^1.0.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
 mypy = "^0.981"
-pytest-asyncio ="^0.21.0"
+pytest-asyncio = "^0.21.0"
 asyncmock = "^0.4.2"
 
 
-
 [tool.poetry.extras]
 pandas = ["pandas", "pyarrow", "fastparquet"]
 docs = ["sphinx", "furo"]
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `servicex-3.0.0a2/servicex_client/__init__.py` & `servicex-3.0.0a3/servicex/app/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a2/servicex_client/app/__init__.py` & `servicex-3.0.0a3/servicex/func_adl/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a2/servicex_client/app/cache.py` & `servicex-3.0.0a3/servicex/app/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import shutil
 
 import rich
 import typer
 from rich.prompt import Confirm
 from rich.table import Table
 
-from servicex_client.servicex_client import ServiceXClient
+from servicex.servicex_client import ServiceXClient
 
 cache_app = typer.Typer(name="cache", no_args_is_help=True)
 
 
 @cache_app.callback()
 def transforms():
     """
@@ -69,14 +69,15 @@
     rich.print(table)
 
 
 @cache_app.command()
 def clear(force: bool = typer.Option(False, "-y", help="Force, don't has permission")):
     if force or Confirm.ask("Really clear cache and delete downloaded files?"):
         sx = ServiceXClient()
+        sx.query_cache.close()
         shutil.rmtree(sx.config.cache_path)
         rich.print("Cache cleared")
 
 
 @cache_app.command(no_args_is_help=True)
 def delete(transform_id: str = typer.Option(None, "-t", "--transform-id", help="Transform ID")):
     sx = ServiceXClient()
```

### Comparing `servicex-3.0.0a2/servicex_client/app/cli_options.py` & `servicex-3.0.0a3/servicex/app/cli_options.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a2/servicex_client/app/main.py` & `servicex-3.0.0a3/servicex/app/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 from typing import Optional
 
 import rich
 import typer
-from servicex_client._version import __version__
-from servicex_client.app.cli_options import url_cli_option, backend_cli_option
-from servicex_client.app.transforms import transforms_app
-from servicex_client.app.cache import cache_app
-from servicex_client.servicex_client import ServiceXClient
+from servicex._version import __version__
+from servicex.app.cli_options import url_cli_option, backend_cli_option
+from servicex.app.transforms import transforms_app
+from servicex.app.cache import cache_app
+from servicex.servicex_client import ServiceXClient
 
 app = typer.Typer(no_args_is_help=True)
 
 app.add_typer(transforms_app)
 app.add_typer(cache_app)
```

### Comparing `servicex-3.0.0a2/servicex_client/app/transforms.py` & `servicex-3.0.0a3/servicex/app/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,58 +30,59 @@
 from typing import Optional, List
 
 import rich
 import typer
 from rich.progress import Progress
 from rich.table import Table
 
-from servicex_client.app.cli_options import url_cli_option, backend_cli_option
-from servicex_client.minio_adpater import MinioAdapter
-from servicex_client.models import Status, ResultFile
-from servicex_client.servicex_client import ServiceXClient
+from servicex.app.cli_options import url_cli_option, backend_cli_option
+from servicex.minio_adapter import MinioAdapter
+from servicex.models import Status, ResultFile
+from servicex.servicex_client import ServiceXClient
 
 transforms_app = typer.Typer(name="transforms", no_args_is_help=True)
 
 
 @transforms_app.callback()
 def transforms():
     """
     sub-commands for creating and manipulating Gardens
     """
     pass
 
 
 @transforms_app.command(no_args_is_help=True)
 def list(
-        url: Optional[str] = url_cli_option,
-        backend: Optional[str] = backend_cli_option,
-        complete: Optional[bool] = typer.Option(
-            None, "--complete", help="Only show successfully completed transforms"
-        )):
+    url: Optional[str] = url_cli_option,
+    backend: Optional[str] = backend_cli_option,
+    complete: Optional[bool] = typer.Option(
+        None, "--complete", help="Only show successfully completed transforms"
+    ),
+):
     sx = ServiceXClient(url=url, backend=backend)
     table = Table(title="ServiceX Transforms")
     table.add_column("Transform ID")
     table.add_column("Title")
     table.add_column("Status")
     table.add_column("Files")
     transforms = sx.get_transforms()
     for t in transforms:
         if not complete or complete and t.status == Status.complete:
-            table.add_row(t.request_id, "Not implemented", t.status,
-                          str(t.files_completed))
+            table.add_row(
+                t.request_id, "Not implemented", t.status, str(t.files_completed)
+            )
 
     rich.print(table)
 
 
 @transforms_app.command(no_args_is_help=True)
 def files(
-        url: Optional[str] = url_cli_option,
-        backend: Optional[str] = backend_cli_option,
-        transform_id: str = typer.Option(None, "-t", "--transform-id",
-                                         help="Transform ID")
+    url: Optional[str] = url_cli_option,
+    backend: Optional[str] = backend_cli_option,
+    transform_id: str = typer.Option(None, "-t", "--transform-id", help="Transform ID"),
 ):
     async def list_files(sx: ServiceXClient, transform_id: str) -> List[ResultFile]:
         transform = await sx.get_transform_status_async(transform_id)
         minio = MinioAdapter.for_transform(transform)
         return await minio.list_bucket()
 
     sx = ServiceXClient(url=url, backend=backend)
@@ -93,37 +94,36 @@
     for f in result_files:
         table.add_row(f.filename, "%.2f" % (f.size / 1e6), f.extension)
     rich.print(table)
 
 
 @transforms_app.command(no_args_is_help=True)
 def download(
-        url: Optional[str] = url_cli_option,
-        backend: Optional[str] = backend_cli_option,
-        transform_id: str = typer.Option(None, "-t", "--transform-id",
-                                         help="Transform ID"),
-        local_dir: str = typer.Option(".", "-d", help="Local dir to download to")
+    url: Optional[str] = url_cli_option,
+    backend: Optional[str] = backend_cli_option,
+    transform_id: str = typer.Option(None, "-t", "--transform-id", help="Transform ID"),
+    local_dir: str = typer.Option(".", "-d", help="Local dir to download to"),
 ):
     async def download_files(sx: ServiceXClient, transform_id: str, local_dir):
         async def download_with_progress(filename) -> Path:
-            p = await minio.download_file(filename,
-                                          local_dir,
-                                          shorten_filename=sx.config.shortened_downloaded_filename)
+            p = await minio.download_file(
+                filename,
+                local_dir,
+                shorten_filename=sx.config.shortened_downloaded_filename,
+            )
             progress.advance(download_progress)
             return p
 
         transform = await sx.get_transform_status_async(transform_id)
         minio = MinioAdapter.for_transform(transform)
         file_list = await minio.list_bucket()
         progress.update(download_progress, total=len(file_list))
         progress.start_task(download_progress)
 
-        tasks = [
-            download_with_progress(f.filename) for f in file_list
-        ]
+        tasks = [download_with_progress(f.filename) for f in file_list]
         return await asyncio.gather(*tasks)
 
     with Progress() as progress:
         download_progress = progress.add_task("Downloading", start=False, total=None)
         sx = ServiceXClient(url=url, backend=backend)
         result_files = asyncio.run(download_files(sx, transform_id, local_dir))
```

### Comparing `servicex-3.0.0a2/servicex_client/configuration.py` & `servicex-3.0.0a3/servicex/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     endpoint: str
     name: str
     token: Optional[str]
 
 
 class Configuration(BaseModel):
     api_endpoints: List[Endpoint]
-    default_endpoint: Optional[str] = Field(alias="default-endpoint")
-    cache_path: Optional[str] = Field(alias="cache-path")
+    default_endpoint: Optional[str] = Field(alias="default-endpoint", default=None)
+    cache_path: Optional[str] = Field(alias="cache-path", default=None)
     shortened_downloaded_filename: Optional[bool] = False
 
     class Config:
         allow_population_by_field_name = True
 
     def endpoint_dict(self) -> Dict[str, Endpoint]:
         return {endpoint.name: endpoint for endpoint in self.api_endpoints}
@@ -56,29 +56,29 @@
     def read(cls, config_path: Optional[str] = None):
         r"""
         Read configuration from .servicex file.
 
         :param config_path: If provided, use this as the path to the .servicex file.
                             Otherwise, search, starting from the current working directory
                             and look in enclosing directories
-        :return: Populated configuraton object
+        :return: Populated configuration object
         """
         if config_path:
             yaml_config = cls._add_from_path(Path(config_path), walk_up_tree=False)
         else:
             yaml_config = cls._add_from_path(walk_up_tree=True)
 
         if yaml_config:
             return Configuration(**yaml_config)
         else:
             path_extra = f"in {config_path}" if config_path else ""
             raise NameError("Can't find .servicex config file " + path_extra)
 
     @classmethod
-    def _add_from_path(cls, path: Path = None, walk_up_tree: bool = False):
+    def _add_from_path(cls, path: Optional[Path] = None, walk_up_tree: bool = False):
         config = None
         if path:
             path.resolve()
             name = path.name
             dir = path.parent.resolve()
         else:
             name = ".servicex"
```

### Comparing `servicex-3.0.0a2/servicex_client/dataset.py` & `servicex-3.0.0a3/servicex/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,54 +25,66 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import abc
 import asyncio
 from abc import ABC
 from asyncio import Task, CancelledError
-from typing import List
+from typing import List, Optional
 
 try:
     import pandas as pd
 except ModuleNotFoundError:
     pass
 
 
-from servicex_client.types import DID
+from servicex.types import DID
 
 try:
     import pandas
 except ModuleNotFoundError:
     pass
 
 import rich
-from rich.progress import Progress, TaskID, TextColumn, BarColumn, MofNCompleteColumn, \
-    TimeRemainingColumn
+from rich.progress import (
+    Progress,
+    TaskID,
+    TextColumn,
+    BarColumn,
+    MofNCompleteColumn,
+    TimeRemainingColumn,
+)
+
+from servicex.configuration import Configuration
+from servicex.minio_adapter import MinioAdapter
+from servicex.models import (
+    TransformRequest,
+    ResultDestination,
+    ResultFormat,
+    Status,
+    TransformedResults,
+)
+from servicex.query_cache import QueryCache
+from servicex.servicex_adapter import ServiceXAdapter
 
-from servicex_client.configuration import Configuration
-from servicex_client.minio_adpater import MinioAdapter
-from servicex_client.models import TransformRequest, ResultDestination, ResultFormat, \
-    Status, TransformedResults
-from servicex_client.query_cache import QueryCache
-from servicex_client.servicex_adapter import ServiceXAdapter
+from make_it_sync import make_sync
 
 
 class Dataset(ABC):
-
     def __init__(
-            self,
-            dataset_identifier: DID = None,
-            title: str = "ServiceX Client",
-            codegen: str = None,
-            sx_adapter: ServiceXAdapter = None,
-            config: Configuration = None,
-            query_cache: QueryCache = None,
-            servicex_polling_interval: int = 10,
-            minio_polling_interval: int = 5,
-            result_format: ResultFormat = None
+        self,
+        dataset_identifier: DID,
+        title: str,
+        codegen: str,
+        sx_adapter: ServiceXAdapter,
+        config: Configuration,
+        query_cache: QueryCache,
+        servicex_polling_interval: int = 10,
+        minio_polling_interval: int = 5,
+        result_format: ResultFormat = ResultFormat.parquet,
     ):
         r"""
         This is the main class for constructing transform requests and receiving the
         results in a format of your choice. It can be run synchronously or asynchronously.
 
         :param dataset_identifier: Either a Rucio DID or a list of files
         :param title: Human readable title for this transform
@@ -113,46 +125,50 @@
     @abc.abstractmethod
     def generate_selection_string(self) -> str:
         pass
 
     @property
     def transform_request(self):
         if not self.result_format:
-            raise ValueError("Unable to determine the result file format. Use set_result_format method")  # NOQA E501
+            raise ValueError(
+                "Unable to determine the result file format. Use set_result_format method"
+            )  # NOQA E501
 
         sx_request = TransformRequest(
             title=self.title,
             codegen=self.codegen,
-            result_destination=ResultDestination.object_store,
-            result_format=self.result_format,
-            selection=self.generate_selection_string()
-        )
+            result_destination=ResultDestination.object_store,  # type: ignore
+            result_format=self.result_format,  # type: ignore
+            selection=self.generate_selection_string(),
+        )  # type: ignore
         # Transfer the DID into the transform request
         self.dataset_identifier.populate_transform_request(sx_request)
         return sx_request
 
     def set_result_format(self, result_format: ResultFormat):
         r"""
         Set the result format - required at constructor time or as part of the query
         chain of methods
         :param result_format:
         :return: self to allow you to chain together query and setup methods
         """
         self.result_format = result_format
         return self
 
-    async def submit_and_download(self, signed_urls_only: bool = False) -> TransformedResults:
+    async def submit_and_download(
+        self, signed_urls_only: bool = False
+    ) -> Optional[TransformedResults]:
         """
         Submit the transform request to ServiceX. Poll the transform status to see when
         the transform completes and to get the number of files in the dataset along with
         current progress and failed file count.
 
         :param signed_urls_only: Set to true to skip actually downloading the files and
                                  just return pre-signed urls
-        :return: Transform results object which contains the list of files downlaoded
+        :return: Transform results object which contains the list of files downloaded
                  or the list of pre-signed urls
         """
         download_files_task = None
         loop = asyncio.get_running_loop()
 
         def transform_complete(task: Task):
             """
@@ -164,70 +180,81 @@
             if task.exception():
                 rich.print("ServiceX Exception", task.exception())
                 if download_files_task:
                     download_files_task.cancel("Transform failed")
                 raise task.exception()
 
             if self.current_status.files_failed:
-                rich.print(f"[bold red]Transforms completed with failures[/bold red] "
-                           f"{self.current_status.files_failed} files failed out of "
-                           f"{self.current_status.files}")
+                rich.print(
+                    f"[bold red]Transforms completed with failures[/bold red] "
+                    f"{self.current_status.files_failed} files failed out of "
+                    f"{self.current_status.files}"
+                )
             else:
                 rich.print("Transforms completed successfully")
 
         sx_request = self.transform_request
 
         # Let's see if this is in the cache already
         cached_record = self.cache.get_transform_by_hash(sx_request.compute_hash())
 
         # And that we grabbed the resulting files in the way that the user requested
         # (Downloaded, or obtained pre-signed URLs)
         if cached_record:
-            if signed_urls_only and cached_record.signed_url_list or \
-                    not signed_urls_only and cached_record.file_list:
+            if (
+                signed_urls_only
+                and cached_record.signed_url_list
+                or not signed_urls_only
+                and cached_record.file_list
+            ):
                 rich.print("Returning results from cache")
                 return cached_record
 
         # If we get here with a cached record, then we know that the transform
         # has been run, but we just didn't get the files from object store in the way
         # requested by user
         with Progress(
-                TextColumn("[progress.description]{task.description}"),
-                BarColumn(),
-                MofNCompleteColumn(),
-                TimeRemainingColumn(compact=True, elapsed_when_finished=True),
+            TextColumn("[progress.description]{task.description}"),
+            BarColumn(),
+            MofNCompleteColumn(),
+            TimeRemainingColumn(compact=True, elapsed_when_finished=True),
         ) as progress:
-
             if not cached_record:
-                transform_progress = progress.add_task("Transform", start=False, total=None)
+                transform_progress = progress.add_task(
+                    "Transform", start=False, total=None
+                )
             else:
                 self.request_id = cached_record.request_id
                 await self.retrieve_current_transform_status()
 
-            minio_progress_bar_title = "Download" \
-                if not signed_urls_only else "Signing URLS"
-
-            download_progress = progress.add_task(minio_progress_bar_title,
-                                                  start=False, total=None)
+            minio_progress_bar_title = (
+                "Download" if not signed_urls_only else "Signing URLS"
+            )
+
+            download_progress = progress.add_task(
+                minio_progress_bar_title, start=False, total=None
+            )
 
             if not cached_record:
                 self.request_id = await self.servicex.submit_transform(sx_request)
 
                 monitor_task = loop.create_task(
-                    self.transform_status_listener(progress,
-                                                   transform_progress,
-                                                   download_progress))
+                    self.transform_status_listener(
+                        progress, transform_progress, download_progress
+                    )
+                )
                 monitor_task.add_done_callback(transform_complete)
             else:
                 self.request_id = cached_record.request_id
 
             download_files_task = loop.create_task(
-                self.download_files(signed_urls_only,
-                                    progress, download_progress,
-                                    cached_record))
+                self.download_files(
+                    signed_urls_only, progress, download_progress, cached_record
+                )
+            )
 
             try:
                 signed_urls = []
                 downloaded_files = []
                 download_result = await download_files_task
                 if signed_urls_only:
                     signed_urls = download_result
@@ -236,28 +263,32 @@
                 else:
                     downloaded_files = download_result
                     if cached_record:
                         cached_record.file_list = download_result
 
                 # Update the cache
                 if not cached_record:
-                    transform_report = self.cache.cache_transform(sx_request,
-                                                                  self.current_status,
-                                                                  self.download_path.as_posix(),
-                                                                  downloaded_files, signed_urls)
+                    transform_report = self.cache.cache_transform(
+                        sx_request,
+                        self.current_status,
+                        self.download_path.as_posix(),
+                        downloaded_files,
+                        signed_urls,
+                    )
                 else:
                     self.cache.update_record(cached_record)
                     transform_report = cached_record
 
                 return transform_report
             except CancelledError:
                 rich.print_json("Aborted file downloads due to transform failure")
 
-    async def transform_status_listener(self, progress: Progress,
-                                        progress_task: TaskID, download_task: TaskID):
+    async def transform_status_listener(
+        self, progress: Progress, progress_task: TaskID, download_task: TaskID
+    ):
         """
         Poll ServiceX for the status of a transform. Update progress bars and keep track
         of status. Once we know the number of files in the dataset, update the progress
         bars.
         """
 
         # Actual number of files in the dataset. We only know this once the DID
@@ -274,15 +305,17 @@
                 final_count = self.current_status.files
                 progress.update(progress_task, total=final_count)
                 progress.start_task(progress_task)
 
                 progress.update(download_task, total=final_count)
                 progress.start_task(download_task)
 
-            progress.update(progress_task, completed=self.current_status.files_completed)
+            progress.update(
+                progress_task, completed=self.current_status.files_completed
+            )
 
             if self.current_status.status == Status.complete:
                 self.files_completed = self.current_status.files_completed
                 self.files_failed = self.current_status.files_failed
                 return
 
             await asyncio.sleep(self.servicex_polling_interval)
@@ -300,40 +333,49 @@
 
         # We can only initialize the minio adapter with data from the transform
         # status. This includes the minio host and credentials. We use the
         # transform id as the bucket.
         if not self.minio:
             self.minio = MinioAdapter.for_transform(self.current_status)
 
-    async def download_files(self, signed_urls_only: bool,
-                             progress: Progress,
-                             download_progress: TaskID,
-                             cached_record: TransformedResults) -> List[str]:
+    async def download_files(
+        self,
+        signed_urls_only: bool,
+        progress: Progress,
+        download_progress: TaskID,
+        cached_record: Optional[TransformedResults],
+    ) -> List[str]:
         """
         Task to monitor the list of files in the transform output's bucket. Any new files
         will be downloaded.
         """
         files_seen = set()
         result_uris = []
         download_tasks = []
         loop = asyncio.get_running_loop()
 
-        async def download_file(minio: MinioAdapter, filename: str,
-                                progress: Progress,
-                                download_progress: TaskID,
-                                shorten_filename: bool = False):
-            downloaded_filename = await minio.download_file(filename,
-                                                            self.download_path,
-                                                            shorten_filename=shorten_filename)
+        async def download_file(
+            minio: MinioAdapter,
+            filename: str,
+            progress: Progress,
+            download_progress: TaskID,
+            shorten_filename: bool = False,
+        ):
+            downloaded_filename = await minio.download_file(
+                filename, self.download_path, shorten_filename=shorten_filename
+            )
             result_uris.append(downloaded_filename.as_posix())
             progress.advance(download_progress)
 
-        async def get_signed_url(minio: MinioAdapter, filename: str,
-                                 progress: Progress,
-                                 download_progress: TaskID):
+        async def get_signed_url(
+            minio: MinioAdapter,
+            filename: str,
+            progress: Progress,
+            download_progress: TaskID,
+        ):
             print(f"get signed url for {filename}")
             url = await minio.get_signed_url(filename)
             result_uris.append(url)
             progress.advance(download_progress)
 
         while True:
             if not cached_record:
@@ -341,68 +383,72 @@
             if self.minio:
                 files = await self.minio.list_bucket()
                 for file in files:
                     if file.filename not in files_seen:
                         if signed_urls_only:
                             download_tasks.append(
                                 loop.create_task(
-                                    get_signed_url(self.minio, file.filename,
-                                                   progress, download_progress))
+                                    get_signed_url(
+                                        self.minio,
+                                        file.filename,
+                                        progress,
+                                        download_progress,
+                                    )
+                                )
                             )
                         else:
                             download_tasks.append(
                                 loop.create_task(
-                                    download_file(self.minio, file.filename,
-                                                  progress, download_progress,
-                                                  shorten_filename=self.configuration.shortened_downloaded_filename))) # NOQA 501
+                                    download_file(
+                                        self.minio,
+                                        file.filename,
+                                        progress,
+                                        download_progress,
+                                        shorten_filename=self.configuration.shortened_downloaded_filename,  # NOQA: E501
+                                    )
+                                )
+                            )  # NOQA 501
                         files_seen.add(file.filename)
 
             # Once the transform is complete we can stop polling since all the files
             # are guaranteed to be in the bucket. Also, if we are just downloading or
             # signing urls for a previous transform then we know it is complete as well
-            if cached_record or \
-                    (self.current_status and self.current_status.status == Status.complete):
+            if cached_record or (
+                self.current_status and self.current_status.status == Status.complete
+            ):
                 break
 
         # Now just wait until all of our tasks complete
         await asyncio.gather(*download_tasks)
         return result_uris
 
     async def as_files_async(self) -> TransformedResults:
         r"""
         Submit the transform and request all the resulting files to be downloaded
         :return: TransformResult instance with the list of complete paths to the downloaded files
         """
         return await self.submit_and_download()
 
-    def as_files(self) -> TransformedResults:
-        r"""
-        Submit the transform and request all the resulting files to be downloaded
-        :return: TransformResult instance with the list of complete paths to the downloaded files
-        """
-        return asyncio.run(self.submit_and_download())
+    as_files = make_sync(as_files_async)
 
     async def as_pandas_async(self):
         r"""
         Return a pandas dataframe containing the results. This only works if you've
         installed pandas extra
 
         :return: Pandas Dataframe
         """
         self.result_format = ResultFormat.parquet
         transformed_result = await self.as_files_async()
-        dataframes = pd.concat([pandas.read_parquet(p) for p in transformed_result.file_list])
+        dataframes = pd.concat(
+            [pandas.read_parquet(p) for p in transformed_result.file_list]
+        )
         return dataframes
 
-    def as_pandas(self):
-        r"""
-        Synchronous version of as_pandas_asynch
-        :return:
-        """
-        return asyncio.run(self.as_pandas_async())
+    as_pandas = make_sync(as_pandas_async)
 
     async def as_signed_urls(self) -> TransformedResults:
         r"""
         Presign URLs for each of the transformed files
 
         :return: TransformedResults object with the presigned_urls list populated
         """
```

### Comparing `servicex-3.0.0a2/servicex_client/dataset_group.py` & `servicex-3.0.0a3/servicex/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,40 +21,34 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-import asyncio
-from typing import Coroutine, List
-
-from servicex_client.models import TransformedResults
-
-
-class DatasetGroup:
-    def __init__(self, datasets: List[Coroutine]):
-        r"""
-        Simultaneously submit a group of transform requests and offer the ability to wait
-        for them all to finish.
-
-        :param datasets: List of transform requests form dataset instances
-        """
-        self.datasets = datasets
-
-    async def gather_results_async(self) -> List[TransformedResults]:
-        r"""
-        Await on all of the transform requests in the group.
-
-        :return: List of TransformedResults instances. Use the title property to relate the
-                 result to your submission
-        """
-        return await asyncio.gather(*self.datasets)
-
-    def gather_results(self) -> List[TransformedResults]:
-        r"""
-        Synchronous wait for all of the transform requests in the group to complete
-
-        :return: List of TransformedResults instances. Use the title property to relate the
-                 result to your submission
-        """
-        return asyncio.run(self.gather_results_async())
+from servicex import dataset
+from servicex import dataset_group
+from servicex import models
+from servicex import servicex_client
+from servicex import dataset_identifier
+
+from .servicex_client import ServiceXClient
+from .dataset import Dataset
+from .models import ResultFormat, ResultDestination
+from .dataset_group import DatasetGroup
+from .dataset_identifier import RucioDatasetIdentifier, FileListDataset
+
+
+__all__ = [
+    "ServiceXClient",
+    "Dataset",
+    "DatasetGroup",
+    "ResultFormat",
+    "ResultDestination",
+    "servicex_client",
+    "dataset",
+    "dataset_group",
+    "models",
+    "dataset_identifier",
+    "RucioDatasetIdentifier",
+    "FileListDataset",
+]
```

### Comparing `servicex-3.0.0a2/servicex_client/dataset_identifier.py` & `servicex-3.0.0a3/servicex/dataset_identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 from typing import List, Union
 
-from servicex_client.models import TransformRequest
+from servicex.models import TransformRequest
 
 
 class DataSetIdentifier:
     r"""
     Base class for specifying the dataset to transform. This can either be a list of
     xRootD URIs or a rucio DID
     """
```

### Comparing `servicex-3.0.0a2/servicex_client/func_adl/__init__.py` & `servicex-3.0.0a3/servicex/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,7 +21,12 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+from typing import Union
+
+from servicex.dataset_identifier import DataSetIdentifier, FileListDataset
+
+DID = Union[DataSetIdentifier, FileListDataset]
```

### Comparing `servicex-3.0.0a2/servicex_client/func_adl/util.py` & `servicex-3.0.0a3/servicex/func_adl/util.py`

 * *Files identical despite different names*

### Comparing `servicex-3.0.0a2/servicex_client/func_adl_dataset.py` & `servicex-3.0.0a3/servicex/func_adl_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,59 +25,83 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 from __future__ import annotations
 
 import ast
 import copy
-from typing import Optional, Any, TypeVar, cast, List, Union, Callable, Iterable, Dict
+from typing import (
+    Optional,
+    Any,
+    Type,
+    TypeVar,
+    cast,
+    List,
+    Union,
+    Callable,
+    Iterable,
+    Dict,
+)
 from pydantic import typing
 from qastle import python_ast_to_text_ast
 
 from func_adl import EventDataset
 from func_adl.object_stream import S
-from servicex_client.configuration import Configuration
-from servicex_client.dataset import Dataset
-from servicex_client.func_adl.util import has_tuple
-from servicex_client.models import ResultFormat
-from servicex_client.query_cache import QueryCache
-from servicex_client.servicex_adapter import ServiceXAdapter
-from servicex_client.types import DID
+from servicex.configuration import Configuration
+from servicex.dataset import Dataset
+from servicex.func_adl.util import has_tuple
+from servicex.models import ResultFormat
+from servicex.query_cache import QueryCache
+from servicex.servicex_adapter import ServiceXAdapter
+from servicex.types import DID
 
 T = TypeVar("T")
 
 
 class FuncADLDataset(Dataset, EventDataset[T]):
     r"""
     ServiceX Dataset class that uses func_adl query syntax.
     """
     # These are methods that are translated locally
     _execute_locally = ["ResultPandasDF", "ResultAwkwardArray"]
 
-    async def execute_result_async(self, a: ast.AST, title: Optional[str] = None) -> Any:
+    async def execute_result_async(
+        self, a: ast.AST, title: Optional[str] = None
+    ) -> Any:
         pass
 
     def check_data_format_request(self, f_name: str):
         pass
 
-    def __init__(self, dataset_identifier: DID,
-                 sx_adapter: ServiceXAdapter = None,
-                 title: str = "ServiceX Client",
-                 codegen: str = None,
-                 config: Configuration = None,
-                 query_cache: QueryCache = None,
-                 result_format: Optional[ResultFormat] = None
-                 ):
-        super().__init__(dataset_identifier=dataset_identifier,
-                         title=title,
-                         codegen=codegen,
-                         sx_adapter=sx_adapter,
-                         config=config,
-                         query_cache=query_cache,
-                         result_format=result_format)
+    def __init__(
+        self,
+        dataset_identifier: DID,
+        sx_adapter: ServiceXAdapter = None,
+        title: str = "ServiceX Client",
+        codegen: str = None,
+        config: Configuration = None,
+        query_cache: QueryCache = None,
+        result_format: Optional[ResultFormat] = None,
+        item_type: Type = Any,
+    ):
+        Dataset.__init__(
+            self,
+            dataset_identifier=dataset_identifier,
+            title=title,
+            codegen=codegen,
+            sx_adapter=sx_adapter,
+            config=config,
+            query_cache=query_cache,
+            result_format=result_format,
+        )
+        EventDataset.__init__(self, item_type=item_type)
+        self.provided_qastle = None
+
+    def set_provided_qastle(self, qastle: str):
+        self.provided_qastle = qastle
 
     def clone_with_new_ast(self, new_ast: ast.AST, new_type: typing.Any):
         """
         Override the method from ObjectStream - We need to be careful because the query
         cache is a tinyDB database that holds an open file pointer. We are not allowed
         to clone an open file handle, so for this property we will copy by reference
         and share it between the clones. Turns out ast class is also picky about copies,
@@ -136,17 +160,22 @@
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
 
         return super().Select(f)
 
     def generate_selection_string(self) -> str:
-        return self.generate_qastle(self.query_ast)
-
-    def Where(self, filter: Union[str, ast.Lambda, Callable[[T], bool]]) -> FuncADLDataset[T]:
+        if self.provided_qastle:
+            return self.provided_qastle
+        else:
+            return self.generate_qastle(self.query_ast)
+
+    def Where(
+        self, filter: Union[str, ast.Lambda, Callable[[T], bool]]
+    ) -> FuncADLDataset[T]:
         r"""
         Filter the object stream, allowing only items for which `filter` evaluates as true through.
 
         Arguments:
 
             filter      A filter lambda that returns True/False.
```

### Comparing `servicex-3.0.0a2/servicex_client/minio_adpater.py` & `servicex-3.0.0a3/servicex/minio_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,83 +28,98 @@
 import os.path
 from hashlib import sha1
 from pathlib import Path
 from typing import List
 
 from miniopy_async import Minio
 
-from servicex_client.models import ResultFile, TransformStatus
+from servicex.models import ResultFile, TransformStatus
 
 
-class MinioAdapter:
-    MAX_PATH_LEN = 32
+def _sanitize_filename(fname: str):
+    "No matter the string given, make it an acceptable filename on all platforms"
+    return fname.replace("*", "_").replace(";", "_").replace(":", "_")
+
 
-    def __init__(self, endpoint_host: str,
-                 secure: bool,
-                 access_key: str,
-                 secret_key: str,
-                 bucket: str):
+class MinioAdapter:
+    # This must be at least 40, the length of the `hash` we are using, or
+    # undefined things will happen.
+    MAX_PATH_LEN = 60
+
+    def __init__(
+        self,
+        endpoint_host: str,
+        secure: bool,
+        access_key: str,
+        secret_key: str,
+        bucket: str,
+    ):
         self.minio = Minio(
-            endpoint_host,
-            access_key=access_key,
-            secret_key=secret_key,
-            secure=secure
+            endpoint_host, access_key=access_key, secret_key=secret_key, secure=secure
         )
 
         self.bucket = bucket
 
     @classmethod
     def for_transform(cls, transform: TransformStatus):
         return MinioAdapter(
             endpoint_host=transform.minio_endpoint,
             secure=transform.minio_secured,
             access_key=transform.minio_access_key,
             secret_key=transform.minio_secret_key,
-            bucket=transform.request_id
+            bucket=transform.request_id,
         )
 
     async def list_bucket(self) -> List[ResultFile]:
         objects = await self.minio.list_objects(self.bucket)
-        return [ResultFile(
-            filename=obj.object_name,
-            size=obj.size,
-            extension=obj.object_name.split(".")[-1]
-        ) for obj in objects]
-
-    async def download_file(self, object_name: str,
-                            local_dir: str,
-                            shorten_filename: bool = False) -> Path:
+        return [
+            ResultFile(
+                filename=obj.object_name,
+                size=obj.size,
+                extension=obj.object_name.split(".")[-1],
+            )
+            for obj in objects
+        ]
+
+    async def download_file(
+        self, object_name: str, local_dir: str, shorten_filename: bool = False
+    ) -> Path:
         os.makedirs(local_dir, exist_ok=True)
-        path = Path(os.path.join(local_dir,
-                                 self.hash_path(object_name) if shorten_filename else object_name))
+        path = Path(
+            os.path.join(
+                local_dir,
+                _sanitize_filename(
+                    self.hash_path(object_name) if shorten_filename else object_name,
+                ),
+            )
+        )
 
         _ = await self.minio.fget_object(
-            bucket_name=self.bucket,
-            object_name=object_name,
-            file_path=path.as_posix()
+            bucket_name=self.bucket, object_name=object_name, file_path=path.as_posix()
         )
         return path.resolve()
 
     async def get_signed_url(self, object_name: str) -> str:
         return await self.minio.get_presigned_url(
-            bucket_name=self.bucket,
-            object_name=object_name,
-            method="GET"
+            bucket_name=self.bucket, object_name=object_name, method="GET"
         )
 
     @classmethod
     def hash_path(cls, file_name):
         """
         Make the path safe for object store or POSIX, by keeping the length
         less than MAX_PATH_LEN. Replace the leading (less interesting) characters with a
         forty character hash.
         :param file_name: Input filename
         :return: Safe path string
         """
         if len(file_name) > cls.MAX_PATH_LEN:
-            hash = sha1(file_name.encode('utf-8')).hexdigest()
-            return ''.join([
-                '_', hash,
-                file_name[-1 * (cls.MAX_PATH_LEN - len(hash) - 1):],
-            ])
+            hash = sha1(file_name.encode("utf-8")).hexdigest()
+            return "".join(
+                [
+                    "_",
+                    hash,
+                    file_name[-1 * (cls.MAX_PATH_LEN - len(hash) - 1) :],  # noqa: E203
+                ]
+            )
         else:
             return file_name
```

### Comparing `servicex-3.0.0a2/servicex_client/models.py` & `servicex-3.0.0a3/servicex/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,65 +33,74 @@
 from typing import List, Optional
 
 
 class ResultDestination(str, Enum):
     r"""
     Direct the output to object store or posix volume
     """
-    object_store = 'object-store'
-    volume = 'volume'
+    object_store = "object-store"
+    volume = "volume"
 
 
 class ResultFormat(str, Enum):
     r"""
     Specify the file format for the generated output
     """
-    parquet = "parquet",
+    parquet = ("parquet",)
     root_file = "root-file"
 
 
 class Status(str, Enum):
     r"""
-    Status of a sumbittied transform
+    Status of a submitted transform
     """
-    complete = "Complete",
-    fatal = "Fatal",
-    canceled = "Canceled",
-    submitted = "Submitted",
+    complete = ("Complete",)
+    fatal = ("Fatal",)
+    canceled = ("Canceled",)
+    submitted = ("Submitted",)
     running = "Running"
 
 
 class TransformRequest(BaseModel):
     r"""
     Transform request sent to ServiceX
     """
     title: Optional[str] = None
     did: Optional[str] = None
-    file_list: Optional[List[str]] = Field(None, alias='file-list')
+    file_list: Optional[List[str]] = Field(default=None, alias="file-list")
     selection: str
     image: Optional[str] = None
     codegen: str
-    tree_name: Optional[str] = Field(None, alias='tree-name')
+    tree_name: Optional[str] = Field(default=None, alias="tree-name")
     result_destination: ResultDestination = Field(alias="result-destination")
     result_format: ResultFormat = Field(alias="result-format")
 
     class Config:
         allow_population_by_field_name = True
 
     def compute_hash(self):
         r"""
-        Compute a hash for this submission. Only include properties that imapact the result
+        Compute a hash for this submission. Only include properties that impact the result
         so we have maximal ability to reuse transforms
 
         :return: SHA256 hash of request
         """
-        sha = hashlib.sha256(str([self.did, self.selection, self.tree_name,
-                                  self.codegen, self.image,
-                                  self.result_format.name, self.file_list]).
-                             encode("utf-8"))
+        sha = hashlib.sha256(
+            str(
+                [
+                    self.did,
+                    self.selection,
+                    self.tree_name,
+                    self.codegen,
+                    self.image,
+                    self.result_format.name,
+                    self.file_list,
+                ]
+            ).encode("utf-8")
+        )
         return sha.hexdigest()
 
 
 class TransformStatus(BaseModel):
     r"""
     Status object returned by servicex
     """
@@ -122,15 +131,15 @@
         if isinstance(v, str) and v == "None":
             return None
         return v
 
 
 class ResultFile(BaseModel):
     r"""
-    Record reporting the properties of a tranformed file result
+    Record reporting the properties of a transformed file result
     """
     filename: str
     size: int
     extension: str
 
 
 class TransformedResults(BaseModel):
```

### Comparing `servicex-3.0.0a2/servicex_client/python_dataset.py` & `servicex-3.0.0a3/servicex/python_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import inspect
 import typing
 from base64 import b64encode
 
-from servicex_client.configuration import Configuration
-from servicex_client.dataset import Dataset
-from servicex_client.models import ResultFormat
-from servicex_client.query_cache import QueryCache
-from servicex_client.servicex_adapter import ServiceXAdapter
-from servicex_client.types import DID
+from servicex.configuration import Configuration
+from servicex.dataset import Dataset
+from servicex.models import ResultFormat
+from servicex.query_cache import QueryCache
+from servicex.servicex_adapter import ServiceXAdapter
+from servicex.types import DID
 
 
 class PythonDataset(Dataset):
 
     def __init__(self, dataset_identifier: DID,
                  sx_adapter: ServiceXAdapter = None,
                  title: str = "ServiceX Client",
```

### Comparing `servicex-3.0.0a2/servicex_client/query_cache.py` & `servicex-3.0.0a3/servicex/query_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 import json
 import os
 from pathlib import Path
 from typing import List, Optional
 
 from tinydb import TinyDB, Query, where
 
-from servicex_client.configuration import Configuration
-from servicex_client.models import TransformRequest, TransformStatus, TransformedResults
+from servicex.configuration import Configuration
+from servicex.models import TransformRequest, TransformStatus, TransformedResults
 
 
 class CacheException(Exception):
     pass
 
 
 class QueryCache:
```

### Comparing `servicex-3.0.0a2/servicex_client/servicex_adapter.py` & `servicex-3.0.0a3/servicex/servicex_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import os
 from datetime import datetime
 from typing import Optional, Dict, List
 
 import httpx
 from google.auth import jwt
 
-from servicex_client.models import TransformRequest, TransformStatus
+from servicex.models import TransformRequest, TransformStatus
 
 
 class AuthorizationError(BaseException):
     pass
 
 
 class ServiceXAdapter:
@@ -105,14 +105,16 @@
             r = await client.post(url=f"{self.url}/servicex/transformation",
                                   headers=headers,
                                   json=transform_request.dict(by_alias=True,
                                                               exclude_none=True))
             if r.status_code == 401:
                 raise AuthorizationError(
                     f"Not authorized to access serviceX at {self.url}")
+            elif r.status_code == 400:
+                raise ValueError(f"Invalid transform request: {r.json()['message']}")
         return r.json()['request_id']
 
     async def get_transform_status(self, request_id: str) -> TransformStatus:
         async with httpx.AsyncClient() as client:
             headers = await self._get_authorization(client)
             r = await client.get(url=f"{self.url}/servicex/transformation/{request_id}",
                                  headers=headers)
```

### Comparing `servicex-3.0.0a2/servicex_client/servicex_client.py` & `servicex-3.0.0a3/servicex/servicex_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,43 +21,47 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-import asyncio
-from typing import Optional, List
+from typing import Optional, List, TypeVar, Any, Type
 
-from servicex_client.configuration import Configuration
-from servicex_client.func_adl_dataset import FuncADLDataset
-from servicex_client.models import ResultFormat, TransformStatus
-from servicex_client.query_cache import QueryCache
-from servicex_client.servicex_adapter import ServiceXAdapter
-from servicex_client.types import DID
-from servicex_client.python_dataset import PythonDataset
+from servicex.configuration import Configuration
+from servicex.func_adl_dataset import FuncADLDataset
+from servicex.models import ResultFormat, TransformStatus
+from servicex.query_cache import QueryCache
+from servicex.servicex_adapter import ServiceXAdapter
+from servicex.types import DID
+from servicex.python_dataset import PythonDataset
+
+from make_it_sync import make_sync
+
+
+T = TypeVar("T")
 
 
 class ServiceXClient:
     r"""
-        Connection to a ServiceX deployment. Instances of this class can deployment
-        data from the service and also interact with previously run transformations.
-        Instances of this class are factories for `Datasets``
+    Connection to a ServiceX deployment. Instances of this class can deployment
+    data from the service and also interact with previously run transformations.
+    Instances of this class are factories for `Datasets``
     """
 
     def __init__(self, backend=None, url=None, config_path=None):
         r"""
         If both `backend` and `url` are unspecified then it will attempt to pick up
         the default backend from `.servicex`
 
         :param backend: Name of a deployment from the .servicex file
         :param url: Direct URL of a serviceX deployment instead of using .servicex.
                     Can only work with hosts without auth, or the token is found
                     in a file pointed to by the environment variable BEARER_TOKEN_FILE
-        :param config_path: Optional path te the `.servicex` file. If not specificed,
+        :param config_path: Optional path te the `.servicex` file. If not specified,
                     will search in local directory and up in enclosing directories
         """
         self.config = Configuration.read(config_path)
         self.endpoints = self.config.endpoint_dict()
 
         if not url and not backend:
             backend = self.config.default_endpoint
@@ -66,92 +70,94 @@
             raise ValueError("Only specify backend or url... not both")
 
         if url:
             self.servicex = ServiceXAdapter(url)
         elif backend:
             if backend not in self.endpoints:
                 raise ValueError(f"Backend {backend} not defined in .servicex file")
-            self.servicex = ServiceXAdapter(self.endpoints[backend].endpoint,
-                                            refresh_token=self.endpoints[backend].token)
+            self.servicex = ServiceXAdapter(
+                self.endpoints[backend].endpoint,
+                refresh_token=self.endpoints[backend].token,
+            )
 
         self.query_cache = QueryCache(self.config)
 
         # Cache available code generators
         # @todo allow complete offline use
         self.code_generators = set(self.get_code_generators().keys())
 
     async def get_transforms_async(self) -> List[TransformStatus]:
         r"""
         Retrieve all transforms you have run on the server
         :return: List of Transform status objects
         """
         return await self.servicex.get_transforms()
 
-    def get_transforms(self) -> List[TransformStatus]:
-        r"""
-        Retrieve all transforms you have run on the server
-        :return: List of Transform status objects
-        """
-        return asyncio.run(self.servicex.get_transforms())
-
-    def get_transform_status(self, transform_id) -> TransformStatus:
-        r"""
-        Get the status of a given transform
-        :param transform_id: The uuid of the transform
-        :return: The current status for the transform
-        """
-        return asyncio.run(self.servicex.get_transform_status(request_id=transform_id))
+    get_transforms = make_sync(get_transforms_async)
 
     async def get_transform_status_async(self, transform_id) -> TransformStatus:
         r"""
         Get the status of a given transform
         :param transform_id: The uuid of the transform
         :return: The current status for the transform
         """
         return await self.servicex.get_transform_status(request_id=transform_id)
 
+    get_transform_status = make_sync(get_transform_status_async)
+
     def get_code_generators(self):
         r"""
         Retrieve the code generators deployed with the serviceX instance
         :return:  The list of code generators as json dictionary
         """
         return self.servicex.get_code_generators()
 
-    def func_adl_dataset(self,
-                         dataset_identifier: DID,
-                         title: str = "ServiceX Client",
-                         codegen: str = "uproot",
-                         result_format: Optional[ResultFormat] = None
-                         ) -> FuncADLDataset:
+    def func_adl_dataset(
+        self,
+        dataset_identifier: DID,
+        title: str = "ServiceX Client",
+        codegen: str = "uproot",
+        result_format: Optional[ResultFormat] = None,
+        item_type: Type[T] = Any,
+    ) -> FuncADLDataset[T]:
         r"""
         Generate a dataset that can use func_adl query language
 
         :param dataset_identifier:  The dataset identifier or filelist to be the source of files
         :param title: Title to be applied to the transform. This is also useful for
                       relating transform results.
         :param codegen: Name of the code generator to use with this transform
         :param result_format:  Do you want Paqrquet or Root? This can be set later with
                                the set_result_format method
         :return: A func_adl dataset ready to accept query statements.
         """
         if codegen not in self.code_generators:
             raise NameError(
                 f"{codegen} code generator not supported by serviceX "
-                f"deployment at {self.servicex.url}")
+                f"deployment at {self.servicex.url}"
+            )
 
-        return FuncADLDataset(dataset_identifier, sx_adapter=self.servicex,
-                              title=title, codegen=codegen, config=self.config,
-                              query_cache=self.query_cache, result_format=result_format)
-
-    def python_dataset(self,
-                       dataset_identifier: DID,
-                       title: str = "ServiceX Client",
-                       codegen: str = "uproot",
-                       result_format: Optional[ResultFormat] = None
-                       ) -> PythonDataset:
+        return FuncADLDataset(
+            dataset_identifier,
+            sx_adapter=self.servicex,
+            title=title,
+            codegen=codegen,
+            config=self.config,
+            query_cache=self.query_cache,
+            result_format=result_format,
+            item_type=item_type,
+        )
+
+    def python_dataset(
+        self,
+        dataset_identifier: DID,
+        title: str = "ServiceX Client",
+        codegen: str = "uproot",
+        result_format: Optional[ResultFormat] = None,
+    ) -> PythonDataset:
         r"""
         Generate a dataset that can use accept a python function for the  query
 
         :param dataset_identifier:  The dataset identifier or filelist to be the source of files
         :param title: Title to be applied to the transform. This is also useful for
                       relating transform results.
         :param codegen: Name of the code generator to use with this transform
@@ -160,12 +166,19 @@
         :return: A func_adl dataset ready to accept a python function statements.
 
         """
 
         if codegen not in self.code_generators:
             raise NameError(
                 f"{codegen} code generator not supported by serviceX "
-                f"deployment at {self.servicex.url}")
+                f"deployment at {self.servicex.url}"
+            )
 
-        return PythonDataset(dataset_identifier, sx_adapter=self.servicex,
-                             title=title, codegen=codegen, config=self.config,
-                             query_cache=self.query_cache, result_format=result_format)
+        return PythonDataset(
+            dataset_identifier,
+            sx_adapter=self.servicex,
+            title=title,
+            codegen=codegen,
+            config=self.config,
+            query_cache=self.query_cache,
+            result_format=result_format,
+        )
```

### Comparing `servicex-3.0.0a2/setup.py` & `servicex-3.0.0a3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['servicex_client', 'servicex_client.app', 'servicex_client.func_adl']
+['servicex', 'servicex.app', 'servicex.func_adl']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
- 'func_adl==3.2.5',
+ 'func_adl>=3.2.6,<4.0.0',
  'google-auth>=2.17,<3.0',
  'httpx>=0.24,<0.25',
+ 'jupyter>=1.0.0,<2.0.0',
+ 'make_it_sync>=1.0.0,<2.0.0',
  'miniopy-async>=1.15,<2.0',
  'pydantic>=1.10,<2.0',
  'qastle>=0.16,<0.17',
  'requests>=2.31,<3.0',
  'tinydb>=4.7,<5.0',
  'typer[all]>=0.9.0,<0.10.0',
  'types-PyYAML>=6.0,<7.0']
@@ -23,19 +25,19 @@
 extras_require = \
 {'docs': ['sphinx>=7.0.1,<8.0.0', 'furo>=2023.5.20,<2024.0.0'],
  'pandas': ['pandas>=2.0.2,<3.0.0',
             'pyarrow>=12.0.0,<13.0.0',
             'fastparquet>=2023.4.0,<2024.0.0']}
 
 entry_points = \
-{'console_scripts': ['servicex = servicex_client.app.main:app']}
+{'console_scripts': ['servicex = servicex.app.main:app']}
 
 setup_kwargs = {
     'name': 'servicex',
-    'version': '3.0.0a2',
+    'version': '3.0.0a3',
     'description': '',
     'long_description': "# servicex_client\nPython SDK and CLI Client for ServiceX\n\n## Configuration\nThe client relies on a YAML file to obtain the URLs of different servicex\ndeployments, as well as tokens to authenticate with the service. The file \nshould be named `.servicex` and the format of this file is as follows:\n```yaml\napi_endpoints:\n  - endpoint: http://localhost:5000\n    name: localhost\n\n  - endpoint: https://servicex-release-testing-4.servicex.ssl-hep.org\n    name: testing4\n    token: ...\n\ndefault_endpoint: testing4\n\ncache_path: /tmp/ServiceX_Client/cache-dir\nshortened_downloaded_filename: true\n\n```\nThe `default_endpoint` will be used if otherwise not specified. The cache \ndatabase and downloaded files will be stored in the directory specified by \n`cache_path`.\n\nThe `shortened_downloaded_filename` property controls whether downloaded files\nwill have their names shortened for convenience. Setting to false preserves\nthe full filename from the dataset.\n`\n\nThe library will search for this file in the current working directory and then\nstart looking in parent directories until a file is found.\n\n## Command Line Interface\nWhen installed, the client provides a new command in your shell, `servicex`.\nThis command uses a series of subcommands to work with various functions of\nserviceX.\n\nCommon command line arguments:\n\n| Flag | Long Flag | What it does                                         |\n|------|-----------|------------------------------------------------------|\n| -u   | --url     | The url of the serviceX ingress                      |\n| -b   | --backend | Named backend from the .servicex file endpoints list |\n\nIf neither url nor backend are specified then the client will attempt to use the\n`default_endpoint` value to determine who to talk to.\n\n### codegens \nThis command will list the code generators deployed.\n\n### transforms\nThese commands interact with transforms that have been run\n\n#### list\nList transforms associated with the current user. Add the `--complete` flag to\nonly show transforms that have completed.\n\n#### files\nList the files along with their size generated by a transform. Specify the \ntransform request id with the `-t` or `--transform-id` flag\n\n#### download\nDownload the files from a transform to a local directory. Specify the transform\nrequest id with `-t` and the directory to download to with `-d`. Defaults to\ndownloading files to the current working directory.\n\n### cache\nThese commands allow you to work with the query cache maintained by the serviceX\nclient.\n\n#### list\nShow all of the cached transforms along with the run time, code generator, and \nnumber of resulting files\n\n#### delete\nDelete a specific transform from the cache. Provide the transform request ID \nwith the `-t` or `--transform-id` arg.\n\n#### clear\nClear all of the transforms from the cache. Add `-y` to force the operation \nwithout confirming with the console.\n\n## Python SDK\nEntry to the SDK starts with constructing an instance of ServiceXClient.  The \nconstructor accepts `backend` argument to specify a named backend from the\n`.servicex` file, or `url` for the direct URL to a serviceX server. With the \nURL option you can't provide a token from `.servicex` so it must either be an\nunsecured endpoint, or the token must be provided via the WLCG standard of a \nfile pointed to by `BEARER_TOKEN_FILE` environment variable.\n\nWith an instance of ServiceXClient you can \n- List the code generators deployed with the ServiceX instance\n- List the transformers that have been run\n- Get the current status of a specific transform\n\n### Create a Dataset Instance to Run Transforms\nThe ServiceX client also can create a `Dataset` instance that \nallows you to specify a query, provide a dataset identifier,\nand retrieve the results of the resulting transform request.\n\nThere are two types of datasets\n- func_adl_dataset\n- Python Function dataset\n\n### Dataset Identifiers\nBefore we get too deeply into the dataset classes, we should look\nat how to specify a dataset.\n- RucioDatasetIdentifier - for retrieving data files registered with Rucio\n- FileListDataset - A list of URIs for accessing files using xRootd\n\n### FuncADL Dataset\nThis dataset is controlled by the func_adl language. The dataset\nsupports the `Select`, `SelectMany`, `Where`, `MetaData`, and `QMetaData` \noperators from func_adl.\n\n\n### Datasets\nThis is the abstract class for requesting data from ServiceX. You have to \nspecify the dataset identifier you want data from and provide some sort of \nselection query. You can set the result format with the `set_result_format` \noperator (it's also a factory method arg for the dataset).\n\nOperators that cause the client to interact with the server: These terminal \noperators will call out to the serviceX server and process results. They\nare all implemented as asynchronous coroutines, but they also come with \nsynchronous versions to make it easy to do easy things.\n\n\n#### \n\n",
     'author': 'Ben Galewsky',
     'author_email': 'bengal1@illinois.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `servicex-3.0.0a2/PKG-INFO` & `servicex-3.0.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: servicex
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: 
 Author: Ben Galewsky
 Author-email: bengal1@illinois.edu
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Provides-Extra: pandas
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: fastparquet (>=2023.4.0,<2024.0.0); extra == "pandas"
-Requires-Dist: func_adl (==3.2.5)
+Requires-Dist: func_adl (>=3.2.6,<4.0.0)
 Requires-Dist: furo (>=2023.5.20,<2024.0.0); extra == "docs"
 Requires-Dist: google-auth (>=2.17,<3.0)
 Requires-Dist: httpx (>=0.24,<0.25)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: make_it_sync (>=1.0.0,<2.0.0)
 Requires-Dist: miniopy-async (>=1.15,<2.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0); extra == "pandas"
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0); extra == "pandas"
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: qastle (>=0.16,<0.17)
 Requires-Dist: requests (>=2.31,<3.0)
 Requires-Dist: sphinx (>=7.0.1,<8.0.0); extra == "docs"
```

