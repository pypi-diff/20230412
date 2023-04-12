# Comparing `tmp/adaux-2.2.0.tar.gz` & `tmp/adaux-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaux-2.2.0.tar", last modified: Tue Apr 11 12:41:58 2023, max compression
+gzip compressed data, was "adaux-2.3.0.tar", last modified: Wed Apr 12 21:34:40 2023, max compression
```

## Comparing `adaux-2.2.0.tar` & `adaux-2.3.0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.881155 adaux-2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-10 20:31:51.000000 adaux-2.2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-11 12:41:58.881155 adaux-2.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-04-11 12:41:58.881155 adaux-2.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.713149 adaux-2.2.0/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.805153 adaux-2.2.0/source/adaux/
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-11 12:31:50.000000 adaux-2.2.0/source/adaux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_base_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    13574 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14120 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_cli_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.833154 adaux-2.2.0/source/adaux/_components/
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_00_extra_level.py
--rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_01_file_io_support.py
--rw-rw-rw-   0 root         (0) root         (0)     4867 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_02_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_03_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_04_monotonic_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6617 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_05_project.py
--rw-rw-rw-   0 root         (0) root         (0)     4979 2023-04-10 21:56:59.000000 adaux-2.2.0/source/adaux/_components/_06_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_07_package.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_08_pip.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_09_gitignore.py
--rw-rw-rw-   0 root         (0) root         (0)     4087 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_10_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     5765 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_11_precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     5277 2023-04-11 12:28:10.000000 adaux-2.2.0/source/adaux/_components/_12_pylint.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_13_executable.py
--rw-rw-rw-   0 root         (0) root         (0)     2257 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_14_mypy.py
--rw-rw-rw-   0 root         (0) root         (0)     2413 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_15_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_16_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_17_docs.py
--rw-rw-rw-   0 root         (0) root         (0)    15797 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_18_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    15575 2023-04-11 12:28:10.000000 adaux-2.2.0/source/adaux/_components/_19_docker.py
--rw-rw-rw-   0 root         (0) root         (0)    10820 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_20_ci.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_98_sentinel.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_99_all.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12817 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_aux_ci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.841154 adaux-2.2.0/source/adaux/_components/_payload/
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-04-11 12:28:10.000000 adaux-2.2.0/source/adaux/_components/_payload/_docker_build.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)    15703 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_docker_executors.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-11 12:28:10.000000 adaux-2.2.0/source/adaux/_components/_payload/_docker_run.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_python.py
--rw-rw-rw-   0 root         (0) root         (0)     1358 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_components/_payload/_with_dependency.py
--rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-10 20:31:51.000000 adaux-2.2.0/source/adaux/_create_badge.py
--rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-11 12:31:50.000000 adaux-2.2.0/source/adaux/_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7082 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_proto_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_tick.py
--rw-rw-rw-   0 root         (0) root         (0)     3388 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_todo.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_util.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.841154 adaux-2.2.0/source/adaux/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.845154 adaux-2.2.0/source/adaux/src/CI/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/CI/00-main.yml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/CI/01-rules.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.845154 adaux-2.2.0/source/adaux/src/CI/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/CI/jinja-snippets/coverage.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/CI/jinja-snippets/tags.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.845154 adaux-2.2.0/source/adaux/src/docker/
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/comp-helper.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.749151 adaux-2.2.0/source/adaux/src/docker/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.845154 adaux-2.2.0/source/adaux/src/docker/services/ansible-deploy/
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.849154 adaux-2.2.0/source/adaux/src/docker/services/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.849154 adaux-2.2.0/source/adaux/src/docker/services/gitlab-release-run/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.849154 adaux-2.2.0/source/adaux/src/docker/services/image/
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/image/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.853155 adaux-2.2.0/source/adaux/src/docker/services/image-pytest/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.861155 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.861155 adaux-2.2.0/source/adaux/src/docker/services/pkg-gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.861155 adaux-2.2.0/source/adaux/src/docker/services/pkg-pypi/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.861155 adaux-2.2.0/source/adaux/src/docker/services/pre-commit/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.861155 adaux-2.2.0/source/adaux/src/docker/services/pycov/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.865155 adaux-2.2.0/source/adaux/src/docker/services/pytest/
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.865155 adaux-2.2.0/source/adaux/src/docker/services/pytest-standalone/
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.869155 adaux-2.2.0/source/adaux/src/docker/services/python-deps/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.869155 adaux-2.2.0/source/adaux/src/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/default_conf.py.jinja2
--rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/postprocess_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.869155 adaux-2.2.0/source/adaux/src/docs/static/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/static/git-link-color.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.873155 adaux-2.2.0/source/adaux/src/docs/user/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/user/conf.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/user/gitignore
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/docs/user/index.rst.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/gitignore
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/install-dev.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.873155 adaux-2.2.0/source/adaux/src/license/
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/license/Apache-2.0.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/license/BSD-3_clause.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/license/MIT.txt.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.757151 adaux-2.2.0/source/adaux/src/payload/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.873155 adaux-2.2.0/source/adaux/src/payload/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.873155 adaux-2.2.0/source/adaux/src/payload/python/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2601 2023-04-11 12:40:54.000000 adaux-2.2.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
--rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/payload/python/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.877155 adaux-2.2.0/source/adaux/src/pip/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/pip/pip.conf.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.877155 adaux-2.2.0/source/adaux/src/pre-commit/
--rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/pre-commit/config.yaml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/pre-commit/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.881155 adaux-2.2.0/source/adaux/src/root/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/root/_setup.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/root/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/root/setup.cfg.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.881155 adaux-2.2.0/source/adaux/src/root/source/
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/root/source/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-10 20:31:52.000000 adaux-2.2.0/source/adaux/src/temp-combination
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:41:58.813153 adaux-2.2.0/source/adaux.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5236 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:40:53.000000 adaux-2.2.0/source/adaux.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-11 12:41:58.000000 adaux-2.2.0/source/adaux.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.981871 adaux-2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-10 20:31:51.000000 adaux-2.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-12 21:34:40.981871 adaux-2.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-12 21:34:40.985871 adaux-2.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.797864 adaux-2.3.0/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.857867 adaux-2.3.0/source/adaux/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-12 15:47:50.000000 adaux-2.3.0/source/adaux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_base_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14762 2023-04-12 21:29:55.000000 adaux-2.3.0/source/adaux/_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14469 2023-04-12 21:20:17.000000 adaux-2.3.0/source/adaux/_cli_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.909868 adaux-2.3.0/source/adaux/_components/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_00_extra_level.py
+-rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_01_file_io_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_02_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_03_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_04_monotonic_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6665 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_05_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_06_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_07_package.py
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_08_pip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_09_gitignore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_10_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5813 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_11_precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6494 2023-04-12 21:27:08.000000 adaux-2.3.0/source/adaux/_components/_12_pylint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_13_executable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_14_mypy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_15_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_16_coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_17_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)    19733 2023-04-12 21:20:17.000000 adaux-2.3.0/source/adaux/_components/_18_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    15938 2023-04-12 20:52:41.000000 adaux-2.3.0/source/adaux/_components/_19_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11985 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_20_ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_98_sentinel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_99_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12836 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_aux_ci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.917869 adaux-2.3.0/source/adaux/_components/_payload/
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-04-12 15:47:50.000000 adaux-2.3.0/source/adaux/_components/_payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-04-11 12:28:10.000000 adaux-2.3.0/source/adaux/_components/_payload/_docker_build.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)    15703 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_docker_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-11 12:28:10.000000 adaux-2.3.0/source/adaux/_components/_payload/_docker_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_with_dependency.py
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_create_badge.py
+-rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-11 12:31:50.000000 adaux-2.3.0/source/adaux/_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     7090 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_proto_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_tick.py
+-rw-rw-rw-   0 root         (0) root         (0)     3388 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_todo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.921869 adaux-2.3.0/source/adaux/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.921869 adaux-2.3.0/source/adaux/src/CI/
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/CI/00-main.yml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/CI/01-rules.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.921869 adaux-2.3.0/source/adaux/src/CI/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/CI/jinja-snippets/coverage.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/CI/jinja-snippets/tags.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.925869 adaux-2.3.0/source/adaux/src/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/comp-helper.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.805865 adaux-2.3.0/source/adaux/src/docker/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.925869 adaux-2.3.0/source/adaux/src/docker/services/ansible-deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.929869 adaux-2.3.0/source/adaux/src/docker/services/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.933869 adaux-2.3.0/source/adaux/src/docker/services/gitlab-release-run/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.937869 adaux-2.3.0/source/adaux/src/docker/services/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/image/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.941870 adaux-2.3.0/source/adaux/src/docker/services/image-pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.957870 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.957870 adaux-2.3.0/source/adaux/src/docker/services/pkg-gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.957870 adaux-2.3.0/source/adaux/src/docker/services/pkg-pypi/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.961870 adaux-2.3.0/source/adaux/src/docker/services/pre-commit/
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.961870 adaux-2.3.0/source/adaux/src/docker/services/pycov/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.965870 adaux-2.3.0/source/adaux/src/docker/services/pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.965870 adaux-2.3.0/source/adaux/src/docker/services/pytest-standalone/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.969870 adaux-2.3.0/source/adaux/src/docker/services/python-deps/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.969870 adaux-2.3.0/source/adaux/src/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/default_conf.py.jinja2
+-rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/postprocess_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.969870 adaux-2.3.0/source/adaux/src/docs/static/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/static/git-link-color.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.973871 adaux-2.3.0/source/adaux/src/docs/user/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/user/conf.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/user/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/user/index.rst.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-12 15:47:50.000000 adaux-2.3.0/source/adaux/src/gitignore
+-rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/install-dev.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.973871 adaux-2.3.0/source/adaux/src/license/
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/license/Apache-2.0.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/license/BSD-3_clause.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/license/MIT.txt.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.809865 adaux-2.3.0/source/adaux/src/payload/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.977871 adaux-2.3.0/source/adaux/src/payload/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.977871 adaux-2.3.0/source/adaux/src/payload/python/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2601 2023-04-12 21:33:51.000000 adaux-2.3.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/payload/python/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.977871 adaux-2.3.0/source/adaux/src/pip/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/pip/pip.conf.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.981871 adaux-2.3.0/source/adaux/src/pre-commit/
+-rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/pre-commit/config.yaml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/pre-commit/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.981871 adaux-2.3.0/source/adaux/src/root/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/root/_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/root/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/root/setup.cfg.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.981871 adaux-2.3.0/source/adaux/src/root/source/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/root/source/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/temp-combination
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.869867 adaux-2.3.0/source/adaux.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5236 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 21:33:50.000000 adaux-2.3.0/source/adaux.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/top_level.txt
```

### Comparing `adaux-2.2.0/LICENSE.txt` & `adaux-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/setup.cfg` & `adaux-2.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 	pytest-cov~=4.0
 
 [tool:pytest]
 markers = 
 	merge_only: run test only on merge request
 	local: run local tests that need docker
 addopts = --strict-markers -m "not merge_only and not local"
