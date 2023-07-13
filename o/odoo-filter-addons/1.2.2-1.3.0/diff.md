# Comparing `tmp/odoo_filter_addons-1.2.2.tar.gz` & `tmp/odoo_filter_addons-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_filter_addons-1.2.2.tar", last modified: Thu Jul 13 09:51:41 2023, max compression
+gzip compressed data, was "odoo_filter_addons-1.3.0.tar", last modified: Thu Jul 13 10:27:51 2023, max compression
```

## Comparing `odoo_filter_addons-1.2.2.tar` & `odoo_filter_addons-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:51:41.561876 odoo_filter_addons-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-13 09:51:41.561876 odoo_filter_addons-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:51:41.561876 odoo_filter_addons-1.2.2/odoo_filter_addons/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/odoo_filter_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/odoo_filter_addons/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/odoo_filter_addons/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:51:41.561876 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:51:41.561876 odoo_filter_addons-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:27:51.518580 odoo_filter_addons-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-13 10:27:51.518580 odoo_filter_addons-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-13 10:27:41.000000 odoo_filter_addons-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:27:51.514580 odoo_filter_addons-1.3.0/odoo_filter_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-13 10:27:41.000000 odoo_filter_addons-1.3.0/odoo_filter_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-07-13 10:27:41.000000 odoo_filter_addons-1.3.0/odoo_filter_addons/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 10:27:41.000000 odoo_filter_addons-1.3.0/odoo_filter_addons/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:27:51.514580 odoo_filter_addons-1.3.0/odoo_filter_addons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-13 10:27:51.000000 odoo_filter_addons-1.3.0/odoo_filter_addons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-13 10:27:51.000000 odoo_filter_addons-1.3.0/odoo_filter_addons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:27:51.000000 odoo_filter_addons-1.3.0/odoo_filter_addons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-13 10:27:51.000000 odoo_filter_addons-1.3.0/odoo_filter_addons.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 10:27:51.000000 odoo_filter_addons-1.3.0/odoo_filter_addons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 10:27:51.000000 odoo_filter_addons-1.3.0/odoo_filter_addons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-13 10:27:41.000000 odoo_filter_addons-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:27:51.518580 odoo_filter_addons-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 10:27:41.000000 odoo_filter_addons-1.3.0/setup.py
```

### Comparing `odoo_filter_addons-1.2.2/PKG-INFO` & `odoo_filter_addons-1.3.0/odoo_filter_addons.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: odoo_filter_addons
-Version: 1.2.2
+Name: odoo-filter-addons
+Version: 1.3.0
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
@@ -36,11 +36,12 @@
 By default, both the input and output path default to the current working directory,
 but can be overridden through the `-i/--input-path` and `-o/--output-path` flags
 respectively. Additionally, some other flags can be provided to alter the behavior of
 the program:
 
 | Flag                          | Default | Description                                               |
 |-------------------------------|---------|-----------------------------------------------------------|
-| -c, --clean / --no-clean      | True    | Clean intermediate output                                 |
+| -c, --clean / --no-clean      | True    | Clean gitaggregate output                                 |
+| -C, --cache / --no-cache      | False   | Cache gitaggregate output, overrides -c                   |
 | -r, --release / --no-release  | False   | Create a release commit if any changes are made           |
 | -p, --push / --no-push        | False   | Push to remote repo if any changes are commited           |
 | -g, --gitlab-ci               | False   | Update client addon repository in GitLab CI               |
