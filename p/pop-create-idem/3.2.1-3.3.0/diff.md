# Comparing `tmp/pop-create-idem-3.2.1.tar.gz` & `tmp/pop-create-idem-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-create-idem-3.2.1.tar", last modified: Tue Apr 11 20:29:41 2023, max compression
+gzip compressed data, was "pop-create-idem-3.3.0.tar", last modified: Wed Apr 12 20:11:21 2023, max compression
```

## Comparing `pop-create-idem-3.2.1.tar` & `pop-create-idem-3.3.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8796 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7947 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/cloudspec/
--rw-r--r--   0 root         (0) root         (0)     8546 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/cloudspec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/cloudspec/conf.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/cloudspec/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/
--rw-r--r--   0 root         (0) root         (0)     2533 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/auto_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/contracts/
--rw-r--r--   0 root         (0) root         (0)       78 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/docs.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/exec_modules.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/state_modules.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/tests.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/tool.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/
--rw-r--r--   0 root         (0) root         (0)     1777 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/function.py
--rw-r--r--   0 root         (0) root         (0)     5321 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/param.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/
--rw-r--r--   0 root         (0) root         (0)     3552 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/auto_state.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/exec.py
--rw-r--r--   0 root         (0) root         (0)      822 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/state.py
--rw-r--r--   0 root         (0) root         (0)      209 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/tool.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)     2091 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1266 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2509 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      626 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      960 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      763 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      917 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      196 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     2649 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/hooks/
--rw-r--r--   0 root         (0) root         (0)      366 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     5763 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/init.py
--rw-r--r--   0 root         (0) root         (0)     6329 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/parse.py
--rw-r--r--   0 root         (0) root         (0)    12404 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1740 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/rest/
--rw-r--r--   0 root         (0) root         (0)      133 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/rest/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/
--rw-r--r--   0 root         (0) root         (0)      587 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/pop_create_idem/tool/format/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/format/case.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/format/html.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/format/inflect.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/format/keyword.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/format/wrap.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/gradle.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/pop_create_idem/tool/jinja.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 20:29:41.792066 pop-create-idem-3.2.1/pop_create_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8796 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4232 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-11 20:29:41.000000 pop-create-idem-3.2.1/pop_create_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 20:29:41.796066 pop-create-idem-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3004 2023-04-11 20:29:27.000000 pop-create-idem-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7947 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/cloudspec/
+-rw-r--r--   0 root         (0) root         (0)     8546 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/cloudspec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/cloudspec/conf.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/cloudspec/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/auto_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/contracts/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/docs.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/exec_modules.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/state_modules.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/tests.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/function.py
+-rw-r--r--   0 root         (0) root         (0)     5321 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/param.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/
+-rw-r--r--   0 root         (0) root         (0)     3552 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/auto_state.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/exec.py
+-rw-r--r--   0 root         (0) root         (0)      822 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/state.py
+-rw-r--r--   0 root         (0) root         (0)      209 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.177679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.177679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.177679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.177679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.177679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/hooks/
+-rw-r--r--   0 root         (0) root         (0)      366 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     6081 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/init.py
+-rw-r--r--   0 root         (0) root         (0)     7306 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/parse.py
+-rw-r--r--   0 root         (0) root         (0)    12534 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/rest/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/rest/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/pop_create_idem/tool/format/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/format/case.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/format/html.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/format/inflect.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/format/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/format/wrap.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/gradle.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/pop_create_idem/tool/jinja.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 20:11:20.000000 pop-create-idem-3.3.0/pop_create_idem/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:11:21.181679 pop-create-idem-3.3.0/pop_create_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4232 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-12 20:11:21.000000 pop-create-idem-3.3.0/pop_create_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 20:11:21.185679 pop-create-idem-3.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-04-12 20:11:05.000000 pop-create-idem-3.3.0/setup.py
```

### Comparing `pop-create-idem-3.2.1/LICENSE` & `pop-create-idem-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/PKG-INFO` & `pop-create-idem-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.2.1
+Version: 3.3.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.2.1/README.rst` & `pop-create-idem-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/cloudspec/__init__.py` & `pop-create-idem-3.3.0/cloudspec/__init__.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/cloudspec/conf.py` & `pop-create-idem-3.3.0/cloudspec/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/auto_state.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/exec_modules.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/exec_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/state_modules.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/state_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/tests.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/tests.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/create/tool.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/create/tool.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/init.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/function.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/param.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/param.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/parse/plugin.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/parse/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/auto_state.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/exec.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/exec.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/plugin.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/cloudspec/template/state.py` & `pop-create-idem-3.3.0/pop_create_idem/cloudspec/template/state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/conf.py` & `pop-create-idem-3.3.0/pop_create_idem/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     },
     "acct_plugin": {
         "subcommands": ["idem-cloud", "openapi3", "swagger"],
         "dyne": "pop_create",
     },
     "specification": {
         "options": ["--spec", "--file", "--url"],
+        "nargs": "+",
         "subcommands": ["openapi3", "swagger", "idem-cloud"],
         "dyne": "pop_create",
     },
 }
 CONFIG = {
     "create_plugin": {
         "default": "auto_states",
```

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/init.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/init.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,62 +16,67 @@
         )
 
     ctx.has_acct_plugin = bool(ctx.acct_plugin)
     if not ctx.has_acct_plugin:
         # Create auth plugins
         ctx.acct_plugin = ctx.service_name
 
-    # Read the spec from URL or local file (Yaml)
-    spec = hub.pop_create.openapi3.init.read(source=ctx.specification)
-    api = openapi3.OpenAPI(spec, validate=True)
-    errors = api.errors()
-    if errors:
-        for e in errors:
-            hub.log.warning(e)
-
-    # list these as defaults in the acct plugin
-    if api.servers:
-        ctx.servers = [x.url for x in api.servers]
-    else:
-        ctx.servers = ctx.get("servers", [""])
-
-    hub.log.debug(f"Working with openapi spec version: {api.openapi}")
-
-    ctx.cloud_api_version = api.info.version or "latest"
-    ctx.clean_api_version = hub.tool.format.case.snake(ctx.cloud_api_version).strip("_")
-
-    if not ctx.clean_api_version:
-        ctx.clean_api_version = ctx.get("clean_api_version")
-
-    if not ctx.cloud_api_version:
-        ctx.cloud_api_version = ctx.get("cloud_api_version")
-
-    # If the api version starts with a digit then make sure it can be used for python namespacing
-    if ctx.clean_api_version[0].isdigit():
-        ctx.clean_api_version = "v" + ctx.clean_api_version
-
-    # Get function plugins
-    plugins = hub.pop_create.openapi3.parse.plugins(ctx, api)
-
-    # Add any missing function which is required for idem resource modules
-    plugins = hub.pop_create.openapi3.init.add_missing_known_functions(ctx, plugins)
-
-    # Create request formats for function
-    request_formats = hub.pop_create.openapi3.init.get_requests_formats(plugins)
-
-    cloud_spec = NamespaceDict(
-        api_version=ctx.cloud_api_version,
-        project_name=ctx.project_name,
-        service_name=ctx.service_name,
-        request_format=request_formats,
-        plugins=plugins,
-    )
-    ctx.cloud_spec = cloud_spec
+    # FIXME: Not an optimal way, it could take longer as for each spec we go through post generation hooks
+    for specification in ctx.specification:
+        # Read the spec from URL or local file (Yaml)
+        spec = hub.pop_create.openapi3.init.read(source=specification)
+        api = openapi3.OpenAPI(spec, validate=True)
+        errors = api.errors()
+        if errors:
+            for e in errors:
+                hub.log.warning(e)
+
+        # list these as defaults in the acct plugin
+        if api.servers:
+            ctx.servers = [x.url for x in api.servers]
+        else:
+            ctx.servers = ctx.get("servers", [""])
+
+        hub.log.debug(f"Working with openapi spec version: {api.openapi}")
+
+        ctx.cloud_api_version = api.info.version or "latest"
+        ctx.clean_api_version = hub.tool.format.case.snake(ctx.cloud_api_version).strip(
+            "_"
+        )
+
+        if not ctx.clean_api_version:
+            ctx.clean_api_version = ctx.get("clean_api_version")
+
+        if not ctx.cloud_api_version:
+            ctx.cloud_api_version = ctx.get("cloud_api_version")
+
+        # If the api version starts with a digit then make sure it can be used for python namespacing
+        if ctx.clean_api_version[0].isdigit():
+            ctx.clean_api_version = "v" + ctx.clean_api_version
+
+        # Get function plugins
+        plugins = hub.pop_create.openapi3.parse.plugins(ctx, api)
+
+        # Add any missing function which is required for idem resource modules
+        plugins = hub.pop_create.openapi3.init.add_missing_known_functions(ctx, plugins)
+
+        # Create request formats for function
+        request_formats = hub.pop_create.openapi3.init.get_requests_formats(plugins)
+
+        cloud_spec = NamespaceDict(
+            api_version=ctx.cloud_api_version,
+            project_name=ctx.project_name,
+            service_name=ctx.service_name,
+            request_format=request_formats,
+            plugins=plugins,
+        )
+        ctx.cloud_spec = cloud_spec
+
+        hub.pop_create.init.run(directory=directory, subparsers=["idem_cloud"], **ctx)
 
-    hub.pop_create.init.run(directory=directory, subparsers=["idem_cloud"], **ctx)
     return ctx
 
 
 def read(hub, source: str or Dict):
     """
     If the path is a file, then parse the json contents of the file,
     If the path is a url, then return a json response from the url.
```

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/parse.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/parse.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,22 +19,39 @@
             continue
 
         # Get the request type that works for this request
         for request_type in path.raw_element.keys():
             func: openapi3.paths.Operation = getattr(path, request_type)
             if not func:
                 continue
-            subs = [hub.tool.format.case.snake(sub) for sub in func.tags]
-            if not subs:
-                plugin = "init"
-            else:
-                plugin = subs.pop()
+
+            plugin = None
+            refs = None
+            if func.tags:
+                subs = [hub.tool.format.case.snake(sub) for sub in func.tags]
+                if not subs:
+                    plugin = "init"
+                else:
+                    plugin = subs.pop()
+
+                refs = subs + [plugin]
+            elif func.get_path():
+                # e.g. "/pets", /pets/{id} -> "pets" become plugin
+                # func.get_path() could look like this "paths./pets/{id}.get
+                # second element is always the actual path itself
+                func_path = func.get_path().split(".")[1]
+                plugin = func_path.lstrip("/").split("/")[0]
+                refs = [plugin]
+
+            if not plugin:
+                raise AttributeError(
+                    f"Not sure how to find plugin for {name}. Try using 'tags'"
+                )
 
             # service name is already added in pop-create
-            refs = subs + [plugin]
             ref = ".".join(refs)
             if ref not in ret:
                 # This is the first time we have looked at this plugin
                 ret[ref] = {
                     "functions": {},
                     "doc": "",
                     "imports": [
@@ -49,21 +66,21 @@
                 hub.pop_create.openapi3.parse.resolve_reserved_function_name(
                     name, plugin, request_type, func
                 )
             )
 
             # Anything that doesn't resolved in reserved function name, would go into tools/{resource_name}/*
             func_name = (
-                hub.pop_create.openapi3.parse.resolve_function_name(name, plugin, func)
+                hub.pop_create.openapi3.parse.resolve_function_name(
+                    name, plugin, request_type, func
+                )
                 if not reserved_func_name
                 else reserved_func_name
             )
 
-            # print(f"{func_name}: {name}: {plugin}")
-
             func_data = hub.pop_create.openapi3.parse.function(func, api)
             func_data["hardcoded"] = {
                 "method": request_type,
                 "path": name.split(" ")[0],
                 "service_name": ctx.service_name,
                 "resource_name": plugin,
             }
@@ -153,33 +170,42 @@
                 return "update"
             elif request_type == "delete":
                 return "delete"
 
     return None
 
 
-def resolve_function_name(hub, name: str, plugin: str, func: openapi3.paths.Operation):
+def resolve_function_name(
+    hub, name: str, plugin: str, request_type: str, func: openapi3.paths.Operation
+):
     # This is the preferred way to get a function name
     # However, some APIs can just put reserved/known operationId which is not helpful here in parsing and codegen
     # Also, we always handle reserved/known operation names in different way
     func_name = (
         func.operationId
         if func.operationId
         not in ["get", "list", "create", "patch", "update", "put", "delete"]
         else None
     )
 
     # Fallback function name based on the pets example
     if not func_name and " " in name:
         func_name = "_".join(name.split(" ")[1:]).lower()
 
-    if not func_name:
+    if not func_name and func.summary:
         # Truncate it to 10 characters and add plugin name in the end
         func_name = f"{func.summary[:10]}_{plugin}"
 
+    if not func_name and request_type:
+        # No operationId, no summary, let's create it with path
+        # GET /pets/{id}/types -> get_pets_id_types
+        func_name = (
+            f"{request_type}_{name.replace('{', '').replace('}', '').replace('/', '_')}"
+        )
+
     if not func_name and func.extensions:
         func_name = func.extensions[sorted(func.extensions.keys())[0]]
 
     # Maybe we need more fallbacks, you tell me
     if not func_name:
         # Maybe a fallback based on the path and method?
         raise AttributeError(f"Not sure how to find func name for {name}, help me out")
```

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/template.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     get = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
         path="{{ function.hardcoded.path }}".format(
             **{{ parameter.mapping.path|default({}) }}
         ),
         query_params={{ parameter.mapping.query|default({}) }},
-        data={{ parameter.mapping.header|default({}) }}
+        data={},
+        headers={{ parameter.mapping.header|default({}) }},
     )
 
     if not get["result"]:
         # Send empty result for not found
         if get["status"] == 404:
             result["comment"].append(f"Get '{name}' result is empty")
             return result
@@ -40,15 +41,16 @@
 
     # TODO: Change function methods params if needed
     list = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
         path="{{ function.hardcoded.path }}",
         query_params={{ parameter.mapping.query|default({}) }},
-        data={{ parameter.mapping.header|default({}) }}
+        data={},
+        headers={{ parameter.mapping.header|default({}) }},
     )
 
     if not list["result"]:
         result["comment"].append(list["comment"])
         result["result"] = False
         return result
 
@@ -64,15 +66,16 @@
 
     # TODO: Change function methods params if needed.
     create = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
         path="{{ function.hardcoded.path }}",
         query_params={{ parameter.mapping.query|default({}) }},
-        data={{ parameter.mapping.header|default({}) }}
+        data={},
+        headers={{ parameter.mapping.header|default({}) }},
     )
 
     if not create["result"]:
         result["comment"].append(create["comment"])
         result["result"] = False
         return result
 
@@ -100,15 +103,16 @@
         update = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
             ctx,
             method="{{ function.hardcoded.method }}",
             path="{{ function.hardcoded.path }}".format(
                 **{{ parameter.mapping.path|default({}) }}
             ),
             query_params={{ parameter.mapping.query|default({}) }},
-            data={{ parameter.mapping.header|default({}) }}
+            data={},
+            headers={{ parameter.mapping.header|default({}) }},
         )
 
         if not create["result"]:
             result["comment"].append(update["comment"])
             result["result"] = False
             return result
 
@@ -124,15 +128,16 @@
     delete = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
         path="{{ function.hardcoded.path }}".format(
             **{{ parameter.mapping.path|default({}) }}
         ),
         query_params={{ parameter.mapping.query|default({}) }},
-        data={{ parameter.mapping.header|default({}) }}
+        data={},
+        headers={{ parameter.mapping.header|default({}) }},
     )
 
     if not delete["result"]:
         result["comment"].append(delete["comment"])
         result["result"] = False
         return result
 
@@ -146,15 +151,16 @@
     ret = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
         path="{{ function.hardcoded.path }}".format(
             **{{ parameter.mapping.path|default({}) }}
         ),
         query_params={{ parameter.mapping.query|default({}) }},
-        data={{ parameter.mapping.header|default({}) }}
+        data={},
+        headers={{ parameter.mapping.header|default({}) }},
     )
 
     if not ret["result"]:
         result["comment"].append(ret["comment"])
         result["result"] = False
         return result
```

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,17 @@
             endpoint_url: {{cookiecutter.servers|join('|')}}
     """
     sub_profiles = {}
     for (
         profile,
         ctx,
     ) in profiles.get("{{cookiecutter.service_name}}", {}).items():
-        api_key = ctx.pop("api_key")
-        endpoint_url = ctx.pop("endpoint_url")
-        api_version = ctx.pop("api_version")
+        api_key = ctx.get("api_key")
+        endpoint_url = ctx.get("endpoint_url")
+        api_version = ctx.get("api_version")
 
         temp_ctx = NamespaceDict(acct={
             "endpoint_url": endpoint_url,
             "api_version": api_version,
         })
 
         ret = await hub.tool.{{cookiecutter.service_name}}.session.request(
```

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,17 +22,17 @@
             endpoint_url: https://{{cookiecutter.service_name}}.com
     """
     sub_profiles = {}
     for (
             profile,
             ctx,
     ) in profiles.get("{{cookiecutter.service_name}}", {}).items():
-        endpoint_url = ctx.pop("endpoint_url")
+        endpoint_url = ctx.get("endpoint_url")
 
-        creds = f"{ctx.pop('username')}:{ctx.pop('password')}"
+        creds = f"{ctx.get('username')}:{ctx.get('password')}"
         temp_ctx = NamespaceDict(acct={
             "endpoint_url": endpoint_url,
             "headers": {
                 "Authorization": f"Basic {base64.b64encode(creds.encode('utf-8')).decode('ascii')}"
             }
         })
```

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,20 @@
             endpoint_url: {{cookiecutter.servers|join('|')}}
     """
     sub_profiles = {}
     for (
         profile,
         ctx,
     ) in profiles.get("{{cookiecutter.service_name}}", {}).items():
-        client_id = ctx.pop("client_id")
-        client_secret = ctx.pop("client_secret")
-        org_id = ctx.pop("org_id")
+        client_id = ctx.get("client_id")
+        client_secret = ctx.get("client_secret")
+        org_id = ctx.get("org_id")
 
-        endpoint_url = ctx.pop("endpoint_url")
-        api_version = ctx.pop("api_version")
+        endpoint_url = ctx.get("endpoint_url")
+        api_version = ctx.get("api_version")
 
         temp_ctx = NamespaceDict(acct={
             "endpoint_url": endpoint_url,
             "api_version": api_version,
         })
 
         ret = await hub.tool.{{cookiecutter.service_name}}.session.request(
@@ -49,15 +49,15 @@
                 "client_id": client_id,
                 "client_secret": client_secret,
                 "org_id": org_id,
             },
             headers={
                 # TODO: Change based on login api request data
                 "content-type": "application/x-www-form-urlencoded",
-                "Authorization": f"Basic {base64.b64encode(f'{client_id}:{client_secret}'.encode('utf-8'))}"
+                "Authorization": f"Basic {base64.b64encode(f'{client_id}:{client_secret}'.encode('utf-8')).decode('ascii')}"
             },
         )
 
         if not ret["result"]:
             error = f"Unable to authenticate: {ret.get('comment', '')}"
             hub.log.error(error)
             raise ConnectionError(error)
```

### Comparing `pop-create-idem-3.2.1/pop_create_idem/pop_create/swagger/init.py` & `pop-create-idem-3.3.0/pop_create_idem/pop_create/swagger/init.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import pathlib
 
 import requests
 
 
 def context(hub, ctx, directory: pathlib.Path):
-    swagger = hub.pop_create.openapi3.init.read(source=hub.OPT.pop_create.specification)
+    openapi_specs = []
+    for specification in ctx.specification:
+        swagger = hub.pop_create.openapi3.init.read(source=specification)
+
+        # Convert swagger to openapi3
+        response = requests.post(
+            "https://converter.swagger.io/api/convert",
+            json=dict(swagger),
+            headers={"Content-Type": "application/json"},
+        )
+        openapi_specs.append(response.json())
 
-    # Convert swagger to openapi3
-    response = requests.post(
-        "https://converter.swagger.io/api/convert",
-        json=dict(swagger),
-        headers={"Content-Type": "application/json"},
-    )
-    ctx.specification = response.json()
+    ctx.specification = openapi_specs
 
     # get ctx from openapi3 with changes that turn swagger into openapi3
     hub.pop_create.init.run(directory=directory, subparsers=["openapi3"], **ctx)
 
     return ctx
```

### Comparing `pop-create-idem-3.2.1/pop_create_idem/tool/format/case.py` & `pop-create-idem-3.3.0/pop_create_idem/tool/format/case.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/tool/format/inflect.py` & `pop-create-idem-3.3.0/pop_create_idem/tool/format/inflect.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem/tool/gradle.py` & `pop-create-idem-3.3.0/pop_create_idem/tool/gradle.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/pop_create_idem.egg-info/PKG-INFO` & `pop-create-idem-3.3.0/pop_create_idem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.2.1
+Version: 3.3.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.2.1/pop_create_idem.egg-info/SOURCES.txt` & `pop-create-idem-3.3.0/pop_create_idem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.2.1/setup.py` & `pop-create-idem-3.3.0/setup.py`

 * *Files identical despite different names*

