# Comparing `tmp/f5project-0.0.5.tar.gz` & `tmp/f5project-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f5project-0.0.5.tar", last modified: Tue Jul 11 00:42:08 2023, max compression
+gzip compressed data, was "f5project-0.0.6.tar", last modified: Thu Jul 13 02:46:17 2023, max compression
```

## Comparing `f5project-0.0.5.tar` & `f5project-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:42:08.532599 f5project-0.0.5/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-28 09:15:27.000000 f5project-0.0.5/LICENSE
--rw-r--r--   0 j3ymac     (501) staff       (20)     7095 2023-07-11 00:42:08.532440 f5project-0.0.5/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)     6646 2023-07-11 00:40:13.000000 f5project-0.0.5/README.md
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:42:08.531663 f5project-0.0.5/f5project/
--rw-r--r--   0 j3ymac     (501) staff       (20)    11747 2023-07-10 23:27:29.000000 f5project-0.0.5/f5project/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:42:08.532279 f5project-0.0.5/f5project.egg-info/
--rw-r--r--   0 j3ymac     (501) staff       (20)     7095 2023-07-11 00:42:08.000000 f5project-0.0.5/f5project.egg-info/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      212 2023-07-11 00:42:08.000000 f5project-0.0.5/f5project.egg-info/SOURCES.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-11 00:42:08.000000 f5project-0.0.5/f5project.egg-info/dependency_links.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-11 00:42:08.000000 f5project-0.0.5/f5project.egg-info/requires.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       10 2023-07-11 00:42:08.000000 f5project-0.0.5/f5project.egg-info/top_level.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-11 00:42:08.532639 f5project-0.0.5/setup.cfg
--rw-r--r--   0 j3ymac     (501) staff       (20)      763 2023-07-11 00:40:25.000000 f5project-0.0.5/setup.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 02:46:17.895207 f5project-0.0.6/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-07-11 00:45:10.000000 f5project-0.0.6/LICENSE
+-rw-r--r--   0 j3ymac     (501) staff       (20)     7095 2023-07-13 02:46:17.895011 f5project-0.0.6/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)     6646 2023-07-11 00:45:10.000000 f5project-0.0.6/README.md
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 02:46:17.858453 f5project-0.0.6/f5project/
+-rw-r--r--   0 j3ymac     (501) staff       (20)    11852 2023-07-13 02:44:43.000000 f5project-0.0.6/f5project/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 02:46:17.894726 f5project-0.0.6/f5project/create_f5project/
+-rw-r--r--   0 j3ymac     (501) staff       (20)      634 2023-07-13 02:44:43.000000 f5project-0.0.6/f5project/create_f5project/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 02:46:17.894472 f5project-0.0.6/f5project.egg-info/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     7095 2023-07-13 02:46:17.000000 f5project-0.0.6/f5project.egg-info/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      287 2023-07-13 02:46:17.000000 f5project-0.0.6/f5project.egg-info/SOURCES.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-13 02:46:17.000000 f5project-0.0.6/f5project.egg-info/dependency_links.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       65 2023-07-13 02:46:17.000000 f5project-0.0.6/f5project.egg-info/entry_points.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-13 02:46:17.000000 f5project-0.0.6/f5project.egg-info/requires.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       10 2023-07-13 02:46:17.000000 f5project-0.0.6/f5project.egg-info/top_level.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-13 02:46:17.895280 f5project-0.0.6/setup.cfg
+-rw-r--r--   0 j3ymac     (501) staff       (20)      891 2023-07-13 02:45:29.000000 f5project-0.0.6/setup.py
```

### Comparing `f5project-0.0.5/LICENSE` & `f5project-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `f5project-0.0.5/PKG-INFO` & `f5project-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5project
-Version: 0.0.5
+Version: 0.0.6
 Summary: F5 project
 Home-page: https://github.com/thejimmylin/f5project
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `f5project-0.0.5/README.md` & `f5project-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `f5project-0.0.5/f5project/__init__.py` & `f5project-0.0.6/f5project/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 import finlab
 import functions_framework
 import keyring
 from finlab.online.fugle_account import FugleAccount
 from flask import Request
 from keyrings.cryptfile.cryptfile import CryptFileKeyring
 from loguru import logger
+from .create_f5project import create_f5project
 
-__all__ = ["F5ProjectConfig", "F5Project"]
+__all__ = ["F5ProjectConfig", "F5Project", "create_f5project"]
 
 
-# Private
 class SimpleConfigParser(RawConfigParser):
     """A simple config parser
 
     It does not convert keys to lowercase and does not write empty lines.
     """
 
     def __init__(self):
@@ -93,49 +93,38 @@
 
     fugle_cert: str
     fugle_api_entry: str
     fugle_api_key: str
     fugle_api_secret: str
     fugle_account: str
 
-    @classmethod
-    def from_f5project_config(cls, config: "F5ProjectConfig") -> "FugleConfig":
-        fugle_cert = config.fugle_cert
-        fugle_api_entry = config.fugle_api_entry
-        fugle_api_key = config.fugle_api_key
-        fugle_api_secret = config.fugle_api_secret
-        fugle_account = config.fugle_account
-        return FugleConfig(fugle_cert, fugle_api_entry, fugle_api_key, fugle_api_secret, fugle_account)
-
     def to_file(self, data_dir: Path | None = None) -> Path:
         data_dir = data_dir or Path(tempfile.gettempdir())
         data_dir.mkdir(parents=True, exist_ok=True)
 
         cert_path = data_dir / "fugle-cert.p12"
         config_path = data_dir / "fugle-config.ini"
 
-        logger.info("Making Fugle certificate and config files")
+        logger.debug("Making Fugle certificate and config files")
         config_dict = {
             "Core": {"Entry": self.fugle_api_entry},
             "Cert": {"Path": str(FugleCert.from_string(self.fugle_cert).to_file(cert_path))},
             "Api": {"Key": self.fugle_api_key, "Secret": self.fugle_api_secret},
             "User": {"Account": self.fugle_account},
         }
         SimpleConfigParser().from_dict(config_dict).to_file(config_path)
+
         return config_path
 
 
-# Public
 @dataclasses.dataclass
 class F5ProjectConfig:
     """F5Project configuration
 
-    It contains all the configuration items required for F5Project.
-
-    The `sync_github_secrets` method is convenient for syncing the configuration to GitHub secrets.
+    It contains the configuration required for F5Project.
     """
 
     BINARY_FILE_FIELDS = ("fugle_cert",)
     JSON_FIELDS = ("gcf_service_account", "repo_synced")
 
     finlab_api_token: str
     fugle_account: str
@@ -146,193 +135,218 @@
     fugle_api_key: str
     fugle_api_secret: str
     fugle_market_api_key: str
     gcf_service_account: dict[str, str] | None = None
     repo_synced: dict[str, str] | None = None
 
     @classmethod
+    @property
     def all_field_names(cls) -> tuple[str]:
         return tuple(f.name for f in dataclasses.fields(F5ProjectConfig))
 
     @classmethod
     def from_json_or_env(cls, json_path: Path) -> "F5ProjectConfig":
         if json_path.exists():
             return cls.from_json(json_path)
         else:
             return cls.from_env()
 
     @classmethod
     def from_json(cls, json_path: Path) -> "F5ProjectConfig":
-        logger.info(f"Get `F5ProjectConfig` from `{json_path}`")
+        logger.debug(f"Getting `F5ProjectConfig` from `{json_path}`")
         all_values = json.loads(json_path.read_text())
 
         field_values = {}
-        for f in F5ProjectConfig.all_field_names():
+        for f in F5ProjectConfig.all_field_names:
             v = all_values.get(f, None)
             if f in cls.BINARY_FILE_FIELDS:
                 field_values[f] = FugleCert.from_file(json_path.parent / Path(v)).to_string()
             else:
                 field_values[f] = v
 
         return F5ProjectConfig(**field_values)
 
     @classmethod
     def from_env(cls) -> "F5ProjectConfig":
-        logger.info("Get `F5ProjectConfig` from environment variables")
+        logger.debug("Get `F5ProjectConfig` from environment variables")
         all_values: Any = dict(environ)
 
         field_values = {}
-        for f in F5ProjectConfig.all_field_names():
+        for f in F5ProjectConfig.all_field_names:
             v = all_values.get(f.upper(), None)
             if f in cls.JSON_FIELDS:
                 field_values[f] = json.loads(v or "null")
             else:
                 field_values[f] = v
 
         return F5ProjectConfig(**field_values)
 
-    def sync_github_secrets(self, gcf_function_target: str) -> None:
-        import github_secret_syncer
-
-        dotenv_path = Path(tempfile.gettempdir()) / "temp.env"
-        dotenv_path.write_text("")
-        for f in F5ProjectConfig.all_field_names():
-            if f in self.JSON_FIELDS:
-                dotenv.set_key(dotenv_path, f.upper(), json.dumps(getattr(self, f)))
-            else:
-                dotenv.set_key(dotenv_path, f.upper(), getattr(self, f))
-
-        dotenv.set_key(dotenv_path, "GCF_FUNCTION_TARGET", gcf_function_target)
-
-        if self.repo_synced is None:
-            raise ValueError("No `repo_synced` field in settings")
-
-        logger.info(f"Syncing secrets to {self.repo_synced['repo']} with dotenv file at {dotenv_path}")
-        github_secret_syncer.sync_secrets(dotenv_path, **self.repo_synced, delete_missing=True)
+    def to_fugle_config(self) -> FugleConfig:
+        args = [
+            self.fugle_cert,
+            self.fugle_api_entry,
+            self.fugle_api_key,
+            self.fugle_api_secret,
+            self.fugle_account,
+        ]
+        return FugleConfig(*args)
 
 
 @dataclasses.dataclass
 class F5Project:
     """F5 Project
 
-    The main class for F5 Project. After initialization, call `login` to log in Finlab and Fugle.
-
-    The `login` method will also do some pre-processing, including:
-    - Setting up Finlab file storage
-    - Setting up Fugle certificate and config files
-
-    After logging in, you can access `finlab.data` and call `get_fugle_account` to trade with Fugle APIs.
+    The main class for F5 Project. After initialization, call `setup` for configuring and logging in everything.
+    After that, you can access `finlab.data` and call `fugle_account` to retrieve Fugle account instance as you need.
 
-    The `run` method will request/call the `@gcf_function` decorated function locally.
+    The `call_gcf_endpoint` method calls the decorated function as a GCF endpoint locally.
     """
 
     config: F5ProjectConfig
     _gcf_endpoint: Callable | None = None
     _fugle_account: FugleAccount | None = None
 
     def __init__(self, config: F5ProjectConfig) -> None:
         self.config = config
 
-    def login(self, data_dir: Path | None = None) -> None:
-        # Pre-process
-        data_dir = data_dir or Path(tempfile.gettempdir())
+    def setup(self, data_dir: Path | None = None) -> None:
+        """A shortcut for `setup_finlab` and `setup_fugle`"""
+
+        self.setup_finlab(data_dir)
+        self.setup_fugle(data_dir)
+
+    def setup_finlab(self, data_dir: Path | None = None) -> None:
+        """Configuring and logging in Finlab"""
+
+        logger.debug("Configuring and logging in Finlab")
+
+        data_dir = data_dir if data_dir is not None else Path(tempfile.gettempdir())
         data_dir.mkdir(parents=True, exist_ok=True)
 
-        # Configure Finlab
-        finlab_storage_path = data_dir / "finlab_db"
-        logger.info(f"Configuring Finlab, setting up file storage at `{finlab_storage_path}`")
-        storage = finlab.data.FileStorage(str(finlab_storage_path))
+        storage_path = data_dir / "finlab_db"
+        logger.debug(f"Using Finlab file storage at `{storage_path}`")
+        storage = finlab.data.FileStorage(str(storage_path))
         finlab.data.set_storage(storage)
 
-        # Log in Finlab
-        logger.info("Logging in Finlab with `self.config.finlab_api_token`")
+        logger.debug("Logging in Finlab with `finlab_api_token`")
         finlab.login(self.config.finlab_api_token)
 
-        # Configure Fugle
-        logger.info("Configuring Fugle")
+    def setup_fugle(self, data_dir: Path | None = None) -> None:
+        """Configuring and logging in Fugle"""
+
+        logger.debug("Configuring and logging in Fugle")
+
+        data_dir = data_dir if data_dir is not None else Path(tempfile.gettempdir())
+        data_dir.mkdir(parents=True, exist_ok=True)
 
-        # Set keyring
+        logger.debug("Using `CryptFileKeyring` as keyring for Fugle login")
         file_keyring = CryptFileKeyring()
         raw_key = self.config.fugle_account
         hashed_key = md5(raw_key.encode("utf-8")).hexdigest()
         file_keyring.keyring_key = hashed_key
         keyring.set_keyring(file_keyring)
         keyring.set_password("fugle_trade_sdk:account", self.config.fugle_account, self.config.fugle_password)
         keyring.set_password("fugle_trade_sdk:cert", self.config.fugle_account, self.config.fugle_cert_password)
 
-        # Make Fugle certificate and config files
-        config_path = FugleConfig.from_f5project_config(self.config).to_file(data_dir)
+        config_path = self.config.to_fugle_config().to_file(data_dir)
 
-        # Log in Fugle
-        logger.info(f"Logging in Fugle with `{config_path}` and `self.config.fugle_market_api_key`")
+        logger.debug(f"Logging in Fugle with config file `{config_path}` and `fugle_market_api_key`")
         fugle_account = FugleAccount(config_path, self.config.fugle_market_api_key)
         self._fugle_account = fugle_account
 
-    def get_fugle_account(self) -> FugleAccount:
+    def fugle_account(self) -> FugleAccount:
+        """Get the Fugle account instance."""
+
         if self._fugle_account is None:
             raise ValueError("The project is not logged in yet. Please call `login` first.")
 
         return self._fugle_account
 
-    def sync_github_secrets(self) -> None:
-        if self._gcf_endpoint is None:
-            raise ValueError("No GCF endpoint registered")
+    def gcf_endpoint(self, func: Callable) -> Callable:
+        """Decorator for registering a function as a GCF endpoint"""
 
-        self.config.sync_github_secrets(gcf_function_target=self._gcf_endpoint.__name__)
+        logger.debug(f"Registering `{func.__name__}` as GCF endpoint")
 
-    def gcf_endpoint(self, func):
-        logger.info(f"Registering `{func.__name__}` as GCF endpoint")
+        if self._gcf_endpoint is not None:
+            raise ValueError("Only one GCF endpoint is allowed")
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
-            from_request = len(args) > 0 and isinstance(args[0], Request)
+            from_request = len(args) == 1 and isinstance(args[0], Request)
             if from_request:
                 request = args[0]
                 payload = request.get_json(force=True)
                 return func(**payload)
-            else:
-                return func(*args, **kwargs)
 
-        if self._gcf_endpoint is None:
-            self._gcf_endpoint = wrapper
-        else:
-            raise ValueError("Only one GCF endpoint is allowed")
+            return func(*args, **kwargs)
+
+        self._gcf_endpoint = wrapper
         return wrapper
 
-    def run_locally(self, with_server: bool | None = None, params: dict | None = None) -> Any:
-        """Request/call the GCF function locally
+    def call_gcf_endpoint(self, directly: bool = False, params: dict = {}) -> Any:
+        """Call the GCF endpoint
+
+        If `directly = False`, simulate performing a request to the GCF endpoint.
+        Otherwise, call the decorated function directly.
 
-        When `with_server` is `True`, it will simulate performing a request to the GCF endpoint.
-        Otherwise, it will call the GCF function directly.
+        If `params` is specified, pass it by request body or as `**params` according to `with_server`.
 
-        When `params` is specified, it will be passed to the GCF function as JSON.
+        They can also be specified by CLI arguments:
+        - `--directly` or `-d` for `directly = True`
+        - `--params '{"foo": "bar"}'` or `-p '{"foo": "bar"}'` for `params = {"foo": "bar"}`
 
-        CLI args `--with-server` (`-w`) and `--params` (`-p`) will be used,
-        if the arguments are not specified explicitly.
+        CLI arguments have higher priority than the arguments passed to this method.
         """
+
         if self._gcf_endpoint is None:
             raise ValueError("No GCF endpoint registered")
 
-        # Get args from CLI
         parser = argparse.ArgumentParser()
-        parser.add_argument("-w", "--with-server", action="store_true", help="Run with server or not")
-        parser.add_argument("-p", "--params", type=json.loads, default={}, help="Run with these JSON params")
+        parser.add_argument("-d", "--directly", action="store_true", help="Call directly or not")
+        parser.add_argument("-p", "--params", type=json.loads, help="Call with what params")
         args = parser.parse_args()
 
-        # If not specified, use args
-        with_server = with_server if with_server is not None else args.with_server
-        params = params if params is not None else args.params
-        logger.debug(f"`{with_server = }`, `{params = }`")
-
-        if with_server:
-            # Request GCF endpoint
-            logger.debug(f"Requesting `{self._gcf_endpoint.__name__}` with `json = {params}`")
+        directly = args.directly or directly
+        params = args.params or params
+
+        if directly:
+            logger.info(f"Calling `{self._gcf_endpoint.__name__}` with `**params` where `params = {params}`")
+            result = self._gcf_endpoint(**params)
+        else:
+            logger.info(f"Requesting `{self._gcf_endpoint.__name__}` with `json = {params}`")
             client = functions_framework.create_app(target=self._gcf_endpoint.__name__).test_client()
             response = client.post("/", json=params)
             result = response.get_json()
-        else:
-            # Call decorated function directly
-            logger.debug(f"Calling `{self._gcf_endpoint.__name__}` with `{params}` as kwargs")
-            result = self._gcf_endpoint(**params)
 
         logger.success(f"{result = }")
         return result
+
+    def setup_github_secrets(self) -> None:
+        """Set up GitHub secrets for the project
+
+        To ensure the secrets are always up-to-date, you may want to call this method in your Git pre-push hook.
+        """
+
+        import github_secret_syncer
+
+        config = self.config
+
+        if config.repo_synced is None:
+            raise ValueError("No `repo_synced` field in settings")
+
+        if self._gcf_endpoint is None:
+            raise ValueError("No GCF endpoint registered")
+
+        dotenv_path = Path(tempfile.gettempdir()) / "temp.env"
+        dotenv_path.write_text("")
+
+        for f in config.all_field_names:
+            if f in config.JSON_FIELDS:
+                dotenv.set_key(dotenv_path, f.upper(), json.dumps(getattr(config, f)))
+            else:
+                dotenv.set_key(dotenv_path, f.upper(), getattr(config, f))
+
+        dotenv.set_key(dotenv_path, "GCF_FUNCTION_TARGET", self._gcf_endpoint.__name__)
+
+        logger.debug(f"Synchronizing secrets to {config.repo_synced['repo']} with dotenv file at {dotenv_path}")
+
+        github_secret_syncer.sync_secrets(dotenv_path, **config.repo_synced, delete_missing=True)
```

### Comparing `f5project-0.0.5/f5project.egg-info/PKG-INFO` & `f5project-0.0.6/f5project.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5project
-Version: 0.0.5
+Version: 0.0.6
 Summary: F5 project
 Home-page: https://github.com/thejimmylin/f5project
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `f5project-0.0.5/setup.py` & `f5project-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import setuptools
 
 from pathlib import Path
 
 base_dir = Path(__file__).parent.resolve()
 long_description = (base_dir / "README.md").read_text(encoding="utf-8")
 
+
 setuptools.setup(
     name="f5project",
-    version="0.0.5",
+    version="0.0.6",
     install_requires=[
         "github-secret-syncer",
     ],
     author="thejimmylin",
     author_email="b00502013@gmail.com",
     description="F5 project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thejimmylin/f5project",
     packages=setuptools.find_packages(),
+    entry_points={
+        "console_scripts": [
+            "create-f5project = f5project:create_f5project",
+        ],
+    },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.10",
 )
```

