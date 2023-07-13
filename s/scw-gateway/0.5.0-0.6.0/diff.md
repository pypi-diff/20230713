# Comparing `tmp/scw_gateway-0.5.0.tar.gz` & `tmp/scw_gateway-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_gateway-0.5.0.tar", max compression
+gzip compressed data, was "scw_gateway-0.6.0.tar", max compression
```

## Comparing `scw_gateway-0.5.0.tar` & `scw_gateway-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     3221 2023-07-11 09:51:56.814417 scw_gateway-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/__init__.py
--rw-r--r--   0        0        0      916 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/cli.py
--rw-r--r--   0        0        0      352 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/client.py
--rw-r--r--   0        0        0      616 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/consumer.py
--rw-r--r--   0        0        0      758 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/dev.py
--rw-r--r--   0        0        0      815 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/domain.py
--rw-r--r--   0        0        0        0 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/human/__init__.py
--rw-r--r--   0        0        0     2618 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/human/progress.py
--rw-r--r--   0        0        0     4101 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/infra.py
--rw-r--r--   0        0        0      538 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/jwt.py
--rw-r--r--   0        0        0     1312 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/commands/route.py
--rw-r--r--   0        0        0     2465 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/conf.py
--rw-r--r--   0        0        0       54 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/console.py
--rw-r--r--   0        0        0     8157 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/gateway.py
--rw-r--r--   0        0        0      281 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/__init__.py
--rw-r--r--   0        0        0     4968 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/cockpit.py
--rw-r--r--   0        0        0     6009 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/container.py
--rw-r--r--   0        0        0      519 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/function.py
--rw-r--r--   0        0        0      317 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/image.py
--rw-r--r--   0        0        0    19375 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/manager.py
--rw-r--r--   0        0        0      999 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/rdb.py
--rw-r--r--   0        0        0     2515 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/infra/secrets.py
--rw-r--r--   0        0        0     1901 2023-07-11 09:51:20.462042 scw_gateway-0.5.0/cli/model.py
--rw-r--r--   0        0        0     1185 2023-07-11 09:51:20.466042 scw_gateway-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4253 1970-01-01 00:00:00.000000 scw_gateway-0.5.0/setup.py
--rw-r--r--   0        0        0     3882 1970-01-01 00:00:00.000000 scw_gateway-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3952 2023-07-13 13:11:32.491560 scw_gateway-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/__init__.py
+-rw-r--r--   0        0        0     1900 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/cli.py
+-rw-r--r--   0        0        0      824 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/client.py
+-rw-r--r--   0        0        0      700 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/consumer.py
+-rw-r--r--   0        0        0     1081 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/dev.py
+-rw-r--r--   0        0        0     1276 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/domain.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/human/__init__.py
+-rw-r--r--   0        0        0     1971 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/human/errors.py
+-rw-r--r--   0        0        0     2633 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/human/progress.py
+-rw-r--r--   0        0        0     5201 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/infra.py
+-rw-r--r--   0        0        0      627 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/jwt.py
+-rw-r--r--   0        0        0      411 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/options.py
+-rw-r--r--   0        0        0     1502 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/commands/route.py
+-rw-r--r--   0        0        0     3588 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/conf.py
+-rw-r--r--   0        0        0       54 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/console.py
+-rw-r--r--   0        0        0     9795 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/gateway.py
+-rw-r--r--   0        0        0      281 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/__init__.py
+-rw-r--r--   0        0        0     5103 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/cockpit.py
+-rw-r--r--   0        0        0     6075 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/container.py
+-rw-r--r--   0        0        0      519 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/function.py
+-rw-r--r--   0        0        0      317 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/image.py
+-rw-r--r--   0        0        0    21063 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/manager.py
+-rw-r--r--   0        0        0      999 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/rdb.py
+-rw-r--r--   0        0        0     2575 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/infra/secrets.py
+-rw-r--r--   0        0        0     1901 2023-07-13 13:10:44.258951 scw_gateway-0.6.0/cli/model.py
+-rw-r--r--   0        0        0     1181 2023-07-13 13:10:44.262951 scw_gateway-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4998 1970-01-01 00:00:00.000000 scw_gateway-0.6.0/setup.py
+-rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 scw_gateway-0.6.0/PKG-INFO
```

### Comparing `scw_gateway-0.5.0/README.md` & `scw_gateway-0.6.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,33 @@
-# Scaleway Serverless Gateway :spider_web:
+# <img src="logo.png" height="32"/> Scaleway Serverless Gateway
 
 [![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)
 [![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)
 [![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)
 
 The Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).
 
 It lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.
 
 It is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.
 
+You can read all about it in [this blog post](https://www.scaleway.com/en/blog/api-gateway-early-access/).
+
+If you would like to join in the discussion on how we continue developing the project, or give us feedback, then join us on the [#api-gateway-beta](https://app.slack.com/client/T7YEXCR7X/C05H07VBKJ4) channel on the Scaleway Community Slack.
+
 ## :page_with_curl: Contents
 
-- [:rocket: Features](#rocket-features)
-- [:computer: Quick-start](#computer-quick-start)
-- [:mortar\_board: Contributing](#mortar_board-contributing)
-- [:mailbox: Reach Us](#mailbox-reach-us)
+- [ Scaleway Serverless Gateway](#-scaleway-serverless-gateway)
+  - [:page\_with\_curl: Contents](#page_with_curl-contents)
+  - [:computer: Quick-start](#computer-quick-start)
+    - [Deploy your gateway](#deploy-your-gateway)
+    - [Add a route](#add-a-route)
+    - [Delete your gateway](#delete-your-gateway)
+  - [:mortar\_board: Contributing](#mortar_board-contributing)
+  - [:mailbox: Reach us](#mailbox-reach-us)
 
 Please see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.
 
 ## :computer: Quick-start
 
 To deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):
 
@@ -35,14 +43,16 @@
 
 To deploy your gateway, you can run:
 
 ```console
 scwgw infra deploy
 ```
 
+For more information on the deployment process, see the [deployment docs](https://serverless-gateway.readthedocs.io/en/latest/deployment.html).
+
 ### Add a route
 
 To check your gateway is working, you can add and remove a route:
 
 ```console
 # Check no routes are configured initially
 scwgw route ls
@@ -76,9 +86,9 @@
 
 Do not hesitate to raise issues and pull requests we will have a look at them.
 
 ## :mailbox: Reach us
 
 We love feedback. Feel free to:
 
-- Open a [Github issue](https://github.com/scaleway/serverless-functions-python/issues/new)
+- Open a [Github issue](https://github.com/scaleway/serverless-gateway/issues/new)
 - Send us a message on the [Scaleway Slack community](https://slack.scaleway.com/), in the [#serverless-functions](https://scaleway-community.slack.com/app_redirect?channel=serverless-functions) channel.
```

### Comparing `scw_gateway-0.5.0/cli/commands/consumer.py` & `scw_gateway-0.6.0/cli/commands/jwt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 import click
 
 from cli.gateway import GatewayManager
 
 
 @click.group()
-def consumer():
-    """Manage gateway consumers"""
+def jwt():
+    """Configure credentials for JWT authorization\n
+    https://serverless-gateway.readthedocs.io/en/latest/auth.html"""
     pass
 
 
-@consumer.command()
-def ls():
-    """Print the consumers configured on the gateway"""
+@jwt.command()
+@click.argument("consumer")
+def add(consumer):
+    """Adds a JWT credential to a consumer"""
     manager = GatewayManager()
-    manager.print_consumers()
+    cred = manager.add_jwt_cred(consumer)
+    manager.print_jwt_creds([cred])
 
 
-@consumer.command()
-@click.argument("name")
-def add(name):
-    """Add a consumer to the gateway"""
+@jwt.command()
+@click.argument("consumer")
+def ls(consumer):
+    """Lists the JWT credentials for a consumer"""
     manager = GatewayManager()
-    manager.add_consumer(name)
-
-
-@consumer.command()
-@click.argument("name")
-def delete(name):
-    """Delete a consumer from the gateway"""
-    manager = GatewayManager()
-    manager.delete_consumer(name)
+    manager.print_jwt_creds_for_consumer(consumer)
```

### Comparing `scw_gateway-0.5.0/cli/commands/human/progress.py` & `scw_gateway-0.6.0/cli/commands/human/progress.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,30 +35,30 @@
 
 
 def database_deployment_progress_cb(
     progress: Progress,
 ) -> t.Callable[[rdb.Instance], None]:
     """Create a callback that handles the database creation progress."""
 
-    db_task = progress.add_task("Deploying database", total=100, start=False)
+    db_task = progress.add_task("Deploying Kong database", total=100, start=False)
 
     def wait_for_database_on_tick(instance: rdb.Instance) -> None:
         progress.start_task(db_task)
         if instance.status == rdb.InstanceStatus.READY:
             progress.update(db_task, completed=100, refresh=True)
             progress.stop()
         elif instance.status == rdb.InstanceStatus.PROVISIONING:
             # First part of creating is provisioning
             task = progress.tasks[db_task]
-            task.description = "Provisioning database (1/2)"
+            task.description = "Provisioning Kong database (1/2)"
             completed = mix(task.completed, 50, STIFFNESS)
             progress.update(db_task, completed=completed)
         elif instance.status == rdb.InstanceStatus.INITIALIZING:
             # Second part of creating is initializing
             task = progress.tasks[db_task]
-            task.description = "Initializing database (2/2)"
+            task.description = "Initializing Kong database (2/2)"
             completed = mix(task.completed, 100, STIFFNESS * 2)
             progress.update(db_task, completed=completed)
         elif instance.status == rdb.InstanceStatus.ERROR:
             progress.stop()
 
     return wait_for_database_on_tick
```

### Comparing `scw_gateway-0.5.0/cli/commands/route.py` & `scw_gateway-0.6.0/cli/commands/route.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import click
 
+from cli.console import console
 from cli.gateway import GatewayManager
 from cli.model import Route
 
 
 @click.group()
 def route():
-    """Manage gateway routes"""
+    """Manage routing to upstream services from the gateway"""
     pass
 
 
 @route.command()
 def ls():
     """Print the routes configured on the gateway"""
     manager = GatewayManager()
     manager.print_routes()
 
+    console.print("\nRelative URLs are accessible from your gateway base URL:")
+    console.print(f"{manager.gateway_url}\n")
+
 
 @route.command()
 @click.argument("relative_url")
 @click.argument("target")
 @click.option(
     "--cors", is_flag=True, default=False, help="Add permissive cors to the route."
 )
```

### Comparing `scw_gateway-0.5.0/cli/conf.py` & `scw_gateway-0.6.0/cli/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,42 @@
 import os
 import typing as t
 from dataclasses import asdict, dataclass
 
+import click
 import yaml
 
+from cli.console import console
+
 if t.TYPE_CHECKING:
     # Importing conditionally to avoid circular imports
     from cli.infra import InfraManager
 
 USER_HOME = os.path.expanduser("~")
 CONFIG_DIR = os.path.join(USER_HOME, ".config", "scw")
 CONFIG_FILE = os.path.join(CONFIG_DIR, "gateway.yml")
 
 # Name is fixed for all managed databases
 DB_DATABASE_NAME = "rdb"
 DB_DATABASE_NAME_LOCAL = "kong"
 
+# Default time to wait for resources
+RESOURCE_AWAIT_TIMEOUT_MINUTES = 15
+RESOURCE_AWAIT_TIMEOUT_SECONDS = 60 * RESOURCE_AWAIT_TIMEOUT_MINUTES
+
+
+def _check_config_file():
+    if not os.path.exists(CONFIG_FILE):
+        console.print(
+            "No gateway config file found. Have you run your gateway setup? Try:",
+            style="red",
+        )
+        console.print("scwgw infra deploy", style="bold red")
+        raise click.Abort()
+
 
 @dataclass
 class InfraConfiguration:
     """Configuration used to store information of a deployed gateway."""
 
     protocol: t.Literal["http", "https"]
     gw_admin_host: str
@@ -67,17 +84,48 @@
             db_port=str(endpoint.port),
             db_name=DB_DATABASE_NAME,
         )
 
     @staticmethod
     def load() -> "InfraConfiguration":
         """Read the configuration from the config file."""
+
+        _check_config_file()
+
         with open(CONFIG_FILE, mode="rt", encoding="utf-8") as file:
             conf = yaml.safe_load(file)
             return InfraConfiguration(**conf)
 
+    @property
+    def gw_url(self):
+        gateway_url = [
+            self.protocol,
+            "://",
+            self.gw_host,
+        ]
+
+        gateway_port = self.gw_port
+        if gateway_port:
+            gateway_url.extend([":", str(gateway_port)])
+
+        return "".join(gateway_url)
+
+    @property
+    def gw_admin_url(self):
+        admin_url = [
+            self.protocol,
+            "://",
+            self.gw_admin_host,
+        ]
+
+        admin_port = self.gw_admin_port
+        if admin_port:
+            admin_url.extend([":", str(admin_port)])
+
+        return "".join(admin_url)
+
     def save(self) -> None:
         """Save the configuration to a file."""
         os.makedirs(CONFIG_DIR, exist_ok=True)
 
         with open(CONFIG_FILE, mode="wt", encoding="utf-8") as file:
             yaml.safe_dump(asdict(self), file)
```

### Comparing `scw_gateway-0.5.0/cli/gateway.py` & `scw_gateway-0.6.0/cli/gateway.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,218 +1,251 @@
-import json
+import typing as t
+from collections import defaultdict
+from dataclasses import dataclass
 
 import requests
 from loguru import logger
+from requests import Response
 from requests.adapters import HTTPAdapter
 from rich.table import Table
 from urllib3 import Retry
 
 from cli import conf
 from cli.console import console
 from cli.model import Consumer, JwtCredential, Route
 
 MAX_RETRIES = 5
 
 
-def response_hook(response: requests.Response, *_args, **_kwargs):
-    """Response hook to log request and call raise_for_status."""
-    req = response.request
-    logger.debug(f"{req.method}: {req.url}")
-    try:
-        response.raise_for_status()
-    except requests.exceptions.HTTPError as err:
-        try:  # Try to parse the body as JSON
-            body_json = err.response.json()
-            logger.error(f"Error: \n{json.dumps(body_json, indent=2)}")
-        except json.decoder.JSONDecodeError:
-            logger.error(f"Error: \n{err.response.text}")
-        raise err
+@dataclass
+class KongAPIException(Exception):
+    """Exception raised when the Kong API returns an error."""
+
+    response: Response
+
+    def __str__(self) -> str:
+        """Return the response text."""
+        return self.response.text
 
 
 class GatewayManager:
     """Configure routes via the Kong admin API."""
 
     admin_url: str
     gateway_url: str
 
-    def __init__(self):
+    def __init__(self, config: t.Optional[conf.InfraConfiguration] = None):
         # Local local config
-        self.config = conf.InfraConfiguration.load()
-
-        admin_url = [
-            self.config.protocol,
-            "://",
-            self.config.gw_admin_host,
-        ]
-
-        admin_port = self.config.gw_admin_port
-        if admin_port:
-            admin_url.extend([":", str(admin_port)])
-
-        self.admin_url = "".join(admin_url)
-
-        gateway_url = [
-            self.config.protocol,
-            "://",
-            self.config.gw_host,
-        ]
-
-        gateway_port = self.config.gw_port
-        if gateway_port:
-            gateway_url.extend([":", str(gateway_port)])
-
-        self.gateway_url = "".join(gateway_url)
+        self.config = config or conf.InfraConfiguration.load()
+        self.admin_url = self.config.gw_admin_url
+        self.gateway_url = self.config.gw_url
 
         self.routes_url = self.admin_url + "/routes"
         self.services_url = self.admin_url + "/services"
         self.consumers_url = self.admin_url + "/consumers"
+        self.plugins_url = self.admin_url + "/plugins"
 
         self.token = self.config.gw_admin_token
 
-        self._create_session()
+        self._session = self._get_session()
 
-    def _create_session(self):
-        self.session = requests.Session()
+    def _get_session(self) -> requests.Session:
+        session = requests.Session()
         if self.token:
-            self.session.headers["X-Auth-Token"] = self.token
-        self.session.headers["Content-Type"] = "application/json"
-        self.session.hooks["response"].append(response_hook)
+            session.headers["X-Auth-Token"] = self.token
 
         retries = Retry(
             total=MAX_RETRIES,
             backoff_factor=2,
             status=MAX_RETRIES,  # Status max retries
             # 403: retry for token refresh
             # 404: retry for Envoy service not found
             status_forcelist=[500, 404, 403],
         )
-        self.session.mount("https://", HTTPAdapter(max_retries=retries))
+        session.mount("https://", HTTPAdapter(max_retries=retries))
+
+        return session
+
+    def _request(self, method: str, url: str, **kwargs) -> requests.Response:
+        """Make a request to the Kong admin API."""
+        try:
+            logger.debug(f"Request: {method} {url}")
+            resp = self._session.request(method, url, **kwargs)
+            logger.debug(f"Response: {resp.status_code} {resp.text}")
+            resp.raise_for_status()
+            return resp
+        except requests.HTTPError as err:
+            raise KongAPIException(err.response) from err
 
     def add_route(self, route: Route) -> requests.Response:
+        """Add a route to Kong."""
+
+        if not route.target.startswith("http"):
+            raise ValueError("Route target must start with http or https")
+
         service_url = f"{self.services_url}/{route.name}"
         route_url = f"{self.routes_url}/{route.name}"
 
-        resp = self.session.put(url=service_url, json=route.service_json())
-        resp = self.session.put(url=route_url, json=route.route_json())
+        resp = self._request(method="PUT", url=service_url, json=route.service_json())
+        resp = self._request(method="PUT", url=route_url, json=route.route_json())
+
+        route_plugins_url = f"{route_url}/plugins"
 
-        plugins_url = f"{route_url}/plugins"
         if route.cors:
             try:
-                self.session.post(url=plugins_url, json=route.cors_json())
-            except requests.HTTPError:
-                # TODO - avoid ignoring this, any way to create or update?
-                pass
+                self._request(
+                    method="POST", url=route_plugins_url, json=route.cors_json()
+                )
+            except KongAPIException as err:
+                # Ignore if the plugin already exists
+                if err.response.status_code != 409:
+                    raise
 
         if route.jwt:
             try:
-                self.session.post(url=plugins_url, json=route.jwt_json())
-            except requests.HTTPError:
-                # TODO - avoid ignoring this, any way to create or update?
-                pass
+                self._request(
+                    method="POST", url=route_plugins_url, json=route.jwt_json()
+                )
+            except KongAPIException as err:
+                # Ignore if the plugin already exists
+                if err.response.status_code != 409:
+                    raise
 
         return resp
 
     def delete_route(self, route: Route) -> requests.Response:
-        self.session.delete(url=f"{self.routes_url}/{route.name}")
-        resp = self.session.delete(url=f"{self.services_url}/{route.name}")
+        """Delete a route from Kong."""
+        self._request(method="DELETE", url=f"{self.routes_url}/{route.name}")
+        resp = self._request(method="DELETE", url=f"{self.services_url}/{route.name}")
         return resp
 
     def print_routes(self) -> None:
+        """Print all routes."""
         routes: list[Route] = self.get_routes()
         routes.sort(key=lambda r: r.relative_url)
 
-        table = Table("RELATIVE URL", "TARGET", "HTTP METHODS", title="Gateway Routes")
-        for r in routes:
-            http_methods = " ".join(r.http_methods) if r.http_methods else "All"
-            table.add_row(r.relative_url, r.target, http_methods)
+        table = Table("Relative url", "Target", "HTTP methods", "JWT", "CORS")
+        for route in routes:
+            jwt = "On" if route.jwt else "-"
+            cors = "On" if route.cors else "-"
+            http_methods = " ".join(route.http_methods) if route.http_methods else "All"
+            table.add_row(route.relative_url, route.target, http_methods, jwt, cors)
+
         console.print(table)
 
     def get_routes(self) -> list[Route]:
-        resp = self.session.get(url=self.routes_url)
+        """Get all routes from Kong."""
+        # Get routes
+        resp = self._request(method="GET", url=self.routes_url)
         route_data = {r.get("name"): r for r in resp.json().get("data")}
 
-        resp = self.session.get(url=self.services_url)
+        # Get services
+        resp = self._request(method="GET", url=self.services_url)
         service_data = {s.get("name"): s for s in resp.json().get("data")}
 
-        routes = list()
-        for _, r in route_data.items():
-            route_name = r["name"]
-            route_path = r["paths"][0]
-            http_methods = r.get("methods")
+        # Get plugins
+        resp = self._request(method="GET", url=self.plugins_url)
+        plugins_json = resp.json().get("data")
+
+        # Work out which plugins apply to which routes
+        route_plugins = defaultdict(list)
+        for p in plugins_json:
+            plugin_route = p.get("route")
+            plugin_id = plugin_route.get("id") if plugin_route else None
+            if plugin_id:
+                route_plugins[plugin_id].append(p)
+
+        routes = []
+        for _, route_json in route_data.items():
+            route_id = route_json["id"]
+            route_name = route_json["name"]
+            route_path = route_json["paths"][0]
+            http_methods = route_json.get("methods")
 
             service = service_data.get(route_name)
             if not service:
                 continue
 
             service_port = service["port"]
             service_host = service["host"]
             service_protocol = service["protocol"]
             service_url = f"{service_protocol}://{service_host}:{service_port}"
 
-            routes.append(
-                Route(
-                    relative_url=route_path,
-                    target=service_url,
-                    http_methods=http_methods,
-                )
+            r = Route(
+                relative_url=route_path,
+                target=service_url,
+                http_methods=http_methods,
             )
 
+            # Check if route has plugins installed
+            # There will be an entry per route per plugin
+            for p in route_plugins.get(route_id) or []:
+                if p.get("name") == "jwt":
+                    r.jwt = True
+                elif p.get("name") == "cors":
+                    r.cors = True
+
+            routes.append(r)
+
         return routes
 
     def get_consumers(self) -> list[Consumer]:
-        resp = self.session.get(url=self.consumers_url)
+        """Get all consumers from Kong."""
+        resp = self._request(method="GET", url=self.consumers_url)
         consumer_data = resp.json().get("data")
         consumer_data.sort(key=lambda x: x["username"])
 
         return [Consumer.from_json(c) for c in consumer_data]
 
     def print_consumers(self) -> None:
+        """Print all consumers."""
         consumers: list[Consumer] = self.get_consumers()
 
-        table = Table("CONSUMER", title="Consumers")
-        for c in consumers:
-            table.add_row(c.username)
+        table = Table("Consumer")
+        for consumer in consumers:
+            table.add_row(consumer.username)
+
         console.print(table)
 
-    def delete_consumer(self, consumer_name: str):
+    def delete_consumer(self, consumer_name: str) -> None:
+        """Delete a consumer from Kong given its name."""
         consumer_url = f"{self.consumers_url}/{consumer_name}"
-        resp = self.session.delete(url=consumer_url)
-        resp.raise_for_status()
+        self._request(method="DELETE", url=consumer_url)
 
-    def add_consumer(self, consumer_name):
+    def add_consumer(self, consumer_name: str) -> None:
+        """Add a consumer to Kong given its name."""
         consumer = Consumer(username=consumer_name)
-        resp = self.session.post(url=self.consumers_url, json=consumer.json())
-        resp.raise_for_status()
+        self._request(method="POST", url=self.consumers_url, json=consumer.json())
 
     def add_jwt_cred(self, consumer_name: str) -> JwtCredential:
+        """Add a JWT credential to a consumer given its name."""
         jwt_url = f"{self.consumers_url}/{consumer_name}/jwt"
 
-        resp = self.session.post(
+        resp = self._request(
+            method="POST",
             url=jwt_url,
             headers={"Content-Type": "application/x-www-form-urlencoded"},
         )
-        resp.raise_for_status()
-
         return JwtCredential.from_json(resp.json())
 
     def get_jwt_creds(self, consumer_name: str) -> list[JwtCredential]:
+        """Get all JWT credentials for a consumer given its name."""
         jwt_url = f"{self.consumers_url}/{consumer_name}/jwt"
 
-        resp = self.session.get(url=jwt_url)
-        resp.raise_for_status()
-
+        resp = self._request(method="GET", url=jwt_url)
         creds_data = resp.json()["data"]
         return [JwtCredential.from_json(d) for d in creds_data]
 
     def print_jwt_creds(self, creds: list[JwtCredential]):
         """Print JWT credentials for a consumer."""
 
-        table = Table("ALGORITHM", "SECRET", "ISS", title="JWT Credentials")
-        for c in creds:
-            table.add_row(c.algorithm, c.secret, c.iss)
+        table = Table("Algorithm", "Secret", "ISS")
+        for cred in creds:
+            table.add_row(cred.algorithm, cred.secret, cred.iss)
+
         console.print(table)
 
     def print_jwt_creds_for_consumer(self, consumer_name):
         creds = self.get_jwt_creds(consumer_name)
         self.print_jwt_creds(creds)
 
     def setup_global_kong_statsd_plugin(self) -> str:
@@ -220,23 +253,25 @@
 
         This plugin is used to send metrics to Cockpit.
         It is installed globally for all services.
         """
         plugins_url = self.admin_url + "/plugins"
 
         # Delete existing statsd plugin if it exists
-        resp = self.session.get(plugins_url)
+        resp = self._request(method="GET", url=plugins_url)
         plugins = resp.json()["data"]
         for plugin in plugins:
             if plugin["name"] == "statsd":
-                self.session.delete(f"{plugins_url}/{plugin['id']}")
+                self._request(method="DELETE", url=f"{plugins_url}/{plugin['id']}")
+                break
 
         # Install statsd plugin
-        resp = self.session.post(
-            plugins_url,
+        resp = self._request(
+            method="POST",
+            url=plugins_url,
             json={
                 "name": "statsd",
                 "config": {
                     "port": 8125,
                     "prefix": "kong",
                 },
             },
```

### Comparing `scw_gateway-0.5.0/cli/infra/cockpit.py` & `scw_gateway-0.6.0/cli/infra/cockpit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from contextlib import contextmanager
 from typing import Generator
 
-import click
 import requests
 import scaleway.cockpit.v1beta1 as sdk
 from requests.auth import HTTPBasicAuth
 from scaleway import ScalewayException
+from scaleway_core.utils import WaitForOptions
 
+from cli import conf
 from cli.console import console
 
 METRICS_TOKEN_NAME = "scw-gw-write-metrics"
 WRITE_METRICS_SCOPE = sdk.TokenScopes(
     query_metrics=False,
     write_metrics=True,
     setup_metrics_rules=False,
@@ -34,19 +35,23 @@
     try:
         api.get_cockpit()
         # If successful, cockpit activated
         return
     except ScalewayException as err:
         if not err.status_code == 404:
             raise
+
         # Activate the cockpit
-        click.secho("Activating Cockpit...", fg="yellow")
+        console.print("Activating Cockpit")
         cockpit = api.activate_cockpit()
-        api.wait_for_cockpit(project_id=cockpit.project_id)
-        console.print("Cockpit activated", style="green")
+
+        options: WaitForOptions[sdk.Cockpit, bool] = WaitForOptions()
+        options.timeout = conf.RESOURCE_AWAIT_TIMEOUT_SECONDS
+
+        api.wait_for_cockpit(project_id=cockpit.project_id, options=options)
 
 
 def get_metrics_push_url(api: sdk.CockpitV1Beta1API) -> str:
     """Get the Cockpit metrics push URL."""
     cockpit = api.get_cockpit()
 
     if not cockpit.endpoints:
```

### Comparing `scw_gateway-0.5.0/cli/infra/container.py` & `scw_gateway-0.6.0/cli/infra/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from cli.infra.rdb import DB_USERNAME
 
 CONTAINER_NAMESPACE = "scw-sls-gw"
 
 CONTAINER_NAME = "scw-sls-gw"
 CONTAINER_MIN_SCALE = 1
 CONTAINER_MAX_SCALE = 5
+CONTAINER_CPU_LIMIT = 2000
 CONTAINER_MEMORY_LIMIT = 1024
 
 CONTAINER_ADMIN_NAME = "scw-sls-gw-admin"
 CONTAINER_ADMIN_MIN_SCALE = 1
 CONTAINER_ADMIN_MAX_SCALE = 1
 CONTAINER_ADMIN_MEMORY_LIMIT = 1024
 CONTAINER_ADMIN_PORT = 8001
@@ -86,14 +87,15 @@
         secret_env_vars.append(sdk.Secret("COCKPIT_METRICS_TOKEN", metrics_token))
         env_vars["FORWARD_METRICS"] = "1"
         env_vars["COCKPIT_METRICS_PUSH_URL"] = metrics_push_url
 
     return api.create_container(
         namespace_id=namespace_id,
         name=CONTAINER_NAME,
+        cpu_limit=CONTAINER_CPU_LIMIT,
         memory_limit=CONTAINER_MEMORY_LIMIT,
         min_scale=CONTAINER_MIN_SCALE,
         max_scale=CONTAINER_MAX_SCALE,
         privacy=sdk.ContainerPrivacy.PUBLIC,
         protocol=sdk.ContainerProtocol.HTTP1,
         http_option=sdk.ContainerHttpOption.REDIRECTED,
         registry_image=IMAGE_TAG,
```

### Comparing `scw_gateway-0.5.0/cli/infra/function.py` & `scw_gateway-0.6.0/cli/infra/function.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.5.0/cli/infra/manager.py` & `scw_gateway-0.6.0/cli/infra/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,27 +156,26 @@
 
     def create_db(self) -> rdb.Instance:
         """Create the database instance."""
 
         instance_name = infra.rdb.DB_INSTANCE_NAME
         instance = infra.rdb.get_database_instance_by_name(self.rdb, instance_name)
         if instance:
-            console.print(f"Database {instance_name} already exists")
+            console.print("Kong database already exists")
             return instance
 
-        console.print(f"Creating database instance {instance_name}...")
+        logger.debug(f"Creating database instance {instance_name}...")
 
         logger.debug("Generating database password")
         password = infra.secrets.generate_database_password()
 
         logger.debug("Saving database password")
         infra.secrets.create_db_password_secret(self.secrets, password)
 
         instance = infra.rdb.create_database_instance(self.rdb, password)
-        console.print("Database created", style="bold green")
         return instance
 
     def check_db(self):
         """Check the status of the database instance."""
         instance = self._get_database_instance_or_abort()
         console.print(f"Database status: {instance.status}", style="bold")
 
@@ -186,32 +185,37 @@
         if instance.status == rdb.InstanceStatus.READY:
             return
 
         options: WaitForOptions[rdb.Instance, bool] = WaitForOptions()
         options.stop = lambda instance: on_tick(instance) or (
             instance.status not in rdb.INSTANCE_TRANSIENT_STATUSES
         )
+        options.timeout = conf.RESOURCE_AWAIT_TIMEOUT_SECONDS
+
         instance = self.rdb.wait_for_instance(
             instance_id=instance.id,
             options=options,
         )
 
         if instance.status != rdb.InstanceStatus.READY:
             console.print("Database is not ready", style="bold red")
             raise click.Abort()
 
     def delete_db(self) -> None:
         """Delete the database instance."""
         # Delete the secret
-        infra.secrets.delete_db_password_secret(self.secrets)
+        infra.secrets.delete_db_password_secret_if_exists(self.secrets)
 
         # Delete the database
-        instance = self._get_database_instance_or_abort()
-        self.rdb.delete_instance(instance_id=instance.id)
-        console.print("Database deleted")
+        try:
+            instance = self._get_database_instance_or_abort()
+            self.rdb.delete_instance(instance_id=instance.id)
+            console.print("Kong database deleted")
+        except click.Abort:
+            logger.debug("Database not found, skipping")
 
     def create_namespace(self):
         """Create the namespace for the gateway."""
         namespace_name = infra.cnt.CONTAINER_NAMESPACE
         namespace = infra.cnt.get_namespace_by_name(self.containers, namespace_name)
 
         if namespace:
@@ -230,98 +234,103 @@
             )
             raise click.Abort()
 
         console.print(f"Namespace status: {namespace.status}", style="bold")
 
     def await_namespace(self):
         """Wait for the namespace to be ready."""
+        namespace = self._get_namespace_or_abort()
 
-        console.print("Waiting for namespace to be ready...", style="blue")
+        options: WaitForOptions[cnt.Namespace, bool] = WaitForOptions()
+        options.timeout = conf.RESOURCE_AWAIT_TIMEOUT_SECONDS
 
-        namespace = self._get_namespace_or_abort()
-        namespace = self.containers.wait_for_namespace(namespace_id=namespace.id)
+        namespace = self.containers.wait_for_namespace(
+            namespace_id=namespace.id, options=options
+        )
         if namespace.status == cnt.NamespaceStatus.ERROR:
             console.print(
                 f"Namespace in error: {namespace.error_message}",
                 style="bold red",
             )
             raise click.Abort()
 
         if namespace.status != cnt.NamespaceStatus.READY:
             console.print("Namespace is not ready", style="bold red")
             raise click.Abort()
 
-        console.print("Namespace ready")
-
     def delete_namespace(self):
         """Delete the namespace."""
-        namespace = self._get_namespace_or_abort()
-        self.containers.delete_namespace(namespace_id=namespace.id)
-        console.print("Namespace deleted")
+        try:
+            namespace = self._get_namespace_or_abort()
+            self.containers.delete_namespace(namespace_id=namespace.id)
+            console.print("Kong container namespace deleted")
+        except click.Abort:
+            logger.debug("Namespace not found, skipping")
 
     def create_containers(self) -> None:
         """Create containers for Kong and Kong Admin."""
         database_instance = self._get_database_instance_or_abort()
         db_password = self._get_db_password_or_abort()
         db_host, db_port = self._get_database_endpoint_or_abort(database_instance)
 
         # Namespace should be created before creating containers
         namespace = self._get_namespace_or_abort()
 
         admin_container_name = infra.cnt.CONTAINER_ADMIN_NAME
         admin_container = infra.cnt.get_container_by_name(
             self.containers, namespace.id, admin_container_name
         )
+
         if admin_container:
             console.print(
-                f"Admin container {admin_container_name} already exists",
+                "Kong Admin API container already exists",
             )
         else:
             console.print(
-                f"Creating admin container {admin_container_name}",
+                "Creating Kong Admin API container",
             )
             created_container = infra.cnt.create_kong_admin_container(
                 self.containers, namespace.id, db_host, db_port, db_password
             )
-            console.print(f"Deploying container {admin_container_name}")
+
+            logger.debug(f"Deploying container {admin_container_name}")
             self.containers.deploy_container(container_id=created_container.id)
 
         container_name = infra.cnt.CONTAINER_NAME
         container = infra.cnt.get_container_by_name(
             self.containers, namespace.id, container_name
         )
         if container:
-            console.print(f"Container {container_name} already exists")
+            console.print("Kong Gateway container already exists")
             return
 
-        console.print(
-            f"Creating container {container_name} from tag {infra.image.IMAGE_TAG}"
-        )
-
         # Check if token exists
         token = infra.cpt.get_metrics_token(self.cockpit)
         if token:
-            console.print("Cockpit token already exists, deleting")
+            logger.debug("Cockpit token already exists, deleting")
             infra.cpt.delete_metrics_token(self.cockpit, token)
 
-        console.print("Creating Cockpit token")
+        logger.debug("Creating Cockpit token")
         token_key = infra.cpt.create_metrics_token(self.cockpit)
         metrics_push_url = infra.cpt.get_metrics_push_url(self.cockpit)
 
+        console.print(
+            "Creating Kong Gateway container",
+        )
         created_container = infra.cnt.create_kong_container(
             self.containers,
             namespace.id,
             db_host,
             db_port,
             db_password,
             metrics_token=token_key,
             metrics_push_url=metrics_push_url,
         )
 
-        console.print(f"Deploying container {container_name}")
+        logger.debug(f"Deploying container {container_name}")
         self.containers.deploy_container(container_id=created_container.id)
 
     def check_containers(self):
         """Check the status of the containers."""
         admin_container = self._get_admin_container_or_abort()
         container = self._get_container_or_abort()
 
@@ -339,28 +348,32 @@
 
         if container.status != cnt.ContainerStatus.READY:
             console.print(f"Container {container.name} is not ready", style="bold red")
             raise click.Abort()
 
     def await_containers(self):
         """Wait for the containers to be ready."""
-
-        console.print("Waiting for containers to be ready...", style="blue")
-
         admin_container = self._get_admin_container_or_abort()
         container = self._get_container_or_abort()
 
+        options: WaitForOptions[cnt.Container, bool] = WaitForOptions()
+        options.timeout = conf.RESOURCE_AWAIT_TIMEOUT_SECONDS
+
         # Execute in parallel
         executor = futures.ThreadPoolExecutor(max_workers=2)
         admin_future = executor.submit(
-            lambda id: self.containers.wait_for_container(container_id=id),
+            lambda id: self.containers.wait_for_container(
+                container_id=id, options=options
+            ),
             admin_container.id,
         )
         container_future = executor.submit(
-            lambda id: self.containers.wait_for_container(container_id=id),
+            lambda id: self.containers.wait_for_container(
+                container_id=id, options=options
+            ),
             container.id,
         )
 
         # Wait for both futures to complete
         futures.wait(
             [admin_future, container_future], return_when=futures.ALL_COMPLETED
         )
@@ -371,22 +384,27 @@
         container = container_future.result()
         self._handle_container_not_ready(container)
 
         console.print("Containers are ready")
 
     def delete_containers(self):
         """Delete the containers."""
-        admin_container = self._get_admin_container_or_abort()
-        container = self._get_container_or_abort()
-
-        self.containers.delete_container(container_id=admin_container.id)
-        console.print("Admin container deleted")
-
-        self.containers.delete_container(container_id=container.id)
-        console.print("Gateway container deleted")
+        try:
+            admin_container = self._get_admin_container_or_abort()
+            self.containers.delete_container(container_id=admin_container.id)
+            console.print("Kong Admin API container deleted")
+        except click.Abort:
+            logger.debug("Admin container not found, skipping")
+
+        try:
+            container = self._get_container_or_abort()
+            self.containers.delete_container(container_id=container.id)
+            console.print("Kong Gateway container deleted")
+        except click.Abort:
+            logger.debug("Gateway container not found, skipping")
 
     def get_function_endpoint(
         self, namespace_name: str, function_name: str
     ) -> str | None:
         """Get the endpoint of a function."""
         return infra.fnc.get_function_endpoint_by_name(
             self.functions, namespace_name, function_name
@@ -401,18 +419,18 @@
     def update_container(self):
         """Update the container."""
         self.update_container_without_deploy()
 
         admin_container = self._get_admin_container_or_abort()
         container = self._get_container_or_abort()
 
-        console.print("Deploying admin container...")
+        console.print("Deploying Kong Admin API container...")
         self.containers.deploy_container(container_id=admin_container.id)
 
-        console.print("Deploying container...")
+        console.print("Deploying Kong Gateway container")
         self.containers.deploy_container(container_id=container.id)
 
     def update_container_without_deploy(self):
         """Update the container without deploying it."""
         admin_container = self._get_admin_container_or_abort()
         container = self._get_container_or_abort()
 
@@ -428,15 +446,15 @@
 
         token, metrics_push_url = None, None
         if container.environment_variables.get("FORWARD_METRICS"):
             token = infra.cpt.get_metrics_token(self.cockpit)
             if token:
                 infra.cpt.delete_metrics_token(self.cockpit, token)
 
-            console.print("Creating Cockpit token to forward metrics...")
+            logger.debug("Creating Cockpit token to forward metrics")
             token_key = infra.cpt.create_metrics_token(self.cockpit)
             metrics_push_url = infra.cpt.get_metrics_push_url(self.cockpit)
 
         infra.cnt.update_kong_container(
             self.containers,
             container.id,
             db_host,
@@ -447,15 +465,15 @@
         )
 
     def print_domains_for_container(self) -> None:
         """Prints the custom domains set on the container"""
         container = self._get_container_or_abort()
         domains = self.containers.list_domains_all(container_id=container.id)
 
-        table = Table("HOSTNAME", "URL", "STATUS", title="Domains")
+        table = Table("Hostname", "URL", "Status")
         for domain in domains:
             table.add_row(domain.hostname, domain.url, domain.status)
         console.print(table)
 
     def _get_domain(self, container_id: str, domain_host: str):
         domains = self.containers.list_domains_all(container_id=container_id)
         for d in domains:
@@ -476,18 +494,23 @@
         click.echo(f"Adding domain {domain_host}")
         self.containers.create_domain(hostname=domain_host, container_id=container.id)
 
     def await_custom_domain(self, domain_host: str) -> None:
         """Wait for the custom domain to be ready."""
         container = self._get_container_or_abort()
 
-        console.log(f"Waiting for domain {domain_host} to be ready...", style="blue")
+        console.log(f"Waiting for domain {domain_host} to be ready")
+
+        options: WaitForOptions[cnt.Domain, bool] = WaitForOptions()
+        options.timeout = conf.RESOURCE_AWAIT_TIMEOUT_SECONDS
 
         domain = self._get_domain(container.id, domain_host)
-        domain_waited = self.containers.wait_for_domain(domain_id=domain.id)
+        domain_waited = self.containers.wait_for_domain(
+            domain_id=domain.id, options=options
+        )
 
         if domain_waited.status != cnt.DomainStatus.READY:
             console.print("Domain is not ready", style="bold red")
             raise click.Abort()
 
         console.print("Domain ready")
 
@@ -507,8 +530,30 @@
         infra.cpt.ensure_cockpit_activated(self.cockpit)
 
     def import_kong_dashboard(self):
         """Import the kong dashboard via the Grafana API."""
         # We need to create a temporary user to import the dashboard
         with infra.cpt.temporary_grafana_user(api=self.cockpit) as user:
             url = infra.cpt.import_kong_statsd_dashboard(api=self.cockpit, user=user)
-            click.secho(f"Kong dashboard available at:\n {url}", fg="green")
+            console.print("\nKong dashboard available at:")
+            console.print(f"{url}\n")
+
+    def print_summary(self):
+        """Print a summary of the gateway components."""
+        c = conf.InfraConfiguration.load()
+
+        console.rule("[bold]Scaleway Serverless Gateway")
+
+        console.print("\nYour gateway is configured at the following URLs:")
+        console.print(f"Kong Gateway:         {c.gw_url}")
+        console.print(f"Kong Admin (private): {c.gw_admin_url}")
+
+        console.print("\nYou can find metrics for your gateway in your Cockpit at:")
+        console.print("https://console.scaleway.com/cockpit/overview")
+
+        console.print(
+            "\nFor more information on using your gateway, you can find the docs at:"
+        )
+        console.print("https://serverless-gateway.readthedocs.io/en/latest")
+
+        console.print("\nFor more information on Kong Gateway, see the docs here:")
+        console.print("https://docs.konghq.com/gateway/latest/\n")
```

### Comparing `scw_gateway-0.5.0/cli/infra/rdb.py` & `scw_gateway-0.6.0/cli/infra/rdb.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.5.0/cli/infra/secrets.py` & `scw_gateway-0.6.0/cli/infra/secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 
     raise RuntimeError("Could not generate a password")
 
 
 def create_db_password_secret(api: sdk.SecretV1Alpha1API, db_password: str):
     """Store the password to Secret Manager."""
 
-    delete_db_password_secret(api)
+    # Delete password if already exists
+    delete_db_password_secret_if_exists(api)
 
     logger.debug("Creating secret for database password")
     secret = api.create_secret(
         name=PASSWORD_NAME,
         tags=["scw-gw"],
         description="Password for the database for scw-gw",
     )
@@ -50,15 +51,15 @@
     api.create_secret_version(
         secret_id=secret.id,
         data=base64.b64encode(data).decode("utf-8"),
         data_crc32=zlib.crc32(data) & 0xFFFFFFFF,
     )
 
 
-def delete_db_password_secret(api: sdk.SecretV1Alpha1API):
+def delete_db_password_secret_if_exists(api: sdk.SecretV1Alpha1API):
     """Delete the password from Secret Manager."""
     try:
         # Delete password if already exists
         secret = api.get_secret_by_name(secret_name=PASSWORD_NAME)
         logger.debug(f"Deleting {PASSWORD_NAME} secret")
         api.delete_secret(secret_id=secret.id)
```

### Comparing `scw_gateway-0.5.0/cli/model.py` & `scw_gateway-0.6.0/cli/model.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.5.0/pyproject.toml` & `scw_gateway-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scw-gateway"
-version = "0.5.0"
+version = "0.6.0"
 description = "CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem"
 authors = ["Simon Shillaker <sshillaker@scaleway.com>"]
 readme = "README.md"
 packages = [{ include = "cli" }]
 
 [tool.poetry.dependencies]
 loguru = "0.6.0"
@@ -36,22 +36,20 @@
 sphinx_rtd_theme = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-scwgw = "cli.cli:cli"
+scwgw = "cli.cli:main"
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 testpaths = ["tests"]
-markers = [
-  "deployed: Integration tests for a fully deployed environment",
-]
+markers = ["deployed: Integration tests for a fully deployed environment"]
 
 [tool.mypy]
 exclude = ["venv", "endpoints"]
```

### Comparing `scw_gateway-0.5.0/setup.py` & `scw_gateway-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,21 +12,21 @@
  'loguru==0.6.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.2,<3.0.0',
  'rich>=13.4.2,<14.0.0',
  'scaleway>=0.12.0,<0.13.0']
 
 entry_points = \
-{'console_scripts': ['scwgw = cli.cli:cli']}
+{'console_scripts': ['scwgw = cli.cli:main']}
 
 setup_kwargs = {
     'name': 'scw-gateway',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem',
-    'long_description': "# Scaleway Serverless Gateway :spider_web:\n\n[![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)\n[![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)\n[![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)\n\nThe Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).\n\nIt lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.\n\nIt is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.\n\n## :page_with_curl: Contents\n\n- [:rocket: Features](#rocket-features)\n- [:computer: Quick-start](#computer-quick-start)\n- [:mortar\\_board: Contributing](#mortar_board-contributing)\n- [:mailbox: Reach Us](#mailbox-reach-us)\n\nPlease see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.\n\n## :computer: Quick-start\n\nTo deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):\n\n```console\npip install scw-gateway\n```\n\nOnce done, the following steps can be run from the root of the project, and will deploy the gateway as a Serverless Container in your Scaleway account.\n\nThe gateway image itself is packaged via our public [Serverless Gateway Docker image](https://hub.docker.com/r/scaleway/serverless-gateway).\n\n### Deploy your gateway\n\nTo deploy your gateway, you can run:\n\n```console\nscwgw infra deploy\n```\n\n### Add a route\n\nTo check your gateway is working, you can add and remove a route:\n\n```console\n# Check no routes are configured initially\nscwgw route ls\n\n# Check the response directly from a given URL\nTARGET_URL=http://worldtimeapi.org/api/timezone/Europe/Paris\ncurl $TARGET_URL\n\n# Add a route to this URL in your gateway\nscwgw route add /time $TARGET_URL\n\n# List routes to see that it's been configured\nscwgw route ls\n\n# Curl the URL via the gateway\nGATEWAY_ENDPOINT=$(scwgw infra endpoint)\ncurl https://${GATEWAY_ENDPOINT}/time\n```\n\n### Delete your gateway\n\nTo delete your gateway, you can run:\n\n```console\nscwgw infra delete\n```\n\n## :mortar_board: Contributing\n\nWe welcome all contributions to our open-source projects, please see our [contributing guidelines](./.github/CONTRIBUTING.md).\n\nDo not hesitate to raise issues and pull requests we will have a look at them.\n\n## :mailbox: Reach us\n\nWe love feedback. Feel free to:\n\n- Open a [Github issue](https://github.com/scaleway/serverless-functions-python/issues/new)\n- Send us a message on the [Scaleway Slack community](https://slack.scaleway.com/), in the [#serverless-functions](https://scaleway-community.slack.com/app_redirect?channel=serverless-functions) channel.\n",
+    'long_description': '# <img src="logo.png" height="32"/> Scaleway Serverless Gateway\n\n[![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)\n[![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)\n[![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)\n\nThe Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).\n\nIt lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.\n\nIt is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.\n\nYou can read all about it in [this blog post](https://www.scaleway.com/en/blog/api-gateway-early-access/).\n\nIf you would like to join in the discussion on how we continue developing the project, or give us feedback, then join us on the [#api-gateway-beta](https://app.slack.com/client/T7YEXCR7X/C05H07VBKJ4) channel on the Scaleway Community Slack.\n\n## :page_with_curl: Contents\n\n- [ Scaleway Serverless Gateway](#-scaleway-serverless-gateway)\n  - [:page\\_with\\_curl: Contents](#page_with_curl-contents)\n  - [:computer: Quick-start](#computer-quick-start)\n    - [Deploy your gateway](#deploy-your-gateway)\n    - [Add a route](#add-a-route)\n    - [Delete your gateway](#delete-your-gateway)\n  - [:mortar\\_board: Contributing](#mortar_board-contributing)\n  - [:mailbox: Reach us](#mailbox-reach-us)\n\nPlease see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.\n\n## :computer: Quick-start\n\nTo deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):\n\n```console\npip install scw-gateway\n```\n\nOnce done, the following steps can be run from the root of the project, and will deploy the gateway as a Serverless Container in your Scaleway account.\n\nThe gateway image itself is packaged via our public [Serverless Gateway Docker image](https://hub.docker.com/r/scaleway/serverless-gateway).\n\n### Deploy your gateway\n\nTo deploy your gateway, you can run:\n\n```console\nscwgw infra deploy\n```\n\nFor more information on the deployment process, see the [deployment docs](https://serverless-gateway.readthedocs.io/en/latest/deployment.html).\n\n### Add a route\n\nTo check your gateway is working, you can add and remove a route:\n\n```console\n# Check no routes are configured initially\nscwgw route ls\n\n# Check the response directly from a given URL\nTARGET_URL=http://worldtimeapi.org/api/timezone/Europe/Paris\ncurl $TARGET_URL\n\n# Add a route to this URL in your gateway\nscwgw route add /time $TARGET_URL\n\n# List routes to see that it\'s been configured\nscwgw route ls\n\n# Curl the URL via the gateway\nGATEWAY_ENDPOINT=$(scwgw infra endpoint)\ncurl https://${GATEWAY_ENDPOINT}/time\n```\n\n### Delete your gateway\n\nTo delete your gateway, you can run:\n\n```console\nscwgw infra delete\n```\n\n## :mortar_board: Contributing\n\nWe welcome all contributions to our open-source projects, please see our [contributing guidelines](./.github/CONTRIBUTING.md).\n\nDo not hesitate to raise issues and pull requests we will have a look at them.\n\n## :mailbox: Reach us\n\nWe love feedback. Feel free to:\n\n- Open a [Github issue](https://github.com/scaleway/serverless-gateway/issues/new)\n- Send us a message on the [Scaleway Slack community](https://slack.scaleway.com/), in the [#serverless-functions](https://scaleway-community.slack.com/app_redirect?channel=serverless-functions) channel.\n',
     'author': 'Simon Shillaker',
     'author_email': 'sshillaker@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `scw_gateway-0.5.0/PKG-INFO` & `scw_gateway-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scw-gateway
-Version: 0.5.0
+Version: 0.6.0
 Summary: CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem
 Author: Simon Shillaker
 Author-email: sshillaker@scaleway.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,32 +12,40 @@
 Requires-Dist: loguru (==0.6.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: scaleway (>=0.12.0,<0.13.0)
 Description-Content-Type: text/markdown
 
-# Scaleway Serverless Gateway :spider_web:
+# <img src="logo.png" height="32"/> Scaleway Serverless Gateway
 
 [![PyPI version](https://badge.fury.io/py/scw-gateway.svg)](https://badge.fury.io/py/scw-gateway)
 [![Documentation Status](https://readthedocs.org/projects/serverless-gateway/badge/?version=latest)](https://serverless-gateway.readthedocs.io/en/latest/?badge=latest)
 [![Build status](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)](https://github.com/scaleway/serverless-gateway/actions/workflows/build.yml/badge.svg)
 
 The Scaleway Serverless Gateway is a self-hosted API gateway that runs on Scaleway [Serverless Containers](https://www.scaleway.com/en/serverless-containers/).
 
 It lets you manage routing from a single base URL, as well as handle transversal concerns such as CORS and authentication.
 
 It is built on [Kong Gateway](https://docs.konghq.com/gateway/latest/), giving you access to the [Kong plugin ecosystem](https://docs.konghq.com/hub/) to customize your own deployments.
 
+You can read all about it in [this blog post](https://www.scaleway.com/en/blog/api-gateway-early-access/).
+
+If you would like to join in the discussion on how we continue developing the project, or give us feedback, then join us on the [#api-gateway-beta](https://app.slack.com/client/T7YEXCR7X/C05H07VBKJ4) channel on the Scaleway Community Slack.
+
 ## :page_with_curl: Contents
 
-- [:rocket: Features](#rocket-features)
-- [:computer: Quick-start](#computer-quick-start)
-- [:mortar\_board: Contributing](#mortar_board-contributing)
-- [:mailbox: Reach Us](#mailbox-reach-us)
+- [ Scaleway Serverless Gateway](#-scaleway-serverless-gateway)
+  - [:page\_with\_curl: Contents](#page_with_curl-contents)
+  - [:computer: Quick-start](#computer-quick-start)
+    - [Deploy your gateway](#deploy-your-gateway)
+    - [Add a route](#add-a-route)
+    - [Delete your gateway](#delete-your-gateway)
+  - [:mortar\_board: Contributing](#mortar_board-contributing)
+  - [:mailbox: Reach us](#mailbox-reach-us)
 
 Please see [the docs](https://serverless-gateway.readthedocs.io) for full documentation and features.
 
 ## :computer: Quick-start
 
 To deploy your gateway you need to install and configure the [Scaleway CLI](https://github.com/scaleway/scaleway-cli), and the [Gateway CLI](https://pypi.org/project/scw-gateway/) via [`pip`](https://pip.pypa.io/en/stable/index.html):
 
@@ -53,14 +61,16 @@
 
 To deploy your gateway, you can run:
 
 ```console
 scwgw infra deploy
 ```
 
+For more information on the deployment process, see the [deployment docs](https://serverless-gateway.readthedocs.io/en/latest/deployment.html).
+
 ### Add a route
 
 To check your gateway is working, you can add and remove a route:
 
 ```console
 # Check no routes are configured initially
 scwgw route ls
@@ -94,10 +104,10 @@
 
 Do not hesitate to raise issues and pull requests we will have a look at them.
 
 ## :mailbox: Reach us
 
 We love feedback. Feel free to:
 
-- Open a [Github issue](https://github.com/scaleway/serverless-functions-python/issues/new)
+- Open a [Github issue](https://github.com/scaleway/serverless-gateway/issues/new)
 - Send us a message on the [Scaleway Slack community](https://slack.scaleway.com/), in the [#serverless-functions](https://scaleway-community.slack.com/app_redirect?channel=serverless-functions) channel.
```

