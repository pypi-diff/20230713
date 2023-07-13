# Comparing `tmp/damn_tool-0.1.1.tar.gz` & `tmp/damn_tool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damn_tool-0.1.1.tar", max compression
+gzip compressed data, was "damn_tool-0.1.2.tar", max compression
```

## Comparing `damn_tool-0.1.1.tar` & `damn_tool-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     3888 2023-07-07 19:27:54.759677 damn_tool-0.1.1/README.md
--rw-r--r--   0        0        0      187 2023-07-06 19:40:14.365512 damn_tool-0.1.1/damn_tool/__init__.py
--rw-r--r--   0        0        0     1620 2023-07-06 20:39:09.261781 damn_tool-0.1.1/damn_tool/ls.py
--rw-r--r--   0        0        0     5471 2023-07-07 18:59:43.079478 damn_tool-0.1.1/damn_tool/metrics.py
--rw-r--r--   0        0        0     9355 2023-07-06 20:39:09.263613 damn_tool-0.1.1/damn_tool/show.py
--rw-r--r--   0        0        0      350 2023-07-06 20:39:09.264928 damn_tool-0.1.1/damn_tool/utils.py
--rw-r--r--   0        0        0      519 2023-07-07 19:29:53.579632 damn_tool-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 damn_tool-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6648 2023-07-13 17:44:30.498247 damn_tool-0.1.2/README.md
+-rw-r--r--   0        0        0      187 2023-07-12 16:58:58.642019 damn_tool-0.1.2/damn_tool/__init__.py
+-rw-r--r--   0        0        0     2118 2023-07-13 13:44:00.049450 damn_tool-0.1.2/damn_tool/ls.py
+-rw-r--r--   0        0        0     7077 2023-07-13 14:37:56.519458 damn_tool-0.1.2/damn_tool/metrics.py
+-rw-r--r--   0        0        0     9781 2023-07-13 13:44:00.051295 damn_tool-0.1.2/damn_tool/show.py
+-rw-r--r--   0        0        0     1729 2023-07-13 13:44:00.051836 damn_tool-0.1.2/damn_tool/utils/aws.py
+-rw-r--r--   0        0        0     1401 2023-07-13 13:44:00.052316 damn_tool-0.1.2/damn_tool/utils/helpers.py
+-rw-r--r--   0        0        0      601 2023-07-13 17:41:40.960924 damn_tool-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7503 1970-01-01 00:00:00.000000 damn_tool-0.1.2/PKG-INFO
```

### Comparing `damn_tool-0.1.1/damn_tool/ls.py` & `damn_tool-0.1.2/damn_tool/ls.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import json
 import click
+import json
+import pyperclip
 import requests
 from termcolor import colored
 
-from .utils import load_config 
+from .utils.helpers import load_config, run_and_capture
 
-@click.command()
-@click.option('--prefix', default=None, help='Get list of assets with a given prefix')
-@click.option('--profile', default='prod', help='Profile to use')
-def ls(prefix, profile):
-    """List your platform's data assets"""
+
+def get_dagster_assets(prefix, profile):
     # Get connector configs
     dagster_config = load_config('dagster', profile)
 
     # Set headers
     headers = {
         "Content-Type": "application/json",
         "Dagster-Cloud-Api-Token": dagster_config['api_token'],
     }
 
+    # Get data
     if prefix:
       prefix_list = prefix.split('/')
       query = f"""
       query AssetsQuery {{
         assetsOrError(prefix: {json.dumps(prefix_list)}) {{
           ... on AssetConnection {{
             nodes {{
@@ -53,15 +52,31 @@
         dagster_config['endpoint'], # type: ignore
         headers=headers, # type: ignore
         json={"query": query}
     )
     
     response.raise_for_status()
     
-    data = response.json()
+    return response.json()
+
 
+def display_assets(data):
     # Extract asset keys and print them
-    click.echo('\n')
     for node in data['data']['assetsOrError']['nodes']:
         asset_key = "/".join(node['key']['path'])
         click.echo(colored(f'- {asset_key}', 'cyan'))
-    click.echo('\n')
+
+
+@click.command()
+@click.option('--prefix', default=None, help='Get list of assets with a given prefix')
+@click.option('--profile', default='prod', help='Profile to use')
+@click.option('--copy-output', is_flag=True, help='Copy command output to clipboard')
+def ls(prefix, profile, copy_output):
+    """List your platform's data assets"""
+    data = get_dagster_assets(prefix, profile)
+
+    if copy_output:
+        output = run_and_capture(display_assets, data)
+        markdown_output = output.replace('\x1b[36m- ', '- ').replace('\x1b[0m', '')  # Removing the color codes
+        pyperclip.copy(markdown_output)
+    else:
+        display_assets(data)
```

### Comparing `damn_tool-0.1.1/damn_tool/show.py` & `damn_tool-0.1.2/damn_tool/show.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-import json
 import click
