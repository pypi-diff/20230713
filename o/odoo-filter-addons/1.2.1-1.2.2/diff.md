# Comparing `tmp/odoo_filter_addons-1.2.1.tar.gz` & `tmp/odoo_filter_addons-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_filter_addons-1.2.1.tar", last modified: Mon Jun 19 07:55:50 2023, max compression
+gzip compressed data, was "odoo_filter_addons-1.2.2.tar", last modified: Thu Jul 13 09:51:41 2023, max compression
```

## Comparing `odoo_filter_addons-1.2.1.tar` & `odoo_filter_addons-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:55:50.505172 odoo_filter_addons-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-19 07:55:50.505172 odoo_filter_addons-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:55:50.505172 odoo_filter_addons-1.2.1/odoo_filter_addons/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/odoo_filter_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/odoo_filter_addons/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/odoo_filter_addons/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:55:50.505172 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:55:50.505172 odoo_filter_addons-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:51:41.561876 odoo_filter_addons-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-13 09:51:41.561876 odoo_filter_addons-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:51:41.561876 odoo_filter_addons-1.2.2/odoo_filter_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/odoo_filter_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/odoo_filter_addons/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/odoo_filter_addons/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:51:41.561876 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 09:51:41.000000 odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:51:41.561876 odoo_filter_addons-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 09:51:29.000000 odoo_filter_addons-1.2.2/setup.py
```

### Comparing `odoo_filter_addons-1.2.1/PKG-INFO` & `odoo_filter_addons-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_filter_addons
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `odoo_filter_addons-1.2.1/README.md` & `odoo_filter_addons-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `odoo_filter_addons-1.2.1/odoo_filter_addons/main.py` & `odoo_filter_addons-1.2.2/odoo_filter_addons/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 
 #####################################################################
 
 class UserException(Exception):
     pass
 
 def print_header(msg, sym):
-    print("{}\n{}".format(sym*len(msg), msg))
+    print(f"{sym*len(msg)}\n{msg}")
 
 def load_yml(path, expand=False):
     if path.with_suffix(".yml").is_file():
         path = path.with_suffix(".yml")
     elif path.with_suffix(".yaml").is_file():
         path = path.with_suffix(".yaml")
     else:
-        raise UserException("YAML file {}.y[a]ml not found".format(path))
+        raise UserException(f"YAML file {path}.y[a]ml not found")
 
     with open(path, "r") as f:
         if expand and path.with_suffix(".env").is_file():
             env = dotenv_values(path.with_suffix(".env"))
             templated = Template(f.read()).substitute(env)
             yml = yaml.safe_load(StringIO(templated).read())
         else:
@@ -59,16 +59,16 @@
 
 # Update remote URLs to use GitLab access token
 def update_remotes(repos):
     try:
         token = os.environ["CI_JOB_TOKEN"]
         host = os.environ["CI_SERVER_HOST"]
     except KeyError as e:
-        raise UserException("Unset environment variable {}".format(e))
-    gitlab_url = "https://gitlab-ci-token:{}@{}/{{}}".format(token, host)
+        raise UserException(f"Unset environment variable {e}")
+    gitlab_url = f"https://gitlab-ci-token:{token}@{host}/{{}}"
     for repo in repos.values():
         for name, url in repo["remotes"].items():
             if "git@gitlab.com:" in url:
                 project = url.split(":")[1]
                 repo["remotes"][name] = gitlab_url.format(project)
     return repos
 
@@ -86,61 +86,67 @@
         git("remote", "set-url", rname, rpath)
     else:
         git("remote", "add", rname, rpath)
     git("fetch", "--depth", "1", rname, rbranch)
     # Checkout changes for each of the modules listed
     for fname in next(os.walk(rpath))[1]:
         if is_module(rpath/fname) and any([fnmatch(fname, m) for m in modules]):
-            git("checkout", "{}/{}".format(rname, rbranch), fname)
-            print("Added module {}".format(fname))
+            git("checkout", f"{rname}/{rbranch}", fname)
+            print(f"Added module {fname}")
     # Create a message that will allow tracing the commit
     lines = [rname]
     for merge in repo["merges"]:
         if "merge-requests" in merge or "pull" in merge:
             last_hash = git("-C", rpath, "ls-remote", "--exit-code", *merge.split()).split()[0]
         else:
             last_hash = git("-C", rpath, "rev-parse", merge.replace(" ", "/"))
-        lines.append("{} {}".format(merge, last_hash).strip())
+        lines.append(f"{merge} {last_hash}".strip())
     message = "\n".join(lines)
