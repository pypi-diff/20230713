# Comparing `tmp/investigraph-0.0.4.tar.gz` & `tmp/investigraph-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investigraph-0.0.4.tar", max compression
+gzip compressed data, was "investigraph-0.1.0.tar", max compression
```

## Comparing `investigraph-0.0.4.tar` & `investigraph-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1077 2023-05-31 13:25:47.750897 investigraph-0.0.4/LICENSE
--rw-r--r--   0        0        0     2010 2023-06-14 10:56:42.758881 investigraph-0.0.4/README.md
--rw-r--r--   0        0        0       22 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/__init__.py
--rw-r--r--   0        0        0     2140 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/cache.py
--rw-r--r--   0        0        0     3598 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/catalog.py
--rw-r--r--   0        0        0     4429 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/cli.py
--rw-r--r--   0        0        0       88 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/exceptions.py
--rw-r--r--   0        0        0     2008 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/inspect.py
--rw-r--r--   0        0        0     1620 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/logging.py
--rw-r--r--   0        0        0        0 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/logic/__init__.py
--rw-r--r--   0        0        0     2038 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/logic/aggregate.py
--rw-r--r--   0        0        0     2068 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/logic/extract.py
--rw-r--r--   0        0        0     1205 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/logic/fetch.py
--rw-r--r--   0        0        0     1628 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/logic/load.py
--rw-r--r--   0        0        0      642 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/logic/transform.py
--rw-r--r--   0        0        0      244 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/model/__init__.py
--rw-r--r--   0        0        0     3464 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/model/block.py
--rw-r--r--   0        0        0     3179 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/model/config.py
--rw-r--r--   0        0        0     1858 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/model/context.py
--rw-r--r--   0        0        0     1135 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/model/flow.py
--rw-r--r--   0        0        0     2873 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/model/source.py
--rw-r--r--   0        0        0     3301 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/pipeline.py
--rw-r--r--   0        0        0      865 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/settings.py
--rw-r--r--   0        0        0      388 2023-06-14 09:53:12.989488 investigraph-0.0.4/investigraph/types.py
--rw-r--r--   0        0        0     1923 2023-06-14 09:53:12.993488 investigraph-0.0.4/investigraph/util.py
--rw-r--r--   0        0        0     1461 2023-06-14 10:55:12.698957 investigraph-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 investigraph-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 13:25:47.750897 investigraph-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3633 2023-07-13 13:59:11.347412 investigraph-0.1.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-13 16:24:30.134594 investigraph-0.1.0/investigraph/__init__.py
+-rw-r--r--   0        0        0     2141 2023-06-14 21:43:38.973865 investigraph-0.1.0/investigraph/cache.py
+-rw-r--r--   0        0        0     3593 2023-06-14 13:34:12.810415 investigraph-0.1.0/investigraph/catalog.py
+-rw-r--r--   0        0        0     4576 2023-07-13 16:23:45.930728 investigraph-0.1.0/investigraph/cli.py
+-rw-r--r--   0        0        0       88 2023-06-14 09:53:12.989488 investigraph-0.1.0/investigraph/exceptions.py
+-rw-r--r--   0        0        0     2461 2023-07-13 11:35:56.367709 investigraph-0.1.0/investigraph/inspect.py
+-rw-r--r--   0        0        0     1665 2023-06-14 21:44:45.663238 investigraph-0.1.0/investigraph/logging.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:53:12.989488 investigraph-0.1.0/investigraph/logic/__init__.py
+-rw-r--r--   0        0        0     2050 2023-07-13 10:07:23.566092 investigraph-0.1.0/investigraph/logic/aggregate.py
+-rw-r--r--   0        0        0     2471 2023-07-13 11:35:25.231677 investigraph-0.1.0/investigraph/logic/extract.py
+-rw-r--r--   0        0        0     1190 2023-06-21 13:03:20.008058 investigraph-0.1.0/investigraph/logic/fetch.py
+-rw-r--r--   0        0        0     1946 2023-07-13 10:07:14.670071 investigraph-0.1.0/investigraph/logic/load.py
+-rw-r--r--   0        0        0     1026 2023-07-13 10:07:14.670071 investigraph-0.1.0/investigraph/logic/transform.py
+-rw-r--r--   0        0        0      366 2023-06-14 21:42:52.836915 investigraph-0.1.0/investigraph/model/__init__.py
+-rw-r--r--   0        0        0     3401 2023-07-13 10:15:09.994990 investigraph-0.1.0/investigraph/model/block.py
+-rw-r--r--   0        0        0     3034 2023-07-13 11:15:04.814247 investigraph-0.1.0/investigraph/model/config.py
+-rw-r--r--   0        0        0     2831 2023-07-13 10:07:29.606107 investigraph-0.1.0/investigraph/model/context.py
+-rw-r--r--   0        0        0     2258 2023-07-13 13:59:11.347412 investigraph-0.1.0/investigraph/model/flow.py
+-rw-r--r--   0        0        0     3177 2023-07-13 10:07:29.398106 investigraph-0.1.0/investigraph/model/source.py
+-rw-r--r--   0        0        0     2379 2023-07-13 11:15:56.038321 investigraph-0.1.0/investigraph/model/stage.py
+-rw-r--r--   0        0        0     3719 2023-07-13 16:23:45.090731 investigraph-0.1.0/investigraph/pipeline.py
+-rw-r--r--   0        0        0     1139 2023-07-13 11:34:39.727630 investigraph-0.1.0/investigraph/settings.py
+-rw-r--r--   0        0        0      440 2023-07-13 10:06:53.830020 investigraph-0.1.0/investigraph/types.py
+-rw-r--r--   0        0        0     1674 2023-07-13 10:49:14.240553 investigraph-0.1.0/investigraph/util.py
+-rw-r--r--   0        0        0     1708 2023-07-13 16:55:31.211980 investigraph-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5414 1970-01-01 00:00:00.000000 investigraph-0.1.0/PKG-INFO
```

### Comparing `investigraph-0.0.4/LICENSE` & `investigraph-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `investigraph-0.0.4/README.md` & `investigraph-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![investigraph on pypi](https://img.shields.io/pypi/v/investigraph)](https://pypi.org/project/investigraph/) [![Python test and package](https://github.com/investigativedata/investigraph-etl/actions/workflows/python.yml/badge.svg)](https://github.com/investigativedata/investigraph-etl/actions/workflows/python.yml) [![Build docker container](https://github.com/investigativedata/investigraph-etl/actions/workflows/build-docker.yml/badge.svg)](https://github.com/investigativedata/investigraph-etl/actions/workflows/build-docker.yml) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![Coverage Status](https://coveralls.io/repos/github/investigativedata/investigraph-etl/badge.svg?branch=main)](https://coveralls.io/github/investigativedata/investigraph-etl?branch=main) [![MIT License](https://img.shields.io/pypi/l/investigraph)](./LICENSE)
+
 # investigraph
 
 **Research and implementation of an ETL process for a curated and up-to-date public and open-source data catalog of frequently used datasets in investigative journalism.**
 
 Using [prefect.io](https://www.prefect.io/) for ftm pipeline processing
 
 [Documentation](https://investigativedata.github.io/investigraph/)
@@ -20,47 +22,64 @@
 
 ### docker
 
 `docker-compose.yml` for local development / testing, use `docker-compose.prod.yml` as a starting point for a production setup. [More instructions here](https://investigativedata.github.io/investigraph/deployment/)
 
 ## run locally
 
-Clone repo first.
-
 Install app and dependencies (use a virtualenv):
 
-    pip install -e .
+    pip install investigraph
+
+Or, e.g. when using [poetry](https://python-poetry.org/):
+
+    poetry add investigraph
 
 After installation, `investigraph` as a command should be available:
 
     investigraph --help
 
 Quick run a local dataset definition:
 
-    investigraph run <dataset_name> -c ./path/to/config.yml
+    investigraph run -c ./path/to/config.yml
 
 Register a local datasets block:
 
     investigraph add-block -b local-file-system/investigraph-local -u ./datasets
 
 Register github datasets block:
 
     investigraph add-block -b github/investigraph-datasets -u https://github.com/investigativedata/investigraph-datasets.git
 
 Run a dataset pipeline from a dataset defined in a registered block:
 
-    investigraph run ec_meetings
+    investigraph run -d ec_meetings -b github/investigraph-datasets
 
 View prefect dashboard:
 
     make server
 
-## test
+## development
+
+This package is using [poetry](https://python-poetry.org/) for packaging and dependencies management, so first [install it](https://python-poetry.org/docs/#installation).
+
+Clone investigraph repository to a local destination.
+
+Within the root directory, run
+
+    poetry install --with dev
+
+This installs a few development dependencies, including [pre-commit](https://pre-commit.com/) which needs to be registered:
+
+    poetry run pre-commit install
+
+Before creating a commit, this checks for correct code formatting (isort, black) and some other useful stuff (see: `.pre-commit-config.yaml`)
+
+### test
 
-    make install
     make test
 
 ## supported by
 
 [Media Tech Lab Bayern batch #3](https://github.com/media-tech-lab)
 
 <a href="https://www.media-lab.de/en/programs/media-tech-lab">
```

