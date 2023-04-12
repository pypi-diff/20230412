# Comparing `tmp/nb-cli-1.1.0.tar.gz` & `tmp/nb-cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-cli-1.1.0.tar", last modified: Wed Apr 12 06:06:29 2023, max compression
+gzip compressed data, was "nb-cli-1.1.1.tar", last modified: Wed Apr 12 06:27:48 2023, max compression
```

## Comparing `nb-cli-1.1.0.tar` & `nb-cli-1.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1065 2023-04-12 06:05:51.076853 nb-cli-1.1.0/LICENSE
--rw-r--r--   0        0        0     3350 2023-04-12 06:05:51.076853 nb-cli-1.1.0/README.md
--rw-r--r--   0        0        0      246 2023-04-12 06:05:51.076853 nb-cli-1.1.0/build.py
--rw-r--r--   0        0        0      795 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/__init__.py
--rw-r--r--   0        0        0      202 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/__main__.py
--rw-r--r--   0        0        0     3305 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/__init__.py
--rw-r--r--   0        0        0      257 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/__init__.py
--rw-r--r--   0        0        0     6866 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/adapter.py
--rw-r--r--   0        0        0     4243 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/driver.py
--rw-r--r--   0        0        0     7195 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/plugin.py
--rw-r--r--   0        0        0    10063 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/project.py
--rw-r--r--   0        0        0     3409 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/commands/self.py
--rw-r--r--   0        0        0     5459 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/customize.py
--rw-r--r--   0        0        0     1966 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/cli/utils.py
--rw-r--r--   0        0        0      429 2023-04-12 06:05:51.076853 nb-cli-1.1.0/nb_cli/config/__init__.py
--rw-r--r--   0        0        0      661 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/config/model.py
--rw-r--r--   0        0        0     6153 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/config/parser.py
--rw-r--r--   0        0        0      347 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/consts.py
--rw-r--r--   0        0        0      373 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/exceptions.py
--rw-r--r--   0        0        0     2906 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/__init__.py
--rw-r--r--   0        0        0      865 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/adapter.py
--rw-r--r--   0        0        0      374 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/driver.py
--rw-r--r--   0        0        0     5756 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/meta.py
--rw-r--r--   0        0        0     3198 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/pip.py
--rw-r--r--   0        0        0     1557 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/plugin.py
--rw-r--r--   0        0        0     2986 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/process.py
--rw-r--r--   0        0        0     2665 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/project.py
--rw-r--r--   0        0        0     5718 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/reloader.py
--rw-r--r--   0        0        0     2063 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/script.py
--rw-r--r--   0        0        0     1860 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/signal.py
--rw-r--r--   0        0        0     3720 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/store.py
--rw-r--r--   0        0        0      734 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/handlers/venv.py
--rw-r--r--   0        0        0     1193 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/i18n.py
--rw-r--r--   0        0        0     8829 2023-04-12 06:06:27.398844 nb-cli-1.1.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
--rw-r--r--   0        0        0    13703 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
--rw-r--r--   0        0        0      635 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/log/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/py.typed
--rw-r--r--   0        0        0      143 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/cookiecutter.json
--rw-r--r--   0        0        0      120 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      847 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
--rw-r--r--   0        0        0      354 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
--rw-r--r--   0        0        0      203 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0      688 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
--rw-r--r--   0        0        0      676 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
--rw-r--r--   0        0        0      164 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/plugin/cookiecutter.json
--rw-r--r--   0        0        0      315 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/plugin/hooks/post_gen_project.py
--rw-r--r--   0        0        0      385 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      114 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0        0 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
--rw-r--r--   0        0        0      259 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/bootstrap/cookiecutter.json
--rw-r--r--   0        0        0      132 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0      235 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      611 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0      452 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/cookiecutter.json
--rw-r--r--   0        0        0      307 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/hooks/post_gen_project.py
--rw-r--r--   0        0        0      148 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
--rw-r--r--   0        0        0       16 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
--rw-r--r--   0        0        0        0 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0     2087 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
--rw-r--r--   0        0        0      331 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      657 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
--rw-r--r--   0        0        0      232 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/meta/_package_version.py.jinja
--rw-r--r--   0        0        0      110 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/meta/nonebot_version.py.jinja
--rw-r--r--   0        0        0      105 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/meta/pip_version.py.jinja
--rw-r--r--   0        0        0      142 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/meta/python_version.py.jinja
--rw-r--r--   0        0        0      181 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
--rw-r--r--   0        0        0     1091 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/project/_prepare.py.jinja
--rw-r--r--   0        0        0      151 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/project/run_project.py.jinja
--rw-r--r--   0        0        0      222 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/script/_entrypoint.py.jinja
--rw-r--r--   0        0        0      158 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/script/list_scripts.py.jinja
--rw-r--r--   0        0        0      333 2023-04-12 06:05:51.080854 nb-cli-1.1.0/nb_cli/template/scripts/script/run_script.py.jinja
--rw-r--r--   0        0        0     2737 2023-04-12 06:05:51.080854 nb-cli-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 nb-cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-12 06:27:17.960344 nb-cli-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3350 2023-04-12 06:27:17.960344 nb-cli-1.1.1/README.md
+-rw-r--r--   0        0        0      246 2023-04-12 06:27:17.960344 nb-cli-1.1.1/build.py
+-rw-r--r--   0        0        0      795 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/__init__.py
+-rw-r--r--   0        0        0      202 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/__main__.py
+-rw-r--r--   0        0        0     3305 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/cli/__init__.py
+-rw-r--r--   0        0        0      257 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6866 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/cli/commands/adapter.py
+-rw-r--r--   0        0        0     4243 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/cli/commands/driver.py
+-rw-r--r--   0        0        0     7195 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/cli/commands/plugin.py
+-rw-r--r--   0        0        0    10063 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/cli/commands/project.py
+-rw-r--r--   0        0        0     3409 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/cli/commands/self.py
+-rw-r--r--   0        0        0     5459 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/cli/customize.py
+-rw-r--r--   0        0        0     1966 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/cli/utils.py
+-rw-r--r--   0        0        0      429 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/config/__init__.py
+-rw-r--r--   0        0        0      661 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/config/model.py
+-rw-r--r--   0        0        0     6153 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/config/parser.py
+-rw-r--r--   0        0        0      347 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/consts.py
+-rw-r--r--   0        0        0      373 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/exceptions.py
+-rw-r--r--   0        0        0     2965 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/__init__.py
+-rw-r--r--   0        0        0      865 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/adapter.py
+-rw-r--r--   0        0        0      374 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/driver.py
+-rw-r--r--   0        0        0     5756 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/meta.py
+-rw-r--r--   0        0        0     3198 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/pip.py
+-rw-r--r--   0        0        0     1557 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/plugin.py
+-rw-r--r--   0        0        0     2986 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/process.py
+-rw-r--r--   0        0        0     2665 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/project.py
+-rw-r--r--   0        0        0     5718 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/reloader.py
+-rw-r--r--   0        0        0     2063 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/script.py
+-rw-r--r--   0        0        0     1860 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/signal.py
+-rw-r--r--   0        0        0     3720 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/store.py
+-rw-r--r--   0        0        0      734 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/handlers/venv.py
+-rw-r--r--   0        0        0     1193 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/i18n.py
+-rw-r--r--   0        0        0     8829 2023-04-12 06:27:46.224700 nb-cli-1.1.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
+-rw-r--r--   0        0        0    13703 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
+-rw-r--r--   0        0        0      635 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/log/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/py.typed
+-rw-r--r--   0        0        0      143 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/adapter/cookiecutter.json
+-rw-r--r--   0        0        0      120 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      847 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      354 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      203 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      688 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      676 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      164 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/plugin/cookiecutter.json
+-rw-r--r--   0        0        0      315 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/plugin/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      385 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      114 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0        0 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      259 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/bootstrap/cookiecutter.json
+-rw-r--r--   0        0        0      132 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0      235 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      611 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      452 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/simple/cookiecutter.json
+-rw-r--r--   0        0        0      307 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/simple/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      148 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
+-rw-r--r--   0        0        0       16 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
+-rw-r--r--   0        0        0        0 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0     2087 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
+-rw-r--r--   0        0        0      331 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      657 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      232 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/scripts/meta/_package_version.py.jinja
+-rw-r--r--   0        0        0      110 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/scripts/meta/nonebot_version.py.jinja
+-rw-r--r--   0        0        0      105 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/scripts/meta/pip_version.py.jinja
+-rw-r--r--   0        0        0      142 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/scripts/meta/python_version.py.jinja
+-rw-r--r--   0        0        0      181 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
+-rw-r--r--   0        0        0     1091 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/scripts/project/_prepare.py.jinja
+-rw-r--r--   0        0        0      151 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/scripts/project/run_project.py.jinja
+-rw-r--r--   0        0        0      222 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/scripts/script/_entrypoint.py.jinja
+-rw-r--r--   0        0        0      158 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/scripts/script/list_scripts.py.jinja
+-rw-r--r--   0        0        0      333 2023-04-12 06:27:17.960344 nb-cli-1.1.1/nb_cli/template/scripts/script/run_script.py.jinja
+-rw-r--r--   0        0        0     2737 2023-04-12 06:27:17.964344 nb-cli-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 nb-cli-1.1.1/PKG-INFO
```

### Comparing `nb-cli-1.1.0/LICENSE` & `nb-cli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/README.md` & `nb-cli-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/__init__.py` & `nb-cli-1.1.1/nb_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/cli/__init__.py` & `nb-cli-1.1.1/nb_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/cli/commands/adapter.py` & `nb-cli-1.1.1/nb_cli/cli/commands/adapter.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/cli/commands/driver.py` & `nb-cli-1.1.1/nb_cli/cli/commands/driver.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/cli/commands/plugin.py` & `nb-cli-1.1.1/nb_cli/cli/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/cli/commands/project.py` & `nb-cli-1.1.1/nb_cli/cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/cli/commands/self.py` & `nb-cli-1.1.1/nb_cli/cli/commands/self.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/cli/customize.py` & `nb-cli-1.1.1/nb_cli/cli/customize.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/cli/utils.py` & `nb-cli-1.1.1/nb_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/config/model.py` & `nb-cli-1.1.1/nb_cli/config/model.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/config/parser.py` & `nb-cli-1.1.1/nb_cli/config/parser.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/__init__.py` & `nb-cli-1.1.1/nb_cli/handlers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .meta import draw_logo as draw_logo
 from .meta import requires_pip as requires_pip
 from .meta import get_pip_version as get_pip_version
 from .meta import requires_python as requires_python
 from .meta import get_project_root as get_project_root
 from .meta import requires_nonebot as requires_nonebot
 from .meta import get_default_python as get_default_python
