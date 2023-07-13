# Comparing `tmp/snk-0.9.2.tar.gz` & `tmp/snk-0.9.3.tar.gz`

## Comparing `snk-0.9.2.tar` & `snk-0.9.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.9.2/Dockerfile
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.9.2/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.9.2/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.9.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 snk-0.9.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.9.2/docs/CNAME
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 snk-0.9.2/docs/index.md
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.9.2/docs/managing_pipelines.md
--rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 snk-0.9.2/docs/pipeline_packages.md
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 snk-0.9.2/docs/snk_config_file.md
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 snk-0.9.2/docs/CLI/env.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 snk-0.9.2/docs/CLI/index.md
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 snk-0.9.2/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.9.2/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.9.2/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.9.2/docs/reference/nest.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 snk-0.9.2/docs/reference/pipeline.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.9.2/snk/__about__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.9.2/snk/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.9.2/snk/errors.py
--rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 snk-0.9.2/snk/main.py
--rw-r--r--   0        0        0    16434 2020-02-02 00:00:00.000000 snk-0.9.2/snk/nest.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 snk-0.9.2/snk/pipeline.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.9.2/snk/cli/__init__.py
--rw-r--r--   0        0        0    19528 2020-02-02 00:00:00.000000 snk-0.9.2/snk/cli/cli.py
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 snk-0.9.2/snk/cli/config.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 snk-0.9.2/snk/cli/dynamic_typer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.9.2/snk/cli/options.py
--rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 snk-0.9.2/snk/cli/utils.py
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 snk-0.9.2/snk/cli/workflow.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 snk-0.9.2/snk/cli/subcommands/__init__.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 snk-0.9.2/snk/cli/subcommands/env.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.9.2/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 snk-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 snk-0.9.2/tests/test_nest.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk-0.9.2/tests/test_pipline_cli.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.9.2/tests/test_snk.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 snk-0.9.2/tests/test_snk_config.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.9.2/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/pipeline/cli.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/pipeline/snk.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/pipeline/resources/data.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/pipeline/workflow/Snakefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/pipeline/workflow/envs/base.yml
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/pipeline/workflow/envs/pandas.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.9.2/tests/data/pipeline/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 snk-0.9.2/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.9.2/LICENSE.txt
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 snk-0.9.2/README.md
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 snk-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 snk-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.9.3/Dockerfile
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.9.3/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.9.3/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.9.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 snk-0.9.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.9.3/docs/CNAME
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 snk-0.9.3/docs/index.md
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.9.3/docs/managing_pipelines.md
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 snk-0.9.3/docs/pipeline_packages.md
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 snk-0.9.3/docs/snk_config_file.md
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 snk-0.9.3/docs/CLI/env.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 snk-0.9.3/docs/CLI/index.md
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 snk-0.9.3/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.9.3/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.9.3/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.9.3/docs/reference/nest.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 snk-0.9.3/docs/reference/pipeline.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.9.3/snk/__about__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.9.3/snk/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.9.3/snk/errors.py
+-rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 snk-0.9.3/snk/main.py
+-rw-r--r--   0        0        0    16434 2020-02-02 00:00:00.000000 snk-0.9.3/snk/nest.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 snk-0.9.3/snk/pipeline.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.9.3/snk/cli/__init__.py
+-rw-r--r--   0        0        0    19528 2020-02-02 00:00:00.000000 snk-0.9.3/snk/cli/cli.py
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 snk-0.9.3/snk/cli/config.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 snk-0.9.3/snk/cli/dynamic_typer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.9.3/snk/cli/options.py
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 snk-0.9.3/snk/cli/utils.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 snk-0.9.3/snk/cli/workflow.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 snk-0.9.3/snk/cli/subcommands/__init__.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 snk-0.9.3/snk/cli/subcommands/env.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.9.3/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 snk-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 snk-0.9.3/tests/test_nest.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk-0.9.3/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.9.3/tests/test_snk.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 snk-0.9.3/tests/test_snk_config.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.9.3/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/pipeline/cli.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/pipeline/snk.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/pipeline/resources/data.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/pipeline/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/pipeline/workflow/envs/base.yml
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/pipeline/workflow/envs/pandas.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.9.3/tests/data/pipeline/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 snk-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.9.3/LICENSE.txt
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 snk-0.9.3/README.md
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 snk-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 snk-0.9.3/PKG-INFO
```

### Comparing `snk-0.9.2/mkdocs.yml` & `snk-0.9.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/.github/workflows/publish.yml` & `snk-0.9.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/.github/workflows/tests.yml` & `snk-0.9.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/docs/index.md` & `snk-0.9.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/docs/managing_pipelines.md` & `snk-0.9.3/docs/managing_pipelines.md`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/docs/pipeline_packages.md` & `snk-0.9.3/docs/pipeline_packages.md`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/docs/snk_config_file.md` & `snk-0.9.3/docs/snk_config_file.md`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/docs/CLI/env.md` & `snk-0.9.3/docs/CLI/env.md`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/docs/CLI/index.md` & `snk-0.9.3/docs/CLI/index.md`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/snk/main.py` & `snk-0.9.3/snk/main.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/snk/nest.py` & `snk-0.9.3/snk/nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/snk/pipeline.py` & `snk-0.9.3/snk/pipeline.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/snk/cli/cli.py` & `snk-0.9.3/snk/cli/cli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,20 @@
         if " " in str(pipeline_dir_path):
             # cannot have spaces!
             self.singularity_prefix_dir = None
         else:
             self.singularity_prefix_dir = pipeline_dir_path / ".singularity"
         self.name = self.pipeline.name
         self.verbose = False
+        if (
+            platform.system() == "Darwin"
+            and platform.processor() == "arm"
+            and not os.environ.get("CONDA_SUBDIR")
+        ):
+            os.environ["CONDA_SUBDIR"] = "osx-64"
 
         def _print_pipline_version(ctx: typer.Context, value: bool):
             if value:
                 typer.echo(self.version)
                 raise typer.Exit()
 
         def _print_pipline_path(ctx: typer.Context, value: bool):
@@ -347,20 +353,14 @@
           verbose (bool): Run pipeline in verbose mode.
           help_snakemake (bool): Print the snakemake help and exit.
         Side Effects:
           Runs the pipeline.
         Examples:
           >>> CLI.run(target='my_target', configfile=Path('/path/to/config.yaml'), resource=[Path('/path/to/resource')], verbose=True)
         """
-        if (
-            platform.system() == "Darwin"
-            and platform.processor() == "arm"
-            and not os.environ.get("CONDA_SUBDIR")
-        ):
-            os.environ["CONDA_SUBDIR"] = "osx-64"
         self.verbose = verbose
         args = []
         if not cores:
             cores = "all"
         args.extend(
             [
                 "--use-conda",
```