-cache_dir = /Users/mskoenz/programming/hobby/administratum/auxilium/devops/cache/pytest
+cache_dir = devops/cache/pytest
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `adaux-2.2.0/source/adaux/_base_parser.py` & `adaux-2.3.0/source/adaux/_base_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_cli.py` & `adaux-2.3.0/source/adaux/_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -366,27 +366,82 @@
 
 @adaux.command()
 @click.pass_context
 @click.argument("payload_names", nargs=-1)
 @click.option(
     "-f", "--force", is_flag=True, default=False, help="runs payload even if up to date"
 )
-@click.option("-d", "--dry", is_flag=True, default=False)
-def run(
-    ctx: click.Context, payload_names: tp.Tuple[str, ...], force: bool, dry: bool
+@click.option(
+    "-d",
+    "--dry",
+    is_flag=True,
+    default=False,
+    help="show what payloads would run, without running them",
+)
+@click.option(
+    "-l", "--show-all", is_flag=True, default=False, help="show all available payloads"
+)
+@click.option(
+    "-p",
+    "--plantuml",
+    is_flag=True,
+    default=False,
+    help="generate a png with the dependency graph",
+)
+def run(  # pylint: disable=too-many-arguments
+    ctx: click.Context,
+    payload_names: tp.Tuple[str, ...],
+    force: bool,
+    dry: bool,
+    show_all: bool,
 ) -> None:
     """
-    Run a specified payload. Use 'ls' to list all available payloads.
+    Run a specified payload.
     """
     with convert_runtime_to_click_error():
+        if show_all:
+            if payload_names or force or dry:
+                raise RuntimeError(
+                    "-l needs to be used without other arguments/options"
+                )
+            payload_names = ("$ls",)
+
         ctx.obj.run(*payload_names, force=force, dry=dry)
 
 
 @adaux.command()
 @click.pass_context
+@click.option(
+    "-v",
+    "--with-detail",
+    is_flag=True,
+    default=False,
+    help="add the parameters to the graph plot",
+)
+@click.option(
+    "-d",
+    "--with-dependency",
+    is_flag=True,
+    default=False,
+    help="add the dependency payloads to the graph plot",
+)
+def graph(  # pylint: disable=too-many-arguments
+    ctx: click.Context,
+    with_detail: bool,
+    with_dependency: bool,
+) -> None:
+    """
+    Plot the payload dependency graph.
+    Requires plantuml to be installed as CLI.
+    """
+    ctx.obj.graph(with_detail, with_dependency)
+
+
+@adaux.command()
+@click.pass_context
 @click.option("-h", "--open-html", is_flag=True, default=False)
 def docs(ctx: click.Context, open_html: bool) -> None:
     """
     Creates the docs.
     """
     with convert_runtime_to_click_error():
         ctx.obj.docs(open_html)
```

