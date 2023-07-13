# Comparing `tmp/wslshot-0.0.5.tar.gz` & `tmp/wslshot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wslshot-0.0.5.tar", last modified: Fri Jul  7 20:31:58 2023, max compression
+gzip compressed data, was "wslshot-0.0.6.tar", last modified: Thu Jul 13 12:05:14 2023, max compression
```

## Comparing `wslshot-0.0.5.tar` & `wslshot-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 20:31:58.066498 wslshot-0.0.5/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-07-07 11:34:57.000000 wslshot-0.0.5/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6779 2023-07-07 20:31:58.066498 wslshot-0.0.5/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6339 2023-07-07 20:06:37.000000 wslshot-0.0.5/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-07 20:31:58.066498 wslshot-0.0.5/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      990 2023-07-07 20:31:39.000000 wslshot-0.0.5/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 20:31:58.066498 wslshot-0.0.5/wslshot/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 12:41:35.000000 wslshot-0.0.5/wslshot/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15616 2023-07-07 20:30:52.000000 wslshot-0.0.5/wslshot/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 20:31:58.066498 wslshot-0.0.5/wslshot.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6779 2023-07-07 20:31:58.000000 wslshot-0.0.5/wslshot.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      249 2023-07-07 20:31:58.000000 wslshot-0.0.5/wslshot.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-07 20:31:58.000000 wslshot-0.0.5/wslshot.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       48 2023-07-07 20:31:58.000000 wslshot-0.0.5/wslshot.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        6 2023-07-07 20:31:58.000000 wslshot-0.0.5/wslshot.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-07-07 20:31:58.000000 wslshot-0.0.5/wslshot.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-13 12:05:14.497689 wslshot-0.0.6/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-07-07 11:34:57.000000 wslshot-0.0.6/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6782 2023-07-13 12:05:14.497689 wslshot-0.0.6/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6342 2023-07-13 11:15:32.000000 wslshot-0.0.6/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-13 12:05:14.497689 wslshot-0.0.6/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      990 2023-07-13 12:04:39.000000 wslshot-0.0.6/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-13 12:05:14.497689 wslshot-0.0.6/wslshot/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 12:41:35.000000 wslshot-0.0.6/wslshot/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16184 2023-07-13 12:01:49.000000 wslshot-0.0.6/wslshot/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-13 12:05:14.497689 wslshot-0.0.6/wslshot.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6782 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      249 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       48 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        6 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/top_level.txt
```

### Comparing `wslshot-0.0.5/LICENSE` & `wslshot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wslshot-0.0.5/PKG-INFO` & `wslshot-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslshot
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/sderev/wslshot
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/wslshot
 Project-URL: Issues, http://github.com/sderev/wslshot/issues
 Project-URL: Changelog, https://github.com/sderev/wslshot/releases
 Requires-Python: >=3.8
@@ -108,15 +108,15 @@
 Remember to consult your VM provider's documentation for specific instructions on how to set up shared folders.
 
 ## Configuration of `wslshot`
 
 Before using `wslshot`, you may want to configure it to suit your needs. You can do this using the `config` command:
 
 ```bash
-wslshot config --source /path/to/source --auto-stage-enabled True --output-format HTML
+wslshot configure --source /path/to/source --auto-stage-enabled True --output-format HTML
 ```
 
 This command allows you to set various options:
 
 * **`--source` or `-s`**: This option lets you specify the default source directory where `wslshot` will look for screenshots.
 
 * **`--auto-stage-enabled`**: This option lets you control whether screenshots are automatically staged when copied to a git repository. By default, this option is set to `False`. If this option is set to `True`, any screenshot copied to a git repo will automatically be staged for commit.
```

### Comparing `wslshot-0.0.5/README.md` & `wslshot-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 Remember to consult your VM provider's documentation for specific instructions on how to set up shared folders.
 
 ## Configuration of `wslshot`
 
 Before using `wslshot`, you may want to configure it to suit your needs. You can do this using the `config` command:
 
 ```bash
-wslshot config --source /path/to/source --auto-stage-enabled True --output-format HTML
+wslshot configure --source /path/to/source --auto-stage-enabled True --output-format HTML
 ```
 
 This command allows you to set various options:
 
 * **`--source` or `-s`**: This option lets you specify the default source directory where `wslshot` will look for screenshots.
 
 * **`--auto-stage-enabled`**: This option lets you control whether screenshots are automatically staged when copied to a git repository. By default, this option is set to `False`. If this option is set to `True`, any screenshot copied to a git repo will automatically be staged for commit.
