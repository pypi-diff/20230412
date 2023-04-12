# Comparing `tmp/tickit-0.2.0.tar.gz` & `tmp/tickit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickit-0.2.0.tar", last modified: Mon Feb 20 18:07:01 2023, max compression
+gzip compressed data, was "tickit-0.2.1.tar", last modified: Wed Apr 12 12:37:01 2023, max compression
```

## Comparing `tickit-0.2.0.tar` & `tickit-0.2.1.tar`

### file list

```diff
@@ -1,305 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.868870 tickit-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.840869 tickit-0.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-02-20 18:06:52.000000 tickit-0.2.0/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-20 18:06:52.000000 tickit-0.2.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-20 18:06:52.000000 tickit-0.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.840869 tickit-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-02-20 18:06:52.000000 tickit-0.2.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.836869 tickit-0.2.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.840869 tickit-0.2.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-02-20 18:06:52.000000 tickit-0.2.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-20 18:06:52.000000 tickit-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.840869 tickit-0.2.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-20 18:06:52.000000 tickit-0.2.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-02-20 18:06:52.000000 tickit-0.2.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.844869 tickit-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-02-20 18:06:52.000000 tickit-0.2.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-02-20 18:06:52.000000 tickit-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-20 18:06:52.000000 tickit-0.2.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-02-20 18:06:52.000000 tickit-0.2.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-02-20 18:06:52.000000 tickit-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-20 18:06:52.000000 tickit-0.2.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-20 18:06:52.000000 tickit-0.2.0/.gitremotes
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-20 18:06:52.000000 tickit-0.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.844869 tickit-0.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-20 18:06:52.000000 tickit-0.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-02-20 18:06:52.000000 tickit-0.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-20 18:06:52.000000 tickit-0.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-20 18:06:52.000000 tickit-0.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-02-20 18:06:52.000000 tickit-0.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-20 18:06:52.000000 tickit-0.2.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-20 18:06:52.000000 tickit-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-02-20 18:07:01.864870 tickit-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-02-20 18:06:52.000000 tickit-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-20 18:06:52.000000 tickit-0.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.844869 tickit-0.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.844869 tickit-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.844869 tickit-0.2.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.844869 tickit-0.2.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.844869 tickit-0.2.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.844869 tickit-0.2.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.844869 tickit-0.2.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.844869 tickit-0.2.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.848869 tickit-0.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/images/example-systems.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)   343434 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/images/tickit-logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/images/tickit-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.848869 tickit-0.2.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.848869 tickit-0.2.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/user/explanations/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/user/explanations/how-component-updates-are-ordered.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.848869 tickit-0.2.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/user/how-to/accomplish-a-task.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.848869 tickit-0.2.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.848869 tickit-0.2.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/user/tutorials/creating-a-device.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/user/tutorials/creating-a-simulation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/user/tutorials/creating-an-adapter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-02-20 18:06:52.000000 tickit-0.2.0/docs/user/tutorials/running-a-simulation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.836869 tickit-0.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.848869 tickit-0.2.0/examples/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/attns.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/counter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/cryo-tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/current-monitor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/eiger-shutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/eiger.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/http-device.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/iobox.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/multi-ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/nested.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/shutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/sunk-tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/configs/sunk-trampoline.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.848869 tickit-0.2.0/examples/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/devices/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/devices/http_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/devices/iobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/devices/remote_controlled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/devices/shutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-02-20 18:06:52.000000 tickit-0.2.0/examples/devices/trampoline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-02-20 18:06:52.000000 tickit-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 18:07:01.868870 tickit-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.836869 tickit-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-20 18:07:01.000000 tickit-0.2.0/src/tickit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/composed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit/adapters/epicsadapter/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/epicsadapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/epicsadapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/epicsadapter/ioc_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/httpadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit/adapters/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit/adapters/interpreters/command/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/command/command_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/command/regex_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit/adapters/interpreters/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/endpoints/http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit/adapters/interpreters/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit/adapters/servers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/servers/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/adapters/zmqadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/components/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/components/device_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/components/system_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.856870 tickit-0.2.0/src/tickit/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/management/event_router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.856870 tickit-0.2.0/src/tickit/core/management/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/management/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/management/schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/management/schedulers/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/management/schedulers/slave.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/management/ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.856870 tickit-0.2.0/src/tickit/core/state_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/state_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/state_interfaces/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/state_interfaces/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/state_interfaces/state_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/core/typedefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.856870 tickit-0.2.0/src/tickit/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.856870 tickit-0.2.0/src/tickit/devices/cryostream/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/cryostream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/cryostream/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/cryostream/cryostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/cryostream/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/cryostream/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.856870 tickit-0.2.0/src/tickit/devices/eiger/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.856870 tickit-0.2.0/src/tickit/devices/eiger/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/data/dummy_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/eiger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/eiger_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/eiger_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/eiger_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/eiger_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.856870 tickit-0.2.0/src/tickit/devices/eiger/filewriter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/filewriter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/filewriter/eiger_filewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/filewriter/filewriter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/filewriter/filewriter_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.856870 tickit-0.2.0/src/tickit/devices/eiger/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/monitor/eiger_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/monitor/monitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/monitor/monitor_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.856870 tickit-0.2.0/src/tickit/devices/eiger/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   514994 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/resources/frame_sample
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/src/tickit/devices/eiger/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/stream/eiger_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/stream/stream_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/eiger/stream/stream_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/src/tickit/devices/femto/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/femto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/femto/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/femto/femto.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/femto/record.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/src/tickit/devices/pneumatic/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/pneumatic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/src/tickit/devices/pneumatic/db_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/pneumatic/db_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/pneumatic/db_files/filter1.db
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/pneumatic/pneumatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/devices/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/src/tickit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/utils/byte_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/src/tickit/utils/compat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/utils/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/utils/compat/functools_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/utils/compat/typing_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/src/tickit/utils/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/utils/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/utils/configuration/configurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/utils/configuration/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-20 18:06:52.000000 tickit-0.2.0/src/tickit/utils/topic_naming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.852870 tickit-0.2.0/src/tickit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-02-20 18:07:01.000000 tickit-0.2.0/src/tickit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-02-20 18:07:01.000000 tickit-0.2.0/src/tickit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 18:07:01.000000 tickit-0.2.0/src/tickit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-20 18:07:01.000000 tickit-0.2.0/src/tickit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-20 18:07:01.000000 tickit-0.2.0/src/tickit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-20 18:07:01.000000 tickit-0.2.0/src/tickit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/tests/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/tests/adapters/interpreters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/tests/adapters/interpreters/command/
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/interpreters/command/test_command_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/interpreters/command/test_regex_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/tests/adapters/interpreters/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/interpreters/endpoints/test_http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/interpreters/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/tests/adapters/interpreters/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/interpreters/wrappers/test_joining_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/tests/adapters/servers/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/servers/test_tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.860870 tickit-0.2.0/tests/adapters/test_epicsadapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/test_epicsadapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/test_epicsadapter/test_epics_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/test_httpadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/adapters/test_zmqadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/components/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/components/test_system_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/core/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/core/management/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/management/schedulers/test_base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/management/schedulers/test_master_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/management/schedulers/test_slave_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/management/test_event_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/management/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/core/state_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/state_interfaces/test_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/state_interfaces/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/state_interfaces/test_state_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/test_device_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/core/test_typedefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/devices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/devices/cryostream/
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/cryostream/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/cryostream/test_cryostream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/devices/eiger/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_filewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_filewriter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_filewriter_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_monitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_monitor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_stream_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/eiger/test_eiger_stream_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/devices/femto/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/femto/test_femto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/devices/multi/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/multi/test_multi_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/devices/pneumatic/
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/pneumatic/test_pneumatic.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/test_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/devices/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:07:01.864870 tickit-0.2.0/tests/utils/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/utils/configuration/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/utils/test_byte_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/utils/test_configurable.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/utils/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-20 18:06:52.000000 tickit-0.2.0/tests/utils/test_topic_naming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.553765 tickit-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.517765 tickit-0.2.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-12 12:36:47.000000 tickit-0.2.1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 12:36:47.000000 tickit-0.2.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 12:36:47.000000 tickit-0.2.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.517765 tickit-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.509765 tickit-0.2.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.517765 tickit-0.2.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.517765 tickit-0.2.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-12 12:36:47.000000 tickit-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-12 12:36:47.000000 tickit-0.2.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 12:36:47.000000 tickit-0.2.1/.gitremotes
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-12 12:36:47.000000 tickit-0.2.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-12 12:36:47.000000 tickit-0.2.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-12 12:36:47.000000 tickit-0.2.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-12 12:36:47.000000 tickit-0.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 12:36:47.000000 tickit-0.2.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-12 12:36:47.000000 tickit-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 12:36:47.000000 tickit-0.2.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 12:36:47.000000 tickit-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18646 2023-04-12 12:37:01.553765 tickit-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-12 12:36:47.000000 tickit-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 12:36:47.000000 tickit-0.2.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/explanations/framework-details.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/explanations/how-component-updates-are-ordered.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/explanations/why-tickit.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.525765 tickit-0.2.1/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.525765 tickit-0.2.1/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.525765 tickit-0.2.1/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.525765 tickit-0.2.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/example-systems.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-create-device-amplifier.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-device-simulation-cpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   343434 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-overview-full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-simple-dag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-simple-overview-with-system-simulation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-simple-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-simple-simulation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-system-simulation-cpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.525765 tickit-0.2.1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.529765 tickit-0.2.1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/framework-summary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/wiring.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.529765 tickit-0.2.1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/how-to/use-command-wrappers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/how-to/use-epics-adapter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.529765 tickit-0.2.1/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.529765 tickit-0.2.1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/tutorials/create-a-device.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/tutorials/creating-a-simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/tutorials/running-a-simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/tutorials/use-composed-adapter.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.513765 tickit-0.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.529765 tickit-0.2.1/examples/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/amplifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/counter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/http-device.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/nested.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/shutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/sunk-tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/sunk-trampoline.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.533765 tickit-0.2.1/examples/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/amplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/http_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/remote_controlled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/trampoline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-12 12:36:47.000000 tickit-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:37:01.553765 tickit-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.513765 tickit-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.533765 tickit-0.2.1/src/tickit/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.533765 tickit-0.2.1/src/tickit/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/composed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/epicsadapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/epicsadapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/epicsadapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/epicsadapter/ioc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/httpadapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/interpreters/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/command/command_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/command/regex_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/interpreters/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/endpoints/http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/servers/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/zmqadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.541765 tickit-0.2.1/src/tickit/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/components/device_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/components/system_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.541765 tickit-0.2.1/src/tickit/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/event_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.541765 tickit-0.2.1/src/tickit/core/management/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/schedulers/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/schedulers/slave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.541765 tickit-0.2.1/src/tickit/core/state_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/state_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/state_interfaces/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/state_interfaces/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/state_interfaces/state_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/typedefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.541765 tickit-0.2.1/src/tickit/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/devices/sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/devices/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/src/tickit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/byte_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/src/tickit/utils/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/compat/functools_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/compat/typing_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/src/tickit/utils/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/configuration/configurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/configuration/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/topic_naming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.533765 tickit-0.2.1/src/tickit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18646 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/interpreters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/interpreters/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/command/test_command_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/command/test_regex_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/interpreters/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/endpoints/test_http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/interpreters/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/wrappers/test_joining_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/servers/test_tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/adapters/test_epicsadapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/test_epicsadapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/test_epicsadapter/test_epics_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/test_httpadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/test_zmqadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/components/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/components/test_device_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/components/test_system_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/core/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/core/management/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/management/schedulers/test_base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/management/schedulers/test_master_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/management/schedulers/test_slave_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/management/test_event_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/management/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/core/state_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/state_interfaces/test_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/state_interfaces/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/state_interfaces/test_state_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/test_typedefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/devices/test_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/devices/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.553765 tickit-0.2.1/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.553765 tickit-0.2.1/tests/utils/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/utils/configuration/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/utils/test_byte_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/utils/test_configurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/utils/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/utils/test_topic_naming.py
```

### Comparing `tickit-0.2.0/.devcontainer/devcontainer.json` & `tickit-0.2.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/.github/CONTRIBUTING.rst` & `tickit-0.2.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/.github/actions/install_requirements/action.yml` & `tickit-0.2.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/.github/dependabot.yml` & `tickit-0.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/.github/pages/make_switcher.py` & `tickit-0.2.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/.github/workflows/code.yml` & `tickit-0.2.1/.github/workflows/code.yml`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             type=raw,value=latest
 
       - name: Set up Docker Buildx
         id: buildx
         uses: docker/setup-buildx-action@v2
 
       - name: Build runtime image
-        uses: docker/build-push-action@v3
+        uses: docker/build-push-action@v4
         with:
           build-args: |
             PIP_OPTIONS=-r lockfiles/requirements.txt dist/*.whl
           push: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags') }}
           load: ${{ ! (github.event_name == 'push' && startsWith(github.ref, 'refs/tags')) }}
           tags: ${{ steps.meta.outputs.tags }}
           labels: ${{ steps.meta.outputs.labels }}
```

