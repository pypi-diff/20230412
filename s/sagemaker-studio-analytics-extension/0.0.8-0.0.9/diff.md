# Comparing `tmp/sagemaker-studio-analytics-extension-0.0.8.tar.gz` & `tmp/sagemaker-studio-analytics-extension-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/workplace/shahvar/MercuryIntegrationTests/src/SagemakerAnalyticsLib/sagemaker_studio_analytics_extension/dist/tmp14m2daf5/sage", last modified: Tue Apr 19 23:04:28 2022, max compression
+gzip compressed data, was "/workplace/shahvar/PublishLib/src/SagemakerAnalyticsLib/sagemaker_studio_analytics_extension/dist/tmp7nmfh6l_/sagemaker-studio-", last modified: Fri Jun  3 19:37:37 2022, max compression
```

## Comparing `sagemaker-studio-analytics-extension-0.0.8.tar` & `sagemaker-studio-analytics-extension-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/
--rw-r--r--   0 shahvar  (12011261) amazon     (100)    11357 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/LICENSE
--rw-r--r--   0 shahvar  (12011261) amazon     (100)      164 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/MANIFEST.in
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     3817 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/PKG-INFO
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     3229 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/README.md
--rw-r--r--   0 shahvar  (12011261) amazon     (100)       38 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/setup.cfg
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     1801 2022-04-19 21:58:04.000000 sagemaker-studio-analytics-extension-0.0.8/setup.py
-drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/
-drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/
--rw-r--r--   0 shahvar  (12011261) amazon     (100)        0 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/__init__.py
-drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/magics/
--rw-r--r--   0 shahvar  (12011261) amazon     (100)      730 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/magics/__init__.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)    29559 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/magics/sagemaker_analytics.py
-drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/resource/
--rw-r--r--   0 shahvar  (12011261) amazon     (100)      166 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/resource/__init__.py
-drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/resource/emr/
--rw-r--r--   0 shahvar  (12011261) amazon     (100)      107 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/resource/emr/__init__.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     1185 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/resource/emr/auth.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     1526 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/resource/resource_metadata.py
-drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/
--rw-r--r--   0 shahvar  (12011261) amazon     (100)      197 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/__init__.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     2521 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/arn_util.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     1284 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/boto_client_utils.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)      591 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/constants.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)      864 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/emr_constants.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     1787 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/logging_utils.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     1389 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/resource_check.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     1655 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/runtime_check.py
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     8431 2022-04-19 21:57:38.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/service_metrics.py
-drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension.egg-info/
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     3817 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension.egg-info/PKG-INFO
--rw-r--r--   0 shahvar  (12011261) amazon     (100)     1438 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension.egg-info/SOURCES.txt
--rw-r--r--   0 shahvar  (12011261) amazon     (100)        1 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension.egg-info/dependency_links.txt
--rw-r--r--   0 shahvar  (12011261) amazon     (100)      109 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension.egg-info/entry_points.txt
--rw-r--r--   0 shahvar  (12011261) amazon     (100)       95 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension.egg-info/requires.txt
--rw-r--r--   0 shahvar  (12011261) amazon     (100)      222 2022-04-19 23:04:28.000000 sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension.egg-info/top_level.txt
+drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)    11357 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/LICENSE
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)      164 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/MANIFEST.in
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     4136 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/PKG-INFO
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     3568 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/README.md
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)       38 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/setup.cfg
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     1801 2022-06-03 18:18:09.000000 sagemaker-studio-analytics-extension-0.0.9/setup.py
+drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/src/
+drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)        0 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/__init__.py
+drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/magics/
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)      730 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/magics/__init__.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)    29659 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/magics/sagemaker_analytics.py
+drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/resource/
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)      166 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/resource/__init__.py
+drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/resource/emr/
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)      107 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/resource/emr/__init__.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     1185 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/resource/emr/auth.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     1526 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/resource/resource_metadata.py
+drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)      197 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/__init__.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     2521 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/arn_util.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     1284 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/boto_client_utils.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)      591 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/constants.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)      864 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/emr_constants.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     1787 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/logging_utils.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     1389 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/resource_check.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     1655 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/runtime_check.py
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     8431 2022-05-11 18:30:15.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/service_metrics.py
+drwxr-xr-x   0 shahvar  (12011261) amazon     (100)        0 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension.egg-info/
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     4136 2022-06-03 19:37:36.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension.egg-info/PKG-INFO
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)     1438 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)        1 2022-06-03 19:37:36.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)      109 2022-06-03 19:37:36.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension.egg-info/entry_points.txt
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)       95 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension.egg-info/requires.txt
+-rw-r--r--   0 shahvar  (12011261) amazon     (100)      222 2022-06-03 19:37:37.000000 sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension.egg-info/top_level.txt
```

### Comparing `sagemaker-studio-analytics-extension-0.0.8/LICENSE` & `sagemaker-studio-analytics-extension-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/PKG-INFO` & `sagemaker-studio-analytics-extension-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: sagemaker-studio-analytics-extension
-Version: 0.0.8
+Version: 0.0.9
 Summary: SageMaker Studio Analytics Extension
 Home-page: https://aws.amazon.com/sagemaker
 Author: Amazon Web Services
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
@@ -31,21 +30,22 @@
   
 Docstring:
 ::
 
   %sm_analytics [--auth-type AUTH_TYPE] [--cluster-id CLUSTER_ID]
                     [--language LANGUAGE]
                     [--assumable-role-arn ASSUMABLE_ROLE_ARN]