#### html2text {}

```diff
@@ -1,24 +1,46 @@
-# investigraph **Research and implementation of an ETL process for a curated
-and up-to-date public and open-source data catalog of frequently used datasets
-in investigative journalism.** Using [prefect.io](https://www.prefect.io/) for
-ftm pipeline processing [Documentation](https://investigativedata.github.io/
-investigraph/) [Tutorial](https://investigativedata.github.io/investigraph/
-tutorial/) ## installation pip install investigraph ## example datasets There
-is a dedicated [repo](https://github.com/investigativedata/investigraph-
-datasets) for example datasets that can be used as a [Block](https://
-docs.prefect.io/2.10.11/concepts/blocks/) within the prefect.io deployment. ##
-deployment ### docker `docker-compose.yml` for local development / testing, use
-`docker-compose.prod.yml` as a starting point for a production setup. [More
-instructions here](https://investigativedata.github.io/investigraph/deployment/
-) ## run locally Clone repo first. Install app and dependencies (use a
-virtualenv): pip install -e . After installation, `investigraph` as a command
-should be available: investigraph --help Quick run a local dataset definition:
-investigraph run  -c ./path/to/config.yml Register a local datasets block:
-investigraph add-block -b local-file-system/investigraph-local -u ./datasets
-Register github datasets block: investigraph add-block -b github/investigraph-
-datasets -u https://github.com/investigativedata/investigraph-datasets.git Run
-a dataset pipeline from a dataset defined in a registered block: investigraph
-run ec_meetings View prefect dashboard: make server ## test make install make
-test ## supported by [Media Tech Lab Bayern batch #3](https://github.com/media-
-tech-lab) [https://raw.githubusercontent.com/media-tech-lab/.github/main/
-assets/mtl-powered-by.png]
+[![investigraph on pypi](https://img.shields.io/pypi/v/investigraph)](https://
+pypi.org/project/investigraph/) [![Python test and package](https://github.com/
+investigativedata/investigraph-etl/actions/workflows/python.yml/badge.svg)]
+(https://github.com/investigativedata/investigraph-etl/actions/workflows/
+python.yml) [![Build docker container](https://github.com/investigativedata/
+investigraph-etl/actions/workflows/build-docker.yml/badge.svg)](https://
+github.com/investigativedata/investigraph-etl/actions/workflows/build-
+docker.yml) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-
+brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [!
+[Coverage Status](https://coveralls.io/repos/github/investigativedata/
+investigraph-etl/badge.svg?branch=main)](https://coveralls.io/github/
+investigativedata/investigraph-etl?branch=main) [![MIT License](https://
+img.shields.io/pypi/l/investigraph)](./LICENSE) # investigraph **Research and
+implementation of an ETL process for a curated and up-to-date public and open-
+source data catalog of frequently used datasets in investigative journalism.**
+Using [prefect.io](https://www.prefect.io/) for ftm pipeline processing
+[Documentation](https://investigativedata.github.io/investigraph/) [Tutorial]
+(https://investigativedata.github.io/investigraph/tutorial/) ## installation
+pip install investigraph ## example datasets There is a dedicated [repo](https:
+//github.com/investigativedata/investigraph-datasets) for example datasets that
+can be used as a [Block](https://docs.prefect.io/2.10.11/concepts/blocks/
+) within the prefect.io deployment. ## deployment ### docker `docker-
+compose.yml` for local development / testing, use `docker-compose.prod.yml` as
+a starting point for a production setup. [More instructions here](https://
+investigativedata.github.io/investigraph/deployment/) ## run locally Install
+app and dependencies (use a virtualenv): pip install investigraph Or, e.g. when
+using [poetry](https://python-poetry.org/): poetry add investigraph After
+installation, `investigraph` as a command should be available: investigraph --
+help Quick run a local dataset definition: investigraph run -c ./path/to/
+config.yml Register a local datasets block: investigraph add-block -b local-
+file-system/investigraph-local -u ./datasets Register github datasets block:
+investigraph add-block -b github/investigraph-datasets -u https://github.com/
+investigativedata/investigraph-datasets.git Run a dataset pipeline from a
+dataset defined in a registered block: investigraph run -d ec_meetings -
+b github/investigraph-datasets View prefect dashboard: make server ##
+development This package is using [poetry](https://python-poetry.org/) for
+packaging and dependencies management, so first [install it](https://python-
+poetry.org/docs/#installation). Clone investigraph repository to a local
+destination. Within the root directory, run poetry install --with dev This
+installs a few development dependencies, including [pre-commit](https://pre-
+commit.com/) which needs to be registered: poetry run pre-commit install Before
+creating a commit, this checks for correct code formatting (isort, black) and
+some other useful stuff (see: `.pre-commit-config.yaml`) ### test make test ##
+supported by [Media Tech Lab Bayern batch #3](https://github.com/media-tech-
+lab) [https://raw.githubusercontent.com/media-tech-lab/.github/main/assets/mtl-
+powered-by.png]
```

