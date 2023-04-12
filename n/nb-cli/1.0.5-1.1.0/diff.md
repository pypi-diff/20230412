# Comparing `tmp/nb-cli-1.0.5.tar.gz` & `tmp/nb-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-cli-1.0.5.tar", last modified: Sat Feb 18 17:28:27 2023, max compression
+gzip compressed data, was "nb-cli-1.1.0.tar", last modified: Wed Apr 12 06:06:29 2023, max compression
```

## Comparing `nb-cli-1.0.5.tar` & `nb-cli-1.1.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
--rw-r--r--   0        0        0     1065 2023-02-18 17:27:51.318459 nb-cli-1.0.5/LICENSE
--rw-r--r--   0        0        0     3350 2023-02-18 17:27:51.318459 nb-cli-1.0.5/README.md
--rw-r--r--   0        0        0      246 2023-02-18 17:27:51.318459 nb-cli-1.0.5/build.py
--rw-r--r--   0        0        0      779 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/__init__.py
--rw-r--r--   0        0        0      202 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/__main__.py
--rw-r--r--   0        0        0     3244 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/cli/__init__.py
--rw-r--r--   0        0        0      257 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/cli/commands/__init__.py
--rw-r--r--   0        0        0     7923 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/cli/commands/adapter.py
--rw-r--r--   0        0        0     5640 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/cli/commands/driver.py
--rw-r--r--   0        0        0     8178 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/cli/commands/plugin.py
--rw-r--r--   0        0        0    10350 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/cli/commands/project.py
--rw-r--r--   0        0        0     3409 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/cli/commands/self.py
--rw-r--r--   0        0        0     6271 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/cli/customize.py
--rw-r--r--   0        0        0     1966 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/cli/utils.py
--rw-r--r--   0        0        0      314 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/config/__init__.py
--rw-r--r--   0        0        0      661 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/config/model.py
--rw-r--r--   0        0        0     3833 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/config/parser.py
--rw-r--r--   0        0        0      347 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/consts.py
--rw-r--r--   0        0        0      373 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/exceptions.py
--rw-r--r--   0        0        0     2675 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/__init__.py
--rw-r--r--   0        0        0      864 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/adapter.py
--rw-r--r--   0        0        0      399 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/driver.py
--rw-r--r--   0        0        0    10301 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/meta.py
--rw-r--r--   0        0        0     3259 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/pip.py
--rw-r--r--   0        0        0     1519 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/plugin.py
--rw-r--r--   0        0        0     2641 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/project.py
--rw-r--r--   0        0        0     5267 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/reloader.py
--rw-r--r--   0        0        0     2042 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/script.py
--rw-r--r--   0        0        0     1163 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/signal.py
--rw-r--r--   0        0        0      996 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/handlers/venv.py
--rw-r--r--   0        0        0     1193 2023-02-18 17:27:51.318459 nb-cli-1.0.5/nb_cli/i18n.py
--rw-r--r--   0        0        0     8196 2023-02-18 17:28:25.086491 nb-cli-1.0.5/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
--rw-r--r--   0        0        0    13483 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
--rw-r--r--   0        0        0        0 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/py.typed
--rw-r--r--   0        0        0      143 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/adapter/cookiecutter.json
--rw-r--r--   0        0        0      120 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      847 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
--rw-r--r--   0        0        0      354 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
--rw-r--r--   0        0        0      203 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0      688 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
--rw-r--r--   0        0        0      676 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
--rw-r--r--   0        0        0      164 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/plugin/cookiecutter.json
--rw-r--r--   0        0        0      315 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/plugin/hooks/post_gen_project.py
--rw-r--r--   0        0        0      402 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      114 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0        0 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
--rw-r--r--   0        0        0      259 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/bootstrap/cookiecutter.json
--rw-r--r--   0        0        0      132 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0      235 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      611 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0      442 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/simple/cookiecutter.json
--rw-r--r--   0        0        0      307 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/simple/hooks/post_gen_project.py
--rw-r--r--   0        0        0      148 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
--rw-r--r--   0        0        0       16 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
--rw-r--r--   0        0        0        0 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0     2087 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
--rw-r--r--   0        0        0      331 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      657 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
--rw-r--r--   0        0        0      232 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/scripts/meta/_package_version.py.jinja
--rw-r--r--   0        0        0      110 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/scripts/meta/nonebot_version.py.jinja
--rw-r--r--   0        0        0      105 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/scripts/meta/pip_version.py.jinja
--rw-r--r--   0        0        0      142 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/scripts/meta/python_version.py.jinja
--rw-r--r--   0        0        0      175 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
--rw-r--r--   0        0        0     1091 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/scripts/project/_prepare.py.jinja
--rw-r--r--   0        0        0      151 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/scripts/project/run_project.py.jinja
--rw-r--r--   0        0        0      222 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/scripts/script/_entrypoint.py.jinja
--rw-r--r--   0        0        0      158 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/scripts/script/list_scripts.py.jinja
--rw-r--r--   0        0        0      333 2023-02-18 17:27:51.322459 nb-cli-1.0.5/nb_cli/template/scripts/script/run_script.py.jinja
--rw-r--r--   0        0        0     2715 2023-02-18 17:27:51.322459 nb-cli-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 nb-cli-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-12 06:05:51.076853 nb-cli-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3350 2023-04-12 06:05:51.076853 nb-cli-1.1.0/README.md
+-rw-r--r--   0        0        0      246 2023-04-12 06:05:51.076853 nb-cli-1.1.0/build.py
+-rw-r--r--   0        0        0      795 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/__init__.py
+-rw-r--r--   0        0        0      202 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/__main__.py
+-rw-r--r--   0        0        0     3305 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/__init__.py
+-rw-r--r--   0        0        0      257 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6866 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/adapter.py
+-rw-r--r--   0        0        0     4243 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/driver.py
+-rw-r--r--   0        0        0     7195 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/plugin.py
+-rw-r--r--   0        0        0    10063 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/project.py
+-rw-r--r--   0        0        0     3409 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/self.py
+-rw-r--r--   0        0        0     5459 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/customize.py
+-rw-r--r--   0        0        0     1966 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/utils.py
+-rw-r--r--   0        0        0      429 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/config/__init__.py
+-rw-r--r--   0        0        0      661 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/config/model.py
+-rw-r--r--   0        0        0     6153 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/config/parser.py
+-rw-r--r--   0        0        0      347 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/consts.py
+-rw-r--r--   0        0        0      373 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/exceptions.py
+-rw-r--r--   0        0        0     2906 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/__init__.py
+-rw-r--r--   0        0        0      865 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/adapter.py
+-rw-r--r--   0        0        0      374 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/driver.py
+-rw-r--r--   0        0        0     5756 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/meta.py
+-rw-r--r--   0        0        0     3198 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/pip.py
+-rw-r--r--   0        0        0     1557 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/plugin.py
+-rw-r--r--   0        0        0     2986 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/process.py
+-rw-r--r--   0        0        0     2665 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/project.py
+-rw-r--r--   0        0        0     5718 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/reloader.py
+-rw-r--r--   0        0        0     2063 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/script.py
+-rw-r--r--   0        0        0     1860 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/signal.py
+-rw-r--r--   0        0        0     3720 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/store.py
+-rw-r--r--   0        0        0      734 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/venv.py
+-rw-r--r--   0        0        0     1193 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/i18n.py
+-rw-r--r--   0        0        0     8829 2023-04-12 06:06:27.398844 nb-cli-1.1.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
+-rw-r--r--   0        0        0    13703 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
+-rw-r--r--   0        0        0      635 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/log/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/py.typed
+-rw-r--r--   0        0        0      143 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/cookiecutter.json
+-rw-r--r--   0        0        0      120 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      847 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      354 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      203 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      688 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      676 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      164 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/plugin/cookiecutter.json
+-rw-r--r--   0        0        0      315 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/plugin/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      385 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      114 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0        0 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      259 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/bootstrap/cookiecutter.json
+-rw-r--r--   0        0        0      132 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0      235 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      611 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      452 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/cookiecutter.json
+-rw-r--r--   0        0        0      307 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      148 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
+-rw-r--r--   0        0        0       16 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
+-rw-r--r--   0        0        0        0 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0     2087 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
+-rw-r--r--   0        0        0      331 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      657 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      232 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/meta/_package_version.py.jinja
+-rw-r--r--   0        0        0      110 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/meta/nonebot_version.py.jinja
+-rw-r--r--   0        0        0      105 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/meta/pip_version.py.jinja
+-rw-r--r--   0        0        0      142 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/meta/python_version.py.jinja
+-rw-r--r--   0        0        0      181 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
+-rw-r--r--   0        0        0     1091 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/project/_prepare.py.jinja
+-rw-r--r--   0        0        0      151 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/project/run_project.py.jinja
+-rw-r--r--   0        0        0      222 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/script/_entrypoint.py.jinja
+-rw-r--r--   0        0        0      158 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/script/list_scripts.py.jinja
+-rw-r--r--   0        0        0      333 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/script/run_script.py.jinja
+-rw-r--r--   0        0        0     2737 2023-04-12 06:05:51.080854 nb-cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 nb-cli-1.1.0/PKG-INFO
```

### Comparing `nb-cli-1.0.5/LICENSE` & `nb-cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/README.md` & `nb-cli-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/__init__.py` & `nb-cli-1.1.0/nb_cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 from .consts import PLUGINS_GROUP
 from .handlers import install_signal_handler
 
 
 def load_plugins():
     entrypoint: EntryPoint
     for entrypoint in entry_points(group=PLUGINS_GROUP):
-        entrypoint.load()()
+        entrypoint.load()()  # type: ignore
 
 
 async def cli_main(*args, **kwargs):
     install_signal_handler()
     load_plugins()
     return await run_sync(cli_sync)(*args, **kwargs)
```

### Comparing `nb-cli-1.0.5/nb_cli/cli/__init__.py` & `nb-cli-1.1.0/nb_cli/cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from pathlib import Path
-from typing import List, cast
+from typing import List, Optional, cast
 
 import click
 from noneprompt import Choice, ListPrompt, CancelledError
 
 from nb_cli import _, __version__
 from nb_cli.handlers import draw_logo