### Comparing `adaux-2.2.0/source/adaux/_cli_mixin.py` & `adaux-2.3.0/source/adaux/_cli_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                 slug=proj.slug,
                 minimal_version=proj.minimal_version,
                 author=proj.author,
             )
 
         with self.extra(ExtraLevel.FORMATTED) as aux, clean.extra(
             ExtraLevel.TEMPLATED
-        ), full.extra(ExtraLevel.TEMPLATED):
+        ), full.extra(ExtraLevel.TEMPLATED_WITH_NEGATIVE):
             self.update_to_template(clean.auxf, full.auxf)
             self.save_auxcon(aux)
 
     def bake(self: "CliMixin") -> None:
         if not self.auxcon_file.exists():
             raise RuntimeError(f"{self.auxcon_file} does not exists! use 'aux init'")
         super().bake()
@@ -224,15 +224,15 @@
 
     def run(
         self: "CliMixin", *payload_names: str, force: bool = False, dry: bool = False
     ) -> None:
         self._raise_if_disabled("payload")
         with self.extra(ExtraLevel.HYDRATED), self.cwd_to_root():
             data = self.auxh.payload
-            if payload_names == ("ls",):
+            if payload_names == ("$ls",):
                 for title, flavor in [
                     ("payloads", "docker_build"),
                     ("with deps", "with_dependency"),
                 ]:
                     list_ = list(data.lookup.level(flavor).values())
                     if not list_:
                         continue
@@ -249,14 +249,21 @@
                 raise RuntimeError(
                     f"payload '{payload_names}' not found! Use aux run ls, or check the {self.auxcon_file.name} file."
                 ) from err
             success = self.payload_run(*payloads, force=force, dry=dry)  # type: ignore
             if not success:
                 sys.exit(1)
 
+    def graph(
+        self: "CliMixin", with_detail: bool = True, with_dependency: bool = True
+    ) -> None:
+        self._raise_if_disabled("payload")
+        with self.extra(ExtraLevel.HYDRATED), self.cwd_to_root():
+            self.plot_dependency_graph(with_detail=with_detail, with_dependency=with_dependency)  # type: ignore
+
     def docs(self: "CliMixin", open_html: bool = False) -> None:
         self._raise_if_disabled("docs")
 
         docs_cache = self.target / "cache" / "docs"
 
         with self.extra() as aux:
             # pylint: disable=no-member
```

### Comparing `adaux-2.2.0/source/adaux/_components/_01_file_io_support.py` & `adaux-2.3.0/source/adaux/_components/_01_file_io_support.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_02_base.py` & `adaux-2.3.0/source/adaux/_components/_02_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         # pylint: disable=attribute-defined-outside-init
         self.auxf = _ProtoNamespace()
 
     def defaulted(self) -> None:
         # pylint: disable=attribute-defined-outside-init
         self.auxd = copy.deepcopy(self.auxf)
 
-    def templated(self) -> None:
+    def templated(self, negative_default: bool = False) -> None:
         # uses auxcon directly
         pass
 
     def demodata(self) -> None:
         # uses auxcon directly
         pass
 
@@ -133,15 +133,18 @@
         scat, parent, data = self._drill_down(cats, source)
         if scat is None:
             return
         parent[scat] = data = _ProtoNamespace(data or {})
 
         if iter_mapping:
             for key in data:
-                self._to_proto_ns(key, source=data)
+                if isinstance(data.get(key, None), tp.Mapping):
+                    self._to_proto_ns(key, source=data, iter_mapping=True)
+                elif data[key] is None:
+                    data[key] = _ProtoNamespace()
 
     def _drill_down(
         self, cats: tp.Tuple[str, ...], data: _ProtoNamespace
     ) -> tp.Tuple[tp.Optional[str], _ProtoNamespace, _ProtoNamespace]:
         cat = None
         for cat in cats:
             parent = data
```

### Comparing `adaux-2.2.0/source/adaux/_components/_03_meta.py` & `adaux-2.3.0/source/adaux/_components/_03_meta.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_04_monotonic_version.py` & `adaux-2.3.0/source/adaux/_components/_04_monotonic_version.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_05_project.py` & `adaux-2.3.0/source/adaux/_components/_05_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from .._parser import ConfigParser
 from .._parser import Jinja2Parser
 from .._proto_namespace import _ProtoNamespace
 from ._02_base import BaseComponent
 
 
 class ProjectMixin(BaseComponent):
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
         data = self.auxcon.setdefault("project", _ProtoNamespace())
         data.creation_year = self.get_current_year()
 
     def demodata(self) -> None:
         super().demodata()
         data = self.auxcon.project
         data.name = "hallo.world"
```

### Comparing `adaux-2.2.0/source/adaux/_components/_06_dependency.py` & `adaux-2.3.0/source/adaux/_components/_06_dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from .._proto_namespace import _ProtoNamespace
 from ._03_meta import MetaMixin
 from ._05_project import ProjectMixin
 
 
 class DependencyMixin(ProjectMixin, MetaMixin):
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
         data = self.auxcon.dependencies = _ProtoNamespace()
         data.default = []
         data.test = []
         data.dev = []
         data.dev_apt = []
 
     def demodata(self) -> None:
@@ -77,15 +77,15 @@
     def enriched(self) -> None:
         super().enriched()
         data = self.auxe.dependencies
         for key in data:
             if not key.endswith("_apt"):
                 continue
             res = _ProtoNamespace()
-            for pkg_or_map in data[key]:
+            for pkg_or_map in data[key] or []:
                 if isinstance(pkg_or_map, str):
                     res.setdefault("all", [])
                     res.all.append(pkg_or_map)
                 elif isinstance(pkg_or_map, tp.Mapping):
                     assert len(pkg_or_map) == 1
                     arch, arch_pkgs = next(iter(pkg_or_map.items()))
                     if isinstance(arch_pkgs, str):
```

### Comparing `adaux-2.2.0/source/adaux/_components/_07_package.py` & `adaux-2.3.0/source/adaux/_components/_07_package.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_08_pip.py` & `adaux-2.3.0/source/adaux/_components/_08_pip.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_09_gitignore.py` & `adaux-2.3.0/source/adaux/_components/_09_gitignore.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_10_gitlab.py` & `adaux-2.3.0/source/adaux/_components/_10_gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from .._proto_namespace import _ProtoNamespace
 from ._03_meta import MetaMixin
 from ._05_project import ProjectMixin
 
 
 class GitlabMixin(ProjectMixin, MetaMixin):
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
         self.auxcon.gitlab = _ProtoNamespace(
             vip_branches=_ProtoNamespace(
                 develop=_ProtoNamespace(push_access_level=40, allow_force_push=True),
                 release=_ProtoNamespace(),
             )
         )
 
