# Comparing `tmp/astro_provider_databricks-0.1.0.tar.gz` & `tmp/astro_provider_databricks-0.1.1.tar.gz`

## Comparing `astro_provider_databricks-0.1.0.tar` & `astro_provider_databricks-0.1.1.tar`

### file list

```diff
@@ -1,71 +1,75 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.deepsource.toml
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/CHANGELOG.rst
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/Tiltfile
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/codecov.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/mlc-config.json
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/noxfile.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/yamllint-config.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.github/ci-test-connections.yaml
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.github/scripts/verify_tag_and_version.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.github/workflows/astro-deploy.yml
--rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.github/workflows/mlc_config.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/dev/.dockerignore
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/dev/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/dev/Dockerfile
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/dev/docker-compose.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/dev/packages.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/dev/requirements.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/dev/.astro/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/dev/dags/.airflowignore
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/dev/dags/example_dag_basic.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/conf.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/contributing.rst
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/requirements.txt
--rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/banner.png
--rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/dbt_dag.png
--rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/dbt_task_group.png
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/logo-dark.png
--rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/logo-light.png
--rw-r--r--   0        0        0    80206 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/connections_doc/bigquery_airflow_connection.png
--rw-r--r--   0        0        0    82236 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/connections_doc/databricks_airflow_connection.png
--rw-r--r--   0        0        0    72389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/connections_doc/postgres_airflow_connection.png
--rw-r--r--   0        0        0    75178 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/connections_doc/redshift_airflow_connection.png
--rw-r--r--   0        0        0   108877 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/connections_doc/snowflake_airflow_connection.png
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/assets/images/dbutils-notebook-success.png
--rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/assets/images/repair-all-failed.png
--rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/docs/assets/images/repair-single-failed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/example_dags/.airflowignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/example_dags/__init__.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/example_dags/example_databricks_notebook.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/example_dags/example_databricks_workflow.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/astro_databricks/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/astro_databricks/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/astro_databricks/operators/__init__.py
--rw-r--r--   0        0        0    10724 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/astro_databricks/operators/notebook.py
--rw-r--r--   0        0        0    15569 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/astro_databricks/operators/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/astro_databricks/plugins/__init__.py
--rw-r--r--   0        0        0    17286 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/astro_databricks/plugins/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/tests/pytest.ini
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/tests/test_example_dags.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/tests/databricks/__init__.py
--rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/tests/databricks/test_notebook.py
--rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/tests/databricks/test_plugin.py
--rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/tests/databricks/test_workflow.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/LICENSE
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/README.md
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.deepsource.toml
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/Tiltfile
+-rw-r--r--   0        0        0    51517 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/airflow.cfg
+-rw-r--r--   0        0        0   552960 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/airflow.db
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/codecov.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/mlc-config.json
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/noxfile.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/webserver_config.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/yamllint-config.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.github/ci-test-connections.yaml
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.github/scripts/verify_tag_and_version.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.github/workflows/astro-deploy.yml
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.github/workflows/mlc_config.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dags/.airflowignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dags/__init__.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dags/example_databricks_notebook.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dags/example_databricks_workflow.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dev/.dockerignore
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dev/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dev/Dockerfile
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dev/docker-compose.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dev/packages.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dev/requirements.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dev/.astro/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dev/dags/.airflowignore
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/dev/dags/example_dag_basic.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/contributing.rst
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/banner.png
+-rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/dbt_dag.png
+-rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/dbt_task_group.png
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/logo-dark.png
+-rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/logo-light.png
+-rw-r--r--   0        0        0    80206 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/connections_doc/bigquery_airflow_connection.png
+-rw-r--r--   0        0        0    82236 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/connections_doc/databricks_airflow_connection.png
+-rw-r--r--   0        0        0    72389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/connections_doc/postgres_airflow_connection.png
+-rw-r--r--   0        0        0    75178 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/connections_doc/redshift_airflow_connection.png
+-rw-r--r--   0        0        0   108877 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/connections_doc/snowflake_airflow_connection.png
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/assets/images/dbutils-notebook-success.png
+-rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/assets/images/repair-all-failed.png
+-rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/docs/assets/images/repair-single-failed.png
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/astro_databricks/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/astro_databricks/constants.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/astro_databricks/databricks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/astro_databricks/operators/__init__.py
+-rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/astro_databricks/operators/notebook.py
+-rw-r--r--   0        0        0    15692 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/astro_databricks/operators/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/astro_databricks/plugins/__init__.py
+-rw-r--r--   0        0        0    17286 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/astro_databricks/plugins/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/tests/pytest.ini
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/tests/test_example_dags.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/tests/databricks/__init__.py
+-rw-r--r--   0        0        0    14857 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/tests/databricks/test_notebook.py
+-rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/tests/databricks/test_plugin.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/tests/databricks/test_workflow.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/README.md
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 astro_provider_databricks-0.1.1/PKG-INFO
```

