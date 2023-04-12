# Comparing `tmp/nb_cli_plugin_docker-0.2.2.tar.gz` & `tmp/nb_cli_plugin_docker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_cli_plugin_docker-0.2.2.tar", max compression
+gzip compressed data, was "nb_cli_plugin_docker-0.3.0.tar", max compression
```

## Comparing `nb_cli_plugin_docker-0.2.2.tar` & `nb_cli_plugin_docker-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1064 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/LICENSE
--rw-r--r--   0        0        0     2195 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/__init__.py
--rw-r--r--   0        0        0     5793 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/cli.py
--rw-r--r--   0        0        0      153 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/exception.py
--rw-r--r--   0        0        0     6541 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/handler.py
--rw-r--r--   0        0        0      226 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/plugin.py
--rw-r--r--   0        0        0     8245 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/static/common/.dockerignore
--rw-r--r--   0        0        0       52 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/static/reverse/docker/_main.py
--rw-r--r--   0        0        0     2472 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/static/reverse/docker/gunicorn_conf.py
--rw-r--r--   0        0        0     1093 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/static/reverse/docker/start.sh
--rw-r--r--   0        0        0      879 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/template/docker/_helpers.Dockerfile.jinja
--rw-r--r--   0        0        0      427 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/template/docker/docker-compose.yml.jinja
--rw-r--r--   0        0        0      517 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/template/docker/forward.Dockerfile.jinja
--rw-r--r--   0        0        0      306 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/template/docker/get_driver_type.py.jinja
--rw-r--r--   0        0        0      753 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/template/docker/reverse.Dockerfile.jinja
--rw-r--r--   0        0        0     1595 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/utils.py
--rw-r--r--   0        0        0     1397 2023-03-12 07:00:57.878952 nb_cli_plugin_docker-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 nb_cli_plugin_docker-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2195 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/__init__.py
+-rw-r--r--   0        0        0     4808 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/cli.py
+-rw-r--r--   0        0        0      153 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/exception.py
+-rw-r--r--   0        0        0     6812 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/handler.py
+-rw-r--r--   0        0        0      226 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/plugin.py
+-rw-r--r--   0        0        0     8245 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/static/common/.dockerignore
+-rw-r--r--   0        0        0       52 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/static/reverse/docker/_main.py
+-rw-r--r--   0        0        0     2472 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/static/reverse/docker/gunicorn_conf.py
+-rw-r--r--   0        0        0     1093 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/static/reverse/docker/start.sh
+-rw-r--r--   0        0        0      879 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/template/docker/_helpers.Dockerfile.jinja
+-rw-r--r--   0        0        0      427 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/template/docker/docker-compose.yml.jinja
+-rw-r--r--   0        0        0      612 2023-04-12 06:51:37.604639 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/template/docker/forward.Dockerfile.jinja
+-rw-r--r--   0        0        0      306 2023-04-12 06:51:37.608640 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/template/docker/get_driver_type.py.jinja
+-rw-r--r--   0        0        0      762 2023-04-12 06:51:37.608640 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/template/docker/reverse.Dockerfile.jinja
+-rw-r--r--   0        0        0     1595 2023-04-12 06:51:37.608640 nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/utils.py
+-rw-r--r--   0        0        0     1397 2023-04-12 06:51:37.608640 nb_cli_plugin_docker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 nb_cli_plugin_docker-0.3.0/PKG-INFO
```

### Comparing `nb_cli_plugin_docker-0.2.2/LICENSE` & `nb_cli_plugin_docker-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_docker-0.2.2/README.md` & `nb_cli_plugin_docker-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/cli.py` & `nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 from typing import List, cast
 
 import click
 from nb_cli import _
+from nb_cli.config import ConfigManager
 from noneprompt import Choice, ListPrompt, CancelledError
-from nb_cli.handlers import detect_virtualenv, get_python_version
 from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedGroup, run_sync, run_async