@@ -61,15 +61,15 @@
             defaults = {}
             defaults["remote_url"], rest = url.split(":", 1)
             defaults["remote_user"], rest = rest.split("/", 1)
             defaults["remote_name"] = rest.replace(".git", "")
             key = "remote_url"
             for key, val in defaults.items():
                 if key not in data:
-                    if key == "remote_name" and val == self.auxd.project.name:
+                    if key == "remote_name" and val == self.auxf.project.name:
                         continue
                     data[key] = val
                     self._print(f"gitlab.{key}: added {data[key]}", fg="green")
 
     def enriched(self) -> None:
         super().enriched()
         data = self.auxe.gitlab
```

### Comparing `adaux-2.2.0/source/adaux/_components/_11_precommit.py` & `adaux-2.3.0/source/adaux/_components/_11_precommit.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 class PrecommitMixin(DependencyMixin, ProjectMixin, MetaMixin):
     @classmethod
     def __keys(cls) -> tp.Tuple[str, ...]:
         return ("hooks", "rev_overwrite")
 
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
 
         data = self.auxcon.dependencies
         data.dev.append(self.versions.pre_commit)
         data.dev_apt.append("git-core")
 
         data = self.auxcon.pre_commit = _ProtoNamespace(hooks=_ProtoNamespace())
         data.hooks["check-yaml"] = _ProtoNamespace(exclude="devops/CI")
```

### Comparing `adaux-2.2.0/source/adaux/_components/_12_pylint.py` & `adaux-2.3.0/source/adaux/_components/_12_pylint.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,32 +24,62 @@
             "argument_rgx",
             "attr_rgx",
             "function_rgx",
             "variable_rgx",
             "method_rgx",
         )
 
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
         data = self.auxcon.pylint = _ProtoNamespace()
         self.auxcon.dependencies.dev.append(self.versions.pylint)
         data.disable = [
-            "use-dict-literal",
-            "too-few-public-methods",
             "line-too-long",
-            "wrong-import-position",
             "wildcard-import",
+            "use-dict-literal",
+            "wrong-import-position",
+            "too-few-public-methods",
         ]
-        if not self.is_enabled("docs"):
+        if not self.is_enabled("docs") or negative_default:
             data.disable += [
                 "missing-class-docstring",
                 "missing-module-docstring",
                 "missing-function-docstring",
             ]
 
+    def update_to_template(self, tpl: _ProtoNamespace, full: _ProtoNamespace) -> None:
+        super().update_to_template(tpl, full)
+        data = self.auxf.pylint
+        data_full = full.pylint
+        data_tpl = tpl.pylint
+        # will be left alone once defined, not removed
+        hysteresis = [
+            "missing-class-docstring",
+            "missing-module-docstring",
+            "missing-function-docstring",
+        ]
+
+        old_disable = data.disable
+        order = data_tpl.disable + old_disable + hysteresis
+
+        def ordered(list_: tp.Iterable[str]) -> tp.List[str]:
+            return list(sorted(list_, key=order.index))
+
+        should_be_present = set(data_tpl.disable)
+        custom = set(old_disable) - (set(data_full.disable) - set(hysteresis))
+
+        data.disable = ordered(should_be_present | custom)
+
+        added = set(data.disable) - set(old_disable)
+        removed = set(old_disable) - set(data.disable)
+        if added:
+            self._print(f"pylint.disable: added {ordered(added)}", fg="green")
+        if removed:
+            self._print(f"pylint.disable: removed {ordered(removed)}", fg="red")
+
     def demodata(self) -> None:
         super().demodata()
         data = self.auxcon.pylint
         data.setdefault("disable", [])
         data.disable += ["too-few-public-methods", "no-self-use"]
         data.good_names = ["t", "dt"]
```

### Comparing `adaux-2.2.0/source/adaux/_components/_13_executable.py` & `adaux-2.3.0/source/adaux/_components/_13_executable.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_14_mypy.py` & `adaux-2.3.0/source/adaux/_components/_14_mypy.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 
 class MypyMixin(DependencyMixin):
     @classmethod
     def __keys(cls) -> tp.Tuple[str, ...]:
         return ("ignore",)
 
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
         self.auxcon.dependencies.dev.append(self.versions.mypy)
 
     def demodata(self) -> None:
         super().demodata()
         self.auxcon.mypy = _ProtoNamespace(ignore=["click_help_colors"])
 
     def formatted(self) -> None:
```

### Comparing `adaux-2.2.0/source/adaux/_components/_15_pytest.py` & `adaux-2.3.0/source/adaux/_components/_15_pytest.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 
 class PytestMixin(DependencyMixin):
     @classmethod
     def __keys(cls) -> tp.Tuple[str, ...]:
         return ("asyncio_mode", "markers", "addopts", "cache_dir")
 
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
         data = self.auxcon.pytest = _ProtoNamespace()
         self.auxcon.dependencies.test.append(self.versions.pytest)
         data.markers = _ProtoNamespace({"merge_only": "run test only on merge request"})
         data.addopts = '--strict-markers -m "not merge_only"'
 
     def demodata(self) -> None:
         super().demodata()
```

### Comparing `adaux-2.2.0/source/adaux/_components/_17_docs.py` & `adaux-2.3.0/source/adaux/_components/_17_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 
 class DocsMixin(ProjectMixin):
     @classmethod
     def __keys(cls) -> tp.Tuple[str, ...]:
         return ("strict", "framework", "root")
 
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
         self.auxcon.dependencies.docs = [
             self.versions.sphinx,
             self.versions.sphinx_rtd_theme,
             self.versions.sphinx_click,
             self.versions.jupyter_sphinx,
             self.versions.bash_kernel,
         ]
```

### Comparing `adaux-2.2.0/source/adaux/_components/_18_payload.py` & `adaux-2.3.0/source/adaux/_components/_18_payload.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .._yaml import yaml  # type: ignore
 from ._05_project import ProjectMixin
 from ._payload import DockerBuildPayload
 from ._payload import DockerComposePayload
 from ._payload import DockerRunPayload
 from ._payload import Payload
 from ._payload import PythonPayload
+from ._payload import subprocess_run
 from ._payload import WithDependencyPayload
 
 
 class PayloadMixin(ProjectMixin):
     @classmethod
     def __keys(cls) -> tp.Tuple[str, ...]:
         return ("docker_settings",) + tuple(cls.payload_types())
@@ -39,26 +40,25 @@
         res = {}
         for flavor, val in cls.payload_types().items():
             res[flavor] = 0
             if val == WithDependencyPayload:
                 res[flavor] = 1
         return res
 
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
         self.auxcon.payload = _ProtoNamespace()
 
     def formatted(self) -> None:
         super().formatted()
         self._copy_keys_over(self.__keys(), "payload")
         for key in self.__keys():
             if key in ["docker_settings"]:
                 continue  # handled by docker
             self._to_proto_ns("payload", key, iter_mapping=True)