```

### Comparing `wslshot-0.0.5/setup.py` & `wslshot-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

### Comparing `wslshot-0.0.5/wslshot/cli.py` & `wslshot-0.0.6/wslshot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Features:
 
 - Fetch and copy the most recent screenshots using the 'wslshot' command.
 - Specify the number of screenshots to be processed with the '--count' option.
 - Customize the source directory using '--source'.
 - Customize the destination directory using '--destination'.
 - Choose your preferred output format (Markdown, HTML, or raw path) with the '--output' option.
-- Configure default settings with the 'config' subcommand.
+- Configure default settings with the 'configure' subcommand.
 
 For detailed usage instructions, use 'wslshot --help' or 'wslshot [command] --help'.
 """
 
 
 import datetime
 import json
@@ -103,23 +103,25 @@
 
     # Output format
     if output_format is None:
         output_format = config["default_output_format"]
 
     if output_format.casefold() not in ("markdown", "html", "plain_text"):
         print(f"Invalid output format: {output_format}")
-        print("Valid options are: markdown, HTML, plain_text")
+        print("Valid options are: markdown, html, plain_text")
         sys.exit(1)
 
     # Copy the screenshot(s) to the destination directory.
     source_screenshots = get_screenshots(source, count)
     copied_screenshots = copy_screenshots(source_screenshots, destination)
 
     # Automatically stage the screenshot(s) if the destination is a git repo.
-    if is_git_repo():
+    # But only if auto_stage is enabled in the config.
+    print(f"{config['auto_stage_enabled']=}")
+    if is_git_repo() and bool(config["auto_stage_enabled"]):
         stage_screenshots(copied_screenshots)
         copied_screenshots = format_screenshots_path_for_git(copied_screenshots)
 
     # Print the screenshot(s)'s path in the specified format.
     print_formatted_path(output_format, copied_screenshots)
 
 
@@ -148,15 +150,17 @@
 
         if len(screenshots) < count:
             raise ValueError(
                 f"Only {len(screenshots)} screenshot(s) found in the source directory:"
                 f" {source}."
             )
     except ValueError as error:
-        click.echo(f"{click.style('An error occurred while fetching the screenshot(s).',fg='red')}")
+        click.echo(
+            f"{click.style('An error occurred while fetching the screenshot(s).',fg='red')}"
+        )
         click.echo(f"{error}\n")
         sys.exit(1)
 
     return tuple(screenshots)
 
 
 def copy_screenshots(screenshots: Tuple[Path], destination: str) -> Tuple[Path]:
@@ -184,16 +188,17 @@
     """
     Rename the screenshot to the current date and time.
 
     Returns:
 
     - The new screenshot name.
     """
+    # Rename screenshot with ISO 8601 date and time, and append the index.
     return (
-        f"screenshot_{datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}_{idx}.png"
+        f"screenshot_{datetime.datetime.now().isoformat(timespec='seconds')}_{idx}.png"
     )
 
 
 def stage_screenshots(screenshots: Tuple[Path]) -> None:
     """
     Automatically stage the screenshot(s) if the destination is a git repo.
 
@@ -202,15 +207,15 @@
     - screenshots: The screenshot(s).
     """
     # Automatically stage the screenshot(s) if the destination is a git repo.
     for screenshot in screenshots:
         try:
             subprocess.run(["git", "add", str(screenshot)], check=True)
         except subprocess.CalledProcessError:
-            print(f"Failed to stage screenshot '{screenshot}'.")
+            click.echo(f"Failed to stage screenshot '{screenshot}'.")
 
 
 def format_screenshots_path_for_git(screenshots: Tuple[Path]) -> Tuple[Path]:
     """
     Format the screenshot(s)'s path for git.
 
     Args:
@@ -232,24 +237,29 @@
 
     Args:
 
     - output_format: The output format.
     - screenshots: The screenshot(s).
     """
     for screenshot in screenshots:
-        rel_screenshot = f"/{screenshot}"
+        # Adding a '/' to the screenshot path if the destination is a git repo.
+        # This is because the screenshot path is relative to the git repo's.
+        if is_git_repo():
+            screenshot_path = f"/{screenshot}"
+        else:
+            screenshot_path = str(screenshot)  # This is an absolute path.
 
         if output_format == "markdown":
-            print(f"![{screenshot.name}]({rel_screenshot})")
+            print(f"![{screenshot.name}]({screenshot_path})")
 
         elif output_format == "html":
-            print(f'<img src="{rel_screenshot}" alt="{screenshot.name}">')
+            print(f'<img src="{screenshot_path}" alt="{screenshot.name}">')
 
         elif output_format == "plain_text":
-            print(rel_screenshot)
+            print(screenshot_path)
 
         else:
             print(f"Invalid output format: {output_format}")
             sys.exit(1)
 
 
 def get_config_file_path() -> Path:
@@ -402,17 +412,14 @@
     if is_git_repo():
         return get_git_repo_img_destination()
 
     config = read_config(get_config_file_path())
     if config["default_destination"]:
         return Path(config["default_destination"])
 
-    # if default_destination:
-    #     return Path(default_destination)
-
     return Path.cwd()
 
 
 def is_git_repo() -> bool:
     """
     Check if the current directory is a git repository.
 
@@ -487,21 +494,22 @@
 def set_default_output_format(output_format: str) -> None:
     """
     Set the default output format.
 
     Args:
         output_format: The default output format.
     """
-    if output_format not in ["markdown", "HTML", "plain_text"]:
+    if output_format.casefold() not in ["markdown", "html", "plain_text"]:
         click.echo(f"Invalid output format: {output_format}")
+        click.echo("Valid options are: markdown, html, plain_text")
         sys.exit(1)
 
     config_file_path = get_config_file_path()
     config = read_config(config_file_path)
-    config["default_output_format"] = output_format
+    config["default_output_format"] = output_format.casefold()
 
     with open(config_file_path, "w", encoding="UTF-8") as file:
         json.dump(config, file)
 
 
 @wslshot.command()
 @click.option(
@@ -511,14 +519,15 @@
     "--destination",
     "-d",
     help="Specify the default destination directory for this operation.",
 )
 @click.option(
     "--auto-stage-enabled",
     "-a",
+    type=bool,
     help=(
         "Control whether screenshots are automatically staged when copied to a git"
         " repository."
     ),
 )
 @click.option(
     "--output-format",
@@ -537,12 +546,12 @@
     """
     if source:
         set_default_source(source)
 
     if destination:
         set_default_destination(destination)
 
-    if auto_stage_enabled:
+    if auto_stage_enabled is not None:
         set_auto_stage(auto_stage_enabled)
 
     if output_format:
         set_default_output_format(output_format)
```

### Comparing `wslshot-0.0.5/wslshot.egg-info/PKG-INFO` & `wslshot-0.0.6/wslshot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslshot
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/sderev/wslshot
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/wslshot
 Project-URL: Issues, http://github.com/sderev/wslshot/issues
 Project-URL: Changelog, https://github.com/sderev/wslshot/releases
 Requires-Python: >=3.8
@@ -108,15 +108,15 @@
 Remember to consult your VM provider's documentation for specific instructions on how to set up shared folders.
 
 ## Configuration of `wslshot`
 
 Before using `wslshot`, you may want to configure it to suit your needs. You can do this using the `config` command:
 
 ```bash
-wslshot config --source /path/to/source --auto-stage-enabled True --output-format HTML
+wslshot configure --source /path/to/source --auto-stage-enabled True --output-format HTML
 ```
 
 This command allows you to set various options:
 
 * **`--source` or `-s`**: This option lets you specify the default source directory where `wslshot` will look for screenshots.
 
 * **`--auto-stage-enabled`**: This option lets you control whether screenshots are automatically staged when copied to a git repository. By default, this option is set to `False`. If this option is set to `True`, any screenshot copied to a git repo will automatically be staged for commit.
```