+from nb_cli.handlers import get_project_root, get_default_python, get_python_version
 
 from .utils import safe_copy_dir, safe_write_file
 from .handler import (
     compose_ps,
     compose_up,
     compose_down,
     compose_logs,
@@ -51,48 +52,35 @@
         ctx.exit()
 
     sub_cmd = result.data
     await run_sync(ctx.invoke)(sub_cmd)
 
 
 @docker.command()
-@click.option("-d", "--cwd", default=".", type=Path, help="The working directory.")
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.option(
     "-f",
     "--force",
     is_flag=True,
     default=False,
     help="Force to re-generate the Dockerfile.",
 )
 @click.pass_context
 @run_async
-async def generate(ctx: click.Context, cwd: Path, venv: bool, force: bool):
+async def generate(ctx: click.Context, force: bool):
     """Generate Dockerfile and docker-compose.yml."""
-    if python_path := detect_virtualenv() if venv else None:
-        click.secho(
-            _("Using virtual environment: {python_path}").format(
-                python_path=python_path
-            ),
-            fg="green",
-        )
-
-    if not cwd.is_dir():
-        click.secho(f"Directory {cwd} does not exist.", fg="red")
-        ctx.exit(1)
+    python_path = await get_default_python()
+    cwd = get_project_root()
 
-    python_version = await get_python_version(python_path)
+    python_version = await get_python_version(python_path=python_path)
     python_version = f"{python_version['major']}.{python_version['minor']}"
+
     is_reverse = await get_driver_type(python_path=python_path, cwd=cwd)
-    build_backend = await get_build_backend()
+    build_backend = await get_build_backend(
+        config_manager=ConfigManager(working_dir=cwd, python_path=python_path)
+    )
 
     try:
         dockerfile = await generate_dockerfile(
             python_version=python_version,
             is_reverse=is_reverse,
             build_backend=build_backend,
         )
@@ -110,77 +98,66 @@
                 Path(__file__).parent / "static" / "reverse", cwd, force=force
             )
     except CancelledError:
         ctx.exit()
 
 
 @docker.command(aliases=["run"], context_settings={"ignore_unknown_options": True})
-@click.option("-d", "--cwd", default=".", type=Path, help="The working directory.")
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.option(
     "-f",
     "--force",
     is_flag=True,
     default=False,
     help="Force to re-generate the Dockerfile.",
 )
 @click.argument("compose_args", nargs=-1)
 @click.pass_context
 @run_async
-async def up(
-    ctx: click.Context, cwd: Path, venv: bool, force: bool, compose_args: List[str]
-):
+async def up(ctx: click.Context, force: bool, compose_args: List[str]):
     """Deploy the bot."""
+    cwd = get_project_root()
+
     if (
         force
         or not Path(cwd, "Dockerfile").exists()
         or not Path(cwd, "docker-compose.yml").exists()
     ):
         await run_sync(ctx.invoke)(generate)
 
     proc = await compose_up(compose_args, cwd=cwd)
     await proc.wait()
 
 
 @docker.command(aliases=["stop"], context_settings={"ignore_unknown_options": True})
-@click.option("-d", "--cwd", default=".", type=Path, help="The working directory.")
 @click.argument("compose_args", nargs=-1)
 @run_async
-async def down(cwd: Path, compose_args: List[str]):
+async def down(compose_args: List[str]):
     """Undeploy the bot."""
-    proc = await compose_down(compose_args, cwd=cwd)
+    proc = await compose_down(compose_args)
     await proc.wait()
 
 
 @docker.command(context_settings={"ignore_unknown_options": True})
-@click.option("-d", "--cwd", default=".", type=Path, help="The working directory.")
 @click.argument("compose_args", nargs=-1)
 @run_async
-async def build(cwd: Path, compose_args: List[str]):
+async def build(compose_args: List[str]):
     """Build the bot image."""
-    proc = await compose_build(compose_args, cwd=cwd)
+    proc = await compose_build(compose_args)
     await proc.wait()
 
 
 @docker.command(context_settings={"ignore_unknown_options": True})
-@click.option("-d", "--cwd", default=".", type=Path, help="The working directory.")
 @click.argument("compose_args", nargs=-1)
 @run_async
