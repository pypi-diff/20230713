# Comparing `tmp/titan-iris-0.9.2.dev5.tar.gz` & `tmp/titan-iris-0.9.3.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.9.2.dev5.tar", last modified: Thu Jul 13 08:48:33 2023, max compression
+gzip compressed data, was "titan-iris-0.9.3.dev99.tar", last modified: Thu Jul 13 14:39:05 2023, max compression
```

## Comparing `titan-iris-0.9.2.dev5.tar` & `titan-iris-0.9.3.dev99.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 08:48:33.345836 titan-iris-0.9.2.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.337836 titan-iris-0.9.2.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.337836 titan-iris-0.9.2.dev5/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    26994 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18417 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 08:48:33.000000 titan-iris-0.9.2.dev5/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:48:33.341836 titan-iris-0.9.2.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-13 08:48:19.000000 titan-iris-0.9.2.dev5/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.743394 titan-iris-0.9.3.dev99/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-07-13 14:39:05.743394 titan-iris-0.9.3.dev99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 14:39:05.743394 titan-iris-0.9.3.dev99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.731394 titan-iris-0.9.3.dev99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.735394 titan-iris-0.9.3.dev99/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.735394 titan-iris-0.9.3.dev99/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.739394 titan-iris-0.9.3.dev99/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29994 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/safe_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.739394 titan-iris-0.9.3.dev99/src/iris/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/utils/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/utils/display_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/utils/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/utils/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/src/iris/sdk/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.743394 titan-iris-0.9.3.dev99/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-07-13 14:39:05.000000 titan-iris-0.9.3.dev99/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-13 14:39:05.000000 titan-iris-0.9.3.dev99/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:39:05.000000 titan-iris-0.9.3.dev99/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 14:39:05.000000 titan-iris-0.9.3.dev99/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-13 14:39:05.000000 titan-iris-0.9.3.dev99/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 14:39:05.000000 titan-iris-0.9.3.dev99/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.743394 titan-iris-0.9.3.dev99/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-13 14:38:51.000000 titan-iris-0.9.3.dev99/tests/test_sdk.py
```

### Comparing `titan-iris-0.9.2.dev5/.gitignore` & `titan-iris-0.9.3.dev99/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2.dev5/Dockerfile` & `titan-iris-0.9.3.dev99/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2.dev5/PKG-INFO` & `titan-iris-0.9.3.dev99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.9.2.dev5
+Version: 0.9.3.dev99
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.9.2.dev5/README.md` & `titan-iris-0.9.3.dev99/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2.dev5/setup.py` & `titan-iris-0.9.3.dev99/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,16 @@
         "tqdm ~=4.64.1",
         "wget ~= 3.2",
         "jmespath ~= 1.0",
         "tritonclient[http] ~= 2.30.0",
         "numpy >= 1.20.0",
         "tabulate ~= 0.9.0",
         "trogon ~= 0.2.1",
+        "shortuuid ~= 1.0.11",
+        "einops ~= 0.6.1",
     ],
     entry_points={"console_scripts": ["iris = iris.main:main"]},
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     use_scm_version={"root": "..", "local_scheme": "no-local-version"},
     setup_requires=["setuptools_scm"],
```

### Comparing `titan-iris-0.9.2.dev5/src/iris/config.yaml` & `titan-iris-0.9.3.dev99/src/iris/config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 auth0_audience: "https://seshat/"
 auth0_flow: "device"
 
 authenticate: true
 telemetry: true
 log_level: WARNING
 
-base_image: "tytn/hephaestus:latest"
+hephaestus_image: "tytn/hephaestus:latest"
+fabulinus_image: "tytn/fabulinus:fastapi-launch"
```

### Comparing `titan-iris-0.9.2.dev5/src/iris/gradio/run.py` & `titan-iris-0.9.3.dev99/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2.dev5/src/iris/main.py` & `titan-iris-0.9.3.dev99/src/iris/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
 import typer
 import yaml
 from trogon import Trogon
 from typer.main import get_group
 import iris.sdk as sdk
 
-from .sdk.utils import exception_to_json_error, valid_qlora
+from .sdk.utils.display_utils import exception_to_json_error
+from .sdk.utils.utils import stream_generate
+from .sdk.utils.docker_utils import list_running_containers, stop_and_remove_container
 
 logger = getLogger(__name__)
 logger.setLevel(sdk.conf_mgr.LOG_LEVEL)
 
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                   sdk CLI Module                                                     #
 
@@ -455,14 +457,15 @@
                 print("Label indices must start at zero")
                 raise typer.Abort()
 
             label_names_list = [label_names_dict[i] for i in range(label_names_num)]
             flags.update({"label_names": label_names_list})
 
     elif task == "language_modelling" or task == "language_modeling":