-
         try:
             for val in self.auxf.payload.with_dependency.values():
                 try:
                     if isinstance(val.deps, str):
                         val.deps = [val.deps]
                 except KeyError:
                     pass
@@ -84,16 +84,16 @@
 
             val.deps = val.deps or []
             val.setdefault("payload", payload_name)
 
     def enriched(self) -> None:
         super().enriched()
         data = self.auxe.payload
-
-        self._add_absend_and_expand_variants(data)
+        data.variant_separator = "-"
+        self._add_absent_and_expand_variants(data)
 
         # helper parameter
         for flavor in self.payload_types():
             for payload_name, payload in data[flavor].items():
                 payload.name = payload_name
                 payload.flavor = flavor
 
@@ -113,15 +113,15 @@
                     payload_cfg = lookup_cfg[(val.payload, val.name, 1)]
                     val.payload = f"{payload_cfg.flavor}:{payload_cfg.name}"
             except KeyError as err:
                 raise RuntimeError(
                     f"did not find matching payload for '{val.name}'. Ensure it exists or use the payload argument."
                 ) from err
 
-    def _add_absend_and_expand_variants(self, data: _ProtoNamespace) -> None:
+    def _add_absent_and_expand_variants(self, data: _ProtoNamespace) -> None:
         # resolve variants
         for flavor in self.payload_types():
             # we should only _add_if_absent after the lower levels
             # had a change to expand their variants
             if flavor == "with_dependency":
                 for payload_name, val in data.with_dependency.items():
                     param = val.get("param", _ProtoNamespace())
@@ -155,50 +155,53 @@
             val = _ProtoNamespace(param=copy.deepcopy(param))
             if after:
                 data[flavor].insert_after(after, payload_name, val)
             else:
                 data[flavor][payload_name] = val
             logger.info("added %s:%s automatically", flavor, payload_name)
 