### Comparing `astro_provider_databricks-0.1.0/.pre-commit-config.yaml` & `astro_provider_databricks-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/CHANGELOG.rst` & `astro_provider_databricks-0.1.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/CODE_OF_CONDUCT.md` & `astro_provider_databricks-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/Tiltfile` & `astro_provider_databricks-0.1.1/Tiltfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/.github/scripts/verify_tag_and_version.py` & `astro_provider_databricks-0.1.1/.github/scripts/verify_tag_and_version.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/.github/workflows/astro-deploy.yml` & `astro_provider_databricks-0.1.1/.github/workflows/astro-deploy.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/.github/workflows/ci.yml` & `astro_provider_databricks-0.1.1/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -200,7 +200,8 @@
           coverage xml
       - name: Upload coverage
         uses: codecov/codecov-action@v2
         with:
           fail_ci_if_error: true
           token: ${{ secrets.CODECOV_TOKEN }}
           files: ./coverage.xml
+
```

### Comparing `astro_provider_databricks-0.1.0/.github/workflows/deploy.yml` & `astro_provider_databricks-0.1.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/.github/workflows/docs.yml` & `astro_provider_databricks-0.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/dev/Dockerfile` & `astro_provider_databricks-0.1.1/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/dev/docker-compose.yaml` & `astro_provider_databricks-0.1.1/dev/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/dev/dags/example_dag_basic.py` & `astro_provider_databricks-0.1.1/dev/dags/example_dag_basic.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/Makefile` & `astro_provider_databricks-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/conf.py` & `astro_provider_databricks-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/contributing.rst` & `astro_provider_databricks-0.1.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/index.rst` & `astro_provider_databricks-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/make.bat` & `astro_provider_databricks-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/_static/banner.png` & `astro_provider_databricks-0.1.1/docs/_static/banner.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/_static/dbt_dag.png` & `astro_provider_databricks-0.1.1/docs/_static/dbt_dag.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/_static/dbt_task_group.png` & `astro_provider_databricks-0.1.1/docs/_static/dbt_task_group.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/_static/logo-dark.png` & `astro_provider_databricks-0.1.1/docs/_static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/_static/logo-light.png` & `astro_provider_databricks-0.1.1/docs/_static/logo-light.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/_static/connections_doc/bigquery_airflow_connection.png` & `astro_provider_databricks-0.1.1/docs/_static/connections_doc/bigquery_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/_static/connections_doc/databricks_airflow_connection.png` & `astro_provider_databricks-0.1.1/docs/_static/connections_doc/databricks_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/_static/connections_doc/postgres_airflow_connection.png` & `astro_provider_databricks-0.1.1/docs/_static/connections_doc/postgres_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/_static/connections_doc/redshift_airflow_connection.png` & `astro_provider_databricks-0.1.1/docs/_static/connections_doc/redshift_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/_static/connections_doc/snowflake_airflow_connection.png` & `astro_provider_databricks-0.1.1/docs/_static/connections_doc/snowflake_airflow_connection.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/assets/images/dbutils-notebook-success.png` & `astro_provider_databricks-0.1.1/docs/assets/images/dbutils-notebook-success.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/assets/images/repair-all-failed.png` & `astro_provider_databricks-0.1.1/docs/assets/images/repair-all-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/docs/assets/images/repair-single-failed.png` & `astro_provider_databricks-0.1.1/docs/assets/images/repair-single-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/example_dags/example_databricks_notebook.py` & `astro_provider_databricks-0.1.1/dags/example_databricks_notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/example_dags/example_databricks_workflow.py` & `astro_provider_databricks-0.1.1/dags/example_databricks_workflow.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/astro_databricks/operators/notebook.py` & `astro_provider_databricks-0.1.1/astro_databricks/operators/notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         **kwargs,
     ):
         self.notebook_path = notebook_path
         self.source = source
         self.notebook_params = notebook_params or {}
         self.notebook_packages = notebook_packages or []
         self.databricks_conn_id = databricks_conn_id