-async def logs(cwd: Path, compose_args: List[str]):
+async def logs(compose_args: List[str]):
     """View the bot logs."""
-    proc = await compose_logs(compose_args, cwd=cwd)
+    proc = await compose_logs(compose_args)
     await proc.wait()
 
 
 @docker.command(context_settings={"ignore_unknown_options": True})
-@click.option("-d", "--cwd", default=".", type=Path, help="The working directory.")
 @click.argument("compose_args", nargs=-1)
 @run_async
-async def ps(cwd: Path, compose_args: List[str]):
+async def ps(compose_args: List[str]):
     """View the bot service status."""
-    proc = await compose_ps(compose_args, cwd=cwd)
+    proc = await compose_ps(compose_args)
     await proc.wait()
```

### Comparing `nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/handler.py` & `nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import asyncio
 from pathlib import Path
 from dataclasses import dataclass
 from typing import IO, TYPE_CHECKING, Any, List, Tuple, Union, Literal, Optional, cast
 
 from nb_cli import cache
 from jinja2 import Environment, FileSystemLoader
-from nb_cli.config import GLOBAL_CONFIG, SimpleInfo
 from nb_cli.handlers import templates as cli_templates
+from nb_cli.config import GLOBAL_CONFIG, SimpleInfo, ConfigManager
 from nb_cli.handlers import (
+    get_project_root,
     requires_nonebot,
     get_default_python,
     get_nonebot_config,
     ensure_process_terminated,
 )
 
 from .exception import GetDriverTypeError, ComposeNotAvailable
@@ -69,14 +70,17 @@
 async def call_compose(
     compose_args: Optional[List[str]] = None,
     cwd: Optional[Path] = None,
     stdin: Optional[Union[IO[Any], int]] = None,
     stdout: Optional[Union[IO[Any], int]] = None,
     stderr: Optional[Union[IO[Any], int]] = None,
 ) -> asyncio.subprocess.Process:
+    if cwd is None:
+        cwd = get_project_root()
+
     compose = await get_compose_command()
     return await asyncio.create_subprocess_exec(
         *compose.command,
         *(compose_args or []),
         cwd=cwd,
         stdin=stdin,
         stdout=stdout,
@@ -174,14 +178,16 @@
     bot_config = get_nonebot_config()
     if adapters is None:
         adapters = bot_config.adapters
     if builtin_plugins is None:
         builtin_plugins = bot_config.builtin_plugins
     if python_path is None:
         python_path = await get_default_python()
+    if cwd is None:
+        cwd = get_project_root()
 
     t = templates.get_template("docker/get_driver_type.py.jinja")
     proc = await asyncio.create_subprocess_exec(
         python_path,
         "-W",
         "ignore",
         "-c",
@@ -193,22 +199,27 @@
     stdout, stderr = await proc.communicate()
     if proc.returncode != 0:
         raise GetDriverTypeError(stderr)
 
     return json.loads(stdout.strip())
 
 
-async def get_build_backend() -> Optional[Literal["poetry", "pdm", "pip"]]:
-    if data := GLOBAL_CONFIG._get_data():
+async def get_build_backend(
+    config_manager: Optional[ConfigManager] = None,
+) -> Optional[Literal["poetry", "pdm", "pip"]]:
+    if config_manager is None:
+        config_manager = GLOBAL_CONFIG
+
+    if data := config_manager._get_data():
         backend = data.get("build-system", {}).get("build-backend", "")
         if "poetry" in backend:
             return "poetry"
         elif "pdm" in backend:
             return "pdm"
-    if (GLOBAL_CONFIG.file.parent / "requirements.txt").exists():
+    if (config_manager.project_root / "requirements.txt").exists():
         return "pip"
 
 
 async def generate_dockerfile(
     python_version: str, is_reverse: bool, build_backend: Optional[str]
 ):
     t = templates.get_template(
```

### Comparing `nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/static/common/.dockerignore` & `nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/static/common/.dockerignore`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/static/reverse/docker/gunicorn_conf.py` & `nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/static/reverse/docker/gunicorn_conf.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/static/reverse/docker/start.sh` & `nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/static/reverse/docker/start.sh`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/template/docker/_helpers.Dockerfile.jinja` & `nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/template/docker/_helpers.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/template/docker/reverse.Dockerfile.jinja` & `nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/template/docker/reverse.Dockerfile.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 
 COPY --from=requirements_stage /tmp/bot.py /app
 COPY ./docker/_main.py /app
 {% if build_backend %}
 COPY --from=requirements_stage /wheel /wheel
 {% endif %}
 
-RUN pip install --no-cache-dir gunicorn uvicorn[standard]{% if build_backend %} \
+RUN pip install --no-cache-dir gunicorn uvicorn[standard] nonebot2{% if build_backend %} \
   && pip install --no-cache-dir --no-index --force-reinstall --find-links=/wheel -r /wheel/requirements.txt && rm -rf /wheel{% endif %}
 
 COPY . /app/
 
 CMD ["/start.sh"]
```

### Comparing `nb_cli_plugin_docker-0.2.2/nb_cli_plugin_docker/utils.py` & `nb_cli_plugin_docker-0.3.0/nb_cli_plugin_docker/utils.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_docker-0.2.2/pyproject.toml` & `nb_cli_plugin_docker-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nb-cli-plugin-docker"
-version = "0.2.2"
+version = "0.3.0"
 description = "docker support for nb-cli"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/nonebot/cli-plugin-docker"
 repository = "https://github.com/nonebot/cli-plugin-docker"
 documentation = "https://github.com/nonebot/cli-plugin-docker#readme"
@@ -16,15 +16,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nb-cli = "^1.0.5"
+nb-cli = "^1.1.0"
 noneprompt = "^0.1.7"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
 black = "^22.3.0"
 nonemoji = "^0.1.2"
 pre-commit = "^2.16.0"
```

### Comparing `nb_cli_plugin_docker-0.2.2/PKG-INFO` & `nb_cli_plugin_docker-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-cli-plugin-docker
-Version: 0.2.2
+Version: 0.3.0
 Summary: docker support for nb-cli
 Home-page: https://github.com/nonebot/cli-plugin-docker
 License: MIT
 Keywords: nonebot,cli,docker
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: nb-cli (>=1.0.5,<2.0.0)
+Requires-Dist: nb-cli (>=1.1.0,<2.0.0)
 Requires-Dist: noneprompt (>=0.1.7,<0.2.0)
 Project-URL: Documentation, https://github.com/nonebot/cli-plugin-docker#readme
 Project-URL: Repository, https://github.com/nonebot/cli-plugin-docker
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD041 -->
 <p align="center">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nb-cli-plugin-docker Version: 0.2.2 Summary: docker
+Metadata-Version: 2.1 Name: nb-cli-plugin-docker Version: 0.3.0 Summary: docker
 support for nb-cli Home-page: https://github.com/nonebot/cli-plugin-docker
 License: MIT Keywords: nonebot,cli,docker Author: yanyongyu Author-email:
 yyy@nonebot.dev Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Framework :: Robot Framework Classifier:
 Framework :: Robot Framework :: Library Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 Requires-Dist:
-nb-cli (>=1.0.5,<2.0.0) Requires-Dist: noneprompt (>=0.1.7,<0.2.0) Project-URL:
+nb-cli (>=1.1.0,<2.0.0) Requires-Dist: noneprompt (>=0.1.7,<0.2.0) Project-URL:
 Documentation, https://github.com/nonebot/cli-plugin-docker#readme Project-URL:
 Repository, https://github.com/nonebot/cli-plugin-docker Description-Content-
 Type: text/markdown
                                    [nonebot]
     # NB CLI Plugin Docker _â¨ NoneBot2 å½ä»¤è¡å·¥å· Docker æä»¶ â¨_
                     [license] [pypi] [python] [pre-commit]
        [QQ_Chat_Group] [QQ_Channel] [Telegram_Channel] [Discord_Server]
```