### Comparing `tickit-0.2.0/.github/workflows/docs.yml` & `tickit-0.2.1/.github/workflows/docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -43,12 +43,12 @@
       - name: Write switcher.json
         run: python .github/pages/make_switcher.py --add $DOCS_VERSION ${{ github.repository }} .github/pages/switcher.json
 
       - name: Publish Docs to gh-pages
         if: github.event_name == 'push' && github.actor != 'dependabot[bot]'
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: peaceiris/actions-gh-pages@64b46b4226a4a12da2239ba3ea5aa73e3163c75b # v3.9.1
+        uses: peaceiris/actions-gh-pages@373f7f263a76c20808c831209c920827a82a2847 # v3.9.3
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
```

### Comparing `tickit-0.2.0/.github/workflows/docs_clean.yml` & `tickit-0.2.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/.github/workflows/linkcheck.yml` & `tickit-0.2.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/.gitignore` & `tickit-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/.gitlab-ci.yml` & `tickit-0.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/.vscode/launch.json` & `tickit-0.2.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/.vscode/settings.json` & `tickit-0.2.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/CHANGELOG.rst` & `tickit-0.2.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/Dockerfile` & `tickit-0.2.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/LICENSE` & `tickit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/PKG-INFO` & `tickit-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Event-based device simulation framework
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,71 +224,97 @@
 An event-based multi-device simulation framework providing configuration and
 orchestration of complex multi-device simulations.
 
 ============== ==============================================================
 PyPI           ``pip install tickit``
 Source code    https://github.com/dls-controls/tickit
 Documentation  https://dls-controls.github.io/tickit
-Changelog      https://github.com/dls-controls/tickit/blob/master/CHANGELOG.rst
+Releases       https://github.com/dls-controls/tickit-devices/releases
 ============== ==============================================================
 
-An example device which emits a random value between *0* and *255* whenever
-called and asks to be called again once the simulation has progressed by the
-``callback_period``.  Additionally, extenal control of **RandomTrampoline** is
-afforded by a **RemoteControlledAdapter** which is exposed extenally through 
-a **TCPServer**:
+An example simulation consits of a simple counter and a sink. The counter
+increments up a given value and then passes this value to a sink.
+
+A simulation is defined using a yaml file, in which the graphing of the required
+components is denoted. This file defines a **Counter** device named **counter** and
+a **Sink** device named **counter_sink**. The output **_value** of **counter** is wired
+to the input of **counter_sink**.
+
+.. code-block:: yaml
+
+    - examples.devices.counter.Counter:
+        name: counter  
+        inputs: {}
+    - tickit.devices.sink.Sink:
+        name: counter_sink
+        inputs:
+          input: counter:_value
+
+
+This file is executed to run the simultation.
+
+.. code-block:: bash
+
+    python -m tickit all examples/configs/counter.yaml
+
+
+The simulation will output logs depicting the incerementing of the counter:
+
+.. code-block:: bash
+
+    DEBUG:examples.devices.counter:Counter initialized with value => 0
+    DEBUG:asyncio:Using selector: EpollSelector
+    DEBUG:tickit.core.management.ticker:Doing tick @ 0
+    DEBUG:tickit.core.components.component:counter got Input(target='counter', time=0, changes=immutables.Map({}))
+    DEBUG:examples.devices.counter:Counter incremented to 1
+    DEBUG:tickit.core.management.schedulers.base:Scheduler got Output(source='counter', time=0, changes=immutables.Map({'value': 1}), call_at=1000000000)
+    DEBUG:tickit.core.management.schedulers.base:Scheduling counter for wakeup at 1000000000
+    DEBUG:tickit.core.components.component:counter_sink got Input(target='counter_sink', time=0, changes=immutables.Map({}))
+    DEBUG:tickit.devices.sink:Sunk {}
+    DEBUG:tickit.core.management.schedulers.base:Scheduler got Output(source='counter_sink', time=0, changes=immutables.Map({}), call_at=None) 
+    DEBUG:tickit.core.management.ticker:Doing tick @ 1000000000
+    DEBUG:tickit.core.components.component:counter got Input(target='counter', time=1000000000, changes=immutables.Map({}))
+    DEBUG:examples.devices.counter:Counter incremented to 2
+    DEBUG:tickit.core.management.schedulers.base:Scheduler got Output(source='counter', time=1000000000, changes=immutables.Map({'value': 2}), call_at=2000000000)
+
+
+The counting device is defined as below. It increments a given value and logs as
+it increments.
 
 .. code-block:: python
 
     @dataclass
-    class RandomTrampoline(ComponentConfig):
+    class Counter(ComponentConfig):
+        """Simple counting device."""
 
         def __call__(self) -> Component:  # noqa: D102
             return DeviceSimulation(
                 name=self.name,
-                device=RandomTrampolineDevice(),
-                adapters=[RemoteControlledAdapter(server=TcpServer(format="%b\r\n"))])
+                device=CounterDevice(),
+                )
 
-
-    class RandomTrampolineDevice(Device):
+    class CounterDevice(Device):
+        """A simple device which increments a value."""
 
         Inputs: TypedDict = TypedDict("Inputs", {})
-        Outputs: TypedDict = TypedDict("Outputs", {"output": int})
+        Outputs: TypedDict = TypedDict("Outputs", {"value":int})
 
-        def __init__(self, callback_period: int = int(1e9)) -> None:
+        def __init__(self, initial_value: int = 0, callback_period: int = int(1e9)) -> None:
+            self._value = initial_value
             self.callback_period = SimTime(callback_period)
+            LOGGER.debug(f"Counter initialized with value => {self._value}")
 
         def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
-            output = randint(0, 255)
-            LOGGER.debug(
-                "Boing! (delta: {}, inputs: {}, output: {})".format(time, inputs, output)
-            )
+            self._value = self._value + 1
+            LOGGER.debug("Counter incremented to {}".format(self._value))
             return DeviceUpdate(
-                RandomTrampoline.Outputs(output=output),
+                CounterDevice.Outputs(value=self._value),
                 SimTime(time + self.callback_period),
             )
 
-
-An example simulation defines a **RemoteControlled** device named **tcp_contr**
-and a **Sink** device named **contr_sink**. The **observed** output of
-**tcp_contr** is wired to the **input** input of **contr_sink**:
-
-.. code-block:: yaml
-
-
-    - examples.devices.remote_controlled.RemoteControlled: {}
-        name: tcp_contr
-        inputs: {}
-    - tickit.devices.sink.Sink: {}
-        name: contr_sink
-        inputs:
-          input: tcp_contr:observed
-
-
-
 .. |code_ci| image:: https://github.com/dls-controls/tickit/workflows/Code%20CI/badge.svg?branch=master
     :target: https://github.com/dls-controls/tickit/actions?query=workflow%3A%22Code+CI%22
     :alt: Code CI
 
 .. |docs_ci| image:: https://github.com/dls-controls/tickit/workflows/Docs%20CI/badge.svg?branch=master
     :target: https://github.com/dls-controls/tickit/actions?query=workflow%3A%22Docs+CI%22
     :alt: Docs CI
```

### Comparing `tickit-0.2.0/docs/_static/theme_overrides.css` & `tickit-0.2.1/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/conf.py` & `tickit-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/developer/explanations/decisions.rst` & `tickit-0.2.1/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/developer/how-to/build-docs.rst` & `tickit-0.2.1/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/developer/how-to/lint.rst` & `tickit-0.2.1/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/developer/how-to/make-release.rst` & `tickit-0.2.1/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/developer/how-to/pin-requirements.rst` & `tickit-0.2.1/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/developer/how-to/test-container.rst` & `tickit-0.2.1/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/developer/how-to/update-tools.rst` & `tickit-0.2.1/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/developer/index.rst` & `tickit-0.2.1/docs/user/index.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-Developer Guide
-===============
+User Guide
+==========
 
 Documentation is split into four categories, also accessible from links in the
 side-bar.
 
 .. grid:: 2
     :gutter: 4
 
-    .. grid-item-card:: :material-regular:`directions_run;3em`
+    .. grid-item-card:: :material-regular:`directions_walk;3em`
 
         .. toctree::
             :caption: Tutorials
             :maxdepth: 1
 
-            tutorials/dev-install
+            tutorials/installation
+            tutorials/running-a-simulation
+            tutorials/creating-a-simulation
+            tutorials/create-a-device
+            tutorials/use-composed-adapter
 
         +++
 
-        Tutorials for getting up and running as a developer.
+        Tutorials for installation and typical usage. New users start here.
 
-    .. grid-item-card:: :material-regular:`task;3em`
+    .. grid-item-card:: :material-regular:`directions;3em`
 
         .. toctree::
             :caption: How-to Guides
             :maxdepth: 1
 
-            how-to/contribute
-            how-to/build-docs
-            how-to/run-tests
-            how-to/static-analysis
-            how-to/lint
-            how-to/update-tools
-            how-to/make-release
-            how-to/pin-requirements
-            how-to/test-container
+            how-to/use-epics-adapter
+            how-to/use-command-wrappers
 
         +++
 
-        Practical step-by-step guides for day-to-day dev tasks.
+        Practical step-by-step guides for the more experienced user.
 
-    .. grid-item-card:: :material-regular:`apartment;3em`
+    .. grid-item-card:: :material-regular:`info;3em`
 
         .. toctree::
             :caption: Explanations
             :maxdepth: 1
 
-            explanations/decisions
+            explanations/framework-summary
+            explanations/components
+            explanations/devices
+            explanations/adapters
+            explanations/wiring
+            explanations/glossary
 
         +++
 
-        Explanations of how and why the architecture is why it is.
+        Explanations of how the library works and why it works that way.
 
-    .. grid-item-card:: :material-regular:`description;3em`
+    .. grid-item-card:: :material-regular:`menu_book;3em`
 
         .. toctree::
             :caption: Reference
             :maxdepth: 1
 