+        self.databricks_run_id = ""
         self.databricks_metadata: dict | None = None
         self.job_cluster_key = job_cluster_key or ""
         self.new_cluster = new_cluster or {}
         self.existing_cluster_id = existing_cluster_id or ""
         super().__init__(**kwargs)
 
         # For Airflow versions <2.3, the `task_group` attribute is unassociated, and hence we need to add that.
@@ -148,14 +149,16 @@
         return self.dag_id + "__" + task_id.replace(".", "__")
 
     def monitor_databricks_job(self):
         """Monitor the Databricks job until it completes. Raises Airflow exception if the job fails."""
         api_client = self._get_api_client()
         runs_api = RunsApi(api_client)
         current_task = self._get_current_databricks_task(runs_api)
+        url = runs_api.get_run(self.databricks_run_id, version=JOBS_API_VERSION)['run_page_url']
+        self.log.info(f"Check the job run in Databricks: {url}")
         self._wait_for_pending_task(current_task, runs_api)
         self._wait_for_running_task(current_task, runs_api)
         self._wait_for_terminating_task(current_task, runs_api)
         final_state = runs_api.get_run(
             current_task["run_id"], version=JOBS_API_VERSION
         )["state"]
         self._handle_final_state(final_state)
```

### Comparing `astro_provider_databricks-0.1.0/astro_databricks/operators/workflow.py` & `astro_provider_databricks-0.1.1/astro_databricks/operators/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from mergedeep import merge
 
 from astro_databricks.plugins.plugin import (
     DatabricksJobRepairAllFailedLink,
     DatabricksJobRunLink,
 )
 
-
 @define
 class DatabricksMetaData:
     databricks_conn_id: str
     databricks_run_id: str
     databricks_job_id: str
 
 
@@ -162,19 +161,21 @@
             job_id=job_id,
             jar_params=self.task_group.jar_params,
             notebook_params=self.task_group.notebook_params,
             python_params=self.task_group.python_params,
             spark_submit_params=self.task_group.spark_submit_params,
         )["run_id"]
         runs_api = RunsApi(api_client)
-
+        url = runs_api.get_run(run_id).get("run_page_url")
+        self.log.info(f"Check the job run in Databricks: {url}")
         while runs_api.get_run(run_id)["state"]["life_cycle_state"] == "PENDING":
             print("job pending")
             time.sleep(5)
         self.databricks_run_id = run_id
+
         return {
             "databricks_conn_id": self.databricks_conn_id,
             "databricks_job_id": job_id,
             "databricks_run_id": run_id,
         }