+        task = "language_modelling"
         # sequence of task specific flags
         # if the flag shouldn't be accepted, set error_message to the error string to print.
         # if it should be, and you want to warn, print, but don't set error_message
         error_message = False
         if type == "athena":
             error_message = "Knowledge distillation is not yet supported for language modelling."
         if label_column and len(label_column):
@@ -472,31 +475,19 @@
         if num_labels is not None:
             print("num_labels is not necessary for language modelling tasks")
         if label_names is not None and len(label_names) > 0:
             print("label_names is not necessary for language modelling tasks")
         if has_negative:
             print("has_negative is not necessary for language modelling tasks")
 
-        if no_qlora and valid_qlora(model):  # If want to disable qlora, but qlora is available:
-            print(f"QLoRA manually disabled for {model}")
-            use_qlora = False
-        elif not no_qlora and not valid_qlora(model):  # If qlora isn't explicitly disabled, but is not available.
-            print(f"QLoRA not available for {model}. Proceeding without QLoRA.")
-            use_qlora = False
-        elif no_qlora and not valid_qlora(model):  # Qlora disabled, but it wasn't available anyways.
-            use_qlora = False
-        else:  # Qlora not explicitly disabled, and qlora is available.
-            print("QLoRA is available and will be used.")
-            use_qlora = True
-
         if error_message:
             print(error_message)
             raise typer.Abort()
         else:
-            flags.update({"text_fields": text_fields, "use_qlora": use_qlora})
+            flags.update({"text_fields": text_fields, "no_qlora": no_qlora})
     else:
         print(f"Unrecognised task {task}")
         raise typer.Abort()
 
     if num_epochs >= 99:
         logging.warning(
             "Woah there cowboy, that's a mighty high number of epochs you got there. "
@@ -750,9 +741,92 @@
     except Exception:
         print({"status": "Failed", "message": "data should be a json string"})
         raise typer.Abort()
     response = sdk.query(artefact_id, data)
     print(response)
 
 
+@main.command()
+def takeoff(
+    model_folder_path: str = typer.Option("...", "--model", help="the path to the model folder"),
+    device: str = typer.Option("cpu", "--device", help="the device to run the model on"),
+    is_infer: bool = typer.Option(False, "--infer", help="if is querying the server"),
+    is_shutdown: bool = typer.Option(False, "--shutdown", help="if is shutting down the server"),
+    port: int = typer.Option(8000, "--port", "-p", help="The port to run the server on."),
+):
+    """Takeoff a model.
+
+    Args:
+        model_folder_path (str, optional): the path to the model folder.
+        device (str, optional): the device to run the model on. Defaults to "cpu".
+        is_infer (bool, optional): if is querying the server. Defaults to False.
+        is_shutdown (bool, optional): if is shutting down the server. Defaults to False.
+        port (int, optional): The port to run the server on. Defaults to 8000.
+    """
+    assert device in {"cpu", "cuda"}, "device should be either cpu or cuda"
+
+    try:
+        if is_infer:
+            chat_cli()
+        elif is_shutdown:
+            shutdown_cli()
+        else:
+            sdk.takeoff(model_folder_path=model_folder_path, device=device, port=port)
+    except Exception as e:
+        print(e)
+        raise typer.Abort()
+
+
+def shutdown_cli():
+    """Helper function to shutdown the server."""
+    containers = list_running_containers()
+    for idx, container in enumerate(containers, start=1):
+        typer.secho(f"{idx}. {container.name}", fg=typer.colors.BRIGHT_CYAN)
+
+    container_idx = int(
+        typer.prompt(
+            typer.style("Enter the index of the container you want to stop and remove: ", fg=typer.colors.BRIGHT_BLUE)
+        )
+    )
+
+    # Check if the index is valid, and if so, stop and remove the container
+    if 1 <= container_idx <= len(containers):
+        stop_and_remove_container(containers[container_idx - 1].name)  # List indices are 0-based
+    else:
+        typer.secho("Invalid index.", fg=typer.colors.RED, bold=True)
+
+
+def chat_cli():
+    """Helper function to run the chatbot CLI demo for iris takeoff."""
+    typer.secho("Welcome to the chatbot CLI demo!", fg=typer.colors.MAGENTA, bold=True)
+    typer.secho(
+        "This command-line interface allows you to engage in a conversation with your local deployed model",
+        fg=typer.colors.BRIGHT_CYAN,
+    )
+
+    typer.secho(
+        "\nBefore you can start chatting, you'll need to spin up a server for your model.", fg=typer.colors.YELLOW
+    )
+    typer.secho("Please use the following command: ", fg=typer.colors.YELLOW, nl=False)
+    typer.secho("`iris takeoff --model <model_folder_path>`", fg=typer.colors.YELLOW, bold=True)
+    typer.secho("Remember to replace <model_folder_path> with the actual path to your model.", fg=typer.colors.YELLOW)
+
+    typer.secho(
+        "\nYou're now all set to start chatting! Just type your query and press Enter.", fg=typer.colors.BRIGHT_CYAN
+    )
+    typer.secho("When you want to quit, simply type ", fg=typer.colors.BRIGHT_CYAN, nl=False)
+    typer.secho("'quit'", fg=typer.colors.RED, bold=True, nl=False)
+    typer.secho(" and press Enter.\n", fg=typer.colors.BRIGHT_CYAN)
+
+    while True:
+        user_input = typer.prompt(typer.style("User", fg=typer.colors.BRIGHT_BLUE))
+        if user_input.lower() == "quit":
+            break
+        typer.secho("Bot: ", fg=typer.colors.BRIGHT_MAGENTA)
+        stream_generate(user_input)  # You need to implement generate_response function.
+        print("\n")
+
+    typer.secho("Thank you for using the chatbot!", fg=typer.colors.BRIGHT_BLUE, bold=True)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `titan-iris-0.9.2.dev5/src/iris/sdk/auth_utils.py` & `titan-iris-0.9.3.dev99/src/iris/sdk/utils/auth_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 from auth0.v3.authentication.token_verifier import (
     AsymmetricSignatureVerifier,
     TokenVerifier,
 )
 from requests import Response
 from rich import print
 
-from .conf_manager import conf_mgr
+from ..conf_manager import conf_mgr
 
 # internal imports
-from .exception import (
+from ..exception import (
     EndpointNotFoundError,
     InvalidLoginError,
     KeyFileDoesntExistError,
     KeyFileExpiredError,
 )
 
 # Logger config
```

### Comparing `titan-iris-0.9.2.dev5/src/iris/sdk/conf_manager.py` & `titan-iris-0.9.3.dev99/src/iris/sdk/conf_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,21 @@
     CREDENTIALS_PATH = Path.home() / config.keyfile_name
     LOG_LEVEL = os.environ.get("IRIS_LOG_LEVEL", config.log_level)
     # pull the credentials flow from the environment (if it's set, otherwise use the config setting)
     # options are "device" and "client_credentials"
     CREDENTIALS_FLOW = os.environ.get("IRIS_OAUTH_FLOW", config.auth0_flow)
 
     # base image config from config
-    BASE_IMAGE = config.base_image
+    HEPHAESTUS_IMAGE = config.hephaestus_image
+
+    # fastapi image config from config
+    FABULINUS_IMAGE = config.fabulinus_image
+
+    # cache directory
+    cache_dir = Path.home() / ".iris_cache"
 
     base = get("IRIS_BASE", "test_base", "stag_base", "prod_base", config, ENVIRONMENT)
 
     # pull base url from environment if set, otherwise use the defaults in the config.
     runner_url = urljoin(base, config.runner_path)
     metrics_url = urljoin(base, config.metrics_path)
```

### Comparing `titan-iris-0.9.2.dev5/src/iris/sdk/exception.py` & `titan-iris-0.9.3.dev99/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2.dev5/src/iris/sdk/iris_sdk.py` & `titan-iris-0.9.3.dev99/src/iris/sdk/iris_sdk.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,45 +14,41 @@
 import numpy as np
 
 # for iris pull
 import requests
 import tritonclient.http
 from rich import print
 
-# internal imports
-from .auth_utils import auth, handle_bad_response
 from .conf_manager import conf_mgr
 from .exception import (
     ArtefactNotFoundError,
     ArtefactTypeInferError,
     ArtefactTypeNotAFolderError,
     BadRequestError,
     InvalidCommandError,
     InvalidDatasetFormatError,
     JobStillRunningError,
     MissingTokenizerError,
     UnknownFamilyError,
     UnsafeTensorsError,
     UploadOnPostError,
 )
-from .utils import (
-    download_model,
-    dump,
-    handle_iris_get_response,
-    make_targz,
-    print_status_dict_results,
-    pull_image,
-    telemetry_decorator,
-    upload_from_file,
-)
+
+# internal imports
+from .utils.auth_utils import auth, handle_bad_response
+from .utils.display_utils import dump, handle_iris_get_response, print_status_dict_results
+from .utils.docker_utils import check_docker, pull_fastapi_image, pull_image
+from .utils.io_utils import download_model, make_targz, upload_from_file
+from .utils.telemetry_utils import telemetry_decorator
+from .utils.utils import valid_qlora
 
 try:
-    from importlib import metadata
+    from importlib import metadata as import_metadata
 except ImportError:  # for Python<3.8
-    import importlib_metadata as metadata
+    import importlib_metadata as import_metadata
 
 
 # ───────────────────────────────────────────────────── imports ────────────────────────────────────────────────────── #
 
 
 # Whether to use tqdm for progress bars
 TQDM = True
@@ -122,32 +118,56 @@
         headers = {}
     endpoint = "experiment"
     # detype the flags, so we can send them
     payload = {k: str(val) if val is not None else None for k, val in flags.items()}
     logger.debug(f"Dispatching job with payload {payload}")
     url = urljoin(conf_mgr.runner_url, f"{endpoint}/")
 
+    local_family = None
     for local_artefact_field in ["model", "dataset"]:
         local_artefact = payload[local_artefact_field]
         if os.path.exists(local_artefact):
             print(
                 f"Local {local_artefact_field} found. \
                 If you intended to use a huggingface module then rename the local file."
             )  # todo
-            local_uuid = upload(
+            server_artefact = upload(
                 name=local_artefact.split("/")[-1],
                 src=local_artefact,
                 description="Experiment model",
                 internal_artefact_type=local_artefact_field,
             )  # todo add more data to the uploaded model?
-            if local_uuid:
-                payload[local_artefact_field] = local_uuid
+            if server_artefact:
+                payload[local_artefact_field] = server_artefact["uuid"]
+                if local_artefact_field == "model":
+                    local_family = json.loads(server_artefact["metadata"])["local_model_family"]
             else:
                 raise UploadOnPostError
 
+    if flags["task"] == "language_modelling":
+        if flags["no_qlora"] and valid_qlora(flags["model"], local_family):
+            # If want to disable qlora, but qlora is available:
+            print(f"QLoRA manually disabled for {flags['model']}")
+            use_qlora = False
+        elif not flags["no_qlora"] and not valid_qlora(flags["model"], local_family):
+            # If qlora isn't explicitly disabled, but is not available.
+            print(f"QLoRA not available for {flags['model']}. Proceeding without QLoRA.")
+            use_qlora = False
+        elif flags["no_qlora"] and not valid_qlora(flags["model"], local_family):
+            # Qlora disabled, but it wasn't available anyways.
+            use_qlora = False
+        else:  # Qlora not explicitly disabled, and qlora is available.
+            print("QLoRA is available and will be used.")
+            use_qlora = True
+        payload.pop("no_qlora")
+    else:
+        use_qlora = False
+    payload.update({"use_qlora": use_qlora})
+    payload.update({"local_model_family": local_family})
+
     headers.update({"Authorization": f"Bearer {conf_mgr.access_token}"})
     response = requests.post(url=url, headers=headers, data=payload)
     if not response.ok:
         raise handle_bad_response(response, endpoint)  # already returns json object
     else:
         dumped_response = dump(response)
         if json_output:
@@ -546,15 +566,15 @@
                 datetime.strptime(existing_artefact["time_created"], "%Y-%m-%dT%H:%M:%S.%fZ").strftime(
                     "%d-%m-%Y %H:%M:%S"
                 )
             )
             # Return artefact data for found/existing artefact.
             if not internal_artefact_type:
                 print(f"Artefact was already uploaded at {created_time} with ID: {existing_artefact['uuid']}")
-            return existing_artefact["uuid"]
+            return existing_artefact
 
     data = post_req_response.json()["artefact"]
     art_uuid = data["uuid"]
     endpoint = "artefact/link/" + art_uuid + "/upload"
     url = urljoin(conf_mgr.runner_url, f"{endpoint}")
     logger.debug(f"Getting link from {url}")
     get_link_resp = requests.get(url=url, headers=headers)
@@ -583,15 +603,15 @@
                 print(json.dumps(result, indent=4))
             else:
                 print(
                     f"Upload validated. This {art_type} can now be used in experiments \
                     by referring to it by UUID: {art_uuid}"
                 )
                 print(f"Alternatively, you can continue to use the {art_type}'s filepath.")
-            return art_uuid
+            return data
     else:
         print("Upload failed")
         for key, value in upload_response.items():
             if isinstance(value, Path):
                 upload_response[key] = str(value)
         return dump(upload_response)
 
@@ -690,18 +710,18 @@
     if failed_packages:
         print(
             "To use the safetensors convert, you must have the following packages installed: ",
             failed_packages,
         )
         print("NB: These packages do not need to be installed with gpu support.")
         return
-    if metadata.version("transformers") < "4.27.0":
+    if import_metadata.version("transformers") < "4.27.0":
         print(
             "To use makesafe you must have transformers >= 4.27.0. You currently have "
-            + metadata.version("transformers")
+            + import_metadata.version("transformers")
         )
         return
     # else
     from .safe_convert import do_convert
 
     do_convert(model)
 
@@ -715,7 +735,40 @@
     """Simple inference test."""
     endpoint = "inference-session"
     url = urljoin(conf_mgr.runner_url, f"{endpoint}/{artefact}")
     headers = {"Authorization": f"Bearer {conf_mgr.access_token}"}
 
     response = requests.post(url=url, headers=headers, json=data)
     return response.json()
+
+
+@auth
+@telemetry_decorator
+def takeoff(model_folder_path: str, device: str, port: int = 8000):
+    """Takeoff the model to fastapi server.
+
+    This function will pull the fastapi image. Start the docker container and mount the model folder.
+    Start the fastapi server and expose the port 8000.
+
+    Args:
+        model_folder_path (str): The path of the model folder to be mounted.
+        device (str): The device to run the model on.
+        port (int, optional): The port to expose the fastapi server. Defaults to 8000.
+    """
+    logger.info("Pulling image from the server")
+
+    # check if docker is installed
+    try:
+        check_docker()
+        logger.info("Docker is running.")
+    except EnvironmentError as e:
+        print(e)
+
+    # pull the fastapi image, notice this will also run the docker container mounting the model folder
+    pull_fastapi_image(
+        image_name=conf_mgr.FABULINUS_IMAGE,
+        model_folder_path=model_folder_path,
+        device=device,
+        port=port,
+    )
+
+    logger.info("All done!")
```

### Comparing `titan-iris-0.9.2.dev5/src/iris/sdk/safe_convert.py` & `titan-iris-0.9.3.dev99/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.9.2.dev5/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.9.3.dev99/src/titan_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.9.2.dev5
+Version: 0.9.3.dev99
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.9.2.dev5/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.9.3.dev99/src/titan_iris.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,20 +9,24 @@
 setup.py
 src/iris/__init__.py
 src/iris/config.yaml
 src/iris/main.py
 src/iris/gradio/__init__.py
 src/iris/gradio/run.py
 src/iris/sdk/__init__.py
-src/iris/sdk/auth_utils.py
 src/iris/sdk/conf_manager.py
 src/iris/sdk/exception.py
 src/iris/sdk/iris_sdk.py
 src/iris/sdk/safe_convert.py
-src/iris/sdk/utils.py
+src/iris/sdk/utils/auth_utils.py
+src/iris/sdk/utils/display_utils.py
+src/iris/sdk/utils/docker_utils.py
+src/iris/sdk/utils/io_utils.py
+src/iris/sdk/utils/telemetry_utils.py
+src/iris/sdk/utils/utils.py
 src/titan_iris.egg-info/PKG-INFO
 src/titan_iris.egg-info/SOURCES.txt
 src/titan_iris.egg-info/dependency_links.txt
 src/titan_iris.egg-info/entry_points.txt
 src/titan_iris.egg-info/requires.txt
 src/titan_iris.egg-info/top_level.txt
 tests/test_cli.py
```

### Comparing `titan-iris-0.9.2.dev5/tests/test_cli.py` & `titan-iris-0.9.3.dev99/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from iris.sdk import download as download
 from iris.sdk.exception import (
     BadRequestError,
     EndpointNotFoundError,
     InvalidCommandError,
     InvalidLoginError,
 )
-from iris.sdk.utils import upload_from_file as upload_from_file
+from iris.sdk.utils.io_utils import upload_from_file
 
 from typer.testing import CliRunner
 
 from iris.main import main
 import json
 
 runner = CliRunner()
```

### Comparing `titan-iris-0.9.2.dev5/tests/test_sdk.py` & `titan-iris-0.9.3.dev99/tests/test_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
         patch_response = mocker.Mock()
         patch_response.json = mocker.Mock(return_value={"status": "success"})
         patch_response.ok = True
         patch_mock = mocker.patch("requests.patch", return_value=patch_response)
         mocker.patch("requests.patch", patch_mock)
 
-        result = upload(json_output=True, src=temp_dir_path, name="test_name", description="test_description")
+        result = upload(json_output=True, src=temp_dir_path, name="test_name", description="test_description")["uuid"]
         try:
             json.loads(result)
         except:
             pytest.fail("upload() did not return valid JSON")
 
 
 # --------------------------------------    iris get     -------------------------------------- #
```