### Comparing `investigraph-0.0.4/investigraph/cache.py` & `investigraph-0.1.0/investigraph/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from investigraph.logging import get_logger
 
 log = get_logger(__name__)
 
 
 class Cache:
     """
-    This is an extremly simple cache interface for sharing tasks data
+    This is an extremely simple cache interface for sharing tasks data
     efficiently via redis (or fakeredis during development)
 
     it creates (prefixed) random keys during data set to cache.
 
     it mimics redis GETDEL so that after fetching data from cache the key is
     deleted (turn of by `delete=False`)
     """
```

### Comparing `investigraph-0.0.4/investigraph/catalog.py` & `investigraph-0.1.0/investigraph/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
               easy-to-use dataset.
 
     ```
 
     """
     log.info("building catalog", catalog=str(catalog_in))
     seen = set()
-    with open(catalog_in, "r") as fh:
+    with open(catalog_in) as fh:
         catalog_in_data = yaml.safe_load(fh)
     catalog_in = str(catalog_in)  # for logging
     catalog = DataCatalog(ZavodDataset, {})
     catalog.updated_at = datetime_iso(datetime.utcnow())
     for ds_data in catalog_in_data["datasets"]:
         include_url: Optional[str] = ds_data.pop("include", None)
         if include_url is not None:
```