+                    [--emr-execution-role-arn EMR_EXECUTION_ROLE_ARN]
                     [command [command ...]]
 
 positional arguments:
   command               Command to execute. The command consists of a service
                         name followed by a ' ' followed by an operation.
-                        Supported services are {'emr'} and supported
-                        operations are {'connect'}. For example a valid
+                        Supported services are ['emr'] and supported
+                        operations are ['connect']. For example a valid
                         command is 'emr connect'.
 
 optional arguments:
   --auth-type AUTH_TYPE
                         The authentication type to be used. Supported
                         authentication types are {'Kerberos', 'None',
                         'Basic_Access'}.
@@ -55,14 +55,18 @@
                         kernel(s) are {'python', 'scala'}. This is a required
                         argument for IPython kernels, but not for magic
                         kernels such as PySpark or SparkScala.
   --assumable-role-arn ASSUMABLE_ROLE_ARN
                         The IAM role to assume when connecting to a cluster in 
                         a different AWS account. This argument is not required 
                         when connecting to a cluster in the same AWS account.
+  --emr-execution-role-arn EMR_EXECUTION_ROLE_ARN
+                        The IAM role passed to EMR to set up EMR job security
+                        context. This argument is optional and used when IAM
+                        Passthrough feature is enabled for EMR.
 ```
 
 ### Examples
 1. Connect Studio notebook using IPython Kernel to EMR cluster protected by Kerberos. 
 ```buildoutcfg
 %sm_analytics emr connect --cluster-id j-1JIIZS02SEVCS --auth-type Kerberos --language python
 ```
@@ -81,9 +85,7 @@
 ```buildoutcfg
 %sm_analytics emr connect --cluster-id j-1KHIOQZAQUF5P --auth-type Basic_Access
 ```
 ## License
 
 This library is licensed under the Apache 2.0 License. See the LICENSE file.
 
-
-
```

### Comparing `sagemaker-studio-analytics-extension-0.0.8/README.md` & `sagemaker-studio-analytics-extension-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,22 @@
   
 Docstring:
 ::
 
   %sm_analytics [--auth-type AUTH_TYPE] [--cluster-id CLUSTER_ID]
                     [--language LANGUAGE]
                     [--assumable-role-arn ASSUMABLE_ROLE_ARN]
+                    [--emr-execution-role-arn EMR_EXECUTION_ROLE_ARN]
                     [command [command ...]]
 
 positional arguments:
   command               Command to execute. The command consists of a service
                         name followed by a ' ' followed by an operation.
-                        Supported services are {'emr'} and supported
-                        operations are {'connect'}. For example a valid
+                        Supported services are ['emr'] and supported
+                        operations are ['connect']. For example a valid
                         command is 'emr connect'.
 
 optional arguments:
   --auth-type AUTH_TYPE
                         The authentication type to be used. Supported
                         authentication types are {'Kerberos', 'None',
                         'Basic_Access'}.
@@ -38,14 +39,18 @@
                         kernel(s) are {'python', 'scala'}. This is a required
                         argument for IPython kernels, but not for magic
                         kernels such as PySpark or SparkScala.
   --assumable-role-arn ASSUMABLE_ROLE_ARN
                         The IAM role to assume when connecting to a cluster in 
                         a different AWS account. This argument is not required 
                         when connecting to a cluster in the same AWS account.
