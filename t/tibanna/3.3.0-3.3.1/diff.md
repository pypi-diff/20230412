# Comparing `tmp/tibanna-3.3.0.tar.gz` & `tmp/tibanna-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibanna-3.3.0.tar", max compression
+gzip compressed data, was "tibanna-3.3.1.tar", max compression
```

## Comparing `tibanna-3.3.0.tar` & `tibanna-3.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rwxr-xr-x   0        0        0     1083 2021-02-24 22:20:32.790882 tibanna-3.3.0/LICENSE.txt
--rwxr-xr-x   0        0        0     2391 2022-04-12 18:14:11.086288 tibanna-3.3.0/README.md
--rwxr-xr-x   0        0        0        0 2021-02-24 22:20:32.794409 tibanna-3.3.0/awsf3/__init__.py
--rwxr-xr-x   0        0        0     5058 2022-03-22 14:50:29.279994 tibanna-3.3.0/awsf3/__main__.py
--rwxr-xr-x   0        0        0    12351 2023-03-20 16:18:32.417979 tibanna-3.3.0/awsf3/aws_run_workflow_generic.sh
--rw-r--r--   0        0        0     1000 2023-03-22 15:34:35.007839 tibanna-3.3.0/awsf3/cloudwatch_agent_config.json
--rw-r--r--   0        0        0     1003 2021-02-24 22:20:32.794931 tibanna-3.3.0/awsf3/log.py
--rw-r--r--   0        0        0     1629 2022-03-22 14:50:29.283309 tibanna-3.3.0/awsf3/spot_failure_detection.sh
--rwxr-xr-x   0        0        0    11814 2022-03-22 14:50:29.284914 tibanna-3.3.0/awsf3/target.py
--rw-r--r--   0        0        0    20670 2022-12-06 18:20:49.560464 tibanna-3.3.0/awsf3/utils.py
--rw-r--r--   0        0        0     1940 2023-03-22 15:34:35.010022 tibanna-3.3.0/pyproject.toml
--rwxr-xr-x   0        0        0      905 2021-02-24 22:20:33.102923 tibanna-3.3.0/tibanna/__init__.py
--rwxr-xr-x   0        0        0    32555 2022-12-06 18:20:49.647426 tibanna-3.3.0/tibanna/__main__.py
--rwxr-xr-x   0        0        0      717 2022-10-31 13:42:10.422020 tibanna-3.3.0/tibanna/_version.py
--rwxr-xr-x   0        0        0     8393 2023-03-16 18:26:02.672939 tibanna-3.3.0/tibanna/ami.py
--rwxr-xr-x   0        0        0    16648 2023-03-16 18:26:02.674092 tibanna-3.3.0/tibanna/awsem.py
--rwxr-xr-x   0        0        0      964 2021-02-24 22:20:33.120382 tibanna-3.3.0/tibanna/base.py
--rwxr-xr-x   0        0        0    12072 2023-03-22 15:34:35.011986 tibanna-3.3.0/tibanna/check_task.py
--rwxr-xr-x   0        0        0    59272 2022-12-06 18:20:49.670461 tibanna-3.3.0/tibanna/core.py
--rw-r--r--   0        0        0      680 2022-12-06 18:20:49.676312 tibanna-3.3.0/tibanna/create_ami_userdata
--rwxr-xr-x   0        0        0    56161 2023-03-22 15:34:35.012952 tibanna-3.3.0/tibanna/cw_utils.py
--rwxr-xr-x   0        0        0     3196 2021-02-24 22:20:33.137619 tibanna-3.3.0/tibanna/dd_utils.py
--rwxr-xr-x   0        0        0    53996 2023-03-22 15:34:35.014084 tibanna-3.3.0/tibanna/ec2_utils.py
--rwxr-xr-x   0        0        0     4326 2022-11-03 20:17:39.217693 tibanna-3.3.0/tibanna/exceptions.py
--rwxr-xr-x   0        0        0    30382 2022-12-06 18:20:49.689939 tibanna-3.3.0/tibanna/iam_utils.py
--rw-r--r--   0        0        0    12760 2023-03-16 18:26:02.674930 tibanna-3.3.0/tibanna/job.py
--rwxr-xr-x   0        0        0      111 2021-03-16 13:52:19.436482 tibanna-3.3.0/tibanna/lambdas/__init__.py
--rwxr-xr-x   0        0        0      522 2022-04-12 18:11:48.701463 tibanna-3.3.0/tibanna/lambdas/check_task_awsem.py
--rwxr-xr-x   0        0        0       68 2023-03-22 15:34:35.015634 tibanna-3.3.0/tibanna/lambdas/requirements.txt
--rwxr-xr-x   0        0        0      471 2022-04-12 18:11:48.711468 tibanna-3.3.0/tibanna/lambdas/run_task_awsem.py
--rwxr-xr-x   0        0        0      491 2022-04-12 18:11:48.719469 tibanna-3.3.0/tibanna/lambdas/update_cost_awsem.py
--rwxr-xr-x   0        0        0     2757 2021-02-24 22:20:33.153185 tibanna-3.3.0/tibanna/nnested_array.py
--rwxr-xr-x   0        0        0    19075 2022-12-06 18:20:49.706362 tibanna-3.3.0/tibanna/pricing_utils.py
--rwxr-xr-x   0        0        0     3215 2021-04-19 16:08:03.718285 tibanna-3.3.0/tibanna/run_task.py
--rwxr-xr-x   0        0        0     3418 2022-10-31 13:42:10.450245 tibanna-3.3.0/tibanna/stepfunction.py
--rwxr-xr-x   0        0        0     2469 2021-09-27 13:44:50.867418 tibanna-3.3.0/tibanna/stepfunction_cost_updater.py
--rw-r--r--   0        0        0    17156 2021-09-27 13:51:09.655388 tibanna-3.3.0/tibanna/top.py
--rwxr-xr-x   0        0        0     2203 2021-03-16 13:52:19.439863 tibanna-3.3.0/tibanna/update_cost.py
--rwxr-xr-x   0        0        0     6671 2022-03-22 14:50:29.302765 tibanna-3.3.0/tibanna/utils.py
--rwxr-xr-x   0        0        0     6290 2023-03-22 15:34:35.016604 tibanna-3.3.0/tibanna/vars.py
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 tibanna-3.3.0/setup.py
--rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 tibanna-3.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1083 2021-02-24 22:20:32.790882 tibanna-3.3.1/LICENSE.txt
+-rwxr-xr-x   0        0        0     2391 2022-04-12 18:14:11.086288 tibanna-3.3.1/README.md
+-rwxr-xr-x   0        0        0        0 2021-02-24 22:20:32.794409 tibanna-3.3.1/awsf3/__init__.py
+-rwxr-xr-x   0        0        0     5058 2022-03-22 14:50:29.279994 tibanna-3.3.1/awsf3/__main__.py
+-rwxr-xr-x   0        0        0    12351 2023-03-20 16:18:32.417979 tibanna-3.3.1/awsf3/aws_run_workflow_generic.sh
+-rw-r--r--   0        0        0     1000 2023-03-22 15:34:35.007839 tibanna-3.3.1/awsf3/cloudwatch_agent_config.json
+-rw-r--r--   0        0        0     1003 2021-02-24 22:20:32.794931 tibanna-3.3.1/awsf3/log.py
+-rw-r--r--   0        0        0     1629 2022-03-22 14:50:29.283309 tibanna-3.3.1/awsf3/spot_failure_detection.sh
+-rwxr-xr-x   0        0        0    11814 2022-03-22 14:50:29.284914 tibanna-3.3.1/awsf3/target.py
+-rw-r--r--   0        0        0    20670 2022-12-06 18:20:49.560464 tibanna-3.3.1/awsf3/utils.py
+-rw-r--r--   0        0        0     1940 2023-04-12 16:25:00.555064 tibanna-3.3.1/pyproject.toml
+-rwxr-xr-x   0        0        0      905 2021-02-24 22:20:33.102923 tibanna-3.3.1/tibanna/__init__.py
+-rwxr-xr-x   0        0        0    32555 2022-12-06 18:20:49.647426 tibanna-3.3.1/tibanna/__main__.py
+-rwxr-xr-x   0        0        0      717 2022-10-31 13:42:10.422020 tibanna-3.3.1/tibanna/_version.py
+-rwxr-xr-x   0        0        0     8393 2023-03-16 18:26:02.672939 tibanna-3.3.1/tibanna/ami.py
+-rwxr-xr-x   0        0        0    16648 2023-03-16 18:26:02.674092 tibanna-3.3.1/tibanna/awsem.py
+-rwxr-xr-x   0        0        0      964 2021-02-24 22:20:33.120382 tibanna-3.3.1/tibanna/base.py
+-rwxr-xr-x   0        0        0    12072 2023-03-22 15:34:35.011986 tibanna-3.3.1/tibanna/check_task.py
+-rwxr-xr-x   0        0        0    59272 2022-12-06 18:20:49.670461 tibanna-3.3.1/tibanna/core.py
+-rw-r--r--   0        0        0      680 2022-12-06 18:20:49.676312 tibanna-3.3.1/tibanna/create_ami_userdata
+-rwxr-xr-x   0        0        0    56161 2023-03-22 15:34:35.012952 tibanna-3.3.1/tibanna/cw_utils.py
+-rwxr-xr-x   0        0        0     3196 2021-02-24 22:20:33.137619 tibanna-3.3.1/tibanna/dd_utils.py
+-rwxr-xr-x   0        0        0    53996 2023-03-22 15:34:35.014084 tibanna-3.3.1/tibanna/ec2_utils.py
+-rwxr-xr-x   0        0        0     4326 2022-11-03 20:17:39.217693 tibanna-3.3.1/tibanna/exceptions.py
+-rwxr-xr-x   0        0        0    30382 2022-12-06 18:20:49.689939 tibanna-3.3.1/tibanna/iam_utils.py
+-rw-r--r--   0        0        0    12760 2023-03-16 18:26:02.674930 tibanna-3.3.1/tibanna/job.py
+-rwxr-xr-x   0        0        0      111 2021-03-16 13:52:19.436482 tibanna-3.3.1/tibanna/lambdas/__init__.py
+-rwxr-xr-x   0        0        0      522 2022-04-12 18:11:48.701463 tibanna-3.3.1/tibanna/lambdas/check_task_awsem.py
+-rwxr-xr-x   0        0        0       68 2023-04-12 16:25:00.555651 tibanna-3.3.1/tibanna/lambdas/requirements.txt
+-rwxr-xr-x   0        0        0      471 2022-04-12 18:11:48.711468 tibanna-3.3.1/tibanna/lambdas/run_task_awsem.py
+-rwxr-xr-x   0        0        0      491 2022-04-12 18:11:48.719469 tibanna-3.3.1/tibanna/lambdas/update_cost_awsem.py
+-rwxr-xr-x   0        0        0     2757 2021-02-24 22:20:33.153185 tibanna-3.3.1/tibanna/nnested_array.py
+-rwxr-xr-x   0        0        0    19075 2022-12-06 18:20:49.706362 tibanna-3.3.1/tibanna/pricing_utils.py
+-rwxr-xr-x   0        0        0     3215 2021-04-19 16:08:03.718285 tibanna-3.3.1/tibanna/run_task.py
+-rwxr-xr-x   0        0        0     3418 2022-10-31 13:42:10.450245 tibanna-3.3.1/tibanna/stepfunction.py
+-rwxr-xr-x   0        0        0     2469 2021-09-27 13:44:50.867418 tibanna-3.3.1/tibanna/stepfunction_cost_updater.py
+-rw-r--r--   0        0        0    17156 2021-09-27 13:51:09.655388 tibanna-3.3.1/tibanna/top.py
+-rwxr-xr-x   0        0        0     2203 2021-03-16 13:52:19.439863 tibanna-3.3.1/tibanna/update_cost.py
+-rwxr-xr-x   0        0        0     6671 2022-03-22 14:50:29.302765 tibanna-3.3.1/tibanna/utils.py
+-rwxr-xr-x   0        0        0     6290 2023-03-22 15:34:35.016604 tibanna-3.3.1/tibanna/vars.py
+-rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 tibanna-3.3.1/setup.py
+-rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 tibanna-3.3.1/PKG-INFO
```

### Comparing `tibanna-3.3.0/LICENSE.txt` & `tibanna-3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/README.md` & `tibanna-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/awsf3/__main__.py` & `tibanna-3.3.1/awsf3/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/awsf3/aws_run_workflow_generic.sh` & `tibanna-3.3.1/awsf3/aws_run_workflow_generic.sh`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/awsf3/cloudwatch_agent_config.json` & `tibanna-3.3.1/awsf3/cloudwatch_agent_config.json`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/awsf3/log.py` & `tibanna-3.3.1/awsf3/log.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/awsf3/spot_failure_detection.sh` & `tibanna-3.3.1/awsf3/spot_failure_detection.sh`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/awsf3/target.py` & `tibanna-3.3.1/awsf3/target.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/awsf3/utils.py` & `tibanna-3.3.1/awsf3/utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/pyproject.toml` & `tibanna-3.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tibanna"
-version = "3.3.0"
+version = "3.3.1"
 description = "Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["tibanna"]
 homepage = "http://github.com/4dn-dcic/tibanna"
 repository = "http://github.com/4dn-dcic/tibanna.git"
@@ -28,15 +28,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.9"
 python-lambda-4dn = "0.12.3"
 boto3 = "^1.9.0"
 botocore = "^1.12.1"
 requests = "2.27.1"
-Benchmark-4dn = "^0.5.21"
+Benchmark-4dn = "^0.5.23"
 tomlkit = "^0.11.0"
 
 [tool.poetry.dev-dependencies]
 invoke = "0.18.1"
 flake8 = "^3.9.0"
 
 # PyTest and its auxiliary support files
```