### Comparing `snk-0.9.2/snk/cli/config.py` & `snk-0.9.3/snk/cli/config.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/snk/cli/dynamic_typer.py` & `snk-0.9.3/snk/cli/dynamic_typer.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/snk/cli/utils.py` & `snk-0.9.3/snk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/snk/cli/workflow.py` & `snk-0.9.3/snk/cli/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from dataclasses import dataclass
 from pathlib import Path
 from snakemake import Workflow, update_config, load_configfile, dict_to_key_value_args, common
-from snakemake.persistence import Persistence
 import os
 
 def create_workflow( 
         snakefile,
         cache=None,
         lint=None,
         cores=1,
@@ -134,10 +134,16 @@
             conda_base_path=conda_base_path,
             check_envvars=not lint,  # for linting, we do not need to check whether requested envvars exist
             all_temp=all_temp,
             local_groupid=local_groupid,
             keep_metadata=keep_metadata,
             latency_wait=latency_wait,
         )
-        workflow.persistence = Persistence(conda_prefix=Path(conda_prefix).resolve() if conda_prefix else None)
+        @dataclass
+        class PersistenceMock:
+            conda_env_path: Path
+
+        workflow.persistence = PersistenceMock(
+            conda_env_path=Path(conda_prefix).resolve() if conda_prefix else None,
+        )
         return workflow
```

### Comparing `snk-0.9.2/snk/cli/subcommands/env.py` & `snk-0.9.3/snk/cli/subcommands/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
             use_conda = True,
             conda_prefix=self.conda_prefix_dir.resolve(),
         )
         self.register_command(self.list, help="List the environments in the pipeline.")
         self.register_command(self.show, help="Show the environments config file contents.")
         self.register_command(self.run, help="Run a command in one of the pipeline environments.")
         self.register_command(self.activate, help="Activate a pipeline conda environment.")
-        self.register_command(self.prune, help="Delete all conda environments")
-        self.register_command(self.create, help="Create all conda environments")
+        self.register_command(self.prune, help="Delete all conda environments.")
+        self.register_command(self.create, help="Create all conda environments.")
 
     def list(self):
         environments_dir_yellow = typer.style(
             self.pipeline.path / "envs", fg=typer.colors.YELLOW
         )
         typer.echo(
             f"Found {len(self.pipeline.environments)} environments in {environments_dir_yellow}"
```

### Comparing `snk-0.9.2/tests/.DS_Store` & `snk-0.9.3/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/tests/conftest.py` & `snk-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/tests/test_nest.py` & `snk-0.9.3/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/tests/test_pipline_cli.py` & `snk-0.9.3/tests/test_pipline_cli.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/tests/test_snk.py` & `snk-0.9.3/tests/test_snk.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/tests/test_snk_config.py` & `snk-0.9.3/tests/test_snk_config.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/tests/utils.py` & `snk-0.9.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/tests/data/artic_v4.1.bed` & `snk-0.9.3/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/tests/data/config.yaml` & `snk-0.9.3/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/tests/data/cov.fasta` & `snk-0.9.3/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/tests/data/pipeline/workflow/envs/pandas.yml` & `snk-0.9.3/tests/data/pipeline/workflow/envs/pandas.yml`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/LICENSE.txt` & `snk-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/README.md` & `snk-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/pyproject.toml` & `snk-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snk-0.9.2/PKG-INFO` & `snk-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.9.2
+Version: 0.9.3
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snk Version: 0.9.2 Project-URL: Documentation,
+Metadata-Version: 2.1 Name: snk Version: 0.9.3 Project-URL: Documentation,
 https://github.com/wytamma/snk#readme Project-URL: Issues, https://github.com/
 wytamma/snk/issues Project-URL: Source, https://github.com/wytamma/snk Author-
 email: Wytamma Wirth
 wirth@me.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

