# Comparing `tmp/cdk-extensions-0.0.54.tar.gz` & `tmp/cdk-extensions-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.54.tar", last modified: Wed Apr 12 20:20:12 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.55.tar", last modified: Wed Apr 12 21:22:10 2023, max compression
```

## Comparing `cdk-extensions-0.0.54.tar` & `cdk-extensions-0.0.55.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.768764 cdk-extensions-0.0.54/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:20:12.768764 cdk-extensions-0.0.54/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.756764 cdk-extensions-0.0.54/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.756764 cdk-extensions-0.0.54/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.756764 cdk-extensions-0.0.54/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.760764 cdk-extensions-0.0.54/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1496139 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/_jsii/cdk-extensions@0.0.54.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.760764 cdk-extensions-0.0.54/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.760764 cdk-extensions-0.0.54/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.760764 cdk-extensions-0.0.54/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.760764 cdk-extensions-0.0.54/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.760764 cdk-extensions-0.0.54/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   621775 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.760764 cdk-extensions-0.0.54/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   153560 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.760764 cdk-extensions-0.0.54/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.760764 cdk-extensions-0.0.54/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   129986 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   208106 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.764764 cdk-extensions-0.0.54/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    53437 2023-04-12 20:20:01.000000 cdk-extensions-0.0.54/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:20:12.756764 cdk-extensions-0.0.54/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-12 20:20:12.000000 cdk-extensions-0.0.54/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-12 20:20:12.000000 cdk-extensions-0.0.54/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:20:12.000000 cdk-extensions-0.0.54/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 20:20:12.000000 cdk-extensions-0.0.54/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 20:20:12.000000 cdk-extensions-0.0.54/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.759313 cdk-extensions-0.0.55/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.759313 cdk-extensions-0.0.55/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.763313 cdk-extensions-0.0.55/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.763313 cdk-extensions-0.0.55/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1496796 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/_jsii/cdk-extensions@0.0.55.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.763313 cdk-extensions-0.0.55/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.763313 cdk-extensions-0.0.55/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.763313 cdk-extensions-0.0.55/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.763313 cdk-extensions-0.0.55/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.763313 cdk-extensions-0.0.55/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   622324 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.763313 cdk-extensions-0.0.55/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   154648 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.763313 cdk-extensions-0.0.55/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    95667 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.763313 cdk-extensions-0.0.55/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   129986 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692448 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    25868 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42370 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   208106 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.767313 cdk-extensions-0.0.55/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    53437 2023-04-12 21:21:59.000000 cdk-extensions-0.0.55/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:22:10.759313 cdk-extensions-0.0.55/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-12 21:22:10.000000 cdk-extensions-0.0.55/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-12 21:22:10.000000 cdk-extensions-0.0.55/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:22:10.000000 cdk-extensions-0.0.55/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 21:22:10.000000 cdk-extensions-0.0.55/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 21:22:10.000000 cdk-extensions-0.0.55/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.54/LICENSE` & `cdk-extensions-0.0.55/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/PKG-INFO` & `cdk-extensions-0.0.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.54
+Version: 0.0.55
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.54/README.md` & `cdk-extensions-0.0.55/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/setup.py` & `cdk-extensions-0.0.55/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.54",
+    "version": "0.0.55",
     "description": "cdk-extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/vibe-io/cdk-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Kevin Lucas<kevinluc08@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -43,15 +43,15 @@
         "cdk_extensions.route53",
         "cdk_extensions.s3_buckets",
         "cdk_extensions.sso",
         "cdk_extensions.stacks"
     ],
     "package_data": {
         "cdk_extensions._jsii": [
-            "cdk-extensions@0.0.54.jsii.tgz"
+            "cdk-extensions@0.0.55.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/ec2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2185,14 +2185,19 @@
         ...
 
     @builtins.property
     @jsii.member(jsii_name="ipamPoolStateMessage")
     def ipam_pool_state_message(self) -> builtins.str:
         ...
 
+    @builtins.property
+    @jsii.member(jsii_name="consumer")
+    def consumer(self) -> typing.Optional["IpamConsumer"]:
+        ...
+
     @jsii.member(jsii_name="addChildPool")
     def add_child_pool(
         self,
         id: builtins.str,
         *,
         address_configuration: typing.Optional[AddressConfiguration] = None,
         auto_import: typing.Optional[builtins.bool] = None,
@@ -2292,14 +2297,19 @@
         return typing.cast(builtins.str, jsii.get(self, "ipamPoolState"))
 
     @builtins.property
     @jsii.member(jsii_name="ipamPoolStateMessage")
     def ipam_pool_state_message(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "ipamPoolStateMessage"))
 
+    @builtins.property
+    @jsii.member(jsii_name="consumer")
+    def consumer(self) -> typing.Optional["IpamConsumer"]:
+        return typing.cast(typing.Optional["IpamConsumer"], jsii.get(self, "consumer"))
+
     @jsii.member(jsii_name="addChildPool")
     def add_child_pool(
         self,
         id: builtins.str,
         *,
         address_configuration: typing.Optional[AddressConfiguration] = None,
         auto_import: typing.Optional[builtins.bool] = None,
@@ -4168,18 +4178,23 @@
         return typing.cast("IpamConsumer", jsii.sinvoke(cls, "of", [name]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="EC2")
     def EC2(cls) -> "IpamConsumer":
         return typing.cast("IpamConsumer", jsii.sget(cls, "EC2"))
 
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="NONE")
+    def NONE(cls) -> "IpamConsumer":
+        return typing.cast("IpamConsumer", jsii.sget(cls, "NONE"))
+
     @builtins.property
     @jsii.member(jsii_name="name")
-    def name(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "name"))
+    def name(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "name"))
 
 
 @jsii.implements(IIpamPool)
 class IpamPool(
     _aws_cdk_ceddda9d.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-extensions.ec2.IpamPool",
```

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from ..ec2 import (
     FlowLogFormat as _FlowLogFormat_b7c2ba34,
     ICidrProvider as _ICidrProvider_28ddf5b0,
     IIpamPool as _IIpamPool_511f311d,
     ITransitGateway as _ITransitGateway_25936657,
     ITransitGatewayAttachment as _ITransitGatewayAttachment_64da8ffd,
     Ipam as _Ipam_1ad3c981,
+    IpamConsumer as _IpamConsumer_e92c8d5d,
     IpamPool as _IpamPool_a6f43771,
     TransitGatewayProps as _TransitGatewayProps_10a60d21,
 )
 from ..networkmanager import GlobalNetwork as _GlobalNetwork_79ec647c
 from ..ram import (
     ISharedPrincipal as _ISharedPrincipal_9cde791b,
     ResourceShare as _ResourceShare_f0180713,
@@ -295,38 +296,48 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
     jsii_type="cdk-extensions.ec2_patterns.AllocatePrivateNetworkOptions",
     jsii_struct_bases=[],
-    name_mapping={"netmask": "netmask", "pool": "pool"},
+    name_mapping={"consumer": "consumer", "netmask": "netmask", "pool": "pool"},
 )
 class AllocatePrivateNetworkOptions:
     def __init__(
         self,
         *,
+        consumer: typing.Optional[_IpamConsumer_e92c8d5d] = None,
         netmask: typing.Optional[jsii.Number] = None,
         pool: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
+        :param consumer: 
         :param netmask: 
         :param pool: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1edcf1c081b844711051faa1818771b547c90031be28d3b0f04a24516485f5eb)
+            check_type(argname="argument consumer", value=consumer, expected_type=type_hints["consumer"])
             check_type(argname="argument netmask", value=netmask, expected_type=type_hints["netmask"])
             check_type(argname="argument pool", value=pool, expected_type=type_hints["pool"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if consumer is not None:
+            self._values["consumer"] = consumer
         if netmask is not None:
             self._values["netmask"] = netmask
         if pool is not None:
             self._values["pool"] = pool
 
     @builtins.property
+    def consumer(self) -> typing.Optional[_IpamConsumer_e92c8d5d]:
+        result = self._values.get("consumer")
+        return typing.cast(typing.Optional[_IpamConsumer_e92c8d5d], result)
+
+    @builtins.property
     def netmask(self) -> typing.Optional[jsii.Number]:
         result = self._values.get("netmask")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def pool(self) -> typing.Optional[builtins.str]:
         result = self._values.get("pool")
@@ -1811,45 +1822,52 @@
         return typing.cast(None, jsii.invoke(self, "addRegion", [region]))
 
     @jsii.member(jsii_name="addStagePool")
     def _add_stage_pool(
         self,
         scope: _constructs_77d1e7e8.IConstruct,
         parent: _IIpamPool_511f311d,
+        consumer: typing.Optional[_IpamConsumer_e92c8d5d] = None,
     ) -> _IpamPool_a6f43771:
         '''
         :param scope: -
         :param parent: -
+        :param consumer: -
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8351763cbc2fc41c8b0d7e2aaa7647da164bdeaebee102597747cddcc0105199)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument parent", value=parent, expected_type=type_hints["parent"])
-        return typing.cast(_IpamPool_a6f43771, jsii.invoke(self, "addStagePool", [scope, parent]))
+            check_type(argname="argument consumer", value=consumer, expected_type=type_hints["consumer"])
+        return typing.cast(_IpamPool_a6f43771, jsii.invoke(self, "addStagePool", [scope, parent, consumer]))
 
     @jsii.member(jsii_name="allocatePrivateNetwork")
     def allocate_private_network(
         self,
         scope: _constructs_77d1e7e8.IConstruct,
         id: builtins.str,
         *,
+        consumer: typing.Optional[_IpamConsumer_e92c8d5d] = None,
         netmask: typing.Optional[jsii.Number] = None,
         pool: typing.Optional[builtins.str] = None,
     ) -> _IpamPool_a6f43771:
         '''
         :param scope: -
         :param id: -
+        :param consumer: 
         :param netmask: 
         :param pool: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__82fd5f0403186614f9952c77f056557e26140d7bf698ba66b0635cfbbb5b2b0f)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        options = AllocatePrivateNetworkOptions(netmask=netmask, pool=pool)
+        options = AllocatePrivateNetworkOptions(
+            consumer=consumer, netmask=netmask, pool=pool
+        )
 
         return typing.cast(_IpamPool_a6f43771, jsii.invoke(self, "allocatePrivateNetwork", [scope, id, options]))
 
     @jsii.member(jsii_name="registerAccount")
     def _register_account(
         self,
         account: builtins.str,
@@ -2561,14 +2579,15 @@
     vpn_route_propagation: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__1edcf1c081b844711051faa1818771b547c90031be28d3b0f04a24516485f5eb(
     *,
+    consumer: typing.Optional[_IpamConsumer_e92c8d5d] = None,
     netmask: typing.Optional[jsii.Number] = None,
     pool: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__61356c6c988a747170b0fff518aeff55bb37140b2f2bb3a8395a7676df11d939(
@@ -2802,22 +2821,24 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__8351763cbc2fc41c8b0d7e2aaa7647da164bdeaebee102597747cddcc0105199(
     scope: _constructs_77d1e7e8.IConstruct,
     parent: _IIpamPool_511f311d,
+    consumer: typing.Optional[_IpamConsumer_e92c8d5d] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__82fd5f0403186614f9952c77f056557e26140d7bf698ba66b0635cfbbb5b2b0f(
     scope: _constructs_77d1e7e8.IConstruct,
     id: builtins.str,
     *,
+    consumer: typing.Optional[_IpamConsumer_e92c8d5d] = None,
     netmask: typing.Optional[jsii.Number] = None,
     pool: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__c82b599c8d1db4dca2c0b4ea748776ad7c5f35028ef3d218517ae47d9e5906d7(
```

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.55/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.55/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.54
+Version: 0.0.55
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.54/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.55/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.54.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.55.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
 src/cdk_extensions/ec2_patterns/__init__.py
```