### Comparing `tibanna-3.3.0/tibanna/__init__.py` & `tibanna-3.3.1/tibanna/__init__.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/__main__.py` & `tibanna-3.3.1/tibanna/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/_version.py` & `tibanna-3.3.1/tibanna/_version.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/ami.py` & `tibanna-3.3.1/tibanna/ami.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/awsem.py` & `tibanna-3.3.1/tibanna/awsem.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/base.py` & `tibanna-3.3.1/tibanna/base.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/check_task.py` & `tibanna-3.3.1/tibanna/check_task.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/core.py` & `tibanna-3.3.1/tibanna/core.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/create_ami_userdata` & `tibanna-3.3.1/tibanna/create_ami_userdata`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/cw_utils.py` & `tibanna-3.3.1/tibanna/cw_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/dd_utils.py` & `tibanna-3.3.1/tibanna/dd_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/ec2_utils.py` & `tibanna-3.3.1/tibanna/ec2_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/exceptions.py` & `tibanna-3.3.1/tibanna/exceptions.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/iam_utils.py` & `tibanna-3.3.1/tibanna/iam_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/job.py` & `tibanna-3.3.1/tibanna/job.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/lambdas/check_task_awsem.py` & `tibanna-3.3.1/tibanna/lambdas/check_task_awsem.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/nnested_array.py` & `tibanna-3.3.1/tibanna/nnested_array.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/pricing_utils.py` & `tibanna-3.3.1/tibanna/pricing_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/run_task.py` & `tibanna-3.3.1/tibanna/run_task.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/stepfunction.py` & `tibanna-3.3.1/tibanna/stepfunction.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/stepfunction_cost_updater.py` & `tibanna-3.3.1/tibanna/stepfunction_cost_updater.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/top.py` & `tibanna-3.3.1/tibanna/top.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/update_cost.py` & `tibanna-3.3.1/tibanna/update_cost.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/utils.py` & `tibanna-3.3.1/tibanna/utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/tibanna/vars.py` & `tibanna-3.3.1/tibanna/vars.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.0/setup.py` & `tibanna-3.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 packages = \
 ['awsf3', 'tibanna', 'tibanna.lambdas']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Benchmark-4dn>=0.5.21,<0.6.0',