```

### Comparing `astro_provider_databricks-0.1.0/astro_databricks/plugins/plugin.py` & `astro_provider_databricks-0.1.1/astro_databricks/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/tests/conftest.py` & `astro_provider_databricks-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/tests/test_example_dags.py` & `astro_provider_databricks-0.1.1/tests/test_example_dags.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/tests/utils.py` & `astro_provider_databricks-0.1.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/tests/databricks/test_notebook.py` & `astro_provider_databricks-0.1.1/tests/databricks/test_notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,14 +353,15 @@
 )
 def test_monitor_databricks_job_success(
     mock_get_databricks_task_id,
     mock_get_api_client,
     mock_runs_api,
     mock_databricks_hook,
     databricks_notebook_operator,
+    caplog
 ):
     mock_get_databricks_task_id.return_value = "1"
     # Define the expected response
     response = {
         "run_page_url": "https://databricks-instance-xyz.cloud.databricks.com/#job/1234/run/1",
         "state": {
             "life_cycle_state": "TERMINATED",
@@ -377,14 +378,15 @@
     mock_runs_api.return_value.get_run.return_value = response
 
     databricks_notebook_operator.databricks_run_id = "1"
     databricks_notebook_operator.monitor_databricks_job()
     mock_runs_api.return_value.get_run.assert_called_with(
         databricks_notebook_operator.databricks_run_id, version="2.1"
     )
+    assert 'Check the job run in Databricks: https://databricks-instance-xyz.cloud.databricks.com/#job/1234/run/1' in caplog.messages
 
 
 @mock.patch("astro_databricks.operators.notebook.DatabricksHook")
 @mock.patch("astro_databricks.operators.notebook.RunsApi")
 @mock.patch(
     "astro_databricks.operators.notebook.DatabricksNotebookOperator._get_api_client"
 )
```

### Comparing `astro_provider_databricks-0.1.0/tests/databricks/test_plugin.py` & `astro_provider_databricks-0.1.1/tests/databricks/test_plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/tests/databricks/test_workflow.py` & `astro_provider_databricks-0.1.1/tests/databricks/test_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             "on_failure": [{"id": "b0aea8ab-ea8c-4a45-a2e9-9a26753fd702"}],
         },
         "email_notifications": {
             "no_alert_for_skipped_runs": True,  # default: False
             "on_start": ["user.name@databricks.com"],
         },
         "git_source": {  # no default value
-            "git_url": "https://github.com/astronomer/astronomer-cosmos",
+            "git_url": "https://github.com/astronomer/astro-provider-databricks",
             "git_provider": "gitHub",
             "git_branch": "main",
         },
     }
     with dag:
         task_group = DatabricksWorkflowTaskGroup(
             group_id="test_workflow",
```

### Comparing `astro_provider_databricks-0.1.0/.gitignore` & `astro_provider_databricks-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/LICENSE` & `astro_provider_databricks-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/README.md` & `astro_provider_databricks-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 <h1 align="center">
   Astro Databricks
 </h1>
   <h3 align="center">
-  Affordable Databricks Workflows in Apache Airflow<br><br>
+  Orchestrate your Databricks notebooks in Airflow and execute them as Databricks Workflows<br><br>
 </h3>
 
 [![Python versions](https://img.shields.io/pypi/pyversions/astro-provider-databricks.svg)](https://pypi.org/pypi/astro-provider-databricks)
 [![License](https://img.shields.io/pypi/l/astro-provider-databricks.svg)](https://pypi.org/pypi/astro-provider-databricks)
 [![Development Status](https://img.shields.io/pypi/status/astro-provider-databricks.svg)](https://pypi.org/pypi/astro-provider-databricks)
 [![PyPI downloads](https://img.shields.io/pypi/dm/astro-provider-databricks.svg)](https://pypistats.org/packages/astro-provider-databricks)
 [![Contributors](https://img.shields.io/github/contributors/astronomer/astro-provider-databricks)](https://github.com/astronomer/astro-provider-databricks)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/astronomer/astro-provider-databricks)](https://github.com/astronomer/astro-provider-databricks)
 [![CI](https://github.com/astronomer/astro-provider-databricks/actions/workflows/ci.yml/badge.svg)](https://github.com/astronomer/astro-provider-databricks)
 [![codecov](https://codecov.io/gh/astronomer/astro-provider-databricks/branch/main/graph/badge.svg?token=MI4SSE50Q6)](https://codecov.io/gh/astronomer/astro-provider-databricks)
 
 
-**Astro Databricks** is an [Apache Airflow](https://github.com/apache/airflow) provider created by [Astronomer](https://www.astronomer.io/) for an **optimal Databricks experience**.  With the `DatabricksTaskGroup`, Astro Datatricks allows you to run from Databricks workflows without
-the need of running Jobs individually, which can result in [75% cost reduction](https://www.databricks.com/product/aws-pricing).
+The **Astro Databricks Provider** is an [Apache Airflow](https://github.com/apache/airflow) provider created by [Astronomer](https://www.astronomer.io/) to run your Databricks notebooks as Databricks Workflows while maintaining Airflow as the authoring interface. When using the `DatabricksTaskGroup` and `DatabricksNotebookOperator`, notebooks run as a Databricks Workflow which can result in a [75% cost reduction](https://www.databricks.com/product/aws-pricing) ($0.40/DBU for all-purpose compute, $0.10/DBU for Jobs compute).
 
 ## Prerequisites
 
 * Apache Airflow >= 2.2.4
 * Python >= 2.7
 * Databricks account
 * Previously created Databricks Notebooks
@@ -43,42 +42,52 @@
 
     ```shell
     export AIRFLOW_HOME=`pwd`
    
     airflow db init
     ```
    
-4. [Create using your preferred way](https://airflow.apache.org/docs/apache-airflow/stable/howto/connection.html) a Databricks Airflow connection (so Airflow can access Databricks using your credentials). This can be done by running the following command, replacing the login and password (with your access token):
+4. [Create a Databricks connection in Airflow](https://airflow.apache.org/docs/apache-airflow/stable/howto/connection.html). This can be done by running the following command, replacing the login and password (with your access token):
 
-```shell
-airflow connections add 'databricks_conn' \
-    --conn-json '{
-        "conn_type": "databricks",
-        "login": "some.email@yourcompany.com",
-        "host": "https://dbc-c9390870-65ef.cloud.databricks.com/",
-        "password": "personal-access-token"
-    }'
-```
+   ```shell
+   # If using Airflow 2.3 or higher:
+   airflow connections add 'databricks_conn' \
+       --conn-json '{
+           "conn_type": "databricks",
+           "login": "some.email@yourcompany.com",
+           "host": "https://dbc-c9390870-65ef.cloud.databricks.com/",
+           "password": "personal-access-token"
+       }'
+   
+   # If using Airflow between 2.2.4 and less than 2.3:
+   airflow connections add 'databricks_conn' --conn-type 'databricks' --conn-login 'some.email@yourcompany.com' --conn-host 'https://dbc-9c390870-65ef.cloud.databricks.com/' --conn-password 'personal-access-token'
+   ```
 
 5. Copy the following workflow into a file named `example_databricks_workflow.py` and add it to the `dags` directory of your Airflow project:
    
    https://github.com/astronomer/astro-provider-databricks/blob/45897543a5e34d446c84b3fbc4f6f7a3ed16cdf7/example_dags/example_databricks_workflow.py#L48-L101
 
    Alternatively, you can download `example_databricks_workflow.py`
    ```shell
-    curl -O https://raw.githubusercontent.com/astronomer/astro-provider-databricks/main/example_dags/example_databricks_workflow.py
+   curl -O https://raw.githubusercontent.com/astronomer/astro-provider-databricks/main/example_dags/example_databricks_workflow.py
    ```
 
 6. Run the example DAG:
 
-    ```sh
+    ```shell
     airflow dags test example_databricks_workflow `date -Iseconds`
     ```
    
-This will create a Databricks Workflow with two Notebook jobs.
+    Which will log, among other lines, the link to the Databricks Job Run URL:
+    ```shell
+    [2023-03-13 15:27:09,934] {notebook.py:158} INFO - Check the job run in Databricks: https://dbc-c9390870-65ef.cloud.databricks.com/?o=4256138892007661#job/950578808520081/run/14940832
+    ```
+   
+    This will create a Databricks Workflow with two Notebook jobs. This workflow may take two minutes to complete if the cluster is already up & running or approximately five minutes depending on your cluster initialisation time.
+ 
 
 ## Available features
 
 * `DatabricksWorkflowTaskGroup`: Airflow [task group](https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/dags.html#taskgroups) that allows users to create a [Databricks Workflow](https://www.databricks.com/product/workflows).
 * `DatabricksNotebookOperator`: Airflow [operator](https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/operators.html) which abstracts a pre-existing [Databricks Notebook](https://docs.databricks.com/notebooks/). Can be used independently to run the Notebook, or within a Databricks Workflow Task Group.
 * `AstroDatabricksPlugin`: An Airflow [plugin](https://airflow.apache.org/docs/apache-airflow/stable/authoring-and-scheduling/plugins.html) which is installed by the default. It allows users, by using the UI, to view a Databricks job and retry running it in case of failure.
 
@@ -98,8 +107,8 @@
 
 Read the [Contribution Guidelines](docs/contributing.rst) for a detailed overview on how to contribute.
 
 Contributors and maintainers should abide by the [Contributor Code of Conduct](CODE_OF_CONDUCT.md).
 
 ## License
 
-[Apache Licence 2.0](LICENSE)
+[Apache Licence 2.0](LICENSE)
```

### Comparing `astro_provider_databricks-0.1.0/pyproject.toml` & `astro_provider_databricks-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.1.0/PKG-INFO` & `astro_provider_databricks-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-provider-databricks
-Version: 0.1.0
+Version: 0.1.1
 Summary: Affordable Databricks Workflows in Apache Airflow
 Project-URL: Homepage, https://github.com/astronomer/astro-provider-databricks/
 Project-URL: Documentation, https://github.com/astronomer/astro-provider-databricks/
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags
@@ -43,29 +43,28 @@
 Requires-Dist: types-requests; extra == 'tests'
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   Astro Databricks
 </h1>
   <h3 align="center">
-  Affordable Databricks Workflows in Apache Airflow<br><br>
+  Orchestrate your Databricks notebooks in Airflow and execute them as Databricks Workflows<br><br>
 </h3>
 
 [![Python versions](https://img.shields.io/pypi/pyversions/astro-provider-databricks.svg)](https://pypi.org/pypi/astro-provider-databricks)
 [![License](https://img.shields.io/pypi/l/astro-provider-databricks.svg)](https://pypi.org/pypi/astro-provider-databricks)
 [![Development Status](https://img.shields.io/pypi/status/astro-provider-databricks.svg)](https://pypi.org/pypi/astro-provider-databricks)
 [![PyPI downloads](https://img.shields.io/pypi/dm/astro-provider-databricks.svg)](https://pypistats.org/packages/astro-provider-databricks)
 [![Contributors](https://img.shields.io/github/contributors/astronomer/astro-provider-databricks)](https://github.com/astronomer/astro-provider-databricks)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/astronomer/astro-provider-databricks)](https://github.com/astronomer/astro-provider-databricks)
 [![CI](https://github.com/astronomer/astro-provider-databricks/actions/workflows/ci.yml/badge.svg)](https://github.com/astronomer/astro-provider-databricks)
 [![codecov](https://codecov.io/gh/astronomer/astro-provider-databricks/branch/main/graph/badge.svg?token=MI4SSE50Q6)](https://codecov.io/gh/astronomer/astro-provider-databricks)
 
 
-**Astro Databricks** is an [Apache Airflow](https://github.com/apache/airflow) provider created by [Astronomer](https://www.astronomer.io/) for an **optimal Databricks experience**.  With the `DatabricksTaskGroup`, Astro Datatricks allows you to run from Databricks workflows without
-the need of running Jobs individually, which can result in [75% cost reduction](https://www.databricks.com/product/aws-pricing).
+The **Astro Databricks Provider** is an [Apache Airflow](https://github.com/apache/airflow) provider created by [Astronomer](https://www.astronomer.io/) to run your Databricks notebooks as Databricks Workflows while maintaining Airflow as the authoring interface. When using the `DatabricksTaskGroup` and `DatabricksNotebookOperator`, notebooks run as a Databricks Workflow which can result in a [75% cost reduction](https://www.databricks.com/product/aws-pricing) ($0.40/DBU for all-purpose compute, $0.10/DBU for Jobs compute).
 
 ## Prerequisites
 
 * Apache Airflow >= 2.2.4
 * Python >= 2.7
 * Databricks account
 * Previously created Databricks Notebooks
@@ -88,42 +87,52 @@
 
     ```shell
     export AIRFLOW_HOME=`pwd`
    
     airflow db init
     ```
    
-4. [Create using your preferred way](https://airflow.apache.org/docs/apache-airflow/stable/howto/connection.html) a Databricks Airflow connection (so Airflow can access Databricks using your credentials). This can be done by running the following command, replacing the login and password (with your access token):
+4. [Create a Databricks connection in Airflow](https://airflow.apache.org/docs/apache-airflow/stable/howto/connection.html). This can be done by running the following command, replacing the login and password (with your access token):
 
-```shell
-airflow connections add 'databricks_conn' \
-    --conn-json '{
-        "conn_type": "databricks",
-        "login": "some.email@yourcompany.com",
-        "host": "https://dbc-c9390870-65ef.cloud.databricks.com/",
-        "password": "personal-access-token"
-    }'
-```
+   ```shell
+   # If using Airflow 2.3 or higher:
+   airflow connections add 'databricks_conn' \
+       --conn-json '{
+           "conn_type": "databricks",
+           "login": "some.email@yourcompany.com",
+           "host": "https://dbc-c9390870-65ef.cloud.databricks.com/",
+           "password": "personal-access-token"
+       }'
+   
+   # If using Airflow between 2.2.4 and less than 2.3:
+   airflow connections add 'databricks_conn' --conn-type 'databricks' --conn-login 'some.email@yourcompany.com' --conn-host 'https://dbc-9c390870-65ef.cloud.databricks.com/' --conn-password 'personal-access-token'
+   ```
 
 5. Copy the following workflow into a file named `example_databricks_workflow.py` and add it to the `dags` directory of your Airflow project:
    
    https://github.com/astronomer/astro-provider-databricks/blob/45897543a5e34d446c84b3fbc4f6f7a3ed16cdf7/example_dags/example_databricks_workflow.py#L48-L101
 
    Alternatively, you can download `example_databricks_workflow.py`
    ```shell
-    curl -O https://raw.githubusercontent.com/astronomer/astro-provider-databricks/main/example_dags/example_databricks_workflow.py
+   curl -O https://raw.githubusercontent.com/astronomer/astro-provider-databricks/main/example_dags/example_databricks_workflow.py
    ```
 
 6. Run the example DAG:
 
-    ```sh
+    ```shell
     airflow dags test example_databricks_workflow `date -Iseconds`
     ```
    
-This will create a Databricks Workflow with two Notebook jobs.
+    Which will log, among other lines, the link to the Databricks Job Run URL:
+    ```shell
+    [2023-03-13 15:27:09,934] {notebook.py:158} INFO - Check the job run in Databricks: https://dbc-c9390870-65ef.cloud.databricks.com/?o=4256138892007661#job/950578808520081/run/14940832
+    ```
+   
+    This will create a Databricks Workflow with two Notebook jobs. This workflow may take two minutes to complete if the cluster is already up & running or approximately five minutes depending on your cluster initialisation time.
+ 
 
 ## Available features
 
 * `DatabricksWorkflowTaskGroup`: Airflow [task group](https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/dags.html#taskgroups) that allows users to create a [Databricks Workflow](https://www.databricks.com/product/workflows).
 * `DatabricksNotebookOperator`: Airflow [operator](https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/operators.html) which abstracts a pre-existing [Databricks Notebook](https://docs.databricks.com/notebooks/). Can be used independently to run the Notebook, or within a Databricks Workflow Task Group.
 * `AstroDatabricksPlugin`: An Airflow [plugin](https://airflow.apache.org/docs/apache-airflow/stable/authoring-and-scheduling/plugins.html) which is installed by the default. It allows users, by using the UI, to view a Databricks job and retry running it in case of failure.
 
@@ -143,8 +152,8 @@
 
 Read the [Contribution Guidelines](docs/contributing.rst) for a detailed overview on how to contribute.
 
 Contributors and maintainers should abide by the [Contributor Code of Conduct](CODE_OF_CONDUCT.md).
 
 ## License
 
-[Apache Licence 2.0](LICENSE)
+[Apache Licence 2.0](LICENSE)
```