```

### Comparing `odoo_filter_addons-1.2.2/README.md` & `odoo_filter_addons-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: odoo_filter_addons
+Version: 1.3.0
+Summary: Simple utlity to filter odoo addons into a single directory
+Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Utilities
+Classifier: Operating System :: POSIX
+Classifier: Framework :: Odoo
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+
 # Odoo filter addons
 
 Simple command line utility used to filter specific odoo addons from
 multiple repositories. It leverages [git-aggregator](https://github.com/acsone/git-aggregator)
 and its **repo.yml** format as well as [doodba](https://github.com/Tecnativa/doodba)'s
 addons **addons.yml** format.
 
@@ -23,11 +36,12 @@
 By default, both the input and output path default to the current working directory,
 but can be overridden through the `-i/--input-path` and `-o/--output-path` flags
 respectively. Additionally, some other flags can be provided to alter the behavior of
 the program:
 
 | Flag                          | Default | Description                                               |
 |-------------------------------|---------|-----------------------------------------------------------|
-| -c, --clean / --no-clean      | True    | Clean intermediate output                                 |
+| -c, --clean / --no-clean      | True    | Clean gitaggregate output                                 |
+| -C, --cache / --no-cache      | False   | Cache gitaggregate output, overrides -c                   |
 | -r, --release / --no-release  | False   | Create a release commit if any changes are made           |
 | -p, --push / --no-push        | False   | Push to remote repo if any changes are commited           |
 | -g, --gitlab-ci               | False   | Update client addon repository in GitLab CI               |
```

### Comparing `odoo_filter_addons-1.2.2/odoo_filter_addons/main.py` & `odoo_filter_addons-1.3.0/odoo_filter_addons/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 
 #####################################################################
 
 def is_module(path):
     path = Path(path)
     return path.is_dir() and (path/"__manifest__.py").is_file()
 
-def filter_repo(tmp_path, rname, repo, modules):
-    rpath = tmp_path/rname
+def filter_repo(agg_path, rname, repo, modules):
+    rpath = agg_path/rname
     rbranch = repo["target"].split()[1] if repo.get("target") else "_git_aggregated"
     # Fetch the specified branch from the remote repo
     if git["remote", "get-url", rname] & TF:
         git("remote", "set-url", rname, rpath)
     else:
         git("remote", "add", rname, rpath)
     git("fetch", "--depth", "1", rname, rbranch)
@@ -100,15 +100,15 @@
         else:
             last_hash = git("-C", rpath, "rev-parse", merge.replace(" ", "/"))
         lines.append(f"{merge} {last_hash}".strip())
     message = "\n".join(lines)
     print(f"Partial message:\n{message}")
     return message
 
-def filter_repos(output_path, tmp_path, repos, addons, release, push, gitlab_ci):
+def filter_repos(output_path, agg_path, repos, addons, release, push, gitlab_ci):
     os.chdir(output_path)
     # Remove old modules
     for fname in next(os.walk("."))[1]:
         if is_module(fname):
             try:
                 # Remove from index and working tree
                 git("rm", "-rf", fname)
@@ -118,15 +118,15 @@
     # Add new modules
     messages = []
     for rname, modules in addons.items():
         print_header(f"Filtering '{rname}'", '-')
         repo = repos.get(rname) or repos.get(f"./{rname}")
         if not repo:
             raise UserException(f"addons.yml entry {rname} not found in repos.yml")
-        repo_message = filter_repo(tmp_path, rname, repo, modules)
+        repo_message = filter_repo(agg_path, rname, repo, modules)
         messages.append(repo_message)
     print_header("Finished filtering", '*')
     # If not in release mode remove files from the index
     if not release:
         git("rm", "-rf", "--cached", ".")
         print("Release disabled, nothing commited")
     # Otherwise, commit changes if any, and push them to remote if specified
@@ -155,70 +155,75 @@
     sys.argv = new_argv
     try:
         yield
     finally:
         sys.argv = old_argv
 
 # Create a git repo if not present and aggregate addon repositories
-def initialize_repos(output_path, tmp_path, repos):
+def initialize_repos(output_path, agg_path, repos):
     if not output_path.is_dir():
         print(f"Initializing git repository in '{output_path}'")
-        Path(output_path).mkdir(parents=True, exist_ok=True)
+        output_path.mkdir(parents=True, exist_ok=True)
     git("-C", output_path, "init")
 
-    os.chdir(tmp_path)
+    os.chdir(agg_path)
     dump_yml("repos.yml", repos)
 
     new_argv = ["gitaggregate", "-c", "repos.yml"]
     with set_argv(new_argv):
         gitaggregate()
-    print(f"gitaggregate output written to '{tmp_path}'")
-
+    print(f"gitaggregate output written to '{agg_path}'")
 #####################################################################
 
 # API entry point
-def api_main(input_path=None, output_path=None, clean=True, release=False, push=False, gitlab_ci=False):
+def api_main(input_path=None, output_path=None, clean=True, cache=False, release=False, push=False, gitlab_ci=False):
     input_path = Path(input_path).resolve() if input_path else Path.cwd()
     output_path = Path(output_path).resolve() if output_path else Path.cwd()
-    tmp_path = Path(mkdtemp())
+    if cache:
+        clean = False
+        agg_path = Path.home()/".cache"/"odoo-filter-addons"
+        agg_path.mkdir(parents=True, exist_ok=True)
+    else:
+        agg_path = Path(mkdtemp())
 
     print(f"Loading configuration files from '{input_path}'")
     repos = load_yml(input_path/"repos", True)
     addons = load_yml(input_path/"addons")
 
     repos = remove_targets(repos)
     if gitlab_ci:
         repos = update_remotes(repos)
 
     try:
         print(f"Filtering addons to '{output_path}'")
-        initialize_repos(output_path, tmp_path, repos)
-        filter_repos(output_path, tmp_path, repos, addons, release, push, gitlab_ci)
+        initialize_repos(output_path, agg_path, repos)
+        filter_repos(output_path, agg_path, repos, addons, release, push, gitlab_ci)
     except Exception as e:
         if clean:
-            rmtree(tmp_path)
+            rmtree(agg_path)
         raise e
     if clean:
         print("Cleaning up intermediate output")
-        rmtree(tmp_path)
+        rmtree(agg_path)
 
 # CLI entry point
 @click.command(context_settings=dict(help_option_names=['-h', '--help']))
 @click.version_option()
 @click.option("-i", "--input-path", help="Path to directory containing configuration files.")
 @click.option("-o", "--output-path", help="Path to the directory that will contain the output.")
-@click.option("-c", "--clean/--no-clean", is_flag=True, default=True, help="Clean intermediate output.")
+@click.option("-c", "--clean/--no-clean", is_flag=True, default=True, help="Clean gitaggregate output.")
+@click.option("-C", "--cache/--no-cache", is_flag=True, default=False, help="Cache gitaggregate output, overrides -c.")
 @click.option("-r", "--release/--no-release", is_flag=True, default=False, help="Create a relase commit if any changes are made.")
 @click.option("-p", "--push/--no-push", is_flag=True, default=False, help="Push to remote repo if any changes are commited.")
 @click.option("-g", "--gitlab-ci", is_flag=True, default=False, help="Update client addon repository in GitLab CI.")
-def cli_main(input_path, output_path, clean, release, push, gitlab_ci):
+def cli_main(input_path, output_path, clean, cache, release, push, gitlab_ci):
     import sys
     import traceback
     try:
-        api_main(input_path, output_path, clean, release, push, gitlab_ci)
+        api_main(input_path, output_path, clean, cache, release, push, gitlab_ci)
         sys.exit(0)
     except UserException as e:
         print("User error:", e)
     except yaml.YAMLError as e:
         print("Invalid YAML content:", e)
     except ProcessExecutionError as e:
         print("Process execution error:", e)
```

### Comparing `odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/PKG-INFO` & `odoo_filter_addons-1.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: odoo-filter-addons
-Version: 1.2.2
-Summary: Simple utlity to filter odoo addons into a single directory
-Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Utilities
-Classifier: Operating System :: POSIX
-Classifier: Framework :: Odoo
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-
 # Odoo filter addons
 
 Simple command line utility used to filter specific odoo addons from
 multiple repositories. It leverages [git-aggregator](https://github.com/acsone/git-aggregator)
 and its **repo.yml** format as well as [doodba](https://github.com/Tecnativa/doodba)'s
 addons **addons.yml** format.
 
@@ -36,11 +23,12 @@
 By default, both the input and output path default to the current working directory,
 but can be overridden through the `-i/--input-path` and `-o/--output-path` flags
 respectively. Additionally, some other flags can be provided to alter the behavior of
 the program:
 
 | Flag                          | Default | Description                                               |
 |-------------------------------|---------|-----------------------------------------------------------|
-| -c, --clean / --no-clean      | True    | Clean intermediate output                                 |
+| -c, --clean / --no-clean      | True    | Clean gitaggregate output                                 |
+| -C, --cache / --no-cache      | False   | Cache gitaggregate output, overrides -c                   |
 | -r, --release / --no-release  | False   | Create a release commit if any changes are made           |
 | -p, --push / --no-push        | False   | Push to remote repo if any changes are commited           |
 | -g, --gitlab-ci               | False   | Update client addon repository in GitLab CI               |
```

### Comparing `odoo_filter_addons-1.2.2/pyproject.toml` & `odoo_filter_addons-1.3.0/pyproject.toml`

 * *Files identical despite different names*