-    def _expand_variant(  # pylint: disable=too-many-arguments
+    def _expand_variant(  # pylint: disable=too-many-arguments,too-many-locals
         self,
         flavor: str,
         base_service_name: str,
         base_val: _ProtoNamespace,
         interfix: str = "",
         prefix_opts: tp.Optional[_ProtoNamespace] = None,
     ) -> None:
         data = self.auxe.payload
+        sepa = data.variant_separator
         base_variants = base_val.pop("variant", _ProtoNamespace())
+        base_variants_wd = base_val.pop("variant-with-deps", _ProtoNamespace())
+        base_variants.update(base_variants_wd)
 
         # sanatize base_variants
         base_variants = _ProtoNamespace(
-            (interfix + key, val or _ProtoNamespace())
+            (interfix + (sepa if interfix else "") + key, val or _ProtoNamespace())
             for key, val in base_variants.items()
         )
 
         if not prefix_opts:
             # prefix opts allows us to reuse the settings of a
             # variant later again, i.e.
             # variant:
-            #     -mr:
+            #     mr:
             #         bla: 1
-            #     -39:
+            #     "39":
             #         version: "3.9"
             #         variant:
-            #             -mr:
+            #             mr:
             #             # has automatically bla: 1
             prefix_opts = _ProtoNamespace(
                 {interfix: base_val.get("param", _ProtoNamespace())}
             )
 
         # prepare the param object for the variants
         for fvariant, mod in base_variants.items():
             if interfix:
-                variant = fvariant.split(interfix, 1)[1]
+                variant = fvariant.split(interfix + sepa, 1)[1]
             else:
                 variant = fvariant
             prefix_opts[fvariant] = copy.deepcopy(prefix_opts[interfix])
             if variant in prefix_opts and interfix != "":
                 prefix_opts[fvariant].update(prefix_opts[variant])
                 logger.info(
                     "%s -> applied %s %s variant options to %s variant",
@@ -207,14 +210,18 @@
                     prefix_opts[variant],
                     fvariant,
                 )
             prefix_opts[fvariant].update(mod)
 
         # create the variants
         for fvariant, mod in reversed(base_variants.items()):
+            if interfix:
+                variant = fvariant.split(interfix + sepa, 1)[1]
+            else:
+                variant = fvariant
             # do subvariants first
             subvariants = mod.pop("variant", _ProtoNamespace())
             base_val_mod = copy.deepcopy(base_val)
             base_val_mod.param = copy.deepcopy(prefix_opts[fvariant])
             base_val_mod.variant = subvariants
             self._expand_variant(
                 flavor,
@@ -230,24 +237,51 @@
             val.param = prefix_opts[fvariant]
             val.param.pop("variant", None)
 
             if flavor == "with_dependency":
                 param = val.param
                 param.setdefault("docker_name", base_val.payload)
                 param.image_name = self.auxe.project.slug + "-" + base_val.payload
-                val.payload += fvariant
+                suffix = sepa + fvariant
+                self._with_build_dependency(
+                    variant, suffix, base_variants_wd, param, val
+                )
+                val.payload += suffix  # needs to happen after _with_build_dependency
                 self._add_if_absent(val.payload, param, data, base_service_name)
             if flavor == "python":
                 val.setdefault("fct", base_service_name)
 
             # finally add it
             data[flavor].insert_after(
-                base_service_name, base_service_name + fvariant, val
+                base_service_name, base_service_name + sepa + fvariant, val
             )
 
+    def _with_build_dependency(  # pylint: disable=too-many-arguments
+        self,
+        variant: str,
+        suffix: str,
+        base_variants_wd: _ProtoNamespace,
+        param: _ProtoNamespace,
+        val: _ProtoNamespace,
+    ) -> None:
+        # the wb variant also makes a variant on the build dependency
+        data = self.auxe.payload
+        if variant in base_variants_wd:
+            param.image_name += suffix
+            for idx, dep in enumerate(val.deps):
+                if dep == "build-" + val.payload:
+                    ndep = val.deps[idx] = dep + suffix
+                    self._add_if_absent(ndep, param, data, dep)
+                else:
+                    logger.info(
+                        "not creating dep variant %s for %s",
+                        ndep,
+                        val.payload + suffix,
+                    )
+
     def hydrated(self) -> None:
         super().hydrated()
         # hydration
         lookup: DoubleDict[Payload] = DoubleDict(self.level_map())
         type_sel = self.payload_types()
         data = self.auxh.payload
         custom_ppyload = self._load_custom_ppyload()
@@ -347,15 +381,15 @@
             return jobs  # type: ignore
 
         demo(*payloads)
 
         if dry:
             jman.prune_unincluded(show=True)
         else:
-            jman.run_pipeline()
+            jman.run_pipeline(show=True)
             jman.show_result()
 
         if jman.has_failed_jobs():
             return False
         return True
 
     def _load_custom_ppyload(self) -> tp.Optional[types.ModuleType]:
@@ -364,14 +398,69 @@
                 custom_ppyload = importlib.import_module("payload.python.functions")
                 logger.info("custom python payloads found")
         except (ImportError, FileNotFoundError):
             custom_ppyload = None
             logger.info("custom python payloads NOT found")
         return custom_ppyload
 
+    def plot_dependency_graph(  # pylint: disable=too-many-locals
+        self, with_detail: bool = True, with_dependency: bool = False
+    ) -> None:
+        lines = ["@startuml"]
+        # lines += ["scale max 1024 width"]
+        data = self.auxh.payload.lookup
+        flv_tag_lookup = dict(
+            python="<< (P,#FFDC52) >>",
+            docker_build="<< (B,#2496ED) >>",
+            docker_run="<< (R,#92CBF5) >>",
+            with_dependency="<< (D,#FF0000) >>",
+        )
+
+        def short(txt: str) -> str:
+            return txt.replace("-", "")
+
+        to_display = [("python", "", with_detail)]
+        if with_dependency:
+            to_display += [("with_dependency", "D", False)]
+        for flavor, prefix, detail in to_display:
+            for key, payload in data.level(flavor).items():
+                lines.append(
+                    f'class {prefix}{short(key)} as "{key}" {flv_tag_lookup[payload.flavor]} {{'
+                )
+                if detail:
+                    for pkey, pval in payload.param.items():
+                        pval = str(pval)
+                        len_ = 50
+                        if len(pval) > len_:
+                            pval = pval[: len_ - 3] + "..."
+                        lines.append(f"+{pkey}={pval}")
+                lines.append("}")
+
+        for key, payload in data.level("with_dependency").items():
+            if with_dependency:
+                lines.append(f"D{short(key)} -d-> {short(payload.payload.name)}")
+
+            for dkey in payload.deps:
+                if with_dependency:
+                    lines.append(f"{short(dkey.name)} -d-> D{short(key)}")
+                else:
+                    lines.append(
+                        f"{short(dkey.name)} -d-> {short(payload.payload.name)}"
+                    )
+
+        lines += ["@enduml"]
+        path = self.target / "payload-dependency-graph.txt"
+        with open(path, "w", encoding="utf-8") as f:
+            for line in lines:
+                f.write(line + "\n")
+
+        subprocess_run(["plantuml", path], check=True)
+        path.unlink()
+        self._print(f"generated plot: {path.with_suffix('.png')}", fg="green")
+
 
 X = tp.TypeVar("X")
 
 
 @dc.dataclass
 class DoubleDict(tp.Generic[X]):
     level_map: tp.Dict[str, int]
@@ -413,14 +502,20 @@
 
         raise KeyError(key)
 
     def level(self, flavor: str) -> tp.Dict[str, X]:
         level = self.level_map[flavor]
         return self.level_dict[level]
 
+    def all_keys(self) -> tp.Sequence[str]:
+        res = []
+        for map_ in self.level_dict.values():
+            res += [x for x in map_.keys() if x not in res]
+        return res
+
 
 def repr_double_dict(
     representer: tp.Any, data: tp.Any  # pylint: disable=unused-argument
 ) -> tp.Any:
     return representer.represent_str("n/a")
```

### Comparing `adaux-2.2.0/source/adaux/_components/_19_docker.py` & `adaux-2.3.0/source/adaux/_components/_19_docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,42 +12,48 @@
 
 
 class DockerMixin(PayloadMixin, DependencyMixin, ProjectMixin, MetaMixin):
     @classmethod
     def __keys(cls) -> tp.Tuple[str, ...]:
         return ("base_match", "platform", "compose_version")
 
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
         data = self.auxcon.payload
 
+        data.setdefault("python", _ProtoNamespace())
+        data.python["check-release-notes"] = _ProtoNamespace()
+
         if self.is_enabled("pre-commit"):
             data.setdefault("with_dependency", _ProtoNamespace())
             run = "pre-commit"
             build = f"build-{run}"
-            data.with_dependency[run] = dict(
-                deps=[build], variant={"-all": dict(cmd="--all")}
-            )
+            data.with_dependency[run] = dict(variant={"all": dict(cmd="--all")})
             data.with_dependency[build] = dict(deps=["build-python-deps"])
 
         if self.is_enabled("pytest"):
             data.setdefault("with_dependency", _ProtoNamespace())
             run = "pytest"
             build = f"build-{run}"
             data.with_dependency[build] = dict(deps=["build-python-deps"])
-            data.with_dependency[run] = dict(deps=[build])
+            data.with_dependency[run] = dict()
             if self.is_enabled("coverage"):
                 data.with_dependency[run]["variant"] = {
-                    "-mr": {"marker": ""},
-                    "-cov": dict(coverage=95, variant={"-mr": None}),
+                    "mr": {"marker": ""},
+                    "cov": dict(coverage=95, variant={"mr": None}),
                 }
 
         if self.is_enabled("docs"):
+            run = "docs"
+            build = f"build-{run}"
             data.setdefault("with_dependency", _ProtoNamespace())
-            data.with_dependency["docs"] = dict(param=dict(extra_req="docs"))
+            data.with_dependency[build] = dict(
+                deps=["build-python-deps"], param=dict(extra_req="docs")
+            )
+            data.with_dependency[run] = None
 
         if self.is_enabled("gitlab"):
             data.setdefault("docker_run", _ProtoNamespace())
             data.setdefault("python", _ProtoNamespace())
             data.docker_run["gitlab-release-run"] = _ProtoNamespace()
             data.python["gitlab-release"] = _ProtoNamespace()
             data.docker_run["pkg-gitlab"] = _ProtoNamespace()
@@ -58,34 +64,34 @@
         data.docker_settings = _ProtoNamespace(
             platform="amd64", base_match={"mybase": dict(fallback="develop")}
         )
 
     def update_to_template(self, tpl: _ProtoNamespace, full: _ProtoNamespace) -> None:
         super().update_to_template(tpl, full)
 
-        for flavor in ["docker_build", "docker_run", "with_dependency"]:
-            if flavor not in self.auxf.payload:
-                continue
+        for flavor in ["docker_build", "docker_run", "python", "with_dependency"]:
             if flavor not in tpl.payload:
                 continue
-            data = self.auxf.payload[flavor]
+            data = self.auxf.payload.get(flavor, _ProtoNamespace())
             old = list(data)
             new = list(tpl.payload[flavor])
             last_idx = 0
             for name, payload in full.payload[flavor].items():
                 if name in new and name not in old:
                     data[name] = payload
                     old.insert(last_idx + 1, name)
                     self._print(f"payload.{flavor}: added {name}", fg="green")
                 elif name in old and name not in new:
                     del data[name]
                     old.remove(name)
                     self._print(f"payload.{flavor}: removed {name}", fg="red")
                 if name in old and name in new:
                     last_idx = old.index(name)
+            if data:
+                self.auxf.payload[flavor] = data
 
     def formatted(self) -> None:
         super().formatted()
         self._copy_keys_over(self.__keys(), "payload", "docker_settings")
         self._to_proto_ns("payload", "docker_settings")
         self._to_proto_ns("payload", "docker_settings", "base_match", iter_mapping=True)
 
@@ -118,14 +124,15 @@
         deps = self.auxe.dependencies
         data = self.auxe.payload
         prefix = "build-"
         for key, payload_cfg in data.docker_build.items():
             assert key.startswith(prefix)
             name = key[len(prefix) :]
             payload_cfg.setdefault("param", _ProtoNamespace())
+            assert isinstance(payload_cfg.param, _ProtoNamespace)
             param = payload_cfg.param
             if "extra_req" in param and isinstance(param.extra_req, str):
                 param.extra_req = [param.extra_req]
 
             param.setdefault("pip_req", [])
             param.setdefault("script", [])
             param.setdefault("base", None)
```

### Comparing `adaux-2.2.0/source/adaux/_components/_20_ci.py` & `adaux-2.3.0/source/adaux/_components/_20_ci.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,59 +2,141 @@
 # pylint: disable=too-many-lines
 import os
 import typing as tp
 
 from .._logging import logger
 from .._proto_namespace import _ProtoNamespace
 from .._util import ApiRequestCommunicator
+from ._00_extra_level import ExtraLevel
 from ._03_meta import MetaMixin
 from ._18_payload import PayloadMixin
 
 
 class CiMixin(PayloadMixin, MetaMixin):
     # pylint: disable=unused-private-member
     @classmethod
     def __keys(cls) -> tp.Tuple[str, ...]:
         return ("mechanism", "docker_image", "runner", "trigger", "use_adaux_img")
 
-    def templated(self) -> None:
-        super().templated()
+    def templated(self, negative_default: bool = False) -> None:
+        super().templated(negative_default)
         self.auxcon.ci = _ProtoNamespace(trigger=_ProtoNamespace())
         data = self.auxcon.ci.trigger
         data["+push"] = {
             "-openmr": {
-                "-release": {"pre-commit": None, "pytest": None},
+                "-release": {"pre-commit": None},
                 "+release": {
                     "+gitlab": {
                         "gitlab-release": None,
                         "pkg-gitlab": None,
-                        "pkg-pypi": None,
                     }
                 },
             }
         }
         data["+mr"] = {
             "+draft": {
                 "pre-commit": None,
-                "pytest": None,
             },
             "-draft": {
                 "pre-commit-all": None,
-                "-vip": {
-                    "pytest-mr": None,
-                },
-                "+vip": {
-                    "pytest-cov-mr": None,
-                },
             },
             "+release": {
                 "check-release-notes": None,
             },
         }
 
+        if self.is_enabled("pytest"):
+            data["+push"]["-openmr"]["-release"]["pytest"] = None
+            data["+mr"]["+draft"]["pytest"] = None
+            if self.is_enabled("coverage"):
+                data["+mr"]["-draft"].update(
+                    {
+                        "-vip": {
+                            "pytest-mr": None,
+                        },
+                        "+vip": {
+                            "pytest-cov-mr": None,
+                        },
+                    }
+                )
+            else:
+                data["+mr"]["-draft"]["pytest-mr"] = None
+
+        if self.is_enabled("docs"):
+            data["+mr"]["-draft"]["+release"] = {"docs": None}
+            data["+push"]["-openmr"]["+release"]["docs"] = None
+
+    def update_to_template(self, tpl: _ProtoNamespace, full: _ProtoNamespace) -> None:
+        super().update_to_template(tpl, full)
+
+        with self.extra(ExtraLevel.HYDRATED) as auxe:  # type: ignore
+            valid_payloads = auxe.payload.lookup.all_keys()
+
+        added = []
+
+        def deep_add(trig_chain: str, obj: tp.Any) -> None:
+            last_key = trig_chain.rsplit(".", 1)[1]
+            if last_key.startswith("+") or last_key.startswith("-"):
+                for key, val in obj.items():
+                    deep_add(trig_chain + "." + key, val)
+            else:
+                added.append(trig_chain)
+
+        def deep_merge(
+            tpl: tp.Optional[_ProtoNamespace],
+            user: tp.Optional[_ProtoNamespace],
+            trig_chain: str = "ci.trigger",
+        ) -> tp.Optional[_ProtoNamespace]:
+            if tpl is None and user is None:
+                return None
+            if tpl is None:
+                return user
+            if user is None:
+                deep_add(trig_chain, tpl)
+                return tpl
+            res = _ProtoNamespace()
+            all_keys = list(tpl.keys())
+            all_keys += [x for x in user.keys() if x not in all_keys]
+
+            for key in all_keys:
+                res[key] = deep_merge(
+                    tpl.get(key), user.get(key), trig_chain=trig_chain + "." + key
+                )
+            return res
+
+        new_trigger = deep_merge(tpl.ci.trigger, self.auxf.ci.trigger)
+
+        removed = []
+
+        def deep_remove(
+            trigger: tp.Optional[_ProtoNamespace], trig_chain: str = "ci.trigger"
+        ) -> None:
+            if trigger is None:
+                return
+            for key, val in list(trigger.items()):
+                if key.startswith("+") or key.startswith("-"):
+                    deep_remove(val, trig_chain=trig_chain + "." + key)
+                    if not trigger[key]:
+                        del trigger[key]
+                elif key not in valid_payloads:
+                    del trigger[key]
+                    removed.append(f"{trig_chain}.{key}")
+
+        deep_remove(new_trigger)
+        overlap = set(added) & set(removed)
+        if overlap:
+            logger.warning("overlap (added and removed) in ci.trigger: %s", overlap)
+        for add in added:
+            if add not in overlap:
+                self._print(f"added  {add}", fg="green")
+        for rem in removed:
+            if rem not in overlap:
+                self._print(f"removed {rem}", fg="red")
+        self.auxf.ci.trigger = new_trigger
+
     def demodata(self) -> None:
         super().demodata()
         self.auxcon.ci.runner = "dind-cached"
         self.auxcon.ci.mechanism = "mixed"
 
     def formatted(self) -> None:
         super().formatted()
@@ -73,36 +155,14 @@
         data.setdefault("docker_image", self.versions.ci_docker_image)
         data.setdefault("trigger", _ProtoNamespace())
         data.setdefault("use_adaux_img", True)
         assert data.trigger is not None
         assert data.mechanism in ["monolith"]
         assert data.runner in ["dind-cached", "normal"]
 
-    # def update_to_template(self, tpl: _ProtoNamespace, full: _ProtoNamespace) -> None:
-    #     super().update_to_template(tpl, full)
-
-    #     data = self.auxd.ci.stages
-    #     for key, stage in data.items():
-    #         old = list(stage)
-    #         new = list(tpl.ci.stages.get(key, {}))
-
-    #         last_idx = 0
-    #         for name, job in full.ci.stages.get(key, {}).items():
-    #             if name in new and name not in old:
-    #                 data.jobs.insert(last_idx + 1, job)
-    #                 stage[name] = job
-    #                 old.insert(last_idx + 1, name)
-    #                 self._print(f"ci.jobs: added {name}", fg="green")
-    #             elif name in old and name not in new:
-    #                 del stage[name]
-    #                 old.remove(name)
-    #                 self._print(f"ci.jobs: removed {name}", fg="red")
-    #             if name in old and name in new:
-    #                 last_idx = old.index(name)
-
     def enriched(self) -> None:
         super().enriched()
         data = self.auxe.ci
 
         rule_used = _ProtoNamespace(
             mr=False,
             web=False,
@@ -119,42 +179,14 @@
                             rule_used["push_no_mr"] &= False
                             rule_used["push"] |= True
                 else:
                     rule_used[key] |= f"+{key}" in reason
 
         data.used_rules = [key for key, val in rule_used.items() if val]
 
-    # infuse shorthands
-    # shorthand = dict(push=["push-no-mr", "mr"])
-    # default_rules: tp.Dict[str, tp.List[str]] = {
-    #     "rules": shorthand["push"] + ["web", "pipeline"],
-    # }
-    # for key in ["rules", "build-rules", "run-rules"]:
-    #     res = []
-    #     for rule in copy.deepcopy(val[key]):
-    #         if rule in shorthand:
-    #             val[key].remove(rule)
-    #             res += shorthand[rule]
-    #         else:
-    #             res += [rule]
-    #     if not val["rules"]:
-    #         res = res or default_rules[key]
-    #     val[key] = res
-
-    # diff = set(val.keys()) - set(valid_opts_keys)
-    # if diff:
-    # raise RuntimeError(f"invalid options: {diff}")
-
-    # data.setdefault("mechanism", "monolith")
-    # data.setdefault("runner", "normal")
-    # data.setdefault("docker_image", self.versions.ci_docker_image)
-    # assert data.mechanism in ["monolith", "gitlab", "mixed"]
-    # assert data.runner in ["dind-cached", "normal"]
-    # yield auxcone
-
     def run_ci(self, trigger_str: str, dry: bool = False) -> int:
         if trigger_str == "gitlab":
             triggers = self._triggers_from_gitlab_ci()
         else:
             triggers = self._triggers_from_str(trigger_str)
 
         # get the payload_names
```

### Comparing `adaux-2.2.0/source/adaux/_components/_99_all.py` & `adaux-2.3.0/source/adaux/_components/_99_all.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_aux_ci.py` & `adaux-2.3.0/source/adaux/_components/_aux_ci.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,16 +327,16 @@
             print(f"{job.ident:>30} {job.state.status_colored}")
 
         self.recurse(show)
 
     def check_necessity(self) -> None:
         self.recurse(self.check_job_necessity)
 
-    def run_pipeline(self) -> None:
-        self.prune_unincluded(show=False)
+    def run_pipeline(self, show: bool = False) -> None:
+        self.prune_unincluded(show=show)
         self.recurse(self.run_if_needed)
 
     def recurse(
         self,
         fct: tp.Callable[[T], None],
         root_jobs: tp.Optional[tp.List[T]] = None,
         seen: tp.Tuple[T, ...] = tuple(),
```

### Comparing `adaux-2.2.0/source/adaux/_components/_payload/__init__.py` & `adaux-2.3.0/source/adaux/_components/_payload/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 from . import _docker_run
 from . import _python
 from . import _with_dependency
 from ._base import *
 from ._docker import *
 from ._docker_build import *
 from ._docker_compose import *
+from ._docker_executors import subprocess_run
 from ._docker_run import *
 from ._python import *
 from ._with_dependency import *
 
 __all__ = (
     _base.__all__
     + _docker_build.__all__
     + _docker_run.__all__
     + _docker_compose.__all__
     + _python.__all__
     + _with_dependency.__all__
     + _docker.__all__
+    + ["subprocess_run"]
 )
```

### Comparing `adaux-2.2.0/source/adaux/_components/_payload/_base.py` & `adaux-2.3.0/source/adaux/_components/_payload/_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_payload/_docker.py` & `adaux-2.3.0/source/adaux/_components/_payload/_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_payload/_docker_build.py` & `adaux-2.3.0/source/adaux/_components/_payload/_docker_build.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_payload/_docker_executors.py` & `adaux-2.3.0/source/adaux/_components/_payload/_docker_executors.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_payload/_python.py` & `adaux-2.3.0/source/adaux/_components/_payload/_python.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_components/_payload/_with_dependency.py` & `adaux-2.3.0/source/adaux/_components/_payload/_with_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_create_badge.py` & `adaux-2.3.0/source/adaux/_create_badge.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_gitlab.py` & `adaux-2.3.0/source/adaux/_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_parser.py` & `adaux-2.3.0/source/adaux/_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     @classmethod
     def to_conf(cls, config: _ProtoNamespace) -> tp.Any:
         return cls.rec_walk(
             config,
             [
                 (
-                    lambda x: isinstance(x, _ProtoNamespace),
+                    lambda x: isinstance(x, (_ProtoNamespace, dict)),
                     lambda x: CommentedMap(x.items()) if x else None,
                 ),
                 (
                     lambda x: isinstance(x, list),
                     lambda x: CommentedSeq(x) if x else None,
                 ),
             ],
```

### Comparing `adaux-2.2.0/source/adaux/_proto_namespace.py` & `adaux-2.3.0/source/adaux/_proto_namespace.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_tick.py` & `adaux-2.3.0/source/adaux/_tick.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_todo.py` & `adaux-2.3.0/source/adaux/_todo.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/_util.py` & `adaux-2.3.0/source/adaux/_util.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/CI/00-main.yml.jinja2` & `adaux-2.3.0/source/adaux/src/CI/00-main.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/CI/01-rules.yml.jinja2` & `adaux-2.3.0/source/adaux/src/CI/01-rules.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/image/Dockerfile.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/image/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2` & `adaux-2.3.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docs/default_conf.py.jinja2` & `adaux-2.3.0/source/adaux/src/docs/default_conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/docs/postprocess_html.py` & `adaux-2.3.0/source/adaux/src/docs/postprocess_html.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/license/Apache-2.0.txt.jinja2` & `adaux-2.3.0/source/adaux/src/license/Apache-2.0.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/license/BSD-3_clause.txt.jinja2` & `adaux-2.3.0/source/adaux/src/license/BSD-3_clause.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/license/MIT.txt.jinja2` & `adaux-2.3.0/source/adaux/src/license/MIT.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc` & `adaux-2.3.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/payload/python/functions.py` & `adaux-2.3.0/source/adaux/src/payload/python/functions.py`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2` & `adaux-2.3.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux/src/pre-commit/config.yaml.jinja2` & `adaux-2.3.0/source/adaux/src/pre-commit/config.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.2.0/source/adaux.egg-info/SOURCES.txt` & `adaux-2.3.0/source/adaux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

