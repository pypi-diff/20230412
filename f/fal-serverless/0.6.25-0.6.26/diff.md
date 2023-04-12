# Comparing `tmp/fal_serverless-0.6.25.tar.gz` & `tmp/fal_serverless-0.6.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.25.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.26.tar", max compression
```

## Comparing `fal_serverless-0.6.25.tar` & `fal_serverless-0.6.26.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0        0 2023-04-03 19:14:50.990258 fal_serverless-0.6.25/README.md
--rw-r--r--   0        0        0      798 2023-04-03 19:15:59.018622 fal_serverless-0.6.25/pyproject.toml
--rw-r--r--   0        0        0      294 2023-04-03 19:14:50.990258 fal_serverless-0.6.25/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    14350 2023-04-03 19:14:50.990258 fal_serverless-0.6.25/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2390 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5295 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0     8846 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0      938 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      326 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2479 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     1127 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    14291 2023-04-03 19:14:50.994258 fal_serverless-0.6.25/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 fal_serverless-0.6.25/setup.py
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 fal_serverless-0.6.25/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/README.md
+-rw-r--r--   0        0        0      956 2023-04-12 21:56:24.441663 fal_serverless-0.6.26/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    14760 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2390 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5292 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    11719 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0      172 2023-04-12 21:56:18.645610 fal_serverless-0.6.26/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      326 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     1127 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0    14988 2023-04-12 21:56:08.573568 fal_serverless-0.6.26/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 fal_serverless-0.6.26/setup.py
+-rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 fal_serverless-0.6.26/PKG-INFO
```

### Comparing `fal_serverless-0.6.25/pyproject.toml` & `fal_serverless-0.6.26/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.25"
+version = "0.6.26"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-auth0-python = "^3.24.0"
+auth0-python = "^4.1.0"
 requests = "^2.28.1"
 isolate = {version = "0.11.1", extras = ["build"]}
 grpcio = "^1.50.0"
 dill = "0.3.5.1"
-isolate-proto = "0.0.23"
+isolate-proto = "^0.0.23"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
 datadog-api-client = "^2.9.0"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 grpc-interceptor = "^0.15.0"
 colorama = "^0.4.6"
 portalocker = "^2.7.0"
 rich = "^13.3.2"
 
+# For 3.10 and later, importlib-metadata's newer versions are included in the standard library.
+importlib-metadata = { version = ">=4.4", python = "<3.10" }
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 fal-serverless = "fal_serverless.cli:cli"
```

### Comparing `fal_serverless-0.6.25/src/fal_serverless/api.py` & `fal_serverless-0.6.26/src/fal_serverless/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,20 @@
     @property
     def _connection(self) -> FalServerlessConnection:
         with self._lock:
             client = FalServerlessClient(self.url, self.credentials)
             return client.connect()
 
     @_handle_grpc_error()
-    def register(self, func: Callable[..., ReturnT], options: Options) -> str | None:
+    def register(
+        self,
+        func: Callable[..., ReturnT],
+        options: Options,
+        application_name: str | None = None,
+    ) -> str | None:
         environment_options = options.environment.copy()
         environment_options.setdefault("python_version", active_python())
         environments = [self._connection.define_environment(**environment_options)]
 
         machine_type = options.host.get(
             "machine_type", FAL_SERVERLESS_DEFAULT_MACHINE_TYPE
         )
@@ -249,24 +254,32 @@
         )
 
         partial_func = _execution_controller(func, tuple(), {})
 
         for partial_result in self._connection.register(
             partial_func,
             environments,
+            application_name=application_name,
             machine_requirements=machine_requirements,
         ):
-
             for log in partial_result.logs:
                 self._log_printer.print(log)
 
             if partial_result.result:
                 return partial_result.result.application_id
 
     @_handle_grpc_error()
+    def schedule(
+        self, func: Callable[..., ReturnT], cron: str, options: Options
+    ) -> str | None:
+        application_id = self.register(func, options)
+        cron_id = self._connection.schedule_cronjob(application_id, cron)
+        return cron_id
+
+    @_handle_grpc_error()
     def run(
         self,
         func: Callable[..., ReturnT],
         options: Options,
         args: tuple[Any, ...],
         kwargs: dict[str, Any],
     ) -> ReturnT:
@@ -340,15 +353,14 @@
 
 def isolated(
     kind: str = "virtualenv",
     *,
     host: Host = _DEFAULT_HOST,
     **config: Any,
 ) -> Callable[[Callable[..., ReturnT]], IsolatedFunction[ReturnT]]:
-
     options = host.parse_options(kind=kind, **config)
 
     def wrapper(func: Callable[..., ReturnT]) -> IsolatedFunction[ReturnT]:
         # wrap it with flask if the serve option is set
         func = templated_flask(func) if options.gateway.get("serve") else func
         proxy = IsolatedFunction(
             host=host,
```

### Comparing `fal_serverless-0.6.25/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.26/src/fal_serverless/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.25/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.26/src/fal_serverless/auth/auth0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import time
 import warnings
 
 import click
 import requests
-from auth0.v3.authentication.token_verifier import (
+from auth0.authentication.token_verifier import (
     AsymmetricSignatureVerifier,
     TokenVerifier,
 )
 from fal_serverless.console import console
 from fal_serverless.console.icons import CHECK_ICON
 from fal_serverless.console.ux import get_browser
 from rich.prompt import Confirm
```

### Comparing `fal_serverless-0.6.25/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.26/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.25/src/fal_serverless/cli.py` & `fal_serverless-0.6.26/src/fal_serverless/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from datetime import datetime
 from sys import argv
+from urllib.parse import quote as urlquote
 from uuid import uuid4
 
 import click
 import fal_serverless.auth as auth
 from fal_serverless import api, sdk
 from fal_serverless.console import console
 from fal_serverless.exceptions import ApplicationExceptionHandler
@@ -54,17 +54,16 @@
         set_debug_logging(execution_info.debug)
 
         with self._tracer.start_as_current_span(
             qualified_name, attributes={"invocation_id": invocation_id}
         ):
             try:
                 log.debug(
-                    f"Executing command",
+                    f"Executing command: {qualified_name}",
                     command=qualified_name,
-                    invocation_id=invocation_id,
                 )
                 return super().invoke(ctx)
             except Exception as exception:
                 log.error(exception)
                 if execution_info.debug:
                     # Here we supress detailed errors on click lines because
                     # they're mostly decorator calls, irrelevant to the dev's error tracing
@@ -143,87 +142,21 @@
         for key in keys:
             table.add_row(key.key_id, str(key.created_at))
 
     console.print(table)
 
 
 @key_cli.command(name="revoke")
-@click.argument("key-id", required=True)
+@click.argument("key_id", required=True)
 @click.pass_obj
 def key_revoke(client: sdk.FalServerlessClient, key_id: str):
     with client.connect() as connection:
         connection.revoke_user_key(key_id)
 
 
-###### Scheduled group ######
-@cli.group("scheduled")
-@click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
-@click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
-@click.pass_context
-def scheduled_cli(ctx, host: str, port: str):
-    ctx.obj = sdk.FalServerlessClient(f"{host}:{port}")
-
-
-@scheduled_cli.command(name="list")
-@click.pass_obj
-def list_scheduled(client: sdk.FalServerlessClient):
-    table = Table(title="Scheduled jobs")
-    table.add_column("Job ID")
-    table.add_column("State")
-    table.add_column("Cron")
-
-    with client.connect() as connection:
-        for cron in connection.list_scheduled_runs():
-            table.add_row(cron.run_id, cron.state.name, cron.cron)
-
-    console.print(table)
-
-
-@scheduled_cli.command(name="activations")
-@click.argument("job-id", required=True)
-@click.argument("limit", default=15)
-@click.pass_obj
-def list_activations(client: sdk.FalServerlessClient, job_id: str, limit: int = 15):
-    table = Table(title="Job activations")
-    table.add_column("Job ID")
-    table.add_column("Activation ID")
-    table.add_column("Activation Date")
-
-    with client.connect() as connection:
-        for cron in connection.list_run_activations(job_id)[-limit:]:
-            table.add_row(
-                cron.run_id,
-                cron.activation_id,
-                str(datetime.fromtimestamp(int(cron.activation_id))),
-            )
-
-    console.print(table)
-
-
-@scheduled_cli.command(name="logs")
-@click.argument("job-id", required=True)
-@click.argument("activation-id", required=True)
-@click.pass_obj
-def print_logs(client: sdk.FalServerlessClient, job_id: str, activation_id: str):
-    with client.connect() as connection:
-        raw_logs = connection.get_activation_logs(
-            sdk.ScheduledRunActivation(job_id, activation_id)
-        )
-        console.print(raw_logs.decode(errors="ignore"), highlight=False)
-
-
-@scheduled_cli.command("cancel")
-@click.argument("job-id", required=True)
-@click.pass_obj
-def cancel_scheduled(client: sdk.FalServerlessClient, job_id: str):
-    with client.connect() as connection:
-        connection.cancel_scheduled_run(job_id)
-        console.print("Cancelled", repr(job_id))
-
-
 ###### Usage group ######
 @cli.group("usage")
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
 def usage_cli(ctx, host: str, port: str):
     ctx.obj = sdk.FalServerlessClient(f"{host}:{port}")
@@ -251,39 +184,193 @@
                 str(ws.end_time),
                 str(ws.duration),
             )
 
     console.print(table)
 
 
-@cli.command("register")
+##### Function group #####
+@cli.group("function")
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
+@click.pass_context
+def function_cli(ctx, host: str, port: str):
+    ctx.obj = api.FalServerlessHost(f"{host}:{port}")
+
+
+@function_cli.command("serve")
+@click.option("--alias", default=None)
 @click.argument("file_path", required=True)
 @click.argument("function_name", required=True)
-def register_application(host: str, port: str, file_path: str, function_name: str):
+@click.pass_obj
+def register_application(
+    host: api.FalServerlessHost,
+    file_path: str,
+    function_name: str,
+    alias: str | None = None,
+):
     import runpy
 
     module = runpy.run_path(file_path)
     isolated_function = module[function_name]
-    if not isolated_function.options.gateway.get(
-        "serve"
-    ) and not isolated_function.options.gateway.get("exposed_port"):
+    gateway_options = isolated_function.options.gateway
+    if "serve" not in gateway_options and "exposed_port" not in gateway_options:
         raise api.FalServerlessError(
             "One of `serve` or `exposed-port` options needs to be specified in the isolated annotation to register a function"
         )
-    id = api.FalServerlessHost(f"{host}:{port}").register(
-        func=isolated_function.func, options=isolated_function.options
+    id = host.register(
+        func=isolated_function.func,
+        options=isolated_function.options,
+        application_name=alias,
     )
     if id:
-        console.print("application id: " + id)
+        # TODO: should we centralize this URL format?
+        gateway_host = host.url.replace("api.", "gateway.")
+
+        # Encode since user_id can contain special characters
+        user_id = auth.USER.info["sub"]
+        base_trigger_url = "https://" + urlquote(f"{gateway_host}/trigger/{user_id}")
+        if alias:
+            console.print(
+                f"Registered a new revision for application '{alias}' (revision='{id}')."
+            )
+            console.print(f"App Access URL: {base_trigger_url}/{urlquote(alias)}")
+            console.print(f"Revision Access URL: {base_trigger_url}/{urlquote(id)}")
+        else:
+            console.print(f"Registered anonymous application '{id}'.")
+            console.print(f"Access URL: {base_trigger_url}/{urlquote(id)}")
+
+
+@function_cli.command("schedule")
+@click.argument("cron_string", required=True)
+@click.argument("file_path", required=True)
+@click.argument("function_name", required=True)
+@click.pass_obj
+def register_schedulded(
+    client: api.FalServerlessHost, cron_string: str, file_path: str, function_name: str
+):
+    import runpy
+
+    module = runpy.run_path(file_path)
+    isolated_function = module[function_name]
+
+    cron_id = client.schedule(
+        func=isolated_function.func, cron=cron_string, options=isolated_function.options
+    )
+    if cron_id:
+        console.print(cron_id)
+
+
+##### Crons group #####
+@cli.group("crons")
+@click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
+@click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
+@click.pass_context
+def crons_cli(ctx, host: str, port: str):
+    ctx.obj = api.FalServerlessHost(f"{host}:{port}")
+
+
+@crons_cli.command(name="list")
+@click.pass_obj
+def list_scheduled(client: api.FalServerlessHost):
+    table = Table(title="Cronjobs")
+    table.add_column("Cron ID")
+    table.add_column("Cron")
+    table.add_column("ETA next run")
+    table.add_column("State")
+
+    for cron in client._connection.list_scheduled_runs():
+        state_string = ["Not Active", "Active"][cron.active]
+        table.add_row(cron.cron_id, cron.cron_string, str(cron.next_run), state_string)
+
+    console.print(table)
+
+
+@crons_cli.command(name="activations")
+@click.argument("cron_id", required=True)
+@click.argument("limit", default=15)
+@click.pass_obj
+def list_activations(client: api.FalServerlessHost, cron_id: str, limit: int = 15):
+    table = Table(title="Cron activations")
+    table.add_column("Cron ID")
+    table.add_column("Activation ID")
+    table.add_column("Activation Start Date")
+    table.add_column("Activation Finish Date")
+
+    for activation in client._connection.list_run_activations(cron_id)[-limit:]:
+        table.add_row(
+            cron_id,
+            str(activation.activation_id),
+            str(activation.started_at),
+            str(activation.finished_at),
+        )
+
+    console.print(table)
+
+
+@crons_cli.command(name="logs")
+@click.argument("cron_id", required=True)
+@click.argument("activation-id", required=True)
+@click.pass_obj
+def print_logs(client: api.FalServerlessHost, cron_id: str, activation_id: str):
+    raw_logs = client._connection.get_activation_logs(activation_id)
+    console.print(raw_logs.decode(errors="ignore"), highlight=False)
+
+
+@crons_cli.command("cancel")
+@click.argument("cron_id", required=True)
+@click.pass_obj
+def cancel_scheduled(client: api.FalServerlessHost, cron_id: str):
+    client._connection.cancel_scheduled_run(cron_id)
+    console.print("Cancelled", repr(cron_id))
+
+
+@cli.group("secrets")
+@click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
+@click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
+@click.pass_context
+def secrets_cli(ctx, host: str, port: str):
+    ctx.obj = sdk.FalServerlessClient(f"{host}:{port}")
+
+
+@secrets_cli.command("list")
+@click.pass_obj
+def list_secrets(client: api.FalServerlessClient):
+    table = Table(title="Secrets")
+    table.add_column("Secret Name")
+    table.add_column("Created At")
+
+    with client.connect() as connection:
+        for secret in connection.list_secrets():
+            table.add_row(secret.name, str(secret.created_at))
+
+    console.print(table)
+
+
+@secrets_cli.command("set")
+@click.argument("secret_name", required=True)
+@click.argument("secret_value", required=True)
+@click.pass_obj
+def set_secret(client: api.FalServerlessClient, secret_name: str, secret_value: str):
+    with client.connect() as connection:
+        connection.set_secret(secret_name, secret_value)
+        console.print(f"Secret '{secret_name}' has set")
+
+
+@secrets_cli.command("delete")
+@click.argument("secret_name", required=True)
+@click.pass_obj
+def delete_secret(client: api.FalServerlessClient, secret_name: str):
+    with client.connect() as connection:
+        connection.delete_secret(secret_name)
+        console.print(f"Secret '{secret_name}' has deleted")
 
 
 cli.add_command(auth_cli, name="auth")
 cli.add_command(key_cli, name="key")
-cli.add_command(scheduled_cli, name="scheduled")
+cli.add_command(function_cli, name="function")
+cli.add_command(crons_cli, name="crons")
 cli.add_command(usage_cli, name="usage")
-cli.add_command(register_application, name="register")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `fal_serverless-0.6.25/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.26/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.25/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.26/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.25/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.26/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.25/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.26/src/fal_serverless/logging/datadog.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 from __future__ import annotations
 
-import os
+import sys
 import traceback
 import warnings
 
 from datadog_api_client import Configuration, ThreadedApiClient
 from datadog_api_client.v2.api.logs_api import LogsApi
 from datadog_api_client.v2.model.http_log import HTTPLog
 from datadog_api_client.v2.model.http_log_item import HTTPLogItem
+from fal_serverless.env import CLI_ENV, DATADOG_API_KEY, DATADOG_APP_KEY
+from fal_serverless.logging.trace import get_current_span_context
 from structlog.typing import EventDict, WrappedLogger
 
-from .trace import get_current_span_context
+if sys.version_info >= (3, 10):
+    import importlib.metadata as importlib_metadata
+else:
+    import importlib_metadata
+
 
-# TODO decide on how to inject datadog keys when publishing the package
 configuration = Configuration()
-configuration.api_key["apiKeyAuth"] = os.getenv("DATADOG_API_KEY")
-configuration.api_key["appKeyAuth"] = os.getenv("DATADOG_APP_KEY")
+configuration.api_key["apiKeyAuth"] = DATADOG_API_KEY
+configuration.api_key["appKeyAuth"] = DATADOG_APP_KEY
 
 
 def _is_error_level(level: str) -> bool:
     return level in ["error", "exception", "critical"]
 
 
 def submit_to_datadog(
     logger: WrappedLogger, method_name: str, event_dict: EventDict
 ) -> EventDict:
     if configuration.api_key["apiKeyAuth"] is None:
         return event_dict
 
-    event = event_dict["event"]
+    log_data = dict(event_dict)
+    event = log_data.pop("event")
+    level = log_data.pop("level")
 
     current_span = get_current_span_context()
-    attributes: dict[str, str] = {}
+    attributes = log_data.copy()
     tags: dict[str, str] = {}
     if current_span is not None:
         tags["invocation_id"] = current_span.invocation_id
         attributes["dd.trace_id"] = current_span.trace_id
         attributes["dd.span_id"] = current_span.span_id
 
     stack = None
@@ -43,21 +50,19 @@
         attributes["error.message"] = str(event)
         attributes["error.kind"] = type(event).__name__
         stack = traceback.format_exc()
 
     ddtags = ",".join([f"{key}:{value}" for (key, value) in tags.items()])
     log_item = HTTPLogItem(
         message=str(event),
-        level=method_name,
+        level=level,
         hostname="client",
-        # TODO: leaving koldstart-cli to keep logs in the same place for now
-        service="koldstart-cli",
-        # TODO: how to set these properly?
-        # env="dev",
-        # version="0.6.18a0",
+        service="fal-serverless-cli",
+        env=CLI_ENV,
+        version=importlib_metadata.version("fal_serverless"),
         ddsource="python",
         ddtags=ddtags,
         traceback=stack,
         **attributes,
     )
     with ThreadedApiClient(configuration) as api_client:
         # Deprecation warning of underlying dependencies should not be shown to users
```

### Comparing `fal_serverless-0.6.25/src/fal_serverless/logging/isolate.py` & `fal_serverless-0.6.26/src/fal_serverless/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.25/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.26/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.25/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.26/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.25/setup.py` & `fal_serverless-0.6.26/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,47 +11,51 @@
  'fal_serverless.exceptions',
  'fal_serverless.logging']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['auth0-python>=3.24.0,<4.0.0',
+['auth0-python>=4.1.0,<5.0.0',
  'click>=8.1.3,<9.0.0',
  'colorama>=0.4.6,<0.5.0',
  'datadog-api-client>=2.9.0,<3.0.0',
  'dill==0.3.5.1',
  'grpc-interceptor>=0.15.0,<0.16.0',
  'grpcio>=1.50.0,<2.0.0',
- 'isolate-proto==0.0.23',
+ 'isolate-proto>=0.0.23,<0.0.24',
  'isolate[build]==0.11.1',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'portalocker>=2.7.0,<3.0.0',
  'requests>=2.28.1,<3.0.0',
  'rich>=13.3.2,<14.0.0',
  'structlog>=22.3.0,<23.0.0',
  'typing-extensions==4.4']
 
+extras_require = \
+{':python_version < "3.10"': ['importlib-metadata>=4.4']}
+
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.25',
+    'version': '0.6.26',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
     'long_description': '',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `fal_serverless-0.6.25/PKG-INFO` & `fal_serverless-0.6.26/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.25
+Version: 0.6.26
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: auth0-python (>=3.24.0,<4.0.0)
+Requires-Dist: auth0-python (>=4.1.0,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: datadog-api-client (>=2.9.0,<3.0.0)
 Requires-Dist: dill (==0.3.5.1)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
-Requires-Dist: isolate-proto (==0.0.23)
+Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
+Requires-Dist: isolate-proto (>=0.0.23,<0.0.24)
 Requires-Dist: isolate[build] (==0.11.1)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
```