+['Benchmark-4dn>=0.5.23,<0.6.0',
  'boto3>=1.9.0,<2.0.0',
  'botocore>=1.12.1,<2.0.0',
  'python-lambda-4dn==0.12.3',
  'requests==2.27.1',
  'tomlkit>=0.11.0,<0.12.0']
 
 entry_points = \
 {'console_scripts': ['awsf3 = awsf3.__main__:main',
                      'tibanna = tibanna.__main__:main']}
 
 setup_kwargs = {
     'name': 'tibanna',
-    'version': '3.3.0',
+    'version': '3.3.1',
     'description': 'Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud.',
     'long_description': "# Tibanna\n\n[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/) [![Build Status](https://travis-ci.org/4dn-dcic/tibanna.svg?branch=master)](https://travis-ci.org/4dn-dcic/tibanna) [![Code Quality](https://api.codacy.com/project/badge/Grade/d2946b5bc0704e5c9a4893426a7e0314)](https://www.codacy.com/app/4dn/tibanna?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=4dn-dcic/tibanna&amp;utm_campaign=Badge_Grade) [![Test Coverage](https://api.codacy.com/project/badge/Coverage/d2946b5bc0704e5c9a4893426a7e0314)](https://www.codacy.com/app/4dn/tibanna?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=4dn-dcic/tibanna&amp;utm_campaign=Badge_Coverage) [![Documentation Status](https://readthedocs.org/projects/tibanna/badge/?version=latest)](https://tibanna.readthedocs.io/en/latest/?badge=latest)\n\n***\n\nTibanna runs portable pipelines (in CWL/WDL/Snakemake/shell) on the AWS Cloud.\n\n<br>\n\nInstall Tibanna.\n```bash\npip install tibanna\n```\n\n<br>\n\nUse CLI to set up the cloud component and run workflow.\n```bash\n# Deploy Unicorn to the Cloud (Unicorn = serverless scheduler/resource allocator).\ntibanna deploy_unicorn --usergroup=mygroup\n\n# Run CWL/WDL workflow on the Cloud.\ntibanna run_workflow --input-json=myrun.json\n```\n\n<br>\n\nAlternatively, use Python API.\n\n```python\nfrom tibanna.core import API\n\n# Deploy Unicorn to the Cloud.\nAPI().deploy_unicorn(usergroup='mygroup')\n\n# Run CWL/WDL workflow on the Cloud.\nAPI().run_workflow(input_json='myrun.json')\n```\n\n<br>\n\n---\nNote: Starting `0.8.2`, Tibanna supports local CWL/WDL files as well as shell commands and Snakemake workflows.\n\nNote 2: As of Tibanna version `2.0.0`, Python 3.6 is no longer supported. Please switch to Python 3.8! Python 3.7 is also supported as a fallback, but please prefer 3.8 if you can.\n\nNote 3: Starting `0.8.0`, one no longer needs to `git clone` the Tibanna repo. \n* Please switch from `invoke <command>` to `tibanna <command>`! \n* We also renovated the Python API as an inheritable class to allow development around tibanna.\n\n\nFor more details, see Tibanna [**Documentation**](http://tibanna.readthedocs.io/en/latest).\n* Also check out our [**paper in _Bioinformatics_**](https://doi.org/10.1093/bioinformatics/btz379).\n* A preprint can also be found on [**biorxiv**](https://www.biorxiv.org/content/10.1101/440974v3).\n\n",
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://github.com/4dn-dcic/tibanna',
```

### Comparing `tibanna-3.3.0/PKG-INFO` & `tibanna-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibanna
-Version: 3.3.0
+Version: 3.3.1
 Summary: Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud.
 Home-page: http://github.com/4dn-dcic/tibanna
 License: MIT
 Keywords: tibanna
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.9
@@ -13,15 +13,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: Benchmark-4dn (>=0.5.21,<0.6.0)
+Requires-Dist: Benchmark-4dn (>=0.5.23,<0.6.0)
 Requires-Dist: boto3 (>=1.9.0,<2.0.0)
 Requires-Dist: botocore (>=1.12.1,<2.0.0)
 Requires-Dist: python-lambda-4dn (==0.12.3)
 Requires-Dist: requests (==2.27.1)
 Requires-Dist: tomlkit (>=0.11.0,<0.12.0)
 Project-URL: Repository, http://github.com/4dn-dcic/tibanna.git
 Description-Content-Type: text/markdown
```