+import json
+import pyperclip
 import requests
 from termcolor import colored
 
-from .utils import load_config 
+from .utils.helpers import load_config, run_and_capture
 
-@click.command()
-@click.argument('asset', required=True)
-@click.option('--profile', default='prod', help='Profile to use')
-def show(asset, profile):
-    """Show details for a specific asset"""
+
+def get_dagster_asset_info(asset, profile):
     # Get connector configs
     dagster_config = load_config('dagster', profile)
 
     # Set headers
     headers = {
         "Content-Type": "application/json",
         "Dagster-Cloud-Api-Token": dagster_config['api_token'],
     }
 
     # Split the asset key into a list of strings
     asset_key = asset.split("/")
 
-    # Insert asset_key directly into the query using f-string formatting
+    # Get data
     query = f"""
     query AssetByKey {{
       assetOrError(assetKey: {{path: {json.dumps(asset_key)}}}) {{
         __typename
         ... on Asset {{
           definition {{
             description
@@ -131,18 +129,18 @@
         dagster_config['endpoint'], # type: ignore
         headers=headers,
         json={"query": query}
     )
     
     response.raise_for_status()
     
-    data = response.json()
+    return response.json()
+
 
-    click.echo('\n')
-    # Check if an error occurred and print the error message or asset details
+def display_asset_info(asset, data):
     if data["data"]["assetOrError"]["__typename"] == "AssetNotFoundError":
         click.echo(f"Error: {data['data']['assetOrError']['message']}")
     else:
         asset_info = data["data"]["assetOrError"]
         # Use the get method to safely access the keys in the dictionary
         description = asset_info['definition'].get('description', 'Not available')
         compute_kind = asset_info['definition'].get('computeKind', 'Not available')
@@ -177,20 +175,20 @@
         if downstream_assets:
             for path in downstream_assets:
                 click.echo(colored(f"- {'/'.join(path['path'])}", 'cyan'))
         else:
             click.echo("- None")
         
         # Handle 'assetMaterializations'
+        click.echo(colored("\nLatest materialization's metadata entries:", 'magenta'))
         asset_materializations = asset_info.get('assetMaterializations', [])
         if asset_materializations:
             # Get the most recent materialization (it should be the first since we limited it to 1)
             last_materialization = asset_materializations[0]
 
-            click.echo(colored("\nLatest materialization's metadata entries:", 'magenta'))
             timestamp = last_materialization.get('timestamp', 'Not available')
             click.echo(colored(f"- Last materialization timestamp: ", 'yellow') + colored(f"{timestamp}", 'green'))
             
             # Handle 'metadataEntries'
             metadata_entries = last_materialization.get('metadataEntries', [])
             if metadata_entries:
                 for entry in metadata_entries:
@@ -223,11 +221,26 @@
                         asset_key_path = entry.get('assetKey', {}).get('path', 'Not available')
                         value = '/'.join(asset_key_path) if asset_key_path != 'Not available' else 'Not available'
                     elif typename == 'NullMetadataEntry':
                         value = 'Null'
 
                     click.echo(colored(f"- {label}: ", 'yellow') + colored(f"{value}", 'green'))
             else:
-                click.echo("No metadata entries.")
+                click.echo(colored(f"- No metadata entries.", 'yellow'))
         else:
-            click.echo("No asset materializations.")
-    click.echo('\n')
+            click.echo(colored(f"- No asset materializations.", 'yellow'))
+
+
+@click.command()
+@click.argument('asset', required=True)
+@click.option('--profile', default='prod', help='Profile to use')
+@click.option('--copy-output', is_flag=True, help='Copy command output to clipboard')
+def show(asset, profile, copy_output):
+    """Show details for a specific asset"""
+    data = get_dagster_asset_info(asset, profile)
+
+    if copy_output:
+        output = run_and_capture(display_asset_info, asset, data)
+        markdown_output = output.replace('\x1b[36m- ', '- ').replace('\x1b[0m', '')  # Removing the color codes
+        pyperclip.copy(markdown_output)
+    else:
+        display_asset_info(asset, data)
```

### Comparing `damn_tool-0.1.1/pyproject.toml` & `damn_tool-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [tool.poetry]
 name = "damn-tool"
-version = "0.1.1"
+version = "0.1.2"
 description = "The DAMN (Data Assets Metric Navigation) tool extracts and reports metrics about your data assets"
 authors = ["Olivier Dupuis <odupuis@lantrns.co>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 requests = "^2.31.0"
 python-dotenv = "^1.0.0"
 termcolor = "^2.3.0"
 pyyaml = "^6.0"
+jinja2 = "^3.1.2"
+boto3 = "^1.28.1"
+pyperclip = "^1.8.2"
+line-profiler = "^4.0.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 damn = "damn_tool.__init__:cli"
```

