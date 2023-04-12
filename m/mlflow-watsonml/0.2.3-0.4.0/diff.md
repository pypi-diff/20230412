# Comparing `tmp/mlflow-watsonml-0.2.3.tar.gz` & `tmp/mlflow-watsonml-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-watsonml-0.2.3.tar", last modified: Thu Mar 30 16:09:44 2023, max compression
+gzip compressed data, was "mlflow-watsonml-0.4.0.tar", last modified: Wed Apr 12 17:46:18 2023, max compression
```

## Comparing `mlflow-watsonml-0.2.3.tar` & `mlflow-watsonml-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:09:44.398040 mlflow-watsonml-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-30 16:09:44.398040 mlflow-watsonml-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-30 16:09:30.000000 mlflow-watsonml-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:09:44.398040 mlflow-watsonml-0.2.3/mlflow_watsonml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:09:44.398040 mlflow-watsonml-0.2.3/mlflow_watsonml/mlflow_watsonml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-30 16:09:44.000000 mlflow-watsonml-0.2.3/mlflow_watsonml/mlflow_watsonml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-30 16:09:44.000000 mlflow-watsonml-0.2.3/mlflow_watsonml/mlflow_watsonml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:09:44.000000 mlflow-watsonml-0.2.3/mlflow_watsonml/mlflow_watsonml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-30 16:09:44.000000 mlflow-watsonml-0.2.3/mlflow_watsonml/mlflow_watsonml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-30 16:09:44.000000 mlflow-watsonml-0.2.3/mlflow_watsonml/mlflow_watsonml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:09:44.000000 mlflow-watsonml-0.2.3/mlflow_watsonml/mlflow_watsonml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 16:09:44.398040 mlflow-watsonml-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-30 16:09:30.000000 mlflow-watsonml-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:46:18.655291 mlflow-watsonml-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-12 17:46:18.655291 mlflow-watsonml-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:46:18.651291 mlflow-watsonml-0.4.0/mlflow_watsonml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/mlflow_watsonml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/mlflow_watsonml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/mlflow_watsonml/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/mlflow_watsonml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/mlflow_watsonml/wml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:46:18.655291 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 17:46:18.000000 mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:46:18.655291 mlflow-watsonml-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-12 17:46:09.000000 mlflow-watsonml-0.4.0/setup.py
```

### Comparing `mlflow-watsonml-0.2.3/PKG-INFO` & `mlflow-watsonml-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,53 @@
-Metadata-Version: 2.1
-Name: mlflow-watsonml
-Version: 0.2.3
-Summary: WatsonML MLflow deployment plugin
-Home-page: https://github.com/IBM/mlflow-watsonml
-Author: IBM AI Model Factory team
-Author-email: dhruv.shah@ibm.com
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+# Mlflow-WatsonML
 