-    print("Partial message:\n{}".format(message))
+    print(f"Partial message:\n{message}")
     return message
 
 def filter_repos(output_path, tmp_path, repos, addons, release, push, gitlab_ci):
     os.chdir(output_path)
     # Remove old modules
     for fname in next(os.walk("."))[1]:
         if is_module(fname):
-            git("rm", "-rf", fname)
+            try:
+                # Remove from index and working tree
+                git("rm", "-rf", fname)
+            except ProcessExecutionError:
+                # Module not in index, remove from working tree
+                rmtree(fname)
     # Add new modules
     messages = []
     for rname, modules in addons.items():
-        print_header("Filtering '{}'".format(rname), '-')
-        repo = repos.get(rname) or repos.get("./{}".format(rname))
+        print_header(f"Filtering '{rname}'", '-')
+        repo = repos.get(rname) or repos.get(f"./{rname}")
         if not repo:
-            raise UserException("addons.yml entry {} not found in repos.yml".format(rname))
+            raise UserException(f"addons.yml entry {rname} not found in repos.yml")
         repo_message = filter_repo(tmp_path, rname, repo, modules)
         messages.append(repo_message)
     print_header("Finished filtering", '*')
-    # Commit changes, if any, and push them to remote if specified
+    # If not in release mode remove files from the index
     if not release:
-        git("restore", "--staged", ".")
+        git("rm", "-rf", "--cached", ".")
         print("Release disabled, nothing commited")
+    # Otherwise, commit changes if any, and push them to remote if specified
     elif filter(None, messages) and git["diff", "--staged", "--quiet"] & TF(1):
         messages = [f"[AUTO] {__package__} {__version__}"] + messages
         message = "\n".join(messages)
         git("commit", "-m", message)
         print("Changes commited")
         if push:
             if git["rev-parse", "@{u}"] & TF:
                 git("push")
             elif gitlab_ci:
                 branch = os.environ.get("CI_COMMIT_BRANCH")
                 if not branch:
                     raise UserException("Unset environment variable CI_COMMIT_BRANCH")
-                git("push", "origin", "HEAD:{}".format(branch))
+                git("push", "origin", f"HEAD:{branch}")
             else:
                 raise UserException("addons.yml entry {} not found in repos.yml".format(rname))
             print("Commit pushed to remote")
     else:
         print("No changes, nothing commited")
 
 @contextmanager
@@ -151,44 +157,44 @@
         yield
     finally:
         sys.argv = old_argv
 
 # Create a git repo if not present and aggregate addon repositories
 def initialize_repos(output_path, tmp_path, repos):
     if not output_path.is_dir():
-        print("Initializing git repository in '{}'".format(output_path))
+        print(f"Initializing git repository in '{output_path}'")
         Path(output_path).mkdir(parents=True, exist_ok=True)
     git("-C", output_path, "init")
 
     os.chdir(tmp_path)
     dump_yml("repos.yml", repos)
 
     new_argv = ["gitaggregate", "-c", "repos.yml"]
     with set_argv(new_argv):
         gitaggregate()
-    print("gitaggregate output written to '{}'".format(tmp_path))
+    print(f"gitaggregate output written to '{tmp_path}'")
 
 #####################################################################
 
 # API entry point
 def api_main(input_path=None, output_path=None, clean=True, release=False, push=False, gitlab_ci=False):
     input_path = Path(input_path).resolve() if input_path else Path.cwd()
     output_path = Path(output_path).resolve() if output_path else Path.cwd()
     tmp_path = Path(mkdtemp())
 
-    print("Loading configuration files from '{}'".format(input_path))
+    print(f"Loading configuration files from '{input_path}'")
     repos = load_yml(input_path/"repos", True)
     addons = load_yml(input_path/"addons")
 
     repos = remove_targets(repos)
     if gitlab_ci:
         repos = update_remotes(repos)
 
     try:
-        print("Filtering addons to '{}'".format(output_path))
+        print(f"Filtering addons to '{output_path}'")
         initialize_repos(output_path, tmp_path, repos)
         filter_repos(output_path, tmp_path, repos, addons, release, push, gitlab_ci)
     except Exception as e:
         if clean:
             rmtree(tmp_path)
         raise e
     if clean:
```

### Comparing `odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/PKG-INFO` & `odoo_filter_addons-1.2.2/odoo_filter_addons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-filter-addons
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `odoo_filter_addons-1.2.1/pyproject.toml` & `odoo_filter_addons-1.2.2/pyproject.toml`

 * *Files identical despite different names*