-from nb_cli.config import GLOBAL_CONFIG
+from nb_cli.config import ConfigManager
 
 from .utils import run_sync as run_sync
 from .utils import run_async as run_async
 from .customize import CLIMainGroup as CLIMainGroup
 from .utils import CLI_DEFAULT_STYLE as CLI_DEFAULT_STYLE
 from .customize import ClickAliasedGroup as ClickAliasedGroup
 from .customize import ClickAliasedCommand as ClickAliasedCommand
 
 
-def prepare_config(ctx: click.Context, param: click.Option, value: str):
-    GLOBAL_CONFIG.file = Path(value)
+def _set_global_working_dir(
+    ctx: click.Context, param: click.Option, value: Optional[Path]
+):
+    ConfigManager._global_working_dir = value
 
 
-def prepare_encoding(ctx: click.Context, param: click.Option, value: str):
-    GLOBAL_CONFIG.encoding = value
+def _set_global_python_path(
+    ctx: click.Context, param: click.Option, value: Optional[str]
+):
+    ConfigManager._global_python_path = value
 
 
-def prepare_python(ctx: click.Context, param: click.Option, value: str):
-    GLOBAL_CONFIG.python = value
+def _set_global_use_venv(ctx: click.Context, param: click.Option, value: bool):
+    ConfigManager._global_use_venv = value
 
 
 @click.group(
     cls=CLIMainGroup,
     invoke_without_command=True,
     context_settings={"help_option_names": ["-h", "--help"]},
 )
@@ -37,40 +41,39 @@
     __version__,
     "-V",
     "--version",
     prog_name="nb",
     message="%(prog)s: nonebot cli version %(version)s",
 )
 @click.option(
-    "-c",
-    "--config",
-    default="pyproject.toml",
-    help=_("Config file path."),
-    type=click.Path(exists=False, dir_okay=False, readable=True),
-    is_eager=True,
-    expose_value=False,
-    callback=prepare_config,
-)
-@click.option(
-    "-e",
-    "--encoding",
-    default="utf-8",
-    help=_("Config file encoding."),
+    "-d",
+    "--cwd",
+    default=None,
+    help=_("The working directory."),
+    type=Path,
     is_eager=True,
     expose_value=False,
-    callback=prepare_encoding,
+    callback=_set_global_working_dir,
 )
 @click.option(
     "-py",
     "--python",
     default=None,
     help=_("Python executable path."),
     is_eager=True,
     expose_value=False,
-    callback=prepare_python,
+    callback=_set_global_python_path,
+)
+@click.option(
+    "--venv/--no-venv",
+    default=True,
+    help=_("Auto detect virtual environment."),
+    is_eager=True,
+    expose_value=False,
+    callback=_set_global_use_venv,
 )
 @click.pass_context
 @run_async
 async def cli(ctx: click.Context):
     # postpone scripts discovery, only when needed (invoked)
     # see {ref}`CLIMainGroup.get_command <nb_cli.cli.customize.CLIMainGroup.get_command>`