-            reference/standards
+            reference/api
+            ../genindex
 
         +++
 
-        Technical reference material on standards in use.
+        Technical reference material including APIs and release notes.
```

### Comparing `tickit-0.2.0/docs/developer/reference/standards.rst` & `tickit-0.2.1/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/developer/tutorials/dev-install.rst` & `tickit-0.2.1/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/images/example-systems.drawio.svg` & `tickit-0.2.1/docs/images/example-systems.drawio.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/images/tickit-logo.ico` & `tickit-0.2.1/docs/images/tickit-logo.ico`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/images/tickit-logo.svg` & `tickit-0.2.1/docs/images/tickit-logo.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/index.rst` & `tickit-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/user/explanations/glossary.rst` & `tickit-0.2.1/docs/user/explanations/glossary.rst`

 * *Files 3% similar despite different names*

```diff
@@ -36,12 +36,13 @@
         An interrupt is a request to immediately update a component - typically
         these are generated by an adapter and handled by the scheduler.
 
     Ticker
         A ticker sequences the update of components during a tick to ensure
         that all wired component interactions are captured faithfully.
 
-        .. seealso:: `How component updates are ordered`
+        .. seealso::  
+            :doc:`How component updates are ordered<../../developer/explanations/how-component-updates-are-ordered>`
 
     Scheduler
         A scheduler oversees and orchestrates the running of a simulation, and
         is responsible for initiating ticks to handle callbacks or interrupts.
```

### Comparing `tickit-0.2.0/docs/user/explanations/how-component-updates-are-ordered.rst` & `tickit-0.2.1/docs/developer/explanations/how-component-updates-are-ordered.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/user/reference/api.rst` & `tickit-0.2.1/docs/user/reference/api.rst`

 * *Files 27% similar despite different names*

```diff
@@ -109,15 +109,16 @@
 
             ``tickit.core.management.ticker``
             ---------------------------------
 
             .. autoclass:: tickit.core.management.ticker.Ticker
                 :members:
                 
-                .. seealso:: `How component updates are ordered`
+                .. seealso:: 
+                    :doc:`How component updates are ordered<../../developer/explanations/how-component-updates-are-ordered>`
     
 
     .. automodule:: tickit.core.state_interfaces
 
         ``tickit.core.state_interfaces``
         --------------------------------
 
@@ -149,51 +150,110 @@
 
         ``tickit.adapters.interpreters``
         --------------------------------
 
         .. automodule:: tickit.adapters.interpreters.command
 
             ``tickit.adapters.interpreters.command``
-            ----------------------------------------------
+            ----------------------------------------
 
             .. automodule:: tickit.adapters.interpreters.command.command_interpreter
                 :members:
 
                 ``tickit.adapters.interpreters.command.command_interpreter``
                 ------------------------------------------------------------
 
             .. automodule:: tickit.adapters.interpreters.command.regex_command
                 :members:
 
                 ``tickit.adapters.interpreters.command.regex_command``
                 ------------------------------------------------------
 
+
+        .. automodule:: tickit.adapters.interpreters.endpoints
+
+            ``tickit.adapters.interpreters.endpoints``
+            ------------------------------------------
+
+            .. automodule:: tickit.adapters.interpreters.endpoints.http_endpoint
+                :members:
+
+                ``tickit.adapters.interpreters.endpoints.http_endpoint``
+                --------------------------------------------------------
+
+        
+        .. automodule:: tickit.adapters.interpreters.wrappers
+
+            ``tickit.adapters.interpreters.wrappers``
+            -----------------------------------------
+
+            .. automodule:: tickit.adapters.interpreters.wrappers.beheading_interpreter
+                :members:
+
+                ``tickit.adapters.interpreters.wrappers.beheading_interpreter``
+                ---------------------------------------------------------------
+
+            .. automodule:: tickit.adapters.interpreters.wrappers.joining_interpreter
+                :members:
+
+                ``tickit.adapters.interpreters.wrappers.joining_interpreter``
+                -------------------------------------------------------------
+            
+            .. automodule:: tickit.adapters.interpreters.wrappers.splitting_interpreter
+                :members:
+
+                ``tickit.adapters.interpreters.wrappers.splitting_interpreter``
+                ---------------------------------------------------------------
+
+
     .. automodule:: tickit.adapters.servers
 
         ``tickit.adapters.servers``
         ---------------------------
 
         .. automodule:: tickit.adapters.servers.tcp
             :members:
 
             ``tickit.adapters.servers.tcp``
             -------------------------------
 
+
     .. automodule:: tickit.adapters.composed
         :members:
         
         ``tickit.adapters.composed``
         ----------------------------
-    
-    .. automodule:: tickit.adapters.epicsadapter
+
+
+    .. automodule:: tickit.adapters.httpadapter
+        :members:
+        
+        ``tickit.adapters.httpadapter``
+        -------------------------------
+
+
+    .. automodule:: tickit.adapters.zmqadapter
         :members:
+        
+        ``tickit.adapters.zmqadapter``
+        ------------------------------
+
+
+    .. automodule:: tickit.adapters.epicsadapter
 
         ``tickit.adapters.epicsadapter``
         --------------------------------
 
+        .. automodule:: tickit.adapters.epicsadapter.adapter
+            :members:
+
+            ``tickit.adapters.epicsadapter.adapter``
+            ----------------------------------------
+
+
 
 .. automodule:: tickit.devices
 
     ``tickit.devices``
     ------------------
 
     .. automodule:: tickit.devices.sink
@@ -204,64 +264,14 @@
 
     .. automodule:: tickit.devices.source
         :members:
 
         ``tickit.devices.source``
         -----------------------------
 
-    .. automodule:: tickit.devices.cryostream
-
-    ``tickit.devices.cryostream``
-    -----------------------------
-
-        .. automodule:: tickit.devices.cryostream.base
-            :members:
-            
-            ``tickit.devices.cryostream.base``
-            ----------------------------------
-        
-        .. automodule:: tickit.devices.cryostream.cryostream
-            :members:
-
-            ``tickit.devices.cryostream.cryostream``
-            ----------------------------------------
-        
-        .. automodule:: tickit.devices.cryostream.status
-            :members:
-
-            ``tickit.devices.cryostream.status``
-            ------------------------------------
-
-        .. automodule:: tickit.devices.cryostream.states   
-            :members:
-
-            ``tickit.device.cryostream.states``
-            -----------------------------------
-        
-    .. automodule:: tickit.devices.femto
-
-    ``tickit.devices.femto``
-    ------------------------
-
-        .. automodule:: tickit.devices.femto.femto
-            :members:
-        
-            ``tickit.devices.femto.femto``
-            ------------------------------
-
-    .. automodule:: tickit.devices.pneumatic
-    
-    ``tickit.devices.pneumatic``
-    ----------------------------
-
-        .. automodule:: tickit.devices.pneumatic.pneumatic
-            :members:
-        
-            ``tickit.devices.pneumatic.pneumatic``
-            --------------------------------------
 
 
 .. automodule:: tickit.utils
 
     ``tickit.utils``
     ----------------
```

### Comparing `tickit-0.2.0/docs/user/tutorials/creating-a-simulation.rst` & `tickit-0.2.1/docs/user/tutorials/creating-a-simulation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Creating a Simulation
 =====================
 
 This tutorial shows how to create a simulated system consisting of several included
-devices using the tickit framework - specifically a RandomTrampoline and a `Sink`.
+devices using the tickit framework - specifically a ``RandomTrampoline`` and a `Sink`.
 
 Configuration File
 ------------------
 
 We shall begin by creating a new YAML file named ``my_simulation.yaml``, and open it
 with our preferred text editor. This file will be used to configure each of the devices
 and wire them together.
@@ -15,15 +15,15 @@
 --------------
 
 In order to be included in a simulation, tickit devices must have a `ComponentConfig`
 dataclass associated with them. This defines the device to be used, as well as any
 adapters to allow the device to be externally controlled. At the top level, tickit 
 simulations comprise a list of these components which are denoted in YAML.
 
-In this example our first device shall be a RandomTrampoline with a callback_period 
+In this example our first device shall be a ``RandomTrampoline`` with a callback_period 
 of :math:`1s` or :math:`10^9n\s` named ``rand_tramp`` with no adapters - denoted 
 in YAML by ``[]`` - and with no mapped inputs - denoted in YAML by ``{}``. As such 
 we may extend our config, as:
 
 .. code-block:: yaml
     
     - examples.devices.trampoline.RandomTrampoline:
@@ -72,8 +72,11 @@
     Boing! (delta: 1000000000, inputs: immutables.Map({}), output: 139)
     Scheduler got Output(source='rand_tramp', time=1000000000, changes=immutables.Map({'output': 139}), call_in=1000000000)
     Scheduling Wakeup(component='rand_tramp', when=2000000000)
     tramp_sink got Input(target='tramp_sink', time=1000000000, changes=immutables.Map({'input': 139}))
     Sunk {'input': 139}
     Scheduler got Output(source='tramp_sink', time=1000000000, changes=immutables.Map({}), call_in=None)
 
-.. seealso:: `Running a Simulation`
+.. seealso:: 
+    :doc:`Running a Simulation<running-a-simulation>`
+
+.. _Sink: <tickit.devices.sink.Sink>
```

### Comparing `tickit-0.2.0/docs/user/tutorials/installation.rst` & `tickit-0.2.1/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/docs/user/tutorials/running-a-simulation.rst` & `tickit-0.2.1/docs/user/tutorials/running-a-simulation.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/examples/configs/nested.yaml` & `tickit-0.2.1/examples/configs/nested.yaml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/examples/devices/counter.py` & `tickit-0.2.1/examples/devices/counter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/examples/devices/http_device.py` & `tickit-0.2.1/examples/devices/http_device.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/examples/devices/iobox.py` & `tickit-0.2.1/examples/devices/amplifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,105 @@
 from dataclasses import dataclass
 
+from typing_extensions import TypedDict
+
 from tickit.adapters.composed import ComposedAdapter
-from tickit.adapters.interpreters.command import CommandInterpreter, RegexCommand
+from tickit.adapters.interpreters.command.command_interpreter import CommandInterpreter
+from tickit.adapters.interpreters.command.regex_command import RegexCommand
 from tickit.adapters.servers.tcp import TcpServer
-from tickit.core.adapter import Server
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
-from tickit.utils.compat.typing_compat import TypedDict
 
 
-class IoBoxDevice(Device):
-    """An isolated toy device which stores a message.
+class AmplifierDevice(Device):
+    """Amplifier device which multiplies an input signal by an amplification value."""
 
-    The device takes no inputs and produces no outputs. It interacts exclusively with
-    an adapter which sets incoming messages to it and reads stored messages from it.
-    """
+    Inputs: TypedDict = TypedDict("Inputs", {"initial_signal": float})
+    Outputs: TypedDict = TypedDict("Outputs", {"amplified_signal": float})
 
-    #: An empty typed mapping of device inputs
-    Inputs: TypedDict = TypedDict("Inputs", {})
-    #: A typed mapping containing the current output value
-    Outputs: TypedDict = TypedDict("Outputs", {})
+    def __init__(self, initial_amplification: float = 2) -> None:
+        """Amplifier constructor which configures the initial amplification.
 
-    def __init__(self, inital_value: str = "Hello") -> None:
-        """The IoBox constructor, sets intial message value."""
-        self.message = inital_value
+        Args:
+            initial_amplification (float): The inital value of amplification of the
+                device. Defaults to 2.
+        """
+        self.amplification = initial_amplification
 
     def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