### Comparing `investigraph-0.0.4/investigraph/cli.py` & `investigraph-0.1.0/investigraph/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,33 +22,35 @@
 configure_logging()
 
 cli = typer.Typer()
 
 
 @cli.command("run")
 def cli_run(
-    dataset: str,
+    dataset: Annotated[Optional[str], typer.Option("-d")] = None,
     block: Annotated[Optional[str], typer.Option("-b")] = None,
     config: Annotated[Optional[str], typer.Option("-c")] = None,
     index_uri: Annotated[Optional[str], typer.Option(...)] = None,
     fragments_uri: Annotated[Optional[str], typer.Option(...)] = None,
     entities_uri: Annotated[Optional[str], typer.Option(...)] = None,
     aggregate: Annotated[Optional[bool], typer.Option(...)] = True,
+    chunk_size: Annotated[Optional[int], typer.Option(...)] = None,
 ):
     """
     Execute a dataset pipeline
     """
     options = FlowOptions(
         dataset=dataset,
         block=block,
         config=config,
         index_uri=index_uri,
         fragments_uri=fragments_uri,
         entities_uri=entities_uri,
         aggregate=aggregate,
+        chunk_size=chunk_size,
     )
     run(options)
 
 
 @cli.command("add-block")
 def cli_add_block(
     block: Annotated[
```

### Comparing `investigraph-0.0.4/investigraph/inspect.py` & `investigraph-0.1.0/investigraph/inspect.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,58 +11,65 @@
 from rich import print
 
 from investigraph.logic.extract import iter_records
 from investigraph.logic.fetch import fetch_source
 from investigraph.model.config import Config, get_config
 from investigraph.model.context import init_context
 from investigraph.model.source import Source
-from investigraph.util import get_func
 
 
 def print_error(msg: str):
     print(f"[bold red]ERROR[/bold red] {msg}")
 
 
 def get_records(source: Source) -> list[dict[str, Any]]:
     records: list[dict[str, Any]] = []
     print("Fetching `%s` ..." % source.uri)
     res = fetch_source(source)
-    for ix, rec in enumerate(iter_records(res)):
+    for ix, rec in enumerate(iter_records(res), 1):
         records.append(rec)
         if ix == 5:
             return records
 
 
 def inspect_config(p: PathLike) -> Config:
     config = get_config(path=p)
     try:
-        func = get_func(config.parse_module_path)
-        if not callable(func):
+        if not callable(config.extract.get_handler()):
+            print_error(f"module not found or not callable: `{config.extract.handler}`")
+    except ModuleNotFoundError:
+        print_error(f"no custom extract module: `{config.extract.handler}`")
+    try:
+        if not callable(config.transform.get_handler()):
             print_error(
-                f"module not found or not callable: `{config.parse_module_path}`"
+                f"module not found or not callable: `{config.transform.handler}`"
             )
     except ModuleNotFoundError:
-        print_error(f"no parsing function: `{config.parse_module_path}`")
+        print_error(f"no custom transform module: `{config.transform.handler}`")
+    try:
+        if not callable(config.load.get_handler()):
+            print_error(f"module not found or not callable: `{config.load.handler}`")
+    except ModuleNotFoundError:
+        print_error(f"no custom load module: `{config.load.handler}`")
     return config
 
 
 def inspect_extract(config: Config) -> Generator[tuple[str, pd.DataFrame], None, None]:
     """
     Preview fetched & extracted records in tabular format
     """
-    for source in config.pipeline.sources:
+    for source in config.extract.sources:
         df = pd.DataFrame(get_records(source))
         yield source.name, df
 
 
 def inspect_transform(config: Config) -> Generator[tuple[str, CE], None, None]:
     """
     Preview first proxies
     """
-    func = get_func(config.parse_module_path)
-    for source in config.pipeline.sources:
+    for source in config.extract.sources:
         ctx = init_context(config, source)
         proxies: list[CE] = []
-        for rec in get_records(source):
-            for proxy in func(ctx, rec):
+        for ix, rec in enumerate(get_records(source)):
+            for proxy in ctx.config.transform.handle(ctx, rec, ix):
                 proxies.append(proxy)
         yield source.name, proxies
```

### Comparing `investigraph-0.0.4/investigraph/logging.py` & `investigraph-0.1.0/investigraph/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import logging
 import sys
 from typing import List
 
 import structlog
+from banal import ensure_list
 from structlog.contextvars import merge_contextvars
 from structlog.stdlib import get_logger as get_raw_logger
 from structlog.types import Processor
 
 
 def configure_logging(
     level: int = logging.INFO,
-    extra_processors: List[Processor] = [],
+    extra_processors: List[Processor] = None,
 ) -> None:
     """Configure log levels and structured logging."""
     processors: List[Processor] = [
         structlog.stdlib.add_log_level,
         structlog.stdlib.add_logger_name,
         structlog.processors.TimeStamper(fmt="%Y-%m-%d %H:%M:%S"),
         structlog.processors.StackInfoRenderer(),
         structlog.dev.set_exc_info,
         structlog.processors.format_exc_info,
         structlog.processors.UnicodeDecoder(),
         merge_contextvars,
     ]
-    processors.extend(extra_processors)
+    processors.extend(ensure_list(extra_processors))
     renderer = structlog.dev.ConsoleRenderer(
         exception_formatter=structlog.dev.plain_traceback
     )
     formatter = structlog.stdlib.ProcessorFormatter(
         foreign_pre_chain=list(processors),
         processor=renderer,
     )
```

### Comparing `investigraph-0.0.4/investigraph/logic/aggregate.py` & `investigraph-0.1.0/investigraph/logic/aggregate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 """
 aggregate fragments
 """
 
 import logging
 from uuid import uuid4
 
+from ftmq.io import smart_read_proxies
 from ftmstore import get_dataset
 
 from investigraph.cache import get_cache
 from investigraph.model import Context
 from investigraph.types import CEGenerator
-from investigraph.util import smart_iter_proxies
 
 log = logging.getLogger(__name__)
 
 
-def get_smart_proxies(uri: str) -> CEGenerator:
+def get_smart_proxies(ctx: Context, uri: str) -> CEGenerator:
     """
     see if we have parts in cache during run time
     (mimics efficient globbing for remote sources)
     """
     cache = get_cache()
-    uris = cache.smembers(uri)
+    uris = cache.smembers(ctx.make_cache_key(uri))
     if uris:
         for uri in uris:
-            yield from smart_iter_proxies(uri)
+            yield from smart_read_proxies(uri)
         return
 
-    yield from smart_iter_proxies(uri)
+    yield from smart_read_proxies(uri)
 
 
 def in_memory(ctx: Context, in_uri: str) -> tuple[int, int]:
     """
     aggregate in memory: read fragments from `in_uri` and write aggregated
     proxies to `out_uri`
 
     as `smart_open` is used here, `in_uri` and `out_uri` can be any local or
     remote locations
     """
     fragments = 0
     buffer = {}
-    for proxy in get_smart_proxies(in_uri):
+    for proxy in get_smart_proxies(ctx, in_uri):
         fragments += 1
         if proxy.id in buffer:
             buffer[proxy.id].merge(proxy)
         else:
             buffer[proxy.id] = proxy
 
-    ctx.entities_loader.write(buffer.values(), serialize=True)
+    ctx.load_entities(buffer.values(), serialize=True)
     return fragments, len(buffer.values())
 
 
 def in_db(ctx: Context, in_uri: str) -> tuple[int, int]:
     """
     use ftm store database to aggregate.
     `in_uri`: database connection string
     """
     dataset = get_dataset("aggregate_%s" % uuid4().hex)
     bulk = dataset.bulk()
-    for ix, proxy in enumerate(get_smart_proxies(in_uri)):
-        if ix % 10000 == 0:
+    for ix, proxy in enumerate(get_smart_proxies(ctx, in_uri)):
+        if ix % 10_000 == 0:
             log.info("Write [%s]: %s entities", dataset.name, ix)
         bulk.put(proxy, fragment=str(ix))
     bulk.flush()
     proxies = []
     for ox, proxy in enumerate(dataset.iterate()):
         proxies.append(proxy)
-        if ox % 10000 == 0:
-            ctx.entities_loader.write(proxies, serialize=True)
+        if ox % 10_000 == 0:
+            ctx.load_entities(proxies, serialize=True)
             proxies = []
-    ctx.entities_loader.write(proxies, serialize=True)
+    ctx.load_entities(proxies, serialize=True)
     dataset.drop()
     return ix, ox
```

### Comparing `investigraph-0.0.4/investigraph/logic/extract.py` & `investigraph-0.1.0/investigraph/logic/extract.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Extract sources to iterate objects to dict records
 """
 
 from io import BytesIO, StringIO
 
+import orjson
 import pandas as pd
 from pantomime import types
 
-from investigraph.model import Source
+from investigraph.model.context import Context
+from investigraph.model.source import TResponse
 from investigraph.types import RecordGenerator
 
 TABULAR = [types.CSV, types.EXCEL, types.XLS, types.XLSX]
 
 
 def read_pandas(mimetype: str, content: str | bytes, **kwargs) -> pd.DataFrame:
     if isinstance(content, bytes):
@@ -22,39 +24,51 @@
     if mimetype in (types.XLS, types.XLSX, types.EXCEL):
         return pd.read_excel(content, **kwargs).fillna("")
     return pd.read_csv(content, **kwargs).fillna("")
 
 
 def yield_pandas(df: pd.DataFrame) -> RecordGenerator:
     for _, row in df.iterrows():
-        yield dict(row)
+        row = {k: v if not pd.isna(v) else None for k, v in row.items()}
+        yield row
 
 
-def iter_records(res: Source) -> RecordGenerator:
+def iter_records(res: TResponse) -> RecordGenerator:
     if res.mimetype in TABULAR:
         kwargs = {**{"dtype": str}, **res.extract_kwargs}
-        if res.is_stream:
+        if res.stream:
             # yield pandas chunks to be able to apply extract_kwargs
             # doesn't work for excel here
             lines = []
             for ix, line in enumerate(res.iter_lines()):
                 lines.append(line)
                 if ix and ix % 10_000 == 0:
                     content = b"\r".join(lines)
                     df = read_pandas(res.mimetype, content, **kwargs)
                     lines = []
                     if ix == 10_000:  # first chunk
                         # fix initial kwargs for next chunk
                         kwargs["names"] = df.columns
                         kwargs["header"] = 0
-                        kwargs.pop("skiprows")  # FIXME what else?
+                        kwargs.pop("skiprows", None)
                     yield from yield_pandas(df)
             if lines:
                 content = b"\r".join(lines)
                 df = read_pandas(res.mimetype, content, **kwargs)
                 yield from yield_pandas(df)
         else:
             df = read_pandas(res.mimetype, res.content, **kwargs)
             yield from yield_pandas(df)
         return
 
+    if res.mimetype == types.JSON:
+        if res.stream:
+            for line in res.iter_lines():
+                yield orjson.loads(line)
+        return
+
     raise NotImplementedError("unsupported mimetype: `%s`" % res.mimetype)
+
+
+# entrypoint
+def handle(ctx: Context, *args, **kwargs) -> RecordGenerator:
+    yield from iter_records(*args, **kwargs)
```

### Comparing `investigraph-0.0.4/investigraph/logic/fetch.py` & `investigraph-0.1.0/investigraph/logic/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 from investigraph.model import Context, HttpSourceResponse, SmartSourceResponse, Source
 from investigraph.util import slugified_dict
 
 
 def fetch_source(source: Source) -> Literal[HttpSourceResponse, SmartSourceResponse]:
     if source.is_http:
         head = source.head()
-        stream = head.should_stream()
-        res = requests.get(source.uri, stream=stream)
+        source.stream = head.should_stream()
+        res = requests.get(source.uri, stream=source.stream)
         assert res.ok
         return HttpSourceResponse(
             **source.dict(),
             header=slugified_dict(res.headers),
             response=res,
-            is_stream=stream,
         )
     return SmartSourceResponse(**source.dict())
 
 
 def get_cache_key(_, params) -> str:
     """
     cache results of fetch tasks based on etag or last_modified
@@ -34,8 +33,8 @@
     if ctx.source.is_http:
         head = ctx.source.head()
         url = ctx.source.uri
         if head.etag:
             return f"{url}-{head.etag}"
         if head.last_modified:
             return f"{url}-{head.last_modified}"
-    return f"{url}-{datetime.now()}"  # actually don't cache
+    return datetime.now().isoformat()  # actually don't cache
```

### Comparing `investigraph-0.0.4/investigraph/model/block.py` & `investigraph-0.1.0/investigraph/model/block.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from normality import slugify
 from prefect import filesystems
 from prefect.blocks.core import Block
 
 from investigraph.exceptions import BlockError
 from investigraph.settings import DATA_ROOT
-from investigraph.util import ensure_path, ensure_pythonpath
+from investigraph.util import ensure_path
 
 BLOCK_TYPES = ("github", "local-file-system")
 
 
 class DatasetBlock:
     def __init__(self, prefix: str, name: str):
         if prefix not in BLOCK_TYPES:
@@ -75,15 +75,14 @@
                 raise e
 
     def load(self, dataset: str) -> None:
         """
         Load dataset from block and add path to python path
         """
         self.load_dataset(dataset)
-        ensure_pythonpath(self.path.parent)
 
 
 class LocalFileSystemBlock(DatasetBlock):
     _block_cls = filesystems.LocalFileSystem
 
     @staticmethod
     def get_create_kwargs(uri: str) -> dict[str, str]:
```

### Comparing `investigraph-0.0.4/investigraph/model/source.py` & `investigraph-0.1.0/investigraph/model/source.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import mimetypes
 from datetime import datetime
+from typing import Literal, TypeAlias
 
 import requests
 from dateparser import parse as parse_date
 from normality import slugify
 from pantomime import normalize_mimetype, types
 from pydantic import BaseModel
 from smart_open import open, parse_uri
@@ -30,72 +31,78 @@
         return self.content_type in (types.CSV, types.JSON)
 
 
 class Source(BaseModel):
     name: str
     uri: str
     scheme: str
+    mimetype: str | None = None
     extract_kwargs: dict | None = {}
+    stream: bool | None = False
+    ijson_path: str | None = "item"
 
     def __init__(self, **data):
         data["uri"] = str(data["uri"])
         data["name"] = data.get("name", slugify(data["uri"]))
         data["scheme"] = data.get("scheme", parse_uri(data["uri"]).scheme)
+        if "mimetype" not in data:
+            mtype, _ = mimetypes.guess_type(data["uri"])
+            data["mimetype"] = normalize_mimetype(mtype)
+        data["stream"] = data.get("stream", data["mimetype"] == types.CSV)
         super().__init__(**data)
 
     @property
     def is_http(self) -> bool:
         return self.scheme.startswith("http")
 
+    @property
+    def is_local(self) -> bool:
+        return self.scheme.startswith("file")
+
     def head(self) -> SourceHead:
         if self.is_http:
             res = requests.head(self.uri)
             return SourceHead(**slugified_dict(res.headers))
         raise NotImplementedError("Cannot fetch head for scheme %s" % self.scheme)
 
     def iter_lines(self) -> BytesGenerator:
         raise NotImplementedError
 
+    def open(self):
+        return open(self.uri)
+
 
 class HttpSourceResponse(Source):
-    is_stream: bool | None = False
     response: requests.Response
     header: SDict
 
     class Config:
         arbitrary_types_allowed = True
 
-    @property
-    def mimetype(self) -> str:
-        return normalize_mimetype(self.header["content_type"])
+    def __init__(self, **data):
+        data["mimetype"] = normalize_mimetype(data["header"]["content_type"])
+        super().__init__(**data)
 
     @property
     def content(self) -> bytes:
-        if self.is_stream:
+        if self.stream:
             raise ImproperlyConfigured("%s is a stream" % self.uri)
         return self.response.content
 
     def iter_lines(self) -> BytesGenerator:
         yield from self.response.iter_lines()
 
 
 class SmartSourceResponse(Source):
     @property
     def content(self) -> bytes:
-        if self.is_stream:
+        if self.stream:
             raise ImproperlyConfigured("%s is a stream" % self.uri)
         with open(self.uri, "rb") as fh:
             return fh.read()
 
     def iter_lines(self) -> BytesGenerator:
         with open(self.uri, "rb") as fh:
-            for line in fh:
-                yield line
+            yield from fh
 
-    @property
-    def mimetype(self) -> str:
-        mtype, _ = mimetypes.guess_type(self.uri)
-        return normalize_mimetype(mtype)
 
-    @property
-    def is_stream(self) -> bool:
-        return self.mimetype in (types.CSV, types.JSON)
+TResponse: TypeAlias = Literal[HttpSourceResponse, SmartSourceResponse]
```

### Comparing `investigraph-0.0.4/investigraph/pipeline.py` & `investigraph-0.1.0/investigraph/pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,64 +2,68 @@
 The main entrypoint for the prefect flow
 """
 
 from typing import Any, Literal
 
 from prefect import flow, get_run_logger, task
 from prefect.task_runners import ConcurrentTaskRunner
+from prefect_dask import DaskTaskRunner
+from prefect_ray import RayTaskRunner
 
 from investigraph import __version__, settings
 from investigraph.logic.aggregate import in_memory
-from investigraph.logic.extract import iter_records
 from investigraph.logic.fetch import fetch_source, get_cache_key
 from investigraph.model import (
     Context,
     Flow,
     FlowOptions,
     HttpSourceResponse,
     SmartSourceResponse,
 )
 from investigraph.model.context import init_context
-from investigraph.util import get_func
+
+
+def get_runner_from_env() -> (
+    Literal[ConcurrentTaskRunner, DaskTaskRunner, RayTaskRunner]
+):
+    if settings.TASK_RUNNER == "dask":
+        return DaskTaskRunner()
+    if settings.TASK_RUNNER == "ray":
+        return RayTaskRunner()
+    return ConcurrentTaskRunner()
 
 
 @task
 def aggregate(ctx: Context):
     logger = get_run_logger()
-    fragments, proxies = in_memory(ctx, ctx.config.fragments_uri)
+    fragments, proxies = in_memory(ctx, ctx.config.load.fragments_uri)
     logger.info("AGGREGATED %d fragments to %d proxies", fragments, proxies)
-    out = ctx.config.entities_uri
+    out = ctx.config.load.entities_uri
     logger.info("OUTPUT: %s", out)
     return out
 
 
 @task
 def load(ctx: Context, ckey: str):
     logger = get_run_logger()
     proxies = ctx.cache.get(ckey)
-    out = ctx.config.fragments_uri
-    if ctx.config.target == "postgres":
-        # write directly to entities instead of fragments
-        # as aggregation is happening within postgres store on write
-        out = ctx.entities_loader.write(proxies)
-    else:
-        out = ctx.fragments_loader.write(proxies)
+    out = ctx.load_fragments(proxies)
     logger.info("LOADED %d proxies", len(proxies))
     logger.info("OUTPUT: %s", out)
     return out
 
 
 @task
 def transform(ctx: Context, ckey: str) -> str:
     logger = get_run_logger()
-    parse_record = get_func(ctx.config.parse_module_path)
     proxies: list[dict[str, Any]] = []
     records = ctx.cache.get(ckey)
-    for rec in records:
-        for proxy in parse_record(ctx, rec):
+    for rec, ix in records:
+        for proxy in ctx.config.transform.handle(ctx, rec, ix):
+            proxy.datasets = {ctx.dataset}
             proxies.append(proxy.to_dict())
     logger.info("TRANSFORMED %d records", len(records))
     return ctx.cache.set(proxies)
 
 
 @task(
     retries=settings.FETCH_RETRIES,
@@ -72,46 +76,56 @@
     return fetch_source(ctx.source)
 
 
 @flow(
     name="investigraph-pipeline",
     version=__version__,
     flow_run_name="{ctx.dataset}-{ctx.source.name}",
-    task_runner=ConcurrentTaskRunner(),
+    task_runner=get_runner_from_env(),
 )
 def run_pipeline(ctx: Context):
-    res = fetch.submit(ctx)
-    res = res.result()
+    if ctx.config.extract.fetch:
+        res = fetch.submit(ctx)
+        res = res.result()
+        enumerator = enumerate(ctx.config.extract.handle(ctx, res), 1)
+    else:
+        enumerator = enumerate(ctx.config.extract.handle(ctx), 1)
+
     ix = 0
     batch = []
     results = []
-    for ix, rec in enumerate(iter_records(res)):
-        batch.append(rec)
-        if ix and ix % 1000 == 0:
+    for ix, rec in enumerator:
+        batch.append((rec, ix))
+        if ix and ix % ctx.config.transform.chunk_size == 0:
             results.append(transform.submit(ctx, ctx.cache.set(batch)))
             batch = []
     if batch:
         results.append(transform.submit(ctx, ctx.cache.set(batch)))
 
     logger = get_run_logger()
-    logger.info("EXTRACTED %d records", ix + 1)
+    logger.info("EXTRACTED %d records", ix)
 
     # write
     for res in results:
         res = res.result()
         load.submit(ctx, res)
 
 
 @flow(
     name="investigraph",
     version=__version__,
     flow_run_name="{options.dataset}",
 )
-def run(options: FlowOptions):
+def run(options: FlowOptions) -> str:
     flow = Flow.from_options(options)
-    for source in flow.config.pipeline.sources:
+    for ix, source in enumerate(flow.config.extract.sources):
         ctx = init_context(config=flow.config, source=source)
-        ctx.export_metadata()
+        if ix == 0:  # only on first time
+            ctx.export_metadata()
+            logger = get_run_logger()
+            logger.info("INDEX: %s" % ctx.config.load.index_uri)
         run_pipeline(ctx)
 
     if flow.should_aggregate:
         aggregate(ctx)
+
+    return flow.config.load.entities_uri
```

### Comparing `investigraph-0.0.4/investigraph/settings.py` & `investigraph-0.1.0/investigraph/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,22 @@
 DEBUG = as_bool(get_env("DEBUG", 1))
 DATA_ROOT = Path(get_env("DATA_ROOT", Path.cwd() / "data")).absolute()
 DATASETS_REPO = get_env(
     "DATASETS_REPO", "https://github.com/investigativedata/investigraph-datasets.git"
 )
 DATASETS_BLOCK = get_env("DATASETS_BLOCK", "github/investigraph-datasets")
 
+DEFAULT_EXTRACTOR = get_env("DEFAULT_EXTRACTOR", "investigraph.logic.extract:handle")
 DEFAULT_TRANSFORMER = get_env(
     "DEFAULT_TRANSFORMER", "investigraph.logic.transform:map_ftm"
 )
+DEFAULT_LOADER = get_env("DEFAULT_LOADER", "investigraph.logic.load:load_proxies")
 
 REDIS_URL = get_env("REDIS_URL", "redis://localhost:6379")
 CACHE_PREFIX = get_env("CACHE_PREFIX", f"investigraph:{__version__}")
 
 FETCH_RETRIES = int(get_env("FETCH_RETRIES", 3))
 FETCH_RETRY_DELAY = int(get_env("FETCH_RETRY_DELAY", 5))
+
+TASK_RUNNER = get_env("PREFECT_TASK_RUNNER", "").lower()
+
+CHUNK_SIZE = int(get_env("CHUNK_SIZE", 1000))
```