-# Mlflow-watsonml
-
-A plugin that integrates [watsonml](http://ibm-wml-api-pyclient.mybluemix.net) with MLflow pipeline.
-``mlflow_watsonml`` enables mlflow users to deploy mlflow pipeline models into watsonml.
+A plugin that integrates [WatsonML](http://ibm-wml-api-pyclient.mybluemix.net) with MLflow pipeline.
+``mlflow_watsonml`` enables mlflow users to deploy mlflow pipeline models into WatsonML.
 Command line APIs of the plugin (also accessible through mlflow's python package) makes the deployment process seamless.
 
-## Prerequisites
-
-Following are the list of packages which needs to be installed before running the watsonml deployment plugin
-
-1. ibm-watson-machine-learning
-2. pydotenv
-3. mlflow
-
-
 ## Installation
 Plugin package which is available in pypi and can be installed using
 
 ```bash
 pip install mlflow-watsonml
 ```
 
 ## What does it do
-Installing this package uses python's entrypoint mechanism to register the plugin into MLflow's
-plugin registry. This registry will be invoked each time you launch MLflow script or command line
-argument.
+Installing this package uses python's entrypoint mechanism to register the plugin into MLflow's plugin registry. This registry will be invoked each time you launch MLflow script or command line argument.
+
+## Authentication
+In order to connect to WatsonML, refer to [.env.template](.env.template)
 
 
 ### Create deployment
 The `create` command line argument and ``create_deployment`` python
-APIs does the deployment of a model built with MLflow to watsonml.
+APIs does the deployment of a model built with MLflow to WatsonML.
 
 ##### CLI
 ```shell script
-mlflow deployments create -t watsonml -m <model-uri> --name <deployment-name> -C "software_spec_type=runtime-22.1-py3.9"
+mlflow deployments create -t watsonml -m <model-uri> --name <deployment-name> -C "software_spec_type=runtime-22.2-py3.10"
 ```
 
 ##### Python API
 ```python
 from mlflow.deployments import get_deploy_client
 
 target_uri = 'watsonml'
 plugin = get_deploy_client(target_uri)
 
 plugin.create_deployment(
     name=<deployment-name>, 
     model_uri=<model-uri>, 
-    config={"software_spec_type": "runtime-22.1-py3.9"}
+    config={"software_spec_type": "runtime-22.2-py3.10"}
 )
 ```
 
 ### Update deployment
 Update API can used to modify the configuration parameters such as number of workers, version etc., of an already deployed model.
-watsonml will make sure the user experience is seamless while changing the model in a live environment.
+WatsonML will make sure the user experience is seamless while changing the model in a live environment.
 
 ##### CLI
 ```shell script
 mlflow deployments update -t watsonml --name <deployment name> -C "software_spec_type=runtime-22.1-py3.10"
 ```
 
 ##### Python API
@@ -80,49 +61,47 @@
 ##### CLI
 ```shell script
 mlflow deployments delete -t watsonml --name <deployment name / version number>
 ```
 
 ##### Python API
 ```python
-plugin.delete_deployment(name=<deployment name / version number>)
+plugin.delete_deployment(name=<deployment name>)
 ```
 
 ### List all deployments
-Lists the names of all the models deployed on the configured watsonml.
+Lists the names of all the models deployed on the configured WatsonML.
 
 ##### CLI
 ```shell script
 mlflow deployments list -t watsonml
 ```
 
 ##### Python API
 ```python
 plugin.list_deployments()
 ```
 
 ### Get deployment details
-Get API fetches the details of the deployed model. By default, Get API fetches all the versions of the 
-deployed model.
+Get API fetches the details of the deployed model. By default, Get API fetches all the versions of the deployed model.
 
 ##### CLI
 ```shell script
 mlflow deployments get -t watsonml --name <deployment name>
 ```
 
 ##### Python API
 ```python
 plugin.get_deployment(name=<deployment name>)
 ```
 
 ### Run Prediction on deployed model
 Predict API enables to run prediction on the deployed model.
 
-For the prediction inputs, DataFrame, Tensor and Json formats are supported. The python API supports all of these
- three formats. When invoked via command line, one needs to pass the json file path that contains the inputs.
+For the prediction inputs, DataFrame and JSON formats are supported. The python API supports all of these three formats. When invoked via command line, one needs to pass the json file path that contains the inputs.
 
 ##### CLI
 ```shell script
 mlflow deployments predict -t watsonml --name <deployment name> --input-path <input file path> --output-path <output file path>
 ```
 
 output-path is an optional parameter. Without output path parameter result will be printed in console.
```

### Comparing `mlflow-watsonml-0.2.3/README.md` & `mlflow-watsonml-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,64 @@
-# Mlflow-watsonml
+Metadata-Version: 2.1
+Name: mlflow-watsonml
+Version: 0.4.0
+Summary: WatsonML MLflow deployment plugin
+Home-page: https://github.com/IBM/mlflow-watsonml
+Author: IBM AI Model Factory team
+Author-email: dhruv.shah@ibm.com
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
 
-A plugin that integrates [watsonml](http://ibm-wml-api-pyclient.mybluemix.net) with MLflow pipeline.
-``mlflow_watsonml`` enables mlflow users to deploy mlflow pipeline models into watsonml.
-Command line APIs of the plugin (also accessible through mlflow's python package) makes the deployment process seamless.
-
-## Prerequisites
-
-Following are the list of packages which needs to be installed before running the watsonml deployment plugin
-
-1. ibm-watson-machine-learning
-2. pydotenv
-3. mlflow
+# Mlflow-WatsonML
 
+A plugin that integrates [WatsonML](http://ibm-wml-api-pyclient.mybluemix.net) with MLflow pipeline.
+``mlflow_watsonml`` enables mlflow users to deploy mlflow pipeline models into WatsonML.
+Command line APIs of the plugin (also accessible through mlflow's python package) makes the deployment process seamless.
 
 ## Installation
 Plugin package which is available in pypi and can be installed using
 
 ```bash
 pip install mlflow-watsonml
 ```
 
 ## What does it do
-Installing this package uses python's entrypoint mechanism to register the plugin into MLflow's
-plugin registry. This registry will be invoked each time you launch MLflow script or command line
-argument.
+Installing this package uses python's entrypoint mechanism to register the plugin into MLflow's plugin registry. This registry will be invoked each time you launch MLflow script or command line argument.
+
+## Authentication
+In order to connect to WatsonML, refer to [.env.template](.env.template)
 
 
 ### Create deployment
 The `create` command line argument and ``create_deployment`` python
-APIs does the deployment of a model built with MLflow to watsonml.
+APIs does the deployment of a model built with MLflow to WatsonML.
 
 ##### CLI
 ```shell script
-mlflow deployments create -t watsonml -m <model-uri> --name <deployment-name> -C "software_spec_type=runtime-22.1-py3.9"
+mlflow deployments create -t watsonml -m <model-uri> --name <deployment-name> -C "software_spec_type=runtime-22.2-py3.10"
 ```
 
 ##### Python API
 ```python
 from mlflow.deployments import get_deploy_client
 
 target_uri = 'watsonml'
 plugin = get_deploy_client(target_uri)
 
 plugin.create_deployment(
     name=<deployment-name>, 
     model_uri=<model-uri>, 
-    config={"software_spec_type": "runtime-22.1-py3.9"}
+    config={"software_spec_type": "runtime-22.2-py3.10"}
 )
 ```
 
 ### Update deployment
 Update API can used to modify the configuration parameters such as number of workers, version etc., of an already deployed model.
-watsonml will make sure the user experience is seamless while changing the model in a live environment.
+WatsonML will make sure the user experience is seamless while changing the model in a live environment.
 
 ##### CLI
 ```shell script
 mlflow deployments update -t watsonml --name <deployment name> -C "software_spec_type=runtime-22.1-py3.10"
 ```
 
 ##### Python API
@@ -69,49 +72,47 @@
 ##### CLI
 ```shell script
 mlflow deployments delete -t watsonml --name <deployment name / version number>
 ```
 
 ##### Python API
 ```python
-plugin.delete_deployment(name=<deployment name / version number>)
+plugin.delete_deployment(name=<deployment name>)
 ```
 
 ### List all deployments
-Lists the names of all the models deployed on the configured watsonml.
+Lists the names of all the models deployed on the configured WatsonML.
 
 ##### CLI
 ```shell script
 mlflow deployments list -t watsonml
 ```
 
 ##### Python API
 ```python
 plugin.list_deployments()
 ```
 
 ### Get deployment details
-Get API fetches the details of the deployed model. By default, Get API fetches all the versions of the 
-deployed model.
+Get API fetches the details of the deployed model. By default, Get API fetches all the versions of the deployed model.
 
 ##### CLI
 ```shell script
 mlflow deployments get -t watsonml --name <deployment name>
 ```
 
 ##### Python API
 ```python
 plugin.get_deployment(name=<deployment name>)
 ```
 
 ### Run Prediction on deployed model
 Predict API enables to run prediction on the deployed model.
 
-For the prediction inputs, DataFrame, Tensor and Json formats are supported. The python API supports all of these
- three formats. When invoked via command line, one needs to pass the json file path that contains the inputs.
+For the prediction inputs, DataFrame and JSON formats are supported. The python API supports all of these three formats. When invoked via command line, one needs to pass the json file path that contains the inputs.
 
 ##### CLI
 ```shell script
 mlflow deployments predict -t watsonml --name <deployment name> --input-path <input file path> --output-path <output file path>
 ```
 
 output-path is an optional parameter. Without output path parameter result will be printed in console.
```

### Comparing `mlflow-watsonml-0.2.3/mlflow_watsonml/mlflow_watsonml.egg-info/PKG-INFO` & `mlflow-watsonml-0.4.0/mlflow_watsonml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,64 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.2.3
+Version: 0.4.0
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-# Mlflow-watsonml
+# Mlflow-WatsonML
 
-A plugin that integrates [watsonml](http://ibm-wml-api-pyclient.mybluemix.net) with MLflow pipeline.
-``mlflow_watsonml`` enables mlflow users to deploy mlflow pipeline models into watsonml.
+A plugin that integrates [WatsonML](http://ibm-wml-api-pyclient.mybluemix.net) with MLflow pipeline.
+``mlflow_watsonml`` enables mlflow users to deploy mlflow pipeline models into WatsonML.
 Command line APIs of the plugin (also accessible through mlflow's python package) makes the deployment process seamless.
 
-## Prerequisites
-
-Following are the list of packages which needs to be installed before running the watsonml deployment plugin
-
-1. ibm-watson-machine-learning
-2. pydotenv
-3. mlflow
-
-
 ## Installation
 Plugin package which is available in pypi and can be installed using
 
 ```bash
 pip install mlflow-watsonml
 ```
 
 ## What does it do
-Installing this package uses python's entrypoint mechanism to register the plugin into MLflow's
-plugin registry. This registry will be invoked each time you launch MLflow script or command line
-argument.
+Installing this package uses python's entrypoint mechanism to register the plugin into MLflow's plugin registry. This registry will be invoked each time you launch MLflow script or command line argument.
+
+## Authentication
+In order to connect to WatsonML, refer to [.env.template](.env.template)
 
 
 ### Create deployment
 The `create` command line argument and ``create_deployment`` python
-APIs does the deployment of a model built with MLflow to watsonml.
+APIs does the deployment of a model built with MLflow to WatsonML.
 
 ##### CLI
 ```shell script
-mlflow deployments create -t watsonml -m <model-uri> --name <deployment-name> -C "software_spec_type=runtime-22.1-py3.9"
+mlflow deployments create -t watsonml -m <model-uri> --name <deployment-name> -C "software_spec_type=runtime-22.2-py3.10"
 ```
 
 ##### Python API
 ```python
 from mlflow.deployments import get_deploy_client
 
 target_uri = 'watsonml'
 plugin = get_deploy_client(target_uri)
 
 plugin.create_deployment(
     name=<deployment-name>, 
     model_uri=<model-uri>, 
-    config={"software_spec_type": "runtime-22.1-py3.9"}
+    config={"software_spec_type": "runtime-22.2-py3.10"}
 )
 ```
 
 ### Update deployment
 Update API can used to modify the configuration parameters such as number of workers, version etc., of an already deployed model.
-watsonml will make sure the user experience is seamless while changing the model in a live environment.
+WatsonML will make sure the user experience is seamless while changing the model in a live environment.
 
 ##### CLI
 ```shell script
 mlflow deployments update -t watsonml --name <deployment name> -C "software_spec_type=runtime-22.1-py3.10"
 ```
 
 ##### Python API
@@ -80,49 +72,47 @@
 ##### CLI
 ```shell script
 mlflow deployments delete -t watsonml --name <deployment name / version number>
 ```
 
 ##### Python API
 ```python
-plugin.delete_deployment(name=<deployment name / version number>)
+plugin.delete_deployment(name=<deployment name>)
 ```
 
 ### List all deployments
-Lists the names of all the models deployed on the configured watsonml.
+Lists the names of all the models deployed on the configured WatsonML.
 
 ##### CLI
 ```shell script
 mlflow deployments list -t watsonml
 ```
 
 ##### Python API
 ```python
 plugin.list_deployments()
 ```
 
 ### Get deployment details
-Get API fetches the details of the deployed model. By default, Get API fetches all the versions of the 
-deployed model.
+Get API fetches the details of the deployed model. By default, Get API fetches all the versions of the deployed model.
 
 ##### CLI
 ```shell script
 mlflow deployments get -t watsonml --name <deployment name>
 ```
 
 ##### Python API
 ```python
 plugin.get_deployment(name=<deployment name>)
 ```
 
 ### Run Prediction on deployed model
 Predict API enables to run prediction on the deployed model.
 
-For the prediction inputs, DataFrame, Tensor and Json formats are supported. The python API supports all of these
- three formats. When invoked via command line, one needs to pass the json file path that contains the inputs.
+For the prediction inputs, DataFrame and JSON formats are supported. The python API supports all of these three formats. When invoked via command line, one needs to pass the json file path that contains the inputs.
 
 ##### CLI
 ```shell script
 mlflow deployments predict -t watsonml --name <deployment name> --input-path <input file path> --output-path <output file path>
 ```
 
 output-path is an optional parameter. Without output path parameter result will be printed in console.
```

### Comparing `mlflow-watsonml-0.2.3/setup.py` & `mlflow-watsonml-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 setup(
     name="mlflow-watsonml",
     version=version,
     description="WatsonML MLflow deployment plugin",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IBM/mlflow-watsonml",
-    package_dir={"": "mlflow_watsonml"},
-    packages=find_packages(where="mlflow_watsonml"),
+    packages=["mlflow_watsonml"],
     author="IBM AI Model Factory team",
     author_email="dhruv.shah@ibm.com",
     install_requires=install_requires,
     extras_require={"dev": ["ipython", "black", "pytest", "build", "wheel", "twine"]},
     entry_points={"mlflow.deployments": "watsonml=mlflow_watsonml.deploy"},
     python_requires=">=3.9",
 )
```