-        """The update method which produces an output mapping containing the observed
-        value.
+        """Update method that amplifies input signal and produces scaled output signal.
 
-        For this device the DeviceUpdate produces no outputs.
+        This update method multiplies the input signal by the amplification value and
+        returns a device update with this new scaled signal as an output.
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             inputs (State): A mapping of inputs to the device and their values.
 
         Returns:
             DeviceUpdate[Outputs]:
-                The produced update event which contains the observed value, in this
-                case nothing is provided. The device never requests a callback.
+                The produced update event which contains the value of the new amplified
+                signal.
         """
-        return DeviceUpdate(IoBoxDevice.Outputs(), None)
+        amplified_value = inputs["initial_signal"] * self.amplification
+        return DeviceUpdate(self.Outputs(amplified_signal=amplified_value), None)
 
 
-class IOBoxAdapater(ComposedAdapter):
-    """A Composed adapter for setting and getting the device property."""
+class AmplifierAdapter(ComposedAdapter):
+    """A composed adapter which gets and sets the value of amplification."""
 
-    device: IoBoxDevice
+    device: AmplifierDevice
 
     def __init__(
         self,
-        server: Server,
+        host: str = "localhost",
+        port: int = 25565,
     ) -> None:
-        """Constructor of the IoBoc Adapter, builds the configured server.
+        """Instantiate a composed amplifier adapter with a configured TCP server.
 
         Args:
-            server (Server): The immutable data container used to configure a
-                server.
+            host (Optional[str]): The host address of the TcpServer. Defaults to
+                "localhost".
+            port (Optional[int]): The bound port of the TcpServer. Defaults to 25565.
+
         """
         super().__init__(
-            server,
+            TcpServer(host, port, ByteFormat(b"%b\r\n")),
             CommandInterpreter(),
         )
 
-    @RegexCommand(r"m=([a-zA-Z0-9_!.?-]+)", interrupt=True, format="utf-8")
-    async def set_message(self, value: str) -> None:
-        """Regex string command which sets the value of the message.
+    @RegexCommand(r"A\?", False, "utf-8")
+    async def get_amplification(self) -> bytes:
+        """Regex string command which returns the utf-8 encoded value of amplification.
 
-        Args:
-            value (str): The new value of the message.
+        Returns:
+            bytes: The utf-8 encoded value of amplification.
         """
-        self.device.message = value
+        return str(self.device.amplification).encode("utf-8")
 
-    @RegexCommand(r"m\?", format="utf-8")
-    async def get_message(self) -> bytes:
-        """Regex string command which returns the utf-8 encoded value of the message.
+    @RegexCommand(r"A=(\d+\.?\d*)", True, "utf-8")
+    async def set_amplification(self, amplification: float) -> None:
+        """Regex string command which sets the value of amplification.
 
-        Returns:
-            bytes: The utf-8 encoded value of the message.
+        Args:
+            amplification (float): The desired value of amplification.
         """
-        return str(self.device.message).encode("utf-8")
+        self.device.amplification = amplification
 
 
 @dataclass
-class IoBox(ComponentConfig):
-    """IO Box you can talk to over TCP."""
+class Amplifier(ComponentConfig):
+    """Amplifier you can set the amplification value of over TCP."""
 
-    host: str = "localhost"
-    port: int = 25565
-    format: ByteFormat = ByteFormat(b"%b\r\n")
+    initial_amplification: int
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
             name=self.name,
-            device=IoBoxDevice(),
-            adapters=[IOBoxAdapater(TcpServer(self.host, self.port, self.format))],
+            device=AmplifierDevice(
+                initial_amplification=self.initial_amplification,
+            ),
+            adapters=[AmplifierAdapter()],
         )
```

### Comparing `tickit-0.2.0/examples/devices/remote_controlled.py` & `tickit-0.2.1/examples/devices/remote_controlled.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/examples/devices/shutter.py` & `tickit-0.2.1/examples/devices/shutter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/examples/devices/trampoline.py` & `tickit-0.2.1/examples/devices/trampoline.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/pyproject.toml` & `tickit-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -96,16 +96,17 @@
 # Run pytest with all our checkers, and don't spam us with massive tracebacks on error
 addopts = """
     --tb=native -vv --doctest-modules --doctest-glob="*.rst"
     --cov=tickit --cov-report term --cov-report xml:cov.xml
     """
 # https://iscinumpy.gitlab.io/post/bound-version-constraints/#watch-for-warnings
 filterwarnings = [
-    # "error",# Suppress warnings as errors untill the depricated asyncio changes have been adressed
+    "error",
     "ignore::DeprecationWarning:aiozmq", # Supress warnings about deprecated asyncio syntax in aiozmq
+    "ignore::ImportWarning" # Import issue in six, used by aiokafa https://github.com/benjaminp/six/issues/368
 ]
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "docs src tests"
 
 [tool.coverage.run]
 data_file = "/tmp/tickit.coverage"
```

### Comparing `tickit-0.2.0/src/tickit/adapters/composed.py` & `tickit-0.2.1/src/tickit/adapters/composed.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/epicsadapter/adapter.py` & `tickit-0.2.1/src/tickit/adapters/epicsadapter/adapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/epicsadapter/ioc_manager.py` & `tickit-0.2.1/src/tickit/adapters/epicsadapter/ioc_manager.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/httpadapter.py` & `tickit-0.2.1/src/tickit/adapters/httpadapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/interpreters/command/command_interpreter.py` & `tickit-0.2.1/src/tickit/adapters/interpreters/command/command_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/interpreters/command/regex_command.py` & `tickit-0.2.1/src/tickit/adapters/interpreters/command/regex_command.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/interpreters/endpoints/http_endpoint.py` & `tickit-0.2.1/src/tickit/adapters/interpreters/endpoints/http_endpoint.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/interpreters/utils.py` & `tickit-0.2.1/src/tickit/adapters/interpreters/utils.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py` & `tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py` & `tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py` & `tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/servers/tcp.py` & `tickit-0.2.1/src/tickit/adapters/servers/tcp.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/adapters/zmqadapter.py` & `tickit-0.2.1/src/tickit/adapters/zmqadapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/cli.py` & `tickit-0.2.1/src/tickit/cli.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/core/adapter.py` & `tickit-0.2.1/src/tickit/core/adapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/core/components/component.py` & `tickit-0.2.1/src/tickit/core/components/component.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import asyncio
 import logging
+import traceback
 from abc import abstractmethod
 from dataclasses import dataclass
 from typing import Dict, Optional, Type, Union
 
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
 from tickit.core.typedefs import (
     Changes,
+    ComponentException,
     ComponentID,
     ComponentPort,
     Input,
     Interrupt,
     Output,
     PortID,
     SimTime,
+    StopComponent,
 )
 from tickit.utils.configuration.configurable import as_tagged_union
 from tickit.utils.topic_naming import input_topic, output_topic
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -33,19 +37,19 @@
 
     name: ComponentID
 
     @abstractmethod
     async def run_forever(
         self, state_consumer: Type[StateConsumer], state_producer: Type[StateProducer]
     ) -> None:
-        """An asynchronous method allowing indefinite running of core logic."""
+        """Asynchronous method allowing indefinite running of core logic."""
 
     @abstractmethod
     async def on_tick(self, time: SimTime, changes: Changes):
-        """An asynchronous method called whenever the component is to be updated.
+        """Asynchronous method called whenever the component is to be updated.
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             changes (Changes): A mapping of changed component inputs and their new
                 values.
         """
 
@@ -67,33 +71,46 @@
         """Create the component from the given config."""
         raise NotImplementedError(self)
 
 
 class BaseComponent(Component):
     """A base class for compnents, implementing state interface related methods."""
 
-    state_consumer: StateConsumer[Input]
-    state_producer: StateProducer[Union[Interrupt, Output]]
+    state_consumer: StateConsumer[Union[Input, StopComponent]]
+    state_producer: StateProducer[Union[Interrupt, Output, ComponentException]]
 
-    async def handle_input(self, input: Input):
-        """Calls on_tick when an input is recieved.
+    async def handle_input(self, message: Union[Input, StopComponent]):
+        """Call on_tick when an input is recieved.
 
         Args:
-            input (Input): An immutable data container for Component inputs.
+            message (Union[Input, StopComponent])): An immutable data container for any
+                message a component recieves.
         """
-        LOGGER.debug("{} got {}".format(self.name, input))
-        await self.on_tick(input.time, input.changes)
+        if isinstance(message, Input):
+            LOGGER.debug(f"{self.name} got {message}")
+            try:
+                await asyncio.gather(
+                    self.on_tick(message.time, message.changes), return_exceptions=False
+                )
+            except Exception as err:
+                LOGGER.exception(f"Exception occured in {self.name} component.")
+                await self.state_producer.produce(
+                    output_topic(self.name),
+                    ComponentException(self.name, err, traceback.format_exc()),
+                )
+        if isinstance(message, StopComponent):
+            await self.stop_component()
 
     async def output(
         self,
         time: SimTime,
         changes: Changes,
         call_at: Optional[SimTime],
     ) -> None:
-        """Constructs and sends an Output message to the component output topic.
+        """Construct and send an Output message to the component output topic.
 
         An asynchronous method which constructs an Output message tagged with the
         component name and sends it to the output topic of this component.
 
         Args:
             time (SimTime): The current time (in nanoseconds).
             changes (Changes): A mapping of the difference between the last observable
@@ -102,29 +119,29 @@
                 requests to be awoken.
         """
         await self.state_producer.produce(
             output_topic(self.name), Output(self.name, time, changes, call_at)
         )
 
     async def raise_interrupt(self) -> None:
-        """Sends an Interrupt message to the component output topic.
+        """Send an Interrupt message to the component output topic.
 
         An asynchronous method whicb constructs an Interrupt message tagged with the
         component name and sends it to the output topic of this component.
         """
         await self.state_producer.produce(output_topic(self.name), Interrupt(self.name))
 
     async def run_forever(
         self, state_consumer: Type[StateConsumer], state_producer: Type[StateProducer]
     ) -> None:
-        """Creates and configures a state consumer and state producer.
+        """Create and configures a state consumer and state producer.
 
         An asynchronous method which creates a state consumer which is subscribed to
         the input topic of the component and calls back to handle_input, and a state
-        producer to produce Interrupt or Output messages.
+        producer to produce Interrupt, Output or ComponentException messages.
         """
         self.state_consumer = state_consumer(self.handle_input)
         await self.state_consumer.subscribe([input_topic(self.name)])
         self.state_producer = state_producer()
 
     @abstractmethod
     async def on_tick(self, time: SimTime, changes: Changes):
@@ -133,7 +150,12 @@
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             changes (Changes): A mapping of changed component inputs and their new
                 values.
         """
         raise NotImplementedError
+
+    @abstractmethod
+    async def stop_component(self) -> None:
+        """Abstract asynchronous method which cancels the running component tasks."""
+        raise NotImplementedError
```

### Comparing `tickit-0.2.0/src/tickit/core/components/device_simulation.py` & `tickit-0.2.1/src/tickit/core/components/device_simulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import logging
 from dataclasses import dataclass, field
 from typing import Awaitable, Callable, Dict, Hashable, List, Mapping, Type, cast
 
 from immutables import Map
 
 from tickit.core.adapter import Adapter
 from tickit.core.components.component import BaseComponent