+  --emr-execution-role-arn EMR_EXECUTION_ROLE_ARN
+                        The IAM role passed to EMR to set up EMR job security
+                        context. This argument is optional and used when IAM
+                        Passthrough feature is enabled for EMR.
 ```
 
 ### Examples
 1. Connect Studio notebook using IPython Kernel to EMR cluster protected by Kerberos. 
 ```buildoutcfg
 %sm_analytics emr connect --cluster-id j-1JIIZS02SEVCS --auth-type Kerberos --language python
 ```
```

### Comparing `sagemaker-studio-analytics-extension-0.0.8/setup.py` & `sagemaker-studio-analytics-extension-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 NAME = "sagemaker-studio-analytics-extension"
 AUTHOR = "Amazon Web Services"
 DESCRIPTION = "SageMaker Studio Analytics Extension"
 LICENSE = "Apache 2.0"
 URL = "https://aws.amazon.com/sagemaker"
 README = "README.md"
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 CLASSIFIERS = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/magics/__init__.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/magics/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/magics/sagemaker_analytics.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/magics/sagemaker_analytics.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,17 @@
                 AUTH_TYPE_SET, usage
             )
         )
 
     if args.assumable_role_arn:
         RoleArnValidator.validate(args.assumable_role_arn)
 
+    if args.emr_execution_role_arn:
+        RoleArnValidator.validate(args.emr_execution_role_arn)
+
     # Only IPython kernel needs language option support
     if kernel_name == IPYTHON_KERNEL:
         if args.language is None:
             raise ValueError(
                 "Missing required argument '{}' for IPython kernel. {}".format(
                     "--language", usage
                 )
```

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/resource/emr/auth.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/resource/emr/auth.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/resource/resource_metadata.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/resource/resource_metadata.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/arn_util.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/arn_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/boto_client_utils.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/boto_client_utils.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/constants.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/emr_constants.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/emr_constants.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/logging_utils.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/resource_check.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/resource_check.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/runtime_check.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/runtime_check.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension/utils/service_metrics.py` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension/utils/service_metrics.py`

 * *Files identical despite different names*

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension.egg-info/PKG-INFO` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: sagemaker-studio-analytics-extension
-Version: 0.0.8
+Version: 0.0.9
 Summary: SageMaker Studio Analytics Extension
 Home-page: https://aws.amazon.com/sagemaker
 Author: Amazon Web Services
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
@@ -31,21 +30,22 @@
   
 Docstring:
 ::
 
   %sm_analytics [--auth-type AUTH_TYPE] [--cluster-id CLUSTER_ID]
                     [--language LANGUAGE]
                     [--assumable-role-arn ASSUMABLE_ROLE_ARN]
+                    [--emr-execution-role-arn EMR_EXECUTION_ROLE_ARN]
                     [command [command ...]]
 
 positional arguments:
   command               Command to execute. The command consists of a service
                         name followed by a ' ' followed by an operation.
-                        Supported services are {'emr'} and supported
-                        operations are {'connect'}. For example a valid
+                        Supported services are ['emr'] and supported
+                        operations are ['connect']. For example a valid
                         command is 'emr connect'.
 
 optional arguments:
   --auth-type AUTH_TYPE
                         The authentication type to be used. Supported
                         authentication types are {'Kerberos', 'None',
                         'Basic_Access'}.
@@ -55,14 +55,18 @@
                         kernel(s) are {'python', 'scala'}. This is a required
                         argument for IPython kernels, but not for magic
                         kernels such as PySpark or SparkScala.
   --assumable-role-arn ASSUMABLE_ROLE_ARN
                         The IAM role to assume when connecting to a cluster in 
                         a different AWS account. This argument is not required 
                         when connecting to a cluster in the same AWS account.
+  --emr-execution-role-arn EMR_EXECUTION_ROLE_ARN
+                        The IAM role passed to EMR to set up EMR job security
+                        context. This argument is optional and used when IAM
+                        Passthrough feature is enabled for EMR.
 ```
 
 ### Examples
 1. Connect Studio notebook using IPython Kernel to EMR cluster protected by Kerberos. 
 ```buildoutcfg
 %sm_analytics emr connect --cluster-id j-1JIIZS02SEVCS --auth-type Kerberos --language python
 ```
@@ -81,9 +85,7 @@
 ```buildoutcfg
 %sm_analytics emr connect --cluster-id j-1KHIOQZAQUF5P --auth-type Basic_Access
 ```
 ## License
 
 This library is licensed under the Apache 2.0 License. See the LICENSE file.
 
-
-
```

### Comparing `sagemaker-studio-analytics-extension-0.0.8/src/sagemaker_studio_analytics_extension.egg-info/SOURCES.txt` & `sagemaker-studio-analytics-extension-0.0.9/src/sagemaker_studio_analytics_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