```

### Comparing `nb-cli-1.0.5/nb_cli/cli/commands/adapter.py` & `nb-cli-1.1.0/nb_cli/cli/commands/adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from nb_cli.cli.utils import find_exact_package
 from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedGroup, run_sync, run_async
 from nb_cli.handlers import (
     list_adapters,
     create_adapter,
     call_pip_update,
     call_pip_install,
-    detect_virtualenv,
     call_pip_uninstall,
     format_package_results,
 )
 
 
 @click.group(
     cls=ClickAliasedGroup, invoke_without_command=True, help=_("Manage bot adapters.")
@@ -72,26 +71,20 @@
 
 
 @adapter.command(
     aliases=["add"],
     context_settings={"ignore_unknown_options": True},
     help=_("Install nonebot adapter to current project."),
 )
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.argument("name", nargs=1, default=None)
 @click.argument("pip_args", nargs=-1, default=None)
 @click.pass_context
 @run_async
 async def install(
-    ctx: click.Context, venv: bool, name: Optional[str], pip_args: Optional[List[str]]
+    ctx: click.Context, name: Optional[str], pip_args: Optional[List[str]]
 ):
     try:
         adapter = await find_exact_package(
             _("Adapter name to install:"), name, await list_adapters()
         )
     except CancelledError:
         ctx.exit()
@@ -103,82 +96,52 @@
     except RuntimeError as e:
         click.echo(
             _("Failed to add adapter {adapter.name} to config: {e}").format(
                 adapter=adapter, e=e
             )
         )
 
-    if python_path := detect_virtualenv() if venv else None:
-        click.secho(
-            _("Using virtual environment: {python_path}").format(
-                python_path=python_path
-            ),
-            fg="green",
-        )
-    proc = await call_pip_install(
-        adapter.project_link, pip_args, python_path=python_path
-    )
+    proc = await call_pip_install(adapter.project_link, pip_args)
     await proc.wait()
 
 
 @adapter.command(
     context_settings={"ignore_unknown_options": True}, help=_("Update nonebot adapter.")
 )
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.argument("name", nargs=1, default=None)
 @click.argument("pip_args", nargs=-1, default=None)
 @click.pass_context
 @run_async
 async def update(
-    ctx: click.Context, venv: bool, name: Optional[str], pip_args: Optional[List[str]]
+    ctx: click.Context, name: Optional[str], pip_args: Optional[List[str]]
 ):
     try:
         adapter = await find_exact_package(
             _("Adapter name to update:"), name, await list_adapters()
         )
     except CancelledError:
         ctx.exit()
     except Exception:
         ctx.exit(1)
 
-    if python_path := detect_virtualenv() if venv else None:
-        click.secho(
-            _("Using virtual environment: {python_path}").format(
-                python_path=python_path
-            ),
-            fg="green",
-        )
-    proc = await call_pip_update(
-        adapter.project_link, pip_args, python_path=python_path
-    )
+    proc = await call_pip_update(adapter.project_link, pip_args)
     await proc.wait()
 
 
 @adapter.command(
     aliases=["remove"],
     context_settings={"ignore_unknown_options": True},
     help=_("Uninstall nonebot adapter from current project."),
 )
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.argument("name", nargs=1, default=None)
 @click.argument("pip_args", nargs=-1, default=None)
 @click.pass_context
 @run_async
 async def uninstall(
-    ctx: click.Context, venv: bool, name: Optional[str], pip_args: Optional[List[str]]
+    ctx: click.Context, name: Optional[str], pip_args: Optional[List[str]]
 ):
     try:
         adapter = await find_exact_package(
             _("Adapter name to uninstall:"), name, await list_adapters()
         )
     except CancelledError:
         ctx.exit()
@@ -190,24 +153,15 @@
     except RuntimeError as e:
         click.echo(
             _("Failed to remove adapter {adapter.name} from config: {e}").format(
                 adapter=adapter, e=e
             )
         )
 
-    if python_path := detect_virtualenv() if venv else None:
-        click.secho(
-            _("Using virtual environment: {python_path}").format(
-                python_path=python_path
-            ),
-            fg="green",
-        )
-    proc = await call_pip_uninstall(
-        adapter.project_link, pip_args, python_path=python_path
-    )
+    proc = await call_pip_uninstall(adapter.project_link, pip_args)
     await proc.wait()
 
 
 @adapter.command(aliases=["new"], help=_("Create a new nonebot adapter."))
 @click.argument("name", default=None)
 @click.option(
     "-o",
@@ -229,15 +183,20 @@
             name = await InputPrompt(_("Adapter name:")).prompt_async(
                 style=CLI_DEFAULT_STYLE
             )
         except CancelledError:
             ctx.exit()
     if output_dir is None:
         detected: List[Choice[None]] = [
-            Choice(str(x)) for x in Path(".").glob("**/adapters/") if x.is_dir()
+            Choice(str(x))
+            for x in Path(".").glob("**/adapters/")
+            if x.is_dir()
+            and not any(
+                p.name.startswith(".") or p.name.startswith("_") for p in x.parents
+            )
         ] or [
             Choice(f"{x}/adapters/")
             for x in Path(".").glob("*/")
             if x.is_dir() and not x.name.startswith(".") and not x.name.startswith("_")
         ]
         try:
             output_dir = (
@@ -252,12 +211,14 @@
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
         except CancelledError:
             ctx.exit()
     elif not Path(output_dir).is_dir():
         click.secho(_("Output dir is not a directory!"), fg="yellow")
         try:
             output_dir = await InputPrompt(
-                _("Output Dir:"), validator=lambda x: len(x) > 0 and Path(x).is_dir()
+                _("Output Dir:"),
+                validator=lambda x: len(x) > 0 and Path(x).is_dir(),
+                error_message=_("Invalid output dir!"),
             ).prompt_async(style=CLI_DEFAULT_STYLE)
         except CancelledError:
             ctx.exit()
     create_adapter(name, output_dir, template=template)
```

### Comparing `nb-cli-1.0.5/nb_cli/cli/commands/driver.py` & `nb-cli-1.1.0/nb_cli/cli/commands/driver.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from nb_cli import _
 from nb_cli.cli.utils import find_exact_package
 from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedGroup, run_sync, run_async
 from nb_cli.handlers import (
     list_drivers,
     call_pip_update,
     call_pip_install,
-    detect_virtualenv,
     call_pip_uninstall,
     format_package_results,
 )
 
 
 @click.group(
     cls=ClickAliasedGroup, invoke_without_command=True, help=_("Manage bot driver.")
@@ -69,124 +68,79 @@
 
 
 @driver.command(
     aliases=["add"],
     context_settings={"ignore_unknown_options": True},
     help=_("Install nonebot driver to current project."),
 )
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.argument("name", nargs=1, default=None)
 @click.argument("pip_args", nargs=-1, default=None)
 @click.pass_context
 @run_async
 async def install(
-    ctx: click.Context, venv: bool, name: Optional[str], pip_args: Optional[List[str]]
+    ctx: click.Context, name: Optional[str], pip_args: Optional[List[str]]
 ):
     try:
         driver = await find_exact_package(
             _("Driver name to install:"), name, await list_drivers()
         )
     except CancelledError:
         ctx.exit()
     except Exception:
         ctx.exit(1)
 
     if driver.project_link:
-        if python_path := detect_virtualenv() if venv else None:
-            click.secho(
-                _("Using virtual environment: {python_path}").format(
-                    python_path=python_path
-                ),
-                fg="green",
-            )
-        proc = await call_pip_install(
-            driver.project_link, pip_args, python_path=python_path
-        )
+        proc = await call_pip_install(driver.project_link, pip_args)
         await proc.wait()
 
 
 @driver.command(
     context_settings={"ignore_unknown_options": True}, help=_("Update nonebot driver.")
 )
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.argument("name", nargs=1, default=None)
 @click.argument("pip_args", nargs=-1, default=None)
 @click.pass_context
 @run_async
 async def update(
-    ctx: click.Context, venv: bool, name: Optional[str], pip_args: Optional[List[str]]
+    ctx: click.Context, name: Optional[str], pip_args: Optional[List[str]]
 ):
     try:
         driver = await find_exact_package(
             _("Driver name to update:"), name, await list_drivers()
         )
     except CancelledError:
         ctx.exit()
     except Exception:
         ctx.exit(1)
 
     if driver.project_link:
-        if python_path := detect_virtualenv() if venv else None:
-            click.secho(
-                _("Using virtual environment: {python_path}").format(
-                    python_path=python_path
-                ),
-                fg="green",
-            )
-        proc = await call_pip_update(
-            driver.project_link, pip_args, python_path=python_path
-        )
+        proc = await call_pip_update(driver.project_link, pip_args)
         await proc.wait()
 
 
 @driver.command(
     aliases=["remove"],
     context_settings={"ignore_unknown_options": True},
     help=_("Uninstall nonebot driver from current project."),
 )
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.argument("name", nargs=1, default=None)
 @click.argument("pip_args", nargs=-1, default=None)
 @click.pass_context
 @run_async
 async def uninstall(
-    ctx: click.Context, venv: bool, name: Optional[str], pip_args: Optional[List[str]]
+    ctx: click.Context, name: Optional[str], pip_args: Optional[List[str]]
 ):
     try:
         driver = await find_exact_package(
             _("Driver name to uninstall:"), name, await list_drivers()
         )
     except CancelledError:
         ctx.exit()
     except Exception:
         ctx.exit(1)
 
     if package := driver.project_link:
         if package.startswith("nonebot2[") and package.endswith("]"):
             package = package[9:-1]
 
-        if python_path := detect_virtualenv() if venv else None:
-            click.secho(
-                _("Using virtual environment: {python_path}").format(
-                    python_path=python_path
-                ),
-                fg="green",
-            )
-        proc = await call_pip_uninstall(
-            driver.project_link, pip_args, python_path=python_path
-        )
+        proc = await call_pip_uninstall(package, pip_args)
         await proc.wait()
```

### Comparing `nb-cli-1.0.5/nb_cli/cli/commands/plugin.py` & `nb-cli-1.1.0/nb_cli/cli/commands/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from nb_cli.cli.utils import find_exact_package
 from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedGroup, run_sync, run_async
 from nb_cli.handlers import (
     list_plugins,
     create_plugin,
     call_pip_update,
     call_pip_install,
-    detect_virtualenv,
     call_pip_uninstall,
     format_package_results,
 )
 
 
 @click.group(
     cls=ClickAliasedGroup, invoke_without_command=True, help=_("Manage bot plugins.")
@@ -72,26 +71,20 @@
 
 
 @plugin.command(
     aliases=["add"],
     context_settings={"ignore_unknown_options": True},
     help=_("Install nonebot plugin to current project."),
 )
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.argument("name", nargs=1, required=False, default=None)
 @click.argument("pip_args", nargs=-1, default=None)
 @click.pass_context
 @run_async
 async def install(
-    ctx: click.Context, venv: bool, name: Optional[str], pip_args: Optional[List[str]]
+    ctx: click.Context, name: Optional[str], pip_args: Optional[List[str]]
 ):
     try:
         plugin = await find_exact_package(
             _("Plugin name to install:"), name, await list_plugins()
         )
     except CancelledError:
         ctx.exit()
@@ -103,80 +96,52 @@
     except RuntimeError as e:
         click.echo(
             _("Failed to add plugin {plugin.name} to config: {e}").format(
                 plugin=plugin, e=e
             )
         )
 
-    if python_path := detect_virtualenv() if venv else None:
-        click.secho(
-            _("Using virtual environment: {python_path}").format(
-                python_path=python_path
-            ),
-            fg="green",
-        )
-    proc = await call_pip_install(
-        plugin.project_link, pip_args, python_path=python_path
-    )
+    proc = await call_pip_install(plugin.project_link, pip_args)
     await proc.wait()
 
 
 @plugin.command(
     context_settings={"ignore_unknown_options": True}, help=_("Update nonebot plugin.")
 )
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.argument("name", nargs=1, required=False, default=None)
 @click.argument("pip_args", nargs=-1, default=None)
 @click.pass_context
 @run_async
 async def update(
-    ctx: click.Context, venv: bool, name: Optional[str], pip_args: Optional[List[str]]
+    ctx: click.Context, name: Optional[str], pip_args: Optional[List[str]]
 ):
     try:
         plugin = await find_exact_package(
             _("Plugin name to update:"), name, await list_plugins()
         )
     except CancelledError:
         ctx.exit()
     except Exception:
         ctx.exit(1)
 
-    if python_path := detect_virtualenv() if venv else None:
-        click.secho(
-            _("Using virtual environment: {python_path}").format(
-                python_path=python_path
-            ),
-            fg="green",
-        )
-    proc = await call_pip_update(plugin.project_link, pip_args, python_path=python_path)
+    proc = await call_pip_update(plugin.project_link, pip_args)
     await proc.wait()
 
 
 @plugin.command(
     aliases=["remove"],
     context_settings={"ignore_unknown_options": True},
     help=_("Uninstall nonebot plugin from current project."),
 )
-@click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
 @click.argument("name", nargs=1, required=False, default=None)
 @click.argument("pip_args", nargs=-1, default=None)
 @click.pass_context
 @run_async
 async def uninstall(
-    ctx: click.Context, venv: bool, name: Optional[str], pip_args: Optional[List[str]]
+    ctx: click.Context, name: Optional[str], pip_args: Optional[List[str]]
 ):
     try:
         plugin = await find_exact_package(
             _("Plugin name to uninstall:"), name, await list_plugins()
         )
     except CancelledError:
         ctx.exit()
@@ -188,24 +153,15 @@
     except RuntimeError as e:
         click.echo(
             _("Failed to remove plugin {plugin.name} from config: {e}").format(
                 plugin=plugin, e=e
             )
         )
 
-    if python_path := detect_virtualenv() if venv else None:
-        click.secho(
-            _("Using virtual environment: {python_path}").format(
-                python_path=python_path
-            ),
-            fg="green",
-        )
-    proc = await call_pip_uninstall(
-        plugin.project_link, pip_args, python_path=python_path
-    )
+    proc = await call_pip_uninstall(plugin.project_link, pip_args)
     await proc.wait()
 
 
 @plugin.command(aliases=["new"], help=_("Create a new nonebot plugin."))
 @click.argument("name", nargs=1, required=False, default=None)
 @click.option("-s", "--sub-plugin", is_flag=True, default=None)
 @click.option(
@@ -237,32 +193,40 @@
                 _("Use nested plugin?"), default_choice=False
             ).prompt_async(style=CLI_DEFAULT_STYLE)
         except CancelledError:
             ctx.exit()
 
     if output_dir is None:
         detected: List[Choice[None]] = [
-            Choice(str(d)) for d in Path(".").glob("**/plugins/") if d.is_dir()
+            Choice(str(d))
+            for d in Path(".").glob("**/plugins/")
+            if d.is_dir()
+            and not any(
+                p.name.startswith("_") or p.name.startswith(".") for p in d.parents
+            )
         ]
         try:
             output_dir = (
                 await ListPrompt(
                     _("Where to store the plugin?"), detected + [Choice(_("Other"))]
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
             ).name
             if output_dir == _("Other"):
                 output_dir = await InputPrompt(
                     _("Output Dir:"),
                     validator=lambda x: len(x) > 0 and Path(x).is_dir(),
+                    error_message=_("Invalid output dir!"),
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
         except CancelledError:
             ctx.exit()
     elif not Path(output_dir).is_dir():
         click.secho(_("Output dir is not a directory!"), fg="yellow")
         try:
             output_dir = await InputPrompt(
-                _("Output Dir:"), validator=lambda x: len(x) > 0 and Path(x).is_dir()
+                _("Output Dir:"),
+                validator=lambda x: len(x) > 0 and Path(x).is_dir(),
+                error_message=_("Invalid output dir!"),
             ).prompt_async(style=CLI_DEFAULT_STYLE)
         except CancelledError:
             ctx.exit()
 
     create_plugin(name, output_dir, sub_plugin=sub_plugin, template=template)
```

### Comparing `nb-cli-1.0.5/nb_cli/cli/commands/project.py` & `nb-cli-1.1.0/nb_cli/cli/commands/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import sys
-import asyncio
 from pathlib import Path
+from logging import Logger
 from functools import partial
 from dataclasses import field, dataclass
 from typing import Any, Dict, List, Optional
 
 import click
 from noneprompt import (
     Choice,
@@ -13,34 +13,33 @@
     InputPrompt,
     ConfirmPrompt,
     CancelledError,
     CheckboxPrompt,
 )
 
 from nb_cli import _
+from nb_cli.log import ClickHandler
 from nb_cli.config import ConfigManager
+from nb_cli.consts import DEFAULT_DRIVER
 from nb_cli.exceptions import ModuleLoadFailed
-from nb_cli.consts import WINDOWS, DEFAULT_DRIVER
 from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedCommand, run_async
 from nb_cli.handlers import (
     Reloader,
     FileFilter,
     run_project,
     list_drivers,
     list_adapters,
     create_project,
     call_pip_install,
+    get_project_root,
     create_virtualenv,
-    detect_virtualenv,
     terminate_process,
     generate_run_script,
     list_builtin_plugins,
-    remove_signal_handler,
     list_project_templates,
-    register_signal_handler,
 )
 
 VALID_PROJECT_NAME = r"^[a-zA-Z][a-zA-Z0-9 _-]*$"
 BLACKLISTED_PROJECT_NAME = {"nonebot", "bot"}
 TEMPLATE_DESCRIPTION = {
     "bootstrap": _("bootstrap (for beginner or user)"),
     "simple": _("simple (for plugin developer)"),
@@ -48,14 +47,21 @@
 
 if sys.version_info >= (3, 10):
     BLACKLISTED_PROJECT_NAME.update(sys.stdlib_module_names)
 
 
 @dataclass
 class ProjectContext:
+    """项目模板生成上下文
+
+    参数:
+        variables: 模板渲染变量字典
+        packages: 项目需要安装的包
+    """
+
     variables: Dict[str, Any] = field(default_factory=dict)
     packages: List[str] = field(default_factory=list)
 
 
 def project_name_validator(name: str) -> bool:
     return (
         bool(re.match(VALID_PROJECT_NAME, name))
@@ -67,27 +73,30 @@
     click.secho(_("Loading adapters..."))
     all_adapters = await list_adapters()
     click.secho(_("Loading drivers..."))
     all_drivers = await list_drivers()
     click.clear()
 
     project_name = await InputPrompt(
-        _("Project Name:"), validator=project_name_validator
+        _("Project Name:"),
+        validator=project_name_validator,
+        error_message=_("Invalid project name!"),
     ).prompt_async(style=CLI_DEFAULT_STYLE)
     context.variables["project_name"] = project_name
 
     drivers = await CheckboxPrompt(
         _("Which driver(s) would you like to use?"),
         [Choice(f"{driver.name} ({driver.desc})", driver) for driver in all_drivers],
         default_select=[
             index
             for index, driver in enumerate(all_drivers)
             if driver.name in DEFAULT_DRIVER
         ],
         validator=bool,
+        error_message=_("Chosen drivers is not valid!"),
     ).prompt_async(style=CLI_DEFAULT_STYLE)
     context.variables["drivers"] = [d.data.dict() for d in drivers]
     context.packages.extend(
         [d.data.project_link for d in drivers if d.data.project_link]
     )
 
     confirm = False
@@ -207,52 +216,51 @@
         try:
             use_venv = await ConfirmPrompt(
                 _("Create virtual environment?"), default_choice=True
             ).prompt_async(style=CLI_DEFAULT_STYLE)
         except CancelledError:
             ctx.exit()
 
-        path = None
         if use_venv:
             click.secho(
                 _("Creating virtual environment in {venv_dir} ...").format(
                     venv_dir=venv_dir
                 ),
                 fg="yellow",
             )
             await create_virtualenv(
                 venv_dir, prompt=project_dir_name, python_path=python_interpreter
             )
-            path = (
-                venv_dir
-                / ("Scripts" if WINDOWS else "bin")
-                / ("python.exe" if WINDOWS else "python")
-            )
+
+        config_manager = ConfigManager(working_dir=project_dir, use_venv=use_venv)
 
         proc = await call_pip_install(
-            ["nonebot2", *context.packages], pip_args, python_path=path
+            ["nonebot2", *context.packages],
+            pip_args,
+            python_path=config_manager.python_path,
         )
         await proc.wait()
 
-        builtin_plugins = await list_builtin_plugins(python_path=path)
+        builtin_plugins = await list_builtin_plugins(
+            python_path=config_manager.python_path
+        )
         try:
             loaded_builtin_plugins = [
                 c.data
                 for c in await CheckboxPrompt(
                     _("Which builtin plugin(s) would you like to use?"),
                     [Choice(p, p) for p in builtin_plugins],
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
             ]
         except CancelledError:
             ctx.exit()
 
         try:
-            m = ConfigManager(python=path, config_file=project_dir / "pyproject.toml")
             for plugin in loaded_builtin_plugins:
-                m.add_builtin_plugin(plugin)
+                config_manager.add_builtin_plugin(plugin)
         except Exception as e:
             click.secho(
                 _(
                     "Failed to add builtin plugins {builtin_plugins} to config: {e}"
                 ).format(builtin_plugin=loaded_builtin_plugins, e=e),
                 fg="red",
             )
@@ -278,35 +286,28 @@
     default="bot.py",
     show_default=True,
     help=_("The file script saved to."),
 )
 @run_async
 async def generate(file: str):
     content = await generate_run_script()
-    Path(file).write_text(content)
+    Path(file).write_text(content, encoding="utf-8")
 
 
 @click.command(
     cls=ClickAliasedCommand, aliases=["start"], help=_("Run the bot in current folder.")
 )
-@click.option("-d", "--cwd", default=".", help=_("The working directory."))
 @click.option(
     "-f",
     "--file",
     default="bot.py",
     show_default=True,
     help=_("Exist entry file of your bot."),
 )
 @click.option(
-    "--venv/--no-venv",
-    default=True,
-    help=_("Auto detect virtual environment."),
-    show_default=True,
-)
-@click.option(
     "-r",
     "--reload",
     is_flag=True,
     default=False,
     help=_("Reload the bot when file changed."),
 )
 @click.option(
@@ -319,34 +320,25 @@
     "--reload-excludes",
     multiple=True,
     default=None,
     help=_("Files to ignore for changes."),
 )
 @run_async
 async def run(
-    cwd: str,
     file: str,
-    venv: bool,
     reload: bool,
     reload_includes: Optional[List[str]],
     reload_excludes: Optional[List[str]],
 ):
-    if python_path := detect_virtualenv(Path(cwd)) if venv else None:
-        click.secho(
-            _("Using virtual environment: {python_path}").format(
-                python_path=python_path
-            ),
-            fg="green",
-        )
-
     if reload:
+        logger = Logger(__name__)
+        logger.addHandler(ClickHandler())
         await Reloader(
-            partial(run_project, exist_bot=Path(file), python_path=python_path),
+            partial(run_project, exist_bot=Path(file)),
             terminate_process,
             file_filter=FileFilter(reload_includes, reload_excludes),
-            cwd=Path(cwd),
+            cwd=get_project_root(),
+            logger=logger,
         ).run()
     else:
-        proc = await run_project(
-            exist_bot=Path(file), python_path=python_path, cwd=Path(cwd)
-        )
+        proc = await run_project(exist_bot=Path(file))
         await proc.wait()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nb-cli-1.0.5/nb_cli/cli/commands/self.py` & `nb-cli-1.1.0/nb_cli/cli/commands/self.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/cli/customize.py` & `nb-cli-1.1.0/nb_cli/cli/customize.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from pathlib import Path
 from functools import partial
 from collections import Counter
 from typing import Dict, List, Optional
 
 import click
 
 from nb_cli import _, cache
-from nb_cli.handlers import run_script, list_scripts, detect_virtualenv
+from nb_cli.handlers import run_script, list_scripts
 
 from .utils import run_async
 
 
 class ClickAliasedCommand(click.Command):
     def __init__(self, *args, **kwargs) -> None:
         aliases = kwargs.pop("aliases", None)
@@ -93,45 +92,20 @@
 
 class CLIMainGroup(ClickAliasedGroup):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @staticmethod
     @run_async
-    async def _run_script_command(
-        script_name: str, cwd: Path, venv: bool, script_args: List[str]
-    ):
-        if python_path := detect_virtualenv(cwd) if venv else None:
-            click.secho(
-                _("Using virtual environment: {python_path}").format(
-                    python_path=python_path
-                ),
-                fg="green",
-            )
-        proc = await run_script(
-            script_name, script_args, cwd=cwd, python_path=python_path
-        )
+    async def _run_script_command(script_name: str, script_args: List[str]):
+        proc = await run_script(script_name, script_args)
         await proc.wait()
 
     def _build_script_command(self, script_name: str) -> click.Command:
-        params = [
-            click.Option(
-                ["-d", "--cwd"],
-                default=".",
-                help=_("The working directory."),
-                type=Path,
-            ),
-            click.Option(
-                ["--venv/--no-venv"],
-                default=True,
-                help=_("Auto detect virtual environment."),
-                show_default=True,
-            ),
-            click.Argument(["script_args"], nargs=-1),
-        ]
+        params = [click.Argument(["script_args"], nargs=-1)]
         return click.command(
             name=script_name,
             params=params,
             help=_("Run script {script_name!r}").format(script_name=script_name),
             add_help_option=False,
             context_settings={"ignore_unknown_options": True},
         )(
```

### Comparing `nb-cli-1.0.5/nb_cli/cli/utils.py` & `nb-cli-1.1.0/nb_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/config/model.py` & `nb-cli-1.1.0/nb_cli/config/model.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/handlers/__init__.py` & `nb-cli-1.1.0/nb_cli/handlers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,33 @@
 templates.filters["repr"] = repr
 
 # meta
 from .meta import draw_logo as draw_logo
 from .meta import requires_pip as requires_pip
 from .meta import get_pip_version as get_pip_version
 from .meta import requires_python as requires_python
-from .meta import load_module_data as load_module_data
+from .meta import get_project_root as get_project_root
 from .meta import requires_nonebot as requires_nonebot
-from .meta import terminate_process as terminate_process
 from .meta import get_default_python as get_default_python
-from .meta import get_nonebot_config as get_nonebot_config
 from .meta import get_python_version as get_python_version
 from .meta import get_nonebot_version as get_nonebot_version
-from .meta import format_package_results as format_package_results
-from .meta import ensure_process_terminated as ensure_process_terminated
+
+# isort: split
+
+# package
+from .store import load_module_data as load_module_data
+from .store import format_package_results as format_package_results
+
+# isort: split
+
+# process
+from .process import create_process as create_process
+from .process import terminate_process as terminate_process
+from .process import create_process_shell as create_process_shell
+from .process import ensure_process_terminated as ensure_process_terminated
 
 # isort: split
 
 # pip
 from .pip import call_pip as call_pip
 from .pip import call_pip_list as call_pip_list
 from .pip import call_pip_update as call_pip_update
@@ -43,14 +53,15 @@
 # virtualenv
 from .venv import create_virtualenv as create_virtualenv
 from .venv import detect_virtualenv as detect_virtualenv
 
 # isort: split
 
 # signal
+from .signal import shield_signals as shield_signals
 from .signal import remove_signal_handler as remove_signal_handler
 from .signal import install_signal_handler as install_signal_handler
 from .signal import register_signal_handler as register_signal_handler
 
 # isort: split
 
 # plugin
```

### Comparing `nb-cli-1.0.5/nb_cli/handlers/adapter.py` & `nb-cli-1.1.0/nb_cli/handlers/adapter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import List, Optional
 
 from cookiecutter.main import cookiecutter
 
 from nb_cli.config import Adapter
 
-from .meta import load_module_data
+from .store import load_module_data
 
 TEMPLATE_ROOT = Path(__file__).parent.parent / "template" / "adapter"
 
 
 def create_adapter(
     adapter_name: str,
     output_dir: str = ".",
```

### Comparing `nb-cli-1.0.5/nb_cli/handlers/pip.py` & `nb-cli-1.1.0/nb_cli/handlers/pip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import asyncio
 from typing import IO, Any, List, Union, Optional
 
-from .meta import requires_pip, get_default_python, ensure_process_terminated
+from .process import create_process
+from .meta import requires_pip, get_default_python
 
 
 @requires_pip
-@ensure_process_terminated
 async def call_pip(
     pip_args: Optional[List[str]] = None,
     *,
     python_path: Optional[str] = None,
     stdin: Optional[Union[IO[Any], int]] = None,
     stdout: Optional[Union[IO[Any], int]] = None,
     stderr: Optional[Union[IO[Any], int]] = None,
 ) -> asyncio.subprocess.Process:
     if pip_args is None:
         pip_args = []
     if python_path is None:
         python_path = await get_default_python()
 
-    return await asyncio.create_subprocess_exec(
+    return await create_process(
         python_path,
         "-m",
         "pip",
         *pip_args,
         stdin=stdin,
         stdout=stdout,
         stderr=stderr,
@@ -99,15 +99,14 @@
         stdin=stdin,
         stdout=stdout,
         stderr=stderr,
     )
 
 
 @requires_pip
-@ensure_process_terminated
 async def call_pip_list(
     pip_args: Optional[List[str]] = None,
     *,
     python_path: Optional[str] = None,
     stdin: Optional[Union[IO[Any], int]] = None,
     stdout: Optional[Union[IO[Any], int]] = None,
     stderr: Optional[Union[IO[Any], int]] = None,
```

### Comparing `nb-cli-1.0.5/nb_cli/handlers/plugin.py` & `nb-cli-1.1.0/nb_cli/handlers/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 from typing import List, Optional
 
 from cookiecutter.main import cookiecutter
 
 from nb_cli.config import Plugin
 
 from . import templates
-from .meta import load_module_data, requires_nonebot, get_default_python
+from .process import create_process
+from .store import load_module_data
+from .meta import requires_nonebot, get_default_python
 
 TEMPLATE_ROOT = Path(__file__).parent.parent / "template" / "plugin"
 
 
 @requires_nonebot
 async def list_builtin_plugins(*, python_path: Optional[str] = None) -> List[str]:
     if python_path is None:
         python_path = await get_default_python()
 
     t = templates.get_template("plugin/list_builtin_plugin.py.jinja")
 
-    proc = await asyncio.create_subprocess_exec(
+    proc = await create_process(
         python_path,
         "-W",
         "ignore",
         "-c",
         await t.render_async(),
         stdout=asyncio.subprocess.PIPE,
     )
```

### Comparing `nb-cli-1.0.5/nb_cli/handlers/project.py` & `nb-cli-1.1.0/nb_cli/handlers/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import sys
 import asyncio
 from pathlib import Path
 from typing import IO, Any, Dict, List, Union, Optional
 
 from cookiecutter.main import cookiecutter
 
 from nb_cli.config import SimpleInfo
 
 from . import templates
+from .process import create_process
 from .meta import (
+    get_project_root,
     requires_nonebot,
     get_default_python,
     get_nonebot_config,
-    ensure_process_terminated,
 )
 
 TEMPLATE_ROOT = Path(__file__).parent.parent / "template" / "project"
 
 
 def list_project_templates() -> List[str]:
     return sorted(t.name for t in (TEMPLATE_ROOT).iterdir())
@@ -50,15 +50,14 @@
         builtin_plugins = bot_config.builtin_plugins
 
     t = templates.get_template("project/run_project.py.jinja")
     return await t.render_async(adapters=adapters, builtin_plugins=builtin_plugins)
 
 
 @requires_nonebot
-@ensure_process_terminated
 async def run_project(
     adapters: Optional[List[SimpleInfo]] = None,
     builtin_plugins: Optional[List[str]] = None,
     exist_bot: Path = Path("bot.py"),
     *,
     python_path: Optional[str] = None,
     cwd: Optional[Path] = None,
@@ -69,26 +68,28 @@
     bot_config = get_nonebot_config()
     if adapters is None:
         adapters = bot_config.adapters
     if builtin_plugins is None:
         builtin_plugins = bot_config.builtin_plugins
     if python_path is None:
         python_path = await get_default_python()
+    if cwd is None:
+        cwd = get_project_root()
 
-    if exist_bot.exists():
-        return await asyncio.create_subprocess_exec(
+    if cwd.joinpath(exist_bot).exists():
+        return await create_process(
             python_path,
             exist_bot,
             cwd=cwd,
             stdin=stdin,
             stdout=stdout,
             stderr=stderr,
         )
 
-    return await asyncio.create_subprocess_exec(
+    return await create_process(
         python_path,
         "-c",
         await generate_run_script(adapters=adapters, builtin_plugins=builtin_plugins),
         cwd=cwd,
         stdin=stdin,
         stdout=stdout,
         stderr=stderr,
```

### Comparing `nb-cli-1.0.5/nb_cli/handlers/script.py` & `nb-cli-1.1.0/nb_cli/handlers/script.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 import asyncio
 from pathlib import Path
 from typing import IO, Any, List, Union, Optional
 
 from nb_cli.config import SimpleInfo
 
 from . import templates
+from .process import create_process
 from .meta import (
     requires_python,
+    get_project_root,
     requires_nonebot,
     get_default_python,
     get_nonebot_config,
-    ensure_process_terminated,
 )
 
 
 @requires_python
 async def list_scripts(*, python_path: Optional[str] = None) -> List[str]:
     if python_path is None:
         python_path = await get_default_python()
 
     t = templates.get_template("script/list_scripts.py.jinja")
-    proc = await asyncio.create_subprocess_exec(
+    proc = await create_process(
         python_path,
         "-W",
         "ignore",
         "-c",
         await t.render_async(),
         stdout=asyncio.subprocess.PIPE,
     )
     stdout, _ = await proc.communicate()
     return json.loads(stdout.strip())
 
 
 @requires_nonebot
-@ensure_process_terminated
 async def run_script(
     script_name: str,
     script_args: Optional[List[str]] = None,
     adapters: Optional[List[SimpleInfo]] = None,
     builtin_plugins: Optional[List[str]] = None,
     *,
     python_path: Optional[str] = None,
@@ -53,18 +53,20 @@
     bot_config = get_nonebot_config()
     if adapters is None:
         adapters = bot_config.adapters
     if builtin_plugins is None:
         builtin_plugins = bot_config.builtin_plugins
     if python_path is None:
         python_path = await get_default_python()
+    if cwd is None:
+        cwd = get_project_root()
 
     t = templates.get_template("script/run_script.py.jinja")
 
-    return await asyncio.create_subprocess_exec(
+    return await create_process(
         python_path,
         "-c",
         await t.render_async(
             adapters=adapters,
             builtin_plugins=builtin_plugins,
             script_name=script_name,
         ),
```

### Comparing `nb-cli-1.0.5/nb_cli/handlers/venv.py` & `nb-cli-1.1.0/nb_cli/handlers/venv.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from pathlib import Path
 from typing import Optional
 
 import virtualenv
 
-from nb_cli.consts import WINDOWS
+from nb_cli.config import ConfigManager
 
 from .meta import requires_python, get_default_python
 
 
 def detect_virtualenv(cwd: Optional[Path] = None) -> Optional[str]:
-    cwd = (cwd or Path.cwd()).resolve()
-    for venv_dir in cwd.iterdir():
-        if venv_dir.is_dir() and (venv_dir / "pyvenv.cfg").is_file():
-            return str(
-                venv_dir
-                / ("Scripts" if WINDOWS else "bin")
-                / ("python.exe" if WINDOWS else "python")
-            )
+    return ConfigManager._detact_virtual_env(cwd)
 
 
 @requires_python
 async def create_virtualenv(
     venv_dir: Path,
     prompt: Optional[str] = None,
     *,
```

### Comparing `nb-cli-1.0.5/nb_cli/i18n.py` & `nb-cli-1.1.0/nb_cli/i18n.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo` & `nb-cli-1.1.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: nb-cli 1.0.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-06 07:36+0000\n"
+"POT-Creation-Date: 2023-04-12 05:58+0000\n"
 "PO-Revision-Date: 2023-01-11 08:56+0000\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "1) In a \"{dir_name}\" folder"
 msgstr "1) 在 \"{dir_name}\" 文件夹中"
 
 msgid "2) In a \"src\" folder"
 msgstr "2) 在 \"src\" 文件夹中"
 
@@ -41,19 +41,19 @@
 
 msgid "Auto detect virtual environment."
 msgstr "自动检测虚拟环境."
 
 msgid "Cannot find a valid Python interpreter."
 msgstr "无法找到可用的 Python 解释器."
 
-msgid "Config file encoding."
-msgstr "配置文件编码."
+msgid "Cannot find project root directory! {config_file} file not exists."
+msgstr "无法找到项目根目录! {config_file} 文件不存在."
 
-msgid "Config file path."
-msgstr "配置文件路径."
+msgid "Chosen drivers is not valid!"
+msgstr "选择的驱动器不合法!"
 
 msgid "Create a NoneBot project."
 msgstr "创建一个 NoneBot 项目."
 
 msgid "Create a new nonebot adapter."
 msgstr "新建适配器"
 
@@ -125,14 +125,20 @@
 
 msgid "Install package to cli venv."
 msgstr "在 cli 虚拟环境中安装包."
 
 msgid "Invalid module type: {module_type}"
 msgstr "无效的模块类型: {module_type}"
 
+msgid "Invalid output dir!"
+msgstr "无效的输出目录!"
+
+msgid "Invalid project name!"
+msgstr "无效的项目名称!"
+
 msgid "List installed packages in cli venv."
 msgstr "列出 cli 虚拟环境中已安装的包."
 
 msgid "List nonebot adapters published on nonebot homepage."
 msgstr "列出 NoneBot 官网上发布的适配器."
 
 msgid "List nonebot drivers published on nonebot homepage."
@@ -203,14 +209,17 @@
 
 msgid "Python {major}.{minor} is not supported."
 msgstr "Python {major}.{minor} 不受支持."
 
 msgid "Reload the bot when file changed."
 msgstr "当文件发生变化时重新加载机器人."
 
+msgid "Restarted process [{pid}]."
+msgstr "重启进程 [{pid}]."
+
 msgid "Run script {script_name!r}"
 msgstr "运行脚本 {script_name!r}"
 
 msgid "Run subcommand {sub_cmd.name!r}"
 msgstr "运行子命令 {sub_cmd.name!r}"
 
 msgid "Run the bot in current folder."
@@ -227,14 +236,23 @@
 
 msgid "Search for nonebot plugins published on nonebot homepage."
 msgstr "搜索 NoneBot 官网上发布的插件."
 
 msgid "Select a template to use:"
 msgstr "选择一个要使用的模板:"
 
+msgid "Shutting down process [{pid}]..."
+msgstr "正在终止进程 [{pid}]..."
+
+msgid "Started reloader with process [{pid}]."
+msgstr "启动重载监视，当前进程 [{pid}]."
+
+msgid "Stopped reloader."
+msgstr "停止重载监视"
+
 msgid "The adapter template to use."
 msgstr "使用的适配器模板."
 
 msgid "The file script saved to."
 msgstr "脚本文件保存路径."
 
 msgid "The plugin template to use."
@@ -272,16 +290,19 @@
 
 msgid "Update nonebot plugin."
 msgstr "更新插件."
 
 msgid "Use nested plugin?"
 msgstr "使用嵌套插件?"
 
-msgid "Using virtual environment: {python_path}"
-msgstr "使用虚拟环境: {python_path}"
+msgid "Using python: {python_path}"
+msgstr "使用 Python: {python_path}"
+
+msgid "Watchfiles detected changes in {paths}. Reloading..."
+msgstr "Watchfiles 在 {paths} 中发现变化. 正在重新加载..."
 
 msgid "Welcome to NoneBot CLI!"
 msgstr "欢迎使用 NoneBot CLI!"
 
 msgid "What do you want to do?"
 msgstr "你想要进行什么操作?"
```

### Comparing `nb-cli-1.0.5/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po` & `nb-cli-1.1.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po`

 * *Files 10% similar despite different names*

```diff
@@ -3,384 +3,375 @@
 # This file is distributed under the same license as the nb-cli project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: nb-cli 1.0.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-06 07:36+0000\n"
+"POT-Creation-Date: 2023-04-12 05:58+0000\n"
 "PO-Revision-Date: 2023-01-11 08:56+0000\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
-#: nb_cli/cli/__init__.py:47
-msgid "Config file path."
-msgstr "配置文件路径."
-
-#: nb_cli/cli/__init__.py:57
-msgid "Config file encoding."
-msgstr "配置文件编码."
+#: nb_cli/cli/__init__.py:51
+msgid "The working directory."
+msgstr "工作目录."
 
-#: nb_cli/cli/__init__.py:66
+#: nb_cli/cli/__init__.py:61
 msgid "Python executable path."
 msgstr "Python 可执行文件路径."
 
-#: nb_cli/cli/__init__.py:89 nb_cli/cli/commands/adapter.py:39
-#: nb_cli/cli/commands/driver.py:36 nb_cli/cli/commands/plugin.py:39
+#: nb_cli/cli/__init__.py:69
+msgid "Auto detect virtual environment."
+msgstr "自动检测虚拟环境."
+
+#: nb_cli/cli/__init__.py:92 nb_cli/cli/commands/adapter.py:38
+#: nb_cli/cli/commands/driver.py:35 nb_cli/cli/commands/plugin.py:38
 #: nb_cli/cli/commands/self.py:34
 msgid "Run subcommand {sub_cmd.name!r}"
 msgstr "运行子命令 {sub_cmd.name!r}"
 
-#: nb_cli/cli/__init__.py:96
+#: nb_cli/cli/__init__.py:99
 msgid "Welcome to NoneBot CLI!"
 msgstr "欢迎使用 NoneBot CLI!"
 
-#: nb_cli/cli/__init__.py:101 nb_cli/cli/commands/adapter.py:46
-#: nb_cli/cli/commands/driver.py:43 nb_cli/cli/commands/plugin.py:46
+#: nb_cli/cli/__init__.py:104 nb_cli/cli/commands/adapter.py:45
+#: nb_cli/cli/commands/driver.py:42 nb_cli/cli/commands/plugin.py:45
 #: nb_cli/cli/commands/self.py:41
 msgid "What do you want to do?"
 msgstr "你想要进行什么操作?"
 
-#: nb_cli/cli/commands/adapter.py:112 nb_cli/cli/commands/adapter.py:150
-#: nb_cli/cli/commands/adapter.py:199 nb_cli/cli/commands/driver.py:101
-#: nb_cli/cli/commands/driver.py:140 nb_cli/cli/commands/driver.py:184
-#: nb_cli/cli/commands/plugin.py:112 nb_cli/cli/commands/plugin.py:150
-#: nb_cli/cli/commands/plugin.py:197 nb_cli/cli/commands/project.py:335
-#: nb_cli/cli/customize.py:105
-msgid "Using virtual environment: {python_path}"
-msgstr "使用虚拟环境: {python_path}"
-
-#: nb_cli/cli/commands/project.py:291 nb_cli/cli/customize.py:120
-msgid "The working directory."
-msgstr "工作目录."
-
-#: nb_cli/cli/commands/adapter.py:82 nb_cli/cli/commands/adapter.py:129
-#: nb_cli/cli/commands/adapter.py:169 nb_cli/cli/commands/driver.py:79
-#: nb_cli/cli/commands/driver.py:118 nb_cli/cli/commands/driver.py:159
-#: nb_cli/cli/commands/plugin.py:82 nb_cli/cli/commands/plugin.py:129
-#: nb_cli/cli/commands/plugin.py:167 nb_cli/cli/commands/project.py:302
-#: nb_cli/cli/customize.py:126
-msgid "Auto detect virtual environment."
-msgstr "自动检测虚拟环境."
-
-#: nb_cli/cli/customize.py:134
+#: nb_cli/cli/customize.py:108
 msgid "Run script {script_name!r}"
 msgstr "运行脚本 {script_name!r}"
 
 #: nb_cli/cli/utils.py:53
 msgid "Package {name} not found."
 msgstr "包 {name} 未找到."
 
-#: nb_cli/cli/commands/adapter.py:23
+#: nb_cli/cli/commands/adapter.py:22
 msgid "Manage bot adapters."
 msgstr "管理 bot 适配器."
 
-#: nb_cli/cli/commands/adapter.py:55
+#: nb_cli/cli/commands/adapter.py:54
 msgid "List nonebot adapters published on nonebot homepage."
 msgstr "列出 NoneBot 官网上发布的适配器."
 
-#: nb_cli/cli/commands/adapter.py:62
+#: nb_cli/cli/commands/adapter.py:61
 msgid "Search for nonebot adapters published on nonebot homepage."
 msgstr "搜索 NoneBot 官网上发布的适配器."
 
-#: nb_cli/cli/commands/adapter.py:67
+#: nb_cli/cli/commands/adapter.py:66
 msgid "Adapter name to search:"
 msgstr "想要搜索的适配器名称:"
 
-#: nb_cli/cli/commands/adapter.py:77
+#: nb_cli/cli/commands/adapter.py:76
 msgid "Install nonebot adapter to current project."
 msgstr "安装适配器到当前项目."
 
-#: nb_cli/cli/commands/adapter.py:94
+#: nb_cli/cli/commands/adapter.py:87
 msgid "Adapter name to install:"
 msgstr "想要安装的适配器名称:"
 
-#: nb_cli/cli/commands/adapter.py:105
+#: nb_cli/cli/commands/adapter.py:98
 msgid "Failed to add adapter {adapter.name} to config: {e}"
 msgstr "添加适配器 {adapter.name} 到配置文件失败: {e}"
 
-#: nb_cli/cli/commands/adapter.py:124
+#: nb_cli/cli/commands/adapter.py:108
 msgid "Update nonebot adapter."
 msgstr "更新适配器."
 
-#: nb_cli/cli/commands/adapter.py:141
+#: nb_cli/cli/commands/adapter.py:119
 msgid "Adapter name to update:"
 msgstr "想要更新的适配器名称:"
 
-#: nb_cli/cli/commands/adapter.py:164
+#: nb_cli/cli/commands/adapter.py:133
 msgid "Uninstall nonebot adapter from current project."
 msgstr "移除当前项目中的适配器."
 
-#: nb_cli/cli/commands/adapter.py:181
+#: nb_cli/cli/commands/adapter.py:144
 msgid "Adapter name to uninstall:"
 msgstr "想要移除的适配器名称:"
 
-#: nb_cli/cli/commands/adapter.py:192
+#: nb_cli/cli/commands/adapter.py:155
 msgid "Failed to remove adapter {adapter.name} from config: {e}"
 msgstr "从配置文件移除适配器 {adapter.name} 失败: {e}"
 
-#: nb_cli/cli/commands/adapter.py:210
+#: nb_cli/cli/commands/adapter.py:164
 msgid "Create a new nonebot adapter."
 msgstr "新建适配器"
 
-#: nb_cli/cli/commands/adapter.py:218
+#: nb_cli/cli/commands/adapter.py:172
 msgid "The adapter template to use."
 msgstr "使用的适配器模板."
 
-#: nb_cli/cli/commands/adapter.py:229
+#: nb_cli/cli/commands/adapter.py:183
 msgid "Adapter name:"
 msgstr "适配器名称:"
 
-#: nb_cli/cli/commands/adapter.py:245
+#: nb_cli/cli/commands/adapter.py:204
 msgid "Where to store the adapter?"
 msgstr "请输入适配器存储的位置:"
 
-#: nb_cli/cli/commands/adapter.py:245 nb_cli/cli/commands/adapter.py:248
-#: nb_cli/cli/commands/plugin.py:249 nb_cli/cli/commands/plugin.py:252
+#: nb_cli/cli/commands/adapter.py:204 nb_cli/cli/commands/adapter.py:207
+#: nb_cli/cli/commands/plugin.py:210 nb_cli/cli/commands/plugin.py:213
 msgid "Other"
 msgstr "其他"
 
-#: nb_cli/cli/commands/adapter.py:250 nb_cli/cli/commands/adapter.py:259
-#: nb_cli/cli/commands/plugin.py:254 nb_cli/cli/commands/plugin.py:263
+#: nb_cli/cli/commands/adapter.py:209 nb_cli/cli/commands/adapter.py:218
+#: nb_cli/cli/commands/plugin.py:215 nb_cli/cli/commands/plugin.py:225
 msgid "Output Dir:"
 msgstr "输出目录:"
 
-#: nb_cli/cli/commands/adapter.py:256 nb_cli/cli/commands/plugin.py:260
+#: nb_cli/cli/commands/adapter.py:215 nb_cli/cli/commands/plugin.py:222
 msgid "Output dir is not a directory!"
 msgstr "输出目录不是一个文件夹!"
 
-#: nb_cli/cli/commands/driver.py:20
+#: nb_cli/cli/commands/adapter.py:220 nb_cli/cli/commands/plugin.py:217
+#: nb_cli/cli/commands/plugin.py:227
+msgid "Invalid output dir!"
+msgstr "无效的输出目录!"
+
+#: nb_cli/cli/commands/driver.py:19
 msgid "Manage bot driver."
 msgstr "管理 bot 驱动器."
 
-#: nb_cli/cli/commands/driver.py:52
+#: nb_cli/cli/commands/driver.py:51
 msgid "List nonebot drivers published on nonebot homepage."
 msgstr "列出 NoneBot 官网上发布的驱动器."
 
-#: nb_cli/cli/commands/driver.py:59
+#: nb_cli/cli/commands/driver.py:58
 msgid "Search for nonebot drivers published on nonebot homepage."
 msgstr "搜索 NoneBot 官网上发布的驱动器."
 
-#: nb_cli/cli/commands/driver.py:64
+#: nb_cli/cli/commands/driver.py:63
 msgid "Driver name to search:"
 msgstr "想要搜索的驱动器名称:"
 
-#: nb_cli/cli/commands/driver.py:74
+#: nb_cli/cli/commands/driver.py:73
 msgid "Install nonebot driver to current project."
 msgstr "安装驱动器到当前项目."
 
-#: nb_cli/cli/commands/driver.py:91
+#: nb_cli/cli/commands/driver.py:84
 msgid "Driver name to install:"
 msgstr "想要安装的驱动器名称:"
 
-#: nb_cli/cli/commands/driver.py:113
+#: nb_cli/cli/commands/driver.py:97
 msgid "Update nonebot driver."
 msgstr "更新驱动器."
 
-#: nb_cli/cli/commands/driver.py:130
+#: nb_cli/cli/commands/driver.py:108
 msgid "Driver name to update:"
 msgstr "想要更新的驱动器名称:"
 
-#: nb_cli/cli/commands/driver.py:154
+#: nb_cli/cli/commands/driver.py:123
 msgid "Uninstall nonebot driver from current project."
 msgstr "移除当前项目中的驱动器."
 
-#: nb_cli/cli/commands/driver.py:171
+#: nb_cli/cli/commands/driver.py:134
 msgid "Driver name to uninstall:"
 msgstr "想要移除的驱动器名称:"
 
-#: nb_cli/cli/commands/plugin.py:23
+#: nb_cli/cli/commands/plugin.py:22
 msgid "Manage bot plugins."
 msgstr "管理 bot 插件."
 
-#: nb_cli/cli/commands/plugin.py:55
+#: nb_cli/cli/commands/plugin.py:54
 msgid "List nonebot plugins published on nonebot homepage."
 msgstr "列出 NoneBot 官网上发布的插件."
 
-#: nb_cli/cli/commands/plugin.py:62
+#: nb_cli/cli/commands/plugin.py:61
 msgid "Search for nonebot plugins published on nonebot homepage."
 msgstr "搜索 NoneBot 官网上发布的插件."
 
-#: nb_cli/cli/commands/plugin.py:67
+#: nb_cli/cli/commands/plugin.py:66
 msgid "Plugin name to search:"
 msgstr "想要搜索的插件名称:"
 
-#: nb_cli/cli/commands/plugin.py:77
+#: nb_cli/cli/commands/plugin.py:76
 msgid "Install nonebot plugin to current project."
 msgstr "安装插件到当前项目."
 
-#: nb_cli/cli/commands/plugin.py:94
+#: nb_cli/cli/commands/plugin.py:87
 msgid "Plugin name to install:"
 msgstr "想要安装的插件名称:"
 
-#: nb_cli/cli/commands/plugin.py:105
+#: nb_cli/cli/commands/plugin.py:98
 msgid "Failed to add plugin {plugin.name} to config: {e}"
 msgstr "添加插件 {plugin.name} 到配置文件失败: {e}"
 
-#: nb_cli/cli/commands/plugin.py:124
+#: nb_cli/cli/commands/plugin.py:108
 msgid "Update nonebot plugin."
 msgstr "更新插件."
 
-#: nb_cli/cli/commands/plugin.py:141
+#: nb_cli/cli/commands/plugin.py:119
 msgid "Plugin name to update:"
 msgstr "想要更新的插件名称:"
 
-#: nb_cli/cli/commands/plugin.py:162
+#: nb_cli/cli/commands/plugin.py:133
 msgid "Uninstall nonebot plugin from current project."
 msgstr "移除当前项目中的插件."
 
-#: nb_cli/cli/commands/plugin.py:179
+#: nb_cli/cli/commands/plugin.py:144
 msgid "Plugin name to uninstall:"
 msgstr "想要移除的插件名称:"
 
-#: nb_cli/cli/commands/plugin.py:190
+#: nb_cli/cli/commands/plugin.py:155
 msgid "Failed to remove plugin {plugin.name} from config: {e}"
 msgstr "从配置文件中移除插件 {plugin.name} 失败: {e}"
 
-#: nb_cli/cli/commands/plugin.py:208
+#: nb_cli/cli/commands/plugin.py:164
 msgid "Create a new nonebot plugin."
 msgstr "创建一个新的插件."
 
-#: nb_cli/cli/commands/plugin.py:217
+#: nb_cli/cli/commands/plugin.py:173
 msgid "The plugin template to use."
 msgstr "使用的插件模板."
 
-#: nb_cli/cli/commands/plugin.py:229
+#: nb_cli/cli/commands/plugin.py:185
 msgid "Plugin name:"
 msgstr "插件名称:"
 
-#: nb_cli/cli/commands/plugin.py:237
+#: nb_cli/cli/commands/plugin.py:193
 msgid "Use nested plugin?"
 msgstr "使用嵌套插件?"
 
-#: nb_cli/cli/commands/plugin.py:249 nb_cli/cli/commands/project.py:127
+#: nb_cli/cli/commands/plugin.py:210 nb_cli/cli/commands/project.py:136
 msgid "Where to store the plugin?"
 msgstr "请输入插件存储位置:"
 
-#: nb_cli/cli/commands/project.py:45
+#: nb_cli/cli/commands/project.py:44
 msgid "bootstrap (for beginner or user)"
 msgstr "bootstrap (初学者或用户)"
 
-#: nb_cli/cli/commands/project.py:46
+#: nb_cli/cli/commands/project.py:45
 msgid "simple (for plugin developer)"
 msgstr "simple (插件开发者)"
 
-#: nb_cli/cli/commands/project.py:67
+#: nb_cli/cli/commands/project.py:73
 msgid "Loading adapters..."
 msgstr "正在加载适配器..."
 
-#: nb_cli/cli/commands/project.py:69
+#: nb_cli/cli/commands/project.py:75
 msgid "Loading drivers..."
 msgstr "正在加载驱动器..."
 
-#: nb_cli/cli/commands/project.py:74
+#: nb_cli/cli/commands/project.py:80
 msgid "Project Name:"
 msgstr "项目名称:"
 
-#: nb_cli/cli/commands/project.py:79
+#: nb_cli/cli/commands/project.py:82
+msgid "Invalid project name!"
+msgstr "无效的项目名称!"
+
+#: nb_cli/cli/commands/project.py:87
 msgid "Which driver(s) would you like to use?"
 msgstr "要使用哪些驱动器?"
 
-#: nb_cli/cli/commands/project.py:97
+#: nb_cli/cli/commands/project.py:95
+msgid "Chosen drivers is not valid!"
+msgstr "选择的驱动器不合法!"
+
+#: nb_cli/cli/commands/project.py:106
 msgid "Which adapter(s) would you like to use?"
 msgstr "要使用哪些适配器?"
 
-#: nb_cli/cli/commands/project.py:107
+#: nb_cli/cli/commands/project.py:116
 msgid "You haven't chosen any adapter! Please confirm."
 msgstr "你没有选择任何适配器! 请确认."
 
-#: nb_cli/cli/commands/project.py:123
+#: nb_cli/cli/commands/project.py:132
 msgid "1) In a \"{dir_name}\" folder"
 msgstr "1) 在 \"{dir_name}\" 文件夹中"
 
-#: nb_cli/cli/commands/project.py:124
+#: nb_cli/cli/commands/project.py:133
 msgid "2) In a \"src\" folder"
 msgstr "2) 在 \"src\" 文件夹中"
 
-#: nb_cli/cli/commands/project.py:144
+#: nb_cli/cli/commands/project.py:153
 msgid "Create a NoneBot project."
 msgstr "创建一个 NoneBot 项目."
 
-#: nb_cli/cli/commands/project.py:152
+#: nb_cli/cli/commands/project.py:161
 msgid "The project template to use."
 msgstr "使用的项目模板."
 
-#: nb_cli/cli/commands/project.py:157
+#: nb_cli/cli/commands/project.py:166
 msgid "The python interpreter virtualenv is installed into."
 msgstr "虚拟环境使用的 Python 解释器."
 
-#: nb_cli/cli/commands/project.py:174
+#: nb_cli/cli/commands/project.py:183
 msgid "Select a template to use:"
 msgstr "选择一个要使用的模板:"
 
-#: nb_cli/cli/commands/project.py:196
+#: nb_cli/cli/commands/project.py:205
 msgid "Install dependencies now?"
 msgstr "立即安装依赖?"
 
-#: nb_cli/cli/commands/project.py:209
+#: nb_cli/cli/commands/project.py:218
 msgid "Create virtual environment?"
 msgstr "创建虚拟环境?"
 
-#: nb_cli/cli/commands/project.py:217
+#: nb_cli/cli/commands/project.py:225
 msgid "Creating virtual environment in {venv_dir} ..."
 msgstr "在 {venv_dir} 中创建虚拟环境..."
 
-#: nb_cli/cli/commands/project.py:241
+#: nb_cli/cli/commands/project.py:250
 msgid "Which builtin plugin(s) would you like to use?"
 msgstr "要使用哪些内置插件?"
 
-#: nb_cli/cli/commands/project.py:254
+#: nb_cli/cli/commands/project.py:262
 msgid "Failed to add builtin plugins {builtin_plugins} to config: {e}"
 msgstr "添加内置插件 {builtin_plugins} 到配置文件失败: {e}"
 
-#: nb_cli/cli/commands/project.py:261
+#: nb_cli/cli/commands/project.py:269
 msgid "Done!"
 msgstr "完成!"
 
-#: nb_cli/cli/commands/project.py:263
+#: nb_cli/cli/commands/project.py:271
 msgid ""
 "Add following packages to your project using dependency manager like "
 "poetry or pdm:"
 msgstr "使用 poetry 或 pdm 等依赖管理工具添加以下包:"
 
-#: nb_cli/cli/commands/project.py:269
+#: nb_cli/cli/commands/project.py:277
 msgid "Run the following command to start your bot:"
 msgstr "运行以下命令来启动你的机器人:"
 
-#: nb_cli/cli/commands/project.py:274
+#: nb_cli/cli/commands/project.py:282
 msgid "Generate entry file of your bot."
 msgstr "生成机器人的入口文件."
 
-#: nb_cli/cli/commands/project.py:280
+#: nb_cli/cli/commands/project.py:288
 msgid "The file script saved to."
 msgstr "脚本文件保存路径."
 
-#: nb_cli/cli/commands/project.py:289
+#: nb_cli/cli/commands/project.py:297
 msgid "Run the bot in current folder."
 msgstr "在当前文件夹中运行机器人."
 
-#: nb_cli/cli/commands/project.py:297
+#: nb_cli/cli/commands/project.py:304
 msgid "Exist entry file of your bot."
 msgstr "存在的机器人入口文件."
 
-#: nb_cli/cli/commands/project.py:310
+#: nb_cli/cli/commands/project.py:311
 msgid "Reload the bot when file changed."
 msgstr "当文件发生变化时重新加载机器人."
 
-#: nb_cli/cli/commands/project.py:316
+#: nb_cli/cli/commands/project.py:317
 msgid "Files to watch for changes."
 msgstr "要监视变化的文件."
 
-#: nb_cli/cli/commands/project.py:322
+#: nb_cli/cli/commands/project.py:323
 msgid "Files to ignore for changes."
 msgstr "要忽略变化的文件."
 
 #: nb_cli/cli/commands/self.py:18
 msgid "Manage NB CLI."
 msgstr "管理 NB CLI."
 
@@ -404,30 +395,58 @@
 msgid "Package name you want to uninstall?"
 msgstr "要卸载的包名?"
 
 #: nb_cli/cli/commands/self.py:110
 msgid "List installed packages in cli venv."
 msgstr "列出 cli 虚拟环境中已安装的包."
 
-#: nb_cli/handlers/meta.py:79
+#: nb_cli/config/parser.py:48
+msgid "Cannot find project root directory! {config_file} file not exists."
+msgstr "无法找到项目根目录! {config_file} 文件不存在."
+
+#: nb_cli/config/parser.py:90
+msgid "Using python: {python_path}"
+msgstr "使用 Python: {python_path}"
+
+#: nb_cli/handlers/meta.py:80
 msgid "Cannot find a valid Python interpreter."
 msgstr "无法找到可用的 Python 解释器."
 
-#: nb_cli/handlers/meta.py:119
+#: nb_cli/handlers/meta.py:129
 msgid "Python {major}.{minor} is not supported."
 msgstr "Python {major}.{minor} 不受支持."
 
-#: nb_cli/handlers/meta.py:161
+#: nb_cli/handlers/meta.py:171
 msgid "NoneBot is not installed."
 msgstr "NoneBot 未安装."
 
-#: nb_cli/handlers/meta.py:200
+#: nb_cli/handlers/meta.py:210
 msgid "pip is not installed."
 msgstr "pip 未安装."
 
-#: nb_cli/handlers/meta.py:238
+#: nb_cli/handlers/reloader.py:120
+msgid "Watchfiles detected changes in {paths}. Reloading..."
+msgstr "Watchfiles 在 {paths} 中发现变化. 正在重新加载..."
+
+#: nb_cli/handlers/reloader.py:132
+msgid "Started reloader with process [{pid}]."
+msgstr "启动重载监视，当前进程 [{pid}]."
+
+#: nb_cli/handlers/reloader.py:141
+msgid "Restarted process [{pid}]."
+msgstr "重启进程 [{pid}]."
+
+#: nb_cli/handlers/reloader.py:150
+msgid "Shutting down process [{pid}]..."
+msgstr "正在终止进程 [{pid}]..."
+
+#: nb_cli/handlers/reloader.py:155
+msgid "Stopped reloader."
+msgstr "停止重载监视"
+
+#: nb_cli/handlers/store.py:48
 msgid "Invalid module type: {module_type}"
 msgstr "无效的模块类型: {module_type}"
 
-#: nb_cli/handlers/meta.py:260
+#: nb_cli/handlers/store.py:73
 msgid "Failed to get {module_type} list."
 msgstr "获取 {module_type} 列表失败."
```

### Comparing `nb-cli-1.0.5/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}` & `nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}` & `nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}` & `nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb-cli-1.1.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore` & `nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/nb_cli/template/scripts/project/_prepare.py.jinja` & `nb-cli-1.1.0/nb_cli/template/scripts/project/_prepare.py.jinja`

 * *Files identical despite different names*

### Comparing `nb-cli-1.0.5/pyproject.toml` & `nb-cli-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nb-cli"
-version = "1.0.5"
+version = "1.1.0"
 description = "CLI for nonebot2"
 authors = [
     { name = "yanyongyu", email = "yyy@nonebot.dev" },
 ]
 readme = "README.md"
 keywords = [
     "bot",
@@ -24,23 +24,23 @@
 ]
 requires-python = ">=3.8, <4.0"
 dependencies = [
     "click ~=8.1",
     "anyio ~=3.6",
     "httpx ~=0.18",
     "jinja2 ~=3.0",
-    "cashews ~=5.0",
+    "cashews ~=6.0",
     "wcwidth ~=0.2",
     "tomlkit ~=0.10",
     "pydantic ~=1.9",
     "watchfiles ~=0.16",
     "cookiecutter ~=2.1",
     "virtualenv ~=20.17.1",
     "typing-extensions ~=4.4",
-    "noneprompt >=0.1.7, <1.0.0",
+    "noneprompt >=0.1.9, <1.0.0",
     "pyfiglet >=0.8.post1, <1.0.0",
     "importlib-metadata >=4.6; python_version < '3.10'",
 ]
 
 [project.license]
 text = "MIT"
 
@@ -55,29 +55,29 @@
 i18n = [
     "babel ~=2.11",
 ]
 dev = [
     "isort ~=5.10",
     "black >=22.3.0",
     "nonemoji ~=0.1",
-    "pre-commit ~=2.18",
+    "pre-commit ~=3.1",
     "importlib-metadata",
 ]
 docs = [
     "nb-autodoc @ git+https://github.com/nonebot/nb-autodoc.git",
 ]
 
 [tool.pdm.scripts]
 extract = "pybabel extract -o messages.pot --project nb-cli --version 1.0.0 nb_cli/"
 _init = "pybabel init -D nb-cli -i messages.pot -d nb_cli/locale/ -l {args}"
 _update = "pybabel update -D nb-cli -i messages.pot -d nb_cli/locale/"
 compile = "pybabel compile -D nb-cli -d nb_cli/locale/"
 
 [tool.pdm.scripts.autodoc]
-shell = "rm -rf ./website/docs/api/* && nb-autodoc nb_cli && cp -r ./build/nb_cli/* ./website/docs/api/"
+shell = "rm -rf ./website/docs/api/* && nb-autodoc nb_cli -s nb_cli.template && cp -r ./build/nb_cli/* ./website/docs/api/"
 
 [tool.pdm.scripts.init]
 composite = [
     "extract",
     "_init {args}",
 ]
 
@@ -89,15 +89,14 @@
 
 [tool.pdm.build]
 setup-script = "build.py"
 run-setuptools = false
 
 [tool.pyright]
 pythonPlatform = "All"
-reportPrivateImportUsage = false
 reportShadowedImports = false
 executionEnvironments = [
     { root = "./website", pythonVersion = "3.10" },
     { root = "./", pythonVersion = "3.8" },
 ]
 
 [tool.black]
@@ -113,13 +112,17 @@
 extra_standard_library = [
     "typing_extensions",
 ]
 extend_skip = [
     "nb_cli/template/",
 ]
 
+[tool.pycln]
+path = "."
+all = false
+
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
     "babel~=2.11",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `nb-cli-1.0.5/PKG-INFO` & `nb-cli-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-cli
-Version: 1.0.5
+Version: 1.1.0
 Summary: CLI for nonebot2
 License: MIT
 Keywords: bot,qq,nonebot,bot,qq,nonebot
 Author-email: yanyongyu <yyy@nonebot.dev>
 Requires-Python: >=3.8, <4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_8u4h5kql_/tmp720kdt6i_TarContainer/0/70", line 148, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_8u4h5kql_/tmp720kdt6i_TarContainer/0/70", line 148, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nb-cli Version: 1.0.5 Summary: CLI for nonebot2
+Metadata-Version: 2.1 Name: nb-cli Version: 1.1.0 Summary: CLI for nonebot2
 License: MIT Keywords: bot,qq,nonebot,bot,qq,nonebot Author-email: yanyongyu
 nonebot.dev> Requires-Python: >=3.8, <4.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: Robot Framework Classifier:
 Framework :: Robot Framework :: Library Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Project-URL: homepage, https://
 cli.nonebot.dev/ Project-URL: repository, https://github.com/nonebot/nb-cli
```