@@ -10,40 +11,45 @@
 from tickit.core.runner import run_all
 from tickit.core.state_interfaces import StateConsumer, StateProducer
 from tickit.core.typedefs import Changes, ComponentID, SimTime, State
 
 InterruptHandler = Callable[[], Awaitable[None]]
 
 
+LOGGER = logging.getLogger(__name__)
+
+
 @dataclass
 class DeviceSimulation(BaseComponent):
     """A component containing a device and the corresponding adapters.
 
     A component which thinly wraps a device and the corresponding adapters, this
     component delegates core behaviour to the update method of the device, whilst
     allowing adapters to raise interrupts.
     """
 
     name: ComponentID
     device: Device
     adapters: List[Adapter] = field(default_factory=list)
     last_outputs: State = field(init=False, default_factory=lambda: State({}))
     device_inputs: Dict[str, Hashable] = field(init=False, default_factory=dict)
+    _tasks: List[asyncio.Task] = field(default_factory=list)
 
     async def run_forever(
         self, state_consumer: Type[StateConsumer], state_producer: Type[StateProducer]
     ) -> None:
-        """Sets up state interfaces, runs adapters and blocks until any complete."""
-        tasks = run_all(
+        """Set up state interfaces, run adapters and blocks until any complete."""
+        self._tasks = run_all(
             adapter.run_forever(self.device, self.raise_interrupt)
             for adapter in self.adapters
         )
+
         await super().run_forever(state_consumer, state_producer)
-        if tasks:
-            await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
+        if self._tasks:
+            await asyncio.wait(self._tasks)
 
     async def on_tick(self, time: SimTime, changes: Changes) -> None:
         """Delegates core behaviour to the device and calls adapter on_update.
 
         An asynchronous method which updates device inputs according to external
         changes, delegates core behaviour to the device update method, informs
         Adapters of the update, computes changes to the state of the component
@@ -70,7 +76,16 @@
                     for k, v in device_update.outputs.items()
                     if k not in self.last_outputs or not self.last_outputs[k] == v
                 }
             )
         )
         self.last_outputs = device_update.outputs
         await self.output(time, out_changes, device_update.call_at)
+
+    async def stop_component(self) -> None:
+        """Cancel all pending tasks associated with the device component.
+
+        Cancels long running adapter tasks associated with the component.
+        """
+        LOGGER.debug("Stopping {}".format(self.name))
+        for task in self._tasks:
+            task.cancel()
```

### Comparing `tickit-0.2.0/src/tickit/core/components/system_simulation.py` & `tickit-0.2.1/src/tickit/core/components/system_simulation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import asyncio
-from dataclasses import dataclass
+import logging
+from dataclasses import dataclass, field
 from typing import Dict, List, Type
 
 from tickit.core.components.component import BaseComponent, Component, ComponentConfig
 from tickit.core.management.event_router import InverseWiring
 from tickit.core.management.schedulers.slave import SlaveScheduler
 from tickit.core.runner import run_all
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
 from tickit.core.typedefs import Changes, ComponentID, ComponentPort, PortID, SimTime
+from tickit.utils.topic_naming import output_topic
+
+LOGGER = logging.getLogger(__name__)
 
 
 @dataclass
 class SystemSimulationComponent(BaseComponent):
     """A component containing a slave scheduler and several components.
 
     A component which acts as a nested tickit simulation by wrapping a slave scheduler
@@ -24,14 +28,16 @@
     #: A list of immutable component configuration data containers, used to
     #: construct internal components.
     components: List[ComponentConfig]
     #: A mapping of outputs which the system simulation exposes and the
     #: corresponding output of an internal component.
     expose: Dict[PortID, ComponentPort]
 
+    _tasks: List[asyncio.Task] = field(default_factory=list)
+
     async def run_forever(
         self, state_consumer: Type[StateConsumer], state_producer: Type[StateProducer]
     ) -> None:
         """Sets up state interfaces, the scheduler, and components and blocks until any
         complete.
 
         An asynchronous method starts the run_forever method of each component, runs
@@ -42,35 +48,59 @@
         self.scheduler = SlaveScheduler(
             inverse_wiring,
             state_consumer,
             state_producer,
             self.expose,
             self.raise_interrupt,
         )
-        tasks = run_all(
+        self._tasks = run_all(
             component().run_forever(state_consumer, state_producer)
             for component in self.components
         ) + run_all([self.scheduler.run_forever()])
         await super().run_forever(state_consumer, state_producer)
-        await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
+        if self._tasks:
+            await asyncio.wait(self._tasks)
 
     async def on_tick(self, time: SimTime, changes: Changes) -> None:
         """Delegates core behaviour to the slave scheduler.
 
         An asynchronous method which delegates core behaviour of computing changes and
         determining a callback period to the slave shceduler and sends the resulting
         Output.
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             changes (Changes): A mapping of changed component inputs and their new
                 values.
         """
-        output_changes, call_in = await self.scheduler.on_tick(time, changes)
-        await self.output(time, output_changes, call_in)
+        on_tick = asyncio.create_task(self.scheduler.on_tick(time, changes))
+        error_state = asyncio.create_task(self.scheduler.error.wait())
+
+        done, _ = await asyncio.wait(
+            [on_tick, error_state],
+            return_when=asyncio.tasks.FIRST_COMPLETED,
+        )
+        if error_state in done:
+            await self.state_producer.produce(
+                output_topic(self.name),
+                self.scheduler.component_error,
+            )
+
+        else:
+            output_changes, call_in = on_tick.result()
+            await self.output(time, output_changes, call_in)
+
+    async def stop_component(self) -> None:
+        """Cancel all pending tasks associated with the System Simulation component.
+
+        Cancels long running adapter tasks associated with the component.
+        """
+        LOGGER.debug("Stopping {}".format(self.name))
+        for task in self._tasks:
+            task.cancel()
 
 
 @dataclass
 class SystemSimulation(ComponentConfig):
     """Simulation of a nested set of components."""
 
     name: ComponentID
```

### Comparing `tickit-0.2.0/src/tickit/core/device.py` & `tickit-0.2.1/src/tickit/core/device.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/core/management/event_router.py` & `tickit-0.2.1/src/tickit/core/management/event_router.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/core/management/schedulers/base.py` & `tickit-0.2.1/src/tickit/core/management/schedulers/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,24 @@
+import asyncio
 import logging
 from abc import abstractmethod
 from typing import Dict, Optional, Set, Tuple, Type, Union
 
 from tickit.core.management.event_router import InverseWiring, Wiring
 from tickit.core.management.ticker import Ticker
 from tickit.core.state_interfaces import StateConsumer, StateProducer
-from tickit.core.typedefs import ComponentID, Input, Interrupt, Output, SimTime
+from tickit.core.typedefs import (
+    ComponentException,
+    ComponentID,
+    Input,
+    Interrupt,
+    Output,
+    SimTime,
+    StopComponent,
+)
 from tickit.utils.topic_naming import input_topic, output_topic
 
 LOGGER = logging.getLogger(__name__)
 
 
 class BaseScheduler:
     """A base scheduler class which implements logic common to all schedulers."""
@@ -31,14 +40,16 @@
                 by the component.
         """
         self._wiring = wiring
         self._state_consumer_cls = state_consumer
         self._state_producer_cls = state_producer
         self.wakeups: Dict[ComponentID, SimTime] = dict()
 
+        self.error = asyncio.Event()
+
     @abstractmethod
     async def schedule_interrupt(self, source: ComponentID) -> None:
         """An abstract asynchronous method which should schedule an interrupt
         immediately.
 
         Args:
             source (ComponentID): The component which should be updated.
@@ -50,48 +61,56 @@
 
         Args:
             input (Input): The input to be included in the message sent to the
                 component.
         """
         await self.state_producer.produce(input_topic(input.target), input)
 
-    async def handle_message(self, message: Union[Interrupt, Output]) -> None:
-        """A callback to handle interrupts or outputs produced by the state consumer.
+    async def handle_message(
+        self, message: Union[Interrupt, Output, ComponentException]
+    ) -> None:
+        """Handle messages recieved by the state consumer.
 
-        An asynchronous callback which handles interrupt and output messages produced by
-        the state consumer; For Outputs, changes are propagated and wakeups scheduled
-        if required, whilst handling of interrupts is deferred.
+        An asynchronous callback which handles Interrupt, Output and ComponentException
+        messages recieved by the state consumer. For Outputs, changes are propagated
+        and wakeups scheduled if required. For interrupts handling is deferred. For
+        exceptions, a StopComponent message is produced to each component in the system
+        to facilitate shut down.
 
         Args:
-            message (Union[Interrupt, Output]): An Interrupt or Output produced by the
-                state consumer.
+            message (Union[Interrupt, Output, ComponentException]): An Interrupt,
+                Output or ComponentException recieved by the state consumer.
         """
-        LOGGER.debug("Scheduler got {}".format(message))
+        LOGGER.debug("Scheduler ({}) got {}".format(type(self).__name__, message))
         if isinstance(message, Output):
             await self.ticker.propagate(message)
             if message.call_at is not None:
                 self.add_wakeup(message.source, message.call_at)
-        if isinstance(message, Interrupt):
+        elif isinstance(message, Interrupt):
             await self.schedule_interrupt(message.source)
+        elif isinstance(message, ComponentException):
+            await self.handle_component_exception(message)
 
     async def setup(self) -> None:
         """Instantiates and configures the ticker and state interfaces.
 
         An asynchronous setup method which creates a ticker, a state consumer which is
         subscribed to the output topics of each component in the system, a state
         producer to produce component inputs.
         """
         self.ticker = Ticker(self._wiring, self.update_component)
         self.state_consumer: StateConsumer[
-            Union[Interrupt, Output]
+            Union[Interrupt, Output, ComponentException]
         ] = self._state_consumer_cls(self.handle_message)
         await self.state_consumer.subscribe(
             {output_topic(component) for component in self.ticker.components}
         )
-        self.state_producer: StateProducer[Input] = self._state_producer_cls()
+        self.state_producer: StateProducer[
+            Union[Input, StopComponent, ComponentException]
+        ] = self._state_producer_cls()
 
     def add_wakeup(self, component: ComponentID, when: SimTime) -> None:
         """Adds a wakeup to the mapping.
 
         Args:
             component (ComponentID): The component which should be updated.
             when (SimTime): The simulation time at which the update should occur.
@@ -115,7 +134,26 @@
         if not self.wakeups:
             return set(), None
         first = min(self.wakeups.values())
         components = {
             component for component, when in self.wakeups.items() if when == first
         }
         return components, first
+
+    async def handle_component_exception(self, message: ComponentException) -> None:
+        """Handle exceptions raised from componenets by shutting down the simulation.
+
+        If a component produces an exception, the scheduler will produce a message to
+        all components in the simulation to cause them to cancel any running component
+        tasks. After which the scheduler shuts its self down.
+
+        """
+        await asyncio.wait(
+            {
+                asyncio.create_task(
+                    self.state_producer.produce(input_topic(component), StopComponent())
+                )
+                for component in self.ticker.components
+            },
+            return_when=asyncio.tasks.ALL_COMPLETED,
+        )
+        self.error.set()
```

### Comparing `tickit-0.2.0/src/tickit/core/management/schedulers/master.py` & `tickit-0.2.1/src/tickit/core/management/schedulers/master.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import asyncio
+import logging
 from time import time_ns
 from typing import Type, Union
 
 from tickit.core.management.event_router import InverseWiring, Wiring
 from tickit.core.management.schedulers.base import BaseScheduler
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
-from tickit.core.typedefs import ComponentID, SimTime
+from tickit.core.typedefs import ComponentException, ComponentID, SimTime
+
+LOGGER = logging.getLogger(__name__)
 
 
 class MasterScheduler(BaseScheduler):
     """A master scheduler which orchestrates the running of a tickit simulation."""
 
     def __init__(
         self,
@@ -62,16 +65,17 @@
 
         An asynchronous method which initially performs setup and an initial tick in
         which all components are updated, subsequently ticks are performed as requested
         by components of the simulation according to the simulation speed.
         """
         await self.setup()
         await self._do_initial_tick()
-        while True:
+        while not self.error.is_set():
             await self._do_tick()
+        LOGGER.debug("Stopping Master Scheduler")
 
     async def _do_initial_tick(self):
         """Performs the initial tick of the system."""
         await self.ticker(
             self._initial_time,
             self.ticker.components,
         )
@@ -127,7 +131,18 @@
         Returns:
             float: The real world duration before the simulation time is reached.
         """
         return (
             (when - self.ticker.time) / self.simulation_speed
             - (time_ns() - self.last_time)
         ) / 1e9
+
+    async def handle_component_exception(self, message: ComponentException) -> None:
+        """Handle exceptions raised from componenets by shutting down the simulation.
+
+        If a component produces an exception, the scheduler will produce a message to
+        all components in the simulation to cause them to cancel any running component
+        tasks. After which the scheduler shuts its self down.
+
+        """
+        await super().handle_component_exception(message)
+        self.ticker.finished.set()
```

### Comparing `tickit-0.2.0/src/tickit/core/management/schedulers/slave.py` & `tickit-0.2.1/src/tickit/core/management/schedulers/slave.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from immutables import Map
 
 from tickit.core.management.event_router import InverseWiring, Wiring
 from tickit.core.management.schedulers.base import BaseScheduler
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
 from tickit.core.typedefs import (
     Changes,
+    ComponentException,
     ComponentID,
     ComponentPort,
     Input,
     Output,
     PortID,
     SimTime,
 )
@@ -46,14 +47,15 @@
                 the slave scheduler is updated immediately.
         """
         wiring = self.add_exposing_wiring(wiring, expose)
         super().__init__(wiring, state_consumer, state_producer)
 
         self.raise_interrupt = raise_interrupt
         self.interrupts: Set[ComponentID] = set()
+        self.component_error: ComponentException
 
     @staticmethod
     def add_exposing_wiring(
         wiring: Union[Wiring, InverseWiring],
         expose: Dict[PortID, ComponentPort],
     ) -> InverseWiring:
         """Adds wiring to expose slave scheduler outputs.
@@ -156,7 +158,20 @@
 
         Args:
             source (ComponentID): The source component of the interrupt.
         """
         LOGGER.debug("Adding {} to interrupts".format(source))
         self.interrupts.add(source)
         await self.raise_interrupt()
+
+    async def handle_component_exception(self, message: ComponentException) -> None:
+        """Handle exceptions raised from componenets by shutting down the simulation.
+
+        If a component inside a system simulation produces an exception, the slave
+        scheduler will produce a message to all components it contains to cause them
+        to cancel any running component tasks (adapter tasks). Afterwards the scheduler
+        stores the ComponentException message, allowing its associated system simulation
+        component to propogate the exception to the master scheduler.
+
+        """
+        await super().handle_component_exception(message)
+        self.component_error = message
```

### Comparing `tickit-0.2.0/src/tickit/core/management/ticker.py` & `tickit-0.2.1/src/tickit/core/management/ticker.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,26 @@
 from tickit.core.management.event_router import EventRouter, InverseWiring, Wiring
 from tickit.core.typedefs import Changes, ComponentID, Input, Output, PortID, SimTime
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Ticker:
-    """A utility class responsible for sequencing the update of components during a
-    tick.
+    """Utility class responsible for sequencing the update of components during a tick.
 
     A utility class responsible for sequencing the update of components during a tick
     by eagerly updating each component which has had all of its dependencies resolved.
     """
 
     def __init__(
         self,
         wiring: Union[Wiring, InverseWiring],
         update_component: Callable[[Input], Coroutine[Any, Any, None]],
     ) -> None:
-        """A Ticker constructor which creates an event router and performs initial
-        setup.
+        """Ticker constructor which creates an event router and performs initial setup.
 
         Args:
             wiring (Union[Wiring, InverseWiring]): A wiring or inverse wiring object
                 representing the connections between components in the system.
             update_component (Callable[[Input], Awaitable[None]]): A function or method
                 which may be called to request a component performs and update, such
                 updates should result in a subsequent call to the propagate method of
@@ -49,15 +47,15 @@
         self.update_component = update_component
         self.to_update: Dict[ComponentID, Optional[asyncio.Task]] = dict()
         self.finished: asyncio.Event = asyncio.Event()
 
     async def __call__(
         self, time: SimTime, update_components: Set[ComponentID]
     ) -> None:
-        """Performs a tick which updates the provided components and their dependants.
+        """Perform a tick which updates the provided components and their dependants.
 
         An asynchronous method which performs a tick by setting up the initial state of
         the system during the tick - including determining dependant components,
         scheduling updates which require no component resolutions to be performed,
         before blocking until the system is resolved by update propagation.
 
         Args:
@@ -68,15 +66,15 @@
         """
         await self._start_tick(time, update_components)
         await self.schedule_possible_updates()
         await self.finished.wait()
         self.finished.clear()
 
     async def _start_tick(self, time: SimTime, update_components: Set[ComponentID]):
-        """Sets up the ticker to perform a tick.
+        """Set up the ticker to perform a tick.
 
         An asynchronous method which sets up the ticker to perform a tick by updating
         time, reseting accumulators and finding the set of components which require
         update.
 
         Args:
             time (SimTime): The simulation time at which the tick occurs (in
@@ -93,15 +91,15 @@
         self.to_update = {
             c: None
             for component in self.roots
             for c in self.event_router.dependants(component)
         }
 
     async def schedule_possible_updates(self) -> None:
-        """Updates components with resolved dependencies.
+        """Update components with resolved dependencies.
 
         An asynchronous method which schedules updates for components with resolved
         dependencies, as determined by the intersection of the components first order
         dependencies and the set of componets which still require an update.
         """
 
         def required_dependencies(component) -> Set[ComponentID]:
```

### Comparing `tickit-0.2.0/src/tickit/core/runner.py` & `tickit-0.2.1/src/tickit/core/runner.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/core/state_interfaces/internal.py` & `tickit-0.2.1/src/tickit/core/state_interfaces/internal.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/core/state_interfaces/kafka.py` & `tickit-0.2.1/src/tickit/core/state_interfaces/kafka.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/core/state_interfaces/state_interface.py` & `tickit-0.2.1/src/tickit/core/state_interfaces/state_interface.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/core/typedefs.py` & `tickit-0.2.1/src/tickit/core/typedefs.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,14 +72,21 @@
     """
 
     target: ComponentID
     time: SimTime
     changes: Changes
 
 
+@dataclass(frozen=True, init=True)
+class StopComponent:
+    """An immutable dataclass to register Component shutdown."""
+
+    ...
+
+
 @dataclass(frozen=True)
 class Output:
     """An immutable data container for Component outputs.
 
     Args:
         source: The Component which produced the Output.
         time: The simulation time at which the Output was produced and is to be handled.
@@ -98,7 +105,20 @@
     """An immutable data container for scheduling Component interrupts.
 
     Args:
         component: The Component which is requesting an interrupt.
     """
 
     source: ComponentID
+
+
+@dataclass(frozen=True)
+class ComponentException:
+    """An immutable data container for raising Component exceptions.
+
+    Args:
+        component: The Component which raised an exception.
+    """
+
+    source: ComponentID
+    error: Exception
+    traceback: str
```

### Comparing `tickit-0.2.0/src/tickit/devices/femto/current.py` & `tickit-0.2.1/src/tickit/devices/sink.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-from random import uniform
+import logging
+from typing import Any
 
+from tickit.core.components.component import Component, ComponentConfig
+from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.compat.typing_compat import TypedDict
 
+LOGGER = logging.getLogger(__name__)
 
-class CurrentDevice(Device):
-    """The current configured device."""
 
-    #: A typed mapping containing the current output value
-    Outputs: TypedDict = TypedDict("Outputs", {"output": float})
+class SinkDevice(Device):
+    """A simple device which can take any input and produces no output."""
 
-    def __init__(self, callback_period: int) -> None:
-        """Initialise the current device.
+    #: A typed mapping containing the 'input' input value
+    Inputs: TypedDict = TypedDict("Inputs", {"input": Any})
+    #: An empty typed mapping of device outputs
+    Outputs: TypedDict = TypedDict("Outputs", {})
 
-        Args:
-            callback_period (Optional[int]): The duration in which the device should \
-                next be updated. Defaults to int(1e9).
-        """
-        self.callback_period = SimTime(callback_period)
-
-    def update(self, time: SimTime, inputs) -> DeviceUpdate[Outputs]:
-        """Updates the state of the current device.
+    def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
+        """The update method which logs the inputs at debug level and produces no
+        outputs.
 
         Args:
-            time (SimTime): The time of the simulation in nanoseconds.
-            inputs (State): The state of the input values of the device.
+            time (SimTime): The current simulation time (in nanoseconds).
+            inputs (State): A mapping of inputs to the device and their values.
 
         Returns:
-            DeviceUpdate: A container for the Device's outputs and a callback time.
+            DeviceUpdate[Outputs]:
+                The produced update event which never contains any changes, and never
+                requests a callback.
         """
-        output = uniform(100, 200)
-        print(
-            "Output! (delta: {}, inputs: {}, output: {})".format(time, inputs, output)
-        )
-        return DeviceUpdate(
-            self.Outputs(output=output), SimTime(time + self.callback_period)
+        LOGGER.debug("Sunk {}".format({k: v for k, v in inputs.items()}))
+        return DeviceUpdate(SinkDevice.Outputs(), None)
+
+
+class Sink(ComponentConfig):
+    """Arbitrary value sink that logs the value."""
+
+    def __call__(self) -> Component:  # noqa: D102
+        return DeviceSimulation(
+            name=self.name,
+            device=SinkDevice(),
         )
```

### Comparing `tickit-0.2.0/src/tickit/devices/sink.py` & `tickit-0.2.1/src/tickit/devices/source.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 import logging
+from dataclasses import dataclass
 from typing import Any
 
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.compat.typing_compat import TypedDict
 
 LOGGER = logging.getLogger(__name__)
 
 
-class SinkDevice(Device):
-    """A simple device which can take any input and produces no output."""
+class SourceDevice(Device):
+    """A simple device which produces a pre-configured value."""
 
-    #: A typed mapping containing the 'input' input value
-    Inputs: TypedDict = TypedDict("Inputs", {"input": Any})
-    #: An empty typed mapping of device outputs
-    Outputs: TypedDict = TypedDict("Outputs", {})
+    #: An empty typed mapping of device inputs
+    Inputs: TypedDict = TypedDict("Inputs", {})
+    #: A typed mapping containing the 'value' output value
+    Outputs: TypedDict = TypedDict("Outputs", {"value": Any})
+
+    def __init__(self, value: Any) -> None:
+        """A constructor of the source, which takes the pre-configured output value.
+
+        Args:
+            value (Any): A pre-configured output value.
+        """
+        self.value = value
 
     def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
-        """The update method which logs the inputs at debug level and produces no
-        outputs.
+        """The update method which produces the pre-configured output value.
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             inputs (State): A mapping of inputs to the device and their values.
 
         Returns:
             DeviceUpdate[Outputs]:
-                The produced update event which never contains any changes, and never
-                requests a callback.
+                The produced update event which contains the pre-configured value, and
+                never requests a callback.
         """
-        LOGGER.debug("Sunk {}".format({k: v for k, v in inputs.items()}))
-        return DeviceUpdate(SinkDevice.Outputs(), None)
+        LOGGER.debug("Sourced {}".format(self.value))
+        return DeviceUpdate(SourceDevice.Outputs(value=self.value), None)
+
 
+@dataclass
+class Source(ComponentConfig):
+    """Source of a fixed value."""
 
-class Sink(ComponentConfig):
-    """Arbitrary value sink that logs the value."""
+    value: Any
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
             name=self.name,
-            device=SinkDevice(),
+            device=SourceDevice(self.value),
         )
```

### Comparing `tickit-0.2.0/src/tickit/utils/byte_format.py` & `tickit-0.2.1/src/tickit/utils/byte_format.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/utils/configuration/configurable.py` & `tickit-0.2.1/src/tickit/utils/configuration/configurable.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit/utils/configuration/loading.py` & `tickit-0.2.1/src/tickit/utils/configuration/loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
     Args:
         config_path ([type]): The path to the config file.
 
     Returns:
         List[Component]: A list of component configuration objects.
     """
-    yaml_struct = yaml.load(open(config_path, "r"), Loader=yaml.Loader)
+    with open(config_path, "r") as config_file:
+        yaml_struct = yaml.load(config_file, Loader=yaml.Loader)
     configs = deserialize(
         List[ComponentConfig],
         yaml_struct,
         default_conversion=importing_conversion,
     )
     return configs
```

### Comparing `tickit-0.2.0/src/tickit/utils/topic_naming.py` & `tickit-0.2.1/src/tickit/utils/topic_naming.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/src/tickit.egg-info/PKG-INFO` & `tickit-0.2.1/src/tickit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Event-based device simulation framework
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,71 +224,97 @@
 An event-based multi-device simulation framework providing configuration and
 orchestration of complex multi-device simulations.
 
 ============== ==============================================================
 PyPI           ``pip install tickit``
 Source code    https://github.com/dls-controls/tickit
 Documentation  https://dls-controls.github.io/tickit
-Changelog      https://github.com/dls-controls/tickit/blob/master/CHANGELOG.rst
+Releases       https://github.com/dls-controls/tickit-devices/releases
 ============== ==============================================================
 
-An example device which emits a random value between *0* and *255* whenever
-called and asks to be called again once the simulation has progressed by the
-``callback_period``.  Additionally, extenal control of **RandomTrampoline** is
-afforded by a **RemoteControlledAdapter** which is exposed extenally through 
-a **TCPServer**:
+An example simulation consits of a simple counter and a sink. The counter
+increments up a given value and then passes this value to a sink.
+
+A simulation is defined using a yaml file, in which the graphing of the required
+components is denoted. This file defines a **Counter** device named **counter** and
+a **Sink** device named **counter_sink**. The output **_value** of **counter** is wired
+to the input of **counter_sink**.
+
+.. code-block:: yaml
+
+    - examples.devices.counter.Counter:
+        name: counter  
+        inputs: {}
+    - tickit.devices.sink.Sink:
+        name: counter_sink
+        inputs:
+          input: counter:_value
+
+
+This file is executed to run the simultation.
+
+.. code-block:: bash
+
+    python -m tickit all examples/configs/counter.yaml
+
+
+The simulation will output logs depicting the incerementing of the counter:
+
+.. code-block:: bash
+
+    DEBUG:examples.devices.counter:Counter initialized with value => 0
+    DEBUG:asyncio:Using selector: EpollSelector
+    DEBUG:tickit.core.management.ticker:Doing tick @ 0
+    DEBUG:tickit.core.components.component:counter got Input(target='counter', time=0, changes=immutables.Map({}))
+    DEBUG:examples.devices.counter:Counter incremented to 1
+    DEBUG:tickit.core.management.schedulers.base:Scheduler got Output(source='counter', time=0, changes=immutables.Map({'value': 1}), call_at=1000000000)
+    DEBUG:tickit.core.management.schedulers.base:Scheduling counter for wakeup at 1000000000
+    DEBUG:tickit.core.components.component:counter_sink got Input(target='counter_sink', time=0, changes=immutables.Map({}))
+    DEBUG:tickit.devices.sink:Sunk {}
+    DEBUG:tickit.core.management.schedulers.base:Scheduler got Output(source='counter_sink', time=0, changes=immutables.Map({}), call_at=None) 
+    DEBUG:tickit.core.management.ticker:Doing tick @ 1000000000
+    DEBUG:tickit.core.components.component:counter got Input(target='counter', time=1000000000, changes=immutables.Map({}))
+    DEBUG:examples.devices.counter:Counter incremented to 2
+    DEBUG:tickit.core.management.schedulers.base:Scheduler got Output(source='counter', time=1000000000, changes=immutables.Map({'value': 2}), call_at=2000000000)
+
+
+The counting device is defined as below. It increments a given value and logs as
+it increments.
 
 .. code-block:: python
 
     @dataclass
-    class RandomTrampoline(ComponentConfig):
+    class Counter(ComponentConfig):
+        """Simple counting device."""
 
         def __call__(self) -> Component:  # noqa: D102
             return DeviceSimulation(
                 name=self.name,
-                device=RandomTrampolineDevice(),
-                adapters=[RemoteControlledAdapter(server=TcpServer(format="%b\r\n"))])
+                device=CounterDevice(),
+                )
 
-
-    class RandomTrampolineDevice(Device):
+    class CounterDevice(Device):
+        """A simple device which increments a value."""
 
         Inputs: TypedDict = TypedDict("Inputs", {})
-        Outputs: TypedDict = TypedDict("Outputs", {"output": int})
+        Outputs: TypedDict = TypedDict("Outputs", {"value":int})
 
-        def __init__(self, callback_period: int = int(1e9)) -> None:
+        def __init__(self, initial_value: int = 0, callback_period: int = int(1e9)) -> None:
+            self._value = initial_value
             self.callback_period = SimTime(callback_period)
+            LOGGER.debug(f"Counter initialized with value => {self._value}")
 
         def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
-            output = randint(0, 255)
-            LOGGER.debug(
-                "Boing! (delta: {}, inputs: {}, output: {})".format(time, inputs, output)
-            )
+            self._value = self._value + 1
+            LOGGER.debug("Counter incremented to {}".format(self._value))
             return DeviceUpdate(
-                RandomTrampoline.Outputs(output=output),
+                CounterDevice.Outputs(value=self._value),
                 SimTime(time + self.callback_period),
             )
 
-
-An example simulation defines a **RemoteControlled** device named **tcp_contr**
-and a **Sink** device named **contr_sink**. The **observed** output of
-**tcp_contr** is wired to the **input** input of **contr_sink**:
-
-.. code-block:: yaml
-
-
-    - examples.devices.remote_controlled.RemoteControlled: {}
-        name: tcp_contr
-        inputs: {}
-    - tickit.devices.sink.Sink: {}
-        name: contr_sink
-        inputs:
-          input: tcp_contr:observed
-
-
-
 .. |code_ci| image:: https://github.com/dls-controls/tickit/workflows/Code%20CI/badge.svg?branch=master
     :target: https://github.com/dls-controls/tickit/actions?query=workflow%3A%22Code+CI%22
     :alt: Code CI
 
 .. |docs_ci| image:: https://github.com/dls-controls/tickit/workflows/Docs%20CI/badge.svg?branch=master
     :target: https://github.com/dls-controls/tickit/actions?query=workflow%3A%22Docs+CI%22
     :alt: Docs CI
```

### Comparing `tickit-0.2.0/tests/adapters/interpreters/command/test_command_interpreter.py` & `tickit-0.2.1/tests/adapters/interpreters/command/test_command_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/adapters/interpreters/command/test_regex_command.py` & `tickit-0.2.1/tests/adapters/interpreters/command/test_regex_command.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/adapters/interpreters/endpoints/test_http_endpoint.py` & `tickit-0.2.1/tests/adapters/interpreters/endpoints/test_http_endpoint.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/adapters/interpreters/test_utils.py` & `tickit-0.2.1/tests/adapters/interpreters/test_utils.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py` & `tickit-0.2.1/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/adapters/interpreters/wrappers/test_joining_interpreter.py` & `tickit-0.2.1/tests/adapters/interpreters/wrappers/test_joining_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py` & `tickit-0.2.1/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/adapters/servers/test_tcp.py` & `tickit-0.2.1/tests/adapters/servers/test_tcp.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/adapters/test_epicsadapter/test_epics_adapter.py` & `tickit-0.2.1/tests/adapters/test_epicsadapter/test_epics_adapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/adapters/test_zmqadapter.py` & `tickit-0.2.1/tests/adapters/test_zmqadapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,23 +48,25 @@
 async def test_zeromq_adapter_start_stream(zeromq_adapter: ZeroMQAdapter):
     await zeromq_adapter.start_stream()
 
     assert isinstance(zeromq_adapter._router, aiozmq.stream.ZmqStream)
     assert isinstance(zeromq_adapter._dealer, aiozmq.stream.ZmqStream)
 
     await zeromq_adapter.close_stream()
+    assert zeromq_adapter.running is False
 
 
 @pytest.mark.asyncio
 async def test_zeromq_adapter_close_stream(zeromq_adapter: ZeroMQAdapter):
     await zeromq_adapter.start_stream()
 
     await zeromq_adapter.close_stream()
     await asyncio.sleep(0.1)
 
+    assert zeromq_adapter.running is False
     assert None is zeromq_adapter._router._transport
     assert None is zeromq_adapter._dealer._transport
 
 
 @pytest.mark.asyncio
 async def test_zeromq_adapter_after_update(zeromq_adapter):
     zeromq_adapter.after_update()
@@ -89,14 +91,17 @@
 ):
     zeromq_adapter._process_message_queue = mock_process_message_queue
 
     await zeromq_adapter.run_forever(mock_device, mock_raise_interrupt)
 
     zeromq_adapter._process_message_queue.assert_called_once()
 
+    await zeromq_adapter.close_stream()
+    assert zeromq_adapter.running is False
+
 
 @pytest.mark.asyncio
 async def test_zeromq_adapter_check_if_running(zeromq_adapter):
     assert zeromq_adapter.check_if_running() is False
 
 
 @pytest.mark.asyncio
@@ -109,14 +114,16 @@
     zeromq_adapter._process_message.assert_awaited_once()
 
 
 @pytest.mark.asyncio
 async def test_zeromq_adapter_process_message(zeromq_adapter):
     mock_message = "test"
 
+    zeromq_adapter._dealer.write = Mock()
+    zeromq_adapter._router.write = Mock()
     zeromq_adapter._dealer.read.return_value = ("Data", "test")
     zeromq_adapter._router.read.return_value = ("Data", "test")
 
     await zeromq_adapter._process_message(mock_message)
 
     zeromq_adapter._dealer.read.assert_awaited_once()
     zeromq_adapter._router.read.assert_awaited_once()
@@ -129,7 +136,10 @@
     zeromq_adapter._dealer.read.return_value = ("Data", None)
     zeromq_adapter._router.read.return_value = ("Data", None)
 
     with caplog.at_level(logging.DEBUG):
         await zeromq_adapter._process_message(mock_message)
 
     assert len(caplog.records) == 1
+
+    zeromq_adapter._dealer.read.assert_not_awaited()
+    zeromq_adapter._router.read.assert_not_awaited()
```

### Comparing `tickit-0.2.0/tests/conftest.py` & `tickit-0.2.1/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,7 +52,18 @@
     tasks = asyncio.tasks.all_tasks()
     for task in tasks:
         task.cancel()
     try:
         await t
     except asyncio.CancelledError:
         pass
+
+
+@pytest.fixture
+def event_loop():
+    """Manage instance of event loop for runner test cases."""
+    try:
+        loop = asyncio.get_running_loop()
+    except RuntimeError:
+        loop = asyncio.new_event_loop()
+    yield loop
+    loop.close()
```

### Comparing `tickit-0.2.0/tests/core/components/test_component.py` & `tickit-0.2.1/tests/core/components/test_component.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/core/management/schedulers/test_base_scheduler.py` & `tickit-0.2.1/tests/core/management/schedulers/test_base_scheduler.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 from mock import Mock, create_autospec, patch
 
 from tickit.core.management.event_router import Wiring
 from tickit.core.management.schedulers.base import BaseScheduler
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
 from tickit.core.typedefs import (
     Changes,
+    ComponentException,
     ComponentID,
     Input,
     Interrupt,
     Output,
     PortID,
     SimTime,
+    StopComponent,
 )
+from tickit.utils.topic_naming import input_topic
 
 
 @pytest.fixture
 def patch_base_schedule_interrupt_method() -> Iterable[Mock]:
     with patch.object(BaseScheduler, "schedule_interrupt") as mock:
         yield mock
 
@@ -39,14 +42,15 @@
 def mock_state_producer_type() -> Mock:
     return create_autospec(StateProducer, instance=False)
 
 
 @pytest.fixture
 def patch_ticker() -> Iterable[Mock]:
     with patch("tickit.core.management.schedulers.base.Ticker", autospec=True) as mock:
+        mock.return_value.components = ["test_component"]
         yield mock
 
 
 @pytest_asyncio.fixture
 async def base_scheduler(
     mock_wiring: Mock,
     mock_state_consumer_type,
@@ -91,14 +95,28 @@
 @pytest.mark.asyncio
 async def test_base_scheduler_handle_interrupt_message(base_scheduler: BaseScheduler):
     message = Interrupt(ComponentID("foo"))
     await base_scheduler.handle_message(message)
     base_scheduler.schedule_interrupt.assert_called_once()  # type: ignore
 
 
+@pytest.mark.asyncio
+async def test_base_scheduler_handle_exception_message(base_scheduler: BaseScheduler):
+    message = ComponentException(
+        ComponentID("Test"), Exception("Test exception"), "test exception traceback"
+    )
+    await base_scheduler.handle_message(message)
+
+    base_scheduler.state_producer.produce.assert_awaited_once_with(  # type: ignore
+        input_topic(ComponentID("test_component")),
+        StopComponent(),
+    )
+    assert base_scheduler.error.is_set()
+
+
 def test_base_scheduler_get_first_wakeups_method(base_scheduler: BaseScheduler):
     expected_component = ComponentID("foo")
     expected_when = SimTime(42)
     base_scheduler.add_wakeup(expected_component, expected_when)
 
     components, when = base_scheduler.get_first_wakeups()
```

### Comparing `tickit-0.2.0/tests/core/management/schedulers/test_master_scheduler.py` & `tickit-0.2.1/tests/core/management/schedulers/test_master_scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import asyncio
 from typing import Awaitable, Iterable, Set
 
 import pytest
 import pytest_asyncio
 from mock import AsyncMock, Mock, create_autospec, patch
 
 from tickit.core.management.event_router import Wiring
 from tickit.core.management.schedulers.master import MasterScheduler
 from tickit.core.management.ticker import Ticker
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
-from tickit.core.typedefs import ComponentID, SimTime
+from tickit.core.typedefs import ComponentException, ComponentID, SimTime
 
 
 @pytest.fixture
 def mock_wiring() -> Mock:
     return create_autospec(Wiring, instance=True)
 
 
@@ -26,21 +27,26 @@
     return create_autospec(StateProducer, instance=False)
 
 
 @pytest.fixture
 def patch_ticker() -> Iterable[Mock]:
     with patch("tickit.core.management.schedulers.base.Ticker", autospec=True) as mock:
         mock.return_value = AsyncMock(spec=Ticker)
+        mock.return_value.components = ["test"]
         mock.return_value.time = SimTime(41)
+        mock.return_value.finished = asyncio.Event()
         yield mock
 
 
 @pytest_asyncio.fixture
 async def master_scheduler(
-    mock_wiring, mock_state_consumer, mock_state_producer, patch_ticker
+    mock_wiring,
+    mock_state_consumer,
+    mock_state_producer,
+    patch_ticker,
 ) -> MasterScheduler:
     master_scheduler = MasterScheduler(
         mock_wiring, mock_state_consumer, mock_state_producer
     )
     await master_scheduler.setup()
     return master_scheduler
 
@@ -177,7 +183,18 @@
     await master_scheduler._do_initial_tick()
     assert master_scheduler.wakeups == {"bar": 42}
     await master_scheduler.schedule_interrupt(ComponentID("me first"))
     assert master_scheduler.wakeups == {
         "me first": master_scheduler.ticker.time,
         "bar": 42,
     }
+
+
+@pytest.mark.asyncio
+async def test_master_scheduler_handle_exception_message(
+    master_scheduler: MasterScheduler,
+):
+    message = ComponentException(
+        ComponentID("Test"), Exception("Test exception"), "test exception traceback"
+    )
+    await master_scheduler.handle_message(message)
+    assert master_scheduler.error.is_set()
```

### Comparing `tickit-0.2.0/tests/core/management/schedulers/test_slave_scheduler.py` & `tickit-0.2.1/tests/core/management/schedulers/test_slave_scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import asyncio
 from typing import Dict, Iterable
 
 import pytest
 from immutables import Map
 from mock import AsyncMock, Mock, create_autospec, patch
 
 from tickit.core.management.event_router import InverseWiring, Wiring
 from tickit.core.management.schedulers.slave import SlaveScheduler
 from tickit.core.management.ticker import Ticker
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
 from tickit.core.typedefs import (
     Changes,
+    ComponentException,
     ComponentID,
     ComponentPort,
     Input,
     Output,
     PortID,
     SimTime,
 )
@@ -45,26 +47,33 @@
     return create_autospec(interrupt)
 
 
 @pytest.fixture
 def patch_ticker() -> Iterable[Mock]:
     with patch("tickit.core.management.schedulers.base.Ticker", autospec=True) as mock:
         mock.return_value = AsyncMock(spec=Ticker)
+        mock.return_value.components = ["test"]
         mock.return_value.time = SimTime(41)
+        mock.return_value.finished = asyncio.Event()
         yield mock
 
 
 @pytest.fixture
 def expose() -> Dict[PortID, ComponentPort]:
     return {PortID("42"): ComponentPort(ComponentID("test_component"), PortID("53"))}
 
 
 @pytest.fixture
 def slave_scheduler(
-    mock_wiring, mock_state_consumer, mock_state_producer, expose, mock_raise_interrupt
+    mock_wiring,
+    mock_state_consumer,
+    mock_state_producer,
+    expose,
+    mock_raise_interrupt,
+    patch_ticker,
 ) -> SlaveScheduler:
     return SlaveScheduler(
         mock_wiring,
         mock_state_consumer,
         mock_state_producer,
         expose,
         mock_raise_interrupt,
@@ -195,7 +204,20 @@
 @pytest.mark.asyncio
 async def test_slave_scheduler_schedule_interrupt_method(
     slave_scheduler: SlaveScheduler,
 ):
     interrupt = ComponentID("interrupt")
     await slave_scheduler.schedule_interrupt(interrupt)
     assert interrupt in slave_scheduler.interrupts
+
+
+@pytest.mark.asyncio
+async def test_slave_scheduler_handle_exception_message(
+    slave_scheduler: SlaveScheduler,
+):
+    await slave_scheduler.setup()
+    message = ComponentException(
+        ComponentID("Test"), Exception("Test exception"), "test exception traceback"
+    )
+    await slave_scheduler.handle_message(message)
+    assert slave_scheduler.error.is_set()
+    assert slave_scheduler.component_error == message
```

### Comparing `tickit-0.2.0/tests/core/management/test_event_router.py` & `tickit-0.2.1/tests/core/management/test_event_router.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/core/management/test_ticker.py` & `tickit-0.2.1/tests/core/management/test_ticker.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/core/state_interfaces/test_internal.py` & `tickit-0.2.1/tests/core/state_interfaces/test_internal.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/core/state_interfaces/test_kafka.py` & `tickit-0.2.1/tests/core/state_interfaces/test_kafka.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/core/state_interfaces/test_state_interface.py` & `tickit-0.2.1/tests/core/state_interfaces/test_state_interface.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/devices/test_sink.py` & `tickit-0.2.1/tests/devices/test_sink.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/devices/test_source.py` & `tickit-0.2.1/tests/devices/test_source.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/test_cli.py` & `tickit-0.2.1/tests/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,26 +48,27 @@
             PortID("42"),
             ComponentPort(ComponentID("foo"), PortID("24")),
         }
         mock.return_value = [mock_config]
         yield mock
 
 
-def test_cli_set_loggging_level(
+def test_cli_set_logging_level(
     patch_logging: Mock,
 ):
     runner: CliRunner = CliRunner()
     result: Result = runner.invoke(main, args=["--log-level", "INFO"])
     assert result.exit_code == 0
     patch_logging.basicConfig.assert_called_with(level="INFO")
 
 
 def test_component_command(
     patch_run_all_forever: Mock,
     patch_read_configs: Mock,
+    event_loop,
 ):
     runner: CliRunner = CliRunner()
 
     result: Result = runner.invoke(
         main, args=["component", "fake_device", "path/to/fake_device.yaml"]
     )
 
@@ -80,26 +81,28 @@
     with patch.object(MasterScheduler, "run_forever", autospec=True) as mock:
         yield mock
 
 
 def test_scheduler(
     patch_read_configs: Mock,
     patch_master_scheduler_run_forever_method: Mock,
+    event_loop,
 ):
     runner: CliRunner = CliRunner()
 
     result: Result = runner.invoke(main, args=["scheduler", "path/to/fake_device.yaml"])
 
     assert result.exit_code == 0
     patch_master_scheduler_run_forever_method.assert_awaited_once()
 
 
 def test_all(
     patch_read_configs: Mock,
     patch_master_scheduler_run_forever_method: Mock,
+    event_loop,
 ):
     runner: CliRunner = CliRunner()
 
     result: Result = runner.invoke(main, args=["all", "path/to/fake_device.yaml"])
 
     assert result.exit_code == 0
     patch_master_scheduler_run_forever_method.assert_awaited_once()
```

### Comparing `tickit-0.2.0/tests/utils/configuration/test_loading.py` & `tickit-0.2.1/tests/utils/configuration/test_loading.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/utils/test_byte_format.py` & `tickit-0.2.1/tests/utils/test_byte_format.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/utils/test_configurable.py` & `tickit-0.2.1/tests/utils/test_configurable.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.0/tests/utils/test_singleton.py` & `tickit-0.2.1/tests/utils/test_singleton.py`

 * *Files identical despite different names*