+from .meta import get_nonebot_config as get_nonebot_config
 from .meta import get_python_version as get_python_version
 from .meta import get_nonebot_version as get_nonebot_version
 
 # isort: split
 
 # package
 from .store import load_module_data as load_module_data
```

### Comparing `nb-cli-1.1.0/nb_cli/handlers/adapter.py` & `nb-cli-1.1.1/nb_cli/handlers/adapter.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/meta.py` & `nb-cli-1.1.1/nb_cli/handlers/meta.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/pip.py` & `nb-cli-1.1.1/nb_cli/handlers/pip.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/plugin.py` & `nb-cli-1.1.1/nb_cli/handlers/plugin.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/process.py` & `nb-cli-1.1.1/nb_cli/handlers/process.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/project.py` & `nb-cli-1.1.1/nb_cli/handlers/project.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/reloader.py` & `nb-cli-1.1.1/nb_cli/handlers/reloader.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/script.py` & `nb-cli-1.1.1/nb_cli/handlers/script.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/signal.py` & `nb-cli-1.1.1/nb_cli/handlers/signal.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/store.py` & `nb-cli-1.1.1/nb_cli/handlers/store.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/handlers/venv.py` & `nb-cli-1.1.1/nb_cli/handlers/venv.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/i18n.py` & `nb-cli-1.1.1/nb_cli/i18n.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo` & `nb-cli-1.1.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po` & `nb-cli-1.1.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/log/__init__.py` & `nb-cli-1.1.1/nb_cli/log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}` & `nb-cli-1.1.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}` & `nb-cli-1.1.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}` & `nb-cli-1.1.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb-cli-1.1.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore` & `nb-cli-1.1.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb-cli-1.1.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/nb_cli/template/scripts/project/_prepare.py.jinja` & `nb-cli-1.1.1/nb_cli/template/scripts/project/_prepare.py.jinja`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.0/pyproject.toml` & `nb-cli-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nb-cli"
-version = "1.1.0"
+version = "1.1.1"
 description = "CLI for nonebot2"
 authors = [
     { name = "yanyongyu", email = "yyy@nonebot.dev" },
 ]
 readme = "README.md"
 keywords = [
     "bot",
```

### Comparing `nb-cli-1.1.0/PKG-INFO` & `nb-cli-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-cli
-Version: 1.1.0
+Version: 1.1.1
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

 * *File "/tmp/diffoscope_g69_xk9y_/tmpl5gsgelt_TarContainer/0/73", line 148, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_g69_xk9y_/tmpl5gsgelt_TarContainer/0/73", line 148, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nb-cli Version: 1.1.0 Summary: CLI for nonebot2
+Metadata-Version: 2.1 Name: nb-cli Version: 1.1.1 Summary: CLI for nonebot2
 License: MIT Keywords: bot,qq,nonebot,bot,qq,nonebot Author-email: yanyongyu
 nonebot.dev> Requires-Python: >=3.8, <4.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: Robot Framework Classifier:
 Framework :: Robot Framework :: Library Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Project-URL: homepage, https://
 cli.nonebot.dev/ Project-URL: repository, https://github.com/nonebot/nb-cli
```

