# Comparing `tmp/cloud_toolkit_aws-0.8.2.tar.gz` & `tmp/cloud_toolkit_aws-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_toolkit_aws-0.8.2.tar", last modified: Mon Apr 10 11:03:47 2023, max compression
+gzip compressed data, was "cloud_toolkit_aws-0.8.3.tar", last modified: Wed Apr 12 10:35:48 2023, max compression
```

## Comparing `cloud_toolkit_aws-0.8.2.tar` & `cloud_toolkit_aws-0.8.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-10 11:03:47.314567 cloud_toolkit_aws-0.8.2/
--rw-r--r--   0 runner     (501) staff       (20)     1533 2023-04-10 11:03:47.314147 cloud_toolkit_aws-0.8.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1346 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-10 11:03:47.282419 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/
--rw-------   0 runner     (501) staff       (20)     4468 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/__init__.py
--rw-------   0 runner     (501) staff       (20)     8114 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/_utilities.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-10 11:03:47.286088 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/commons/
--rw-------   0 runner     (501) staff       (20)      276 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/commons/__init__.py
--rw-------   0 runner     (501) staff       (20)     5892 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/commons/certificate.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-10 11:03:47.288705 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/databases/
--rw-------   0 runner     (501) staff       (20)      343 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/databases/__init__.py
--rw-------   0 runner     (501) staff       (20)      708 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/databases/_enums.py
--rw-------   0 runner     (501) staff       (20)    16805 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/databases/_inputs.py
--rw-------   0 runner     (501) staff       (20)    14551 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/databases/aurora_mysql.py
--rw-------   0 runner     (501) staff       (20)    11020 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/databases/mysql.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-10 11:03:47.291321 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/email/
--rw-------   0 runner     (501) staff       (20)      344 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/email/__init__.py
--rw-------   0 runner     (501) staff       (20)      839 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/email/_enums.py
--rw-------   0 runner     (501) staff       (20)     6826 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/email/_inputs.py
--rw-------   0 runner     (501) staff       (20)    22208 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/email/email_sender.py
--rw-------   0 runner     (501) staff       (20)     1780 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/email/outputs.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-10 11:03:47.303497 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/
--rw-------   0 runner     (501) staff       (20)      865 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/__init__.py
--rw-------   0 runner     (501) staff       (20)      349 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/_enums.py
--rw-------   0 runner     (501) staff       (20)    32928 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/_inputs.py
--rw-------   0 runner     (501) staff       (20)     6667 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/adot_application.py
--rw-------   0 runner     (501) staff       (20)     3421 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/adot_operator.py
--rw-------   0 runner     (501) staff       (20)     6837 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/application_addon.py
--rw-------   0 runner     (501) staff       (20)     4637 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/argo_cd.py
--rw-------   0 runner     (501) staff       (20)     3652 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/aws_ebs_csi_driver.py
--rw-------   0 runner     (501) staff       (20)     4659 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/aws_load_balancer_controller.py
--rw-------   0 runner     (501) staff       (20)     3822 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/calico.py
--rw-------   0 runner     (501) staff       (20)     4906 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/cert_manager.py
--rw-------   0 runner     (501) staff       (20)    20850 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/cluster.py
--rw-------   0 runner     (501) staff       (20)    16051 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/cluster_addons.py
--rw-------   0 runner     (501) staff       (20)     6577 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/cluster_admins.py
--rw-------   0 runner     (501) staff       (20)     4547 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/cluster_autoscaler.py
--rw-------   0 runner     (501) staff       (20)     4312 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/dashboard.py
--rw-------   0 runner     (501) staff       (20)     4948 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/external_dns.py
--rw-------   0 runner     (501) staff       (20)     7586 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/fluentbit.py
--rw-------   0 runner     (501) staff       (20)    14509 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/iam_authenticator.py
--rw-------   0 runner     (501) staff       (20)     8603 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/ingress_nginx.py
--rw-------   0 runner     (501) staff       (20)    10726 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/irsa.py
--rw-------   0 runner     (501) staff       (20)    14006 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/node_group.py
--rw-------   0 runner     (501) staff       (20)    13051 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/project.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-10 11:03:47.308205 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/
--rw-------   0 runner     (501) staff       (20)      477 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/__init__.py
--rw-------   0 runner     (501) staff       (20)    30048 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/_inputs.py
--rw-------   0 runner     (501) staff       (20)     5385 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/account_iam.py
--rw-------   0 runner     (501) staff       (20)    11354 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/audit_logging.py
--rw-------   0 runner     (501) staff       (20)     6133 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/iam_trusted_account.py
--rw-------   0 runner     (501) staff       (20)     5578 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/iam_trusting_account.py
--rw-------   0 runner     (501) staff       (20)     5626 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/landing_zone.py
--rw-------   0 runner     (501) staff       (20)    11948 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/organization.py
--rw-------   0 runner     (501) staff       (20)     9328 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/outputs.py
--rw-------   0 runner     (501) staff       (20)     2763 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/provider.py
--rw-------   0 runner     (501) staff       (20)      125 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/pulumi-plugin.json
--rw-------   0 runner     (501) staff       (20)        0 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/py.typed
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-10 11:03:47.311356 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/
--rw-------   0 runner     (501) staff       (20)      363 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/__init__.py
--rw-------   0 runner     (501) staff       (20)      640 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/_enums.py
--rw-------   0 runner     (501) staff       (20)     8840 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/_inputs.py
--rw-------   0 runner     (501) staff       (20)     1778 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/outputs.py
--rw-------   0 runner     (501) staff       (20)     9773 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/queue.py
--rw-------   0 runner     (501) staff       (20)    11927 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/static_web.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-10 11:03:47.313417 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/storage/
--rw-------   0 runner     (501) staff       (20)      316 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/storage/__init__.py
--rw-------   0 runner     (501) staff       (20)      678 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/storage/_enums.py
--rw-------   0 runner     (501) staff       (20)     2670 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/storage/_inputs.py
--rw-------   0 runner     (501) staff       (20)    13890 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/storage/bucket.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-10 11:03:47.285127 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1533 2023-04-10 11:03:47.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2709 2023-04-10 11:03:47.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-10 11:03:47.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-10 11:03:47.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      116 2023-04-10 11:03:47.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       18 2023-04-10 11:03:47.000000 cloud_toolkit_aws-0.8.2/cloud_toolkit_aws.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-10 11:03:47.314681 cloud_toolkit_aws-0.8.2/setup.cfg
--rw-------   0 runner     (501) staff       (20)     2122 2023-04-10 11:03:46.000000 cloud_toolkit_aws-0.8.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 10:35:48.446318 cloud_toolkit_aws-0.8.3/
+-rw-r--r--   0 runner     (501) staff       (20)     1533 2023-04-12 10:35:48.445910 cloud_toolkit_aws-0.8.3/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1346 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 10:35:48.417400 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/
+-rw-------   0 runner     (501) staff       (20)     4468 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/__init__.py
+-rw-------   0 runner     (501) staff       (20)     8114 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/_utilities.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 10:35:48.420840 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/commons/
+-rw-------   0 runner     (501) staff       (20)      276 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/commons/__init__.py
+-rw-------   0 runner     (501) staff       (20)     5892 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/commons/certificate.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 10:35:48.423371 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/databases/
+-rw-------   0 runner     (501) staff       (20)      343 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/databases/__init__.py
+-rw-------   0 runner     (501) staff       (20)      548 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/databases/_enums.py
+-rw-------   0 runner     (501) staff       (20)    16805 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/databases/_inputs.py
+-rw-------   0 runner     (501) staff       (20)    14410 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/databases/aurora_mysql.py
+-rw-------   0 runner     (501) staff       (20)    11020 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/databases/mysql.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 10:35:48.425638 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/email/
+-rw-------   0 runner     (501) staff       (20)      344 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/email/__init__.py
+-rw-------   0 runner     (501) staff       (20)      839 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/email/_enums.py
+-rw-------   0 runner     (501) staff       (20)     6826 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/email/_inputs.py
+-rw-------   0 runner     (501) staff       (20)    22208 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/email/email_sender.py
+-rw-------   0 runner     (501) staff       (20)     1780 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/email/outputs.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 10:35:48.436359 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/
+-rw-------   0 runner     (501) staff       (20)      865 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/__init__.py
+-rw-------   0 runner     (501) staff       (20)      349 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/_enums.py
+-rw-------   0 runner     (501) staff       (20)    32928 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/_inputs.py
+-rw-------   0 runner     (501) staff       (20)     6667 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/adot_application.py
+-rw-------   0 runner     (501) staff       (20)     3421 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/adot_operator.py
+-rw-------   0 runner     (501) staff       (20)     6837 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/application_addon.py
+-rw-------   0 runner     (501) staff       (20)     4637 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/argo_cd.py
+-rw-------   0 runner     (501) staff       (20)     3652 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/aws_ebs_csi_driver.py
+-rw-------   0 runner     (501) staff       (20)     4659 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/aws_load_balancer_controller.py
+-rw-------   0 runner     (501) staff       (20)     3822 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/calico.py
+-rw-------   0 runner     (501) staff       (20)     4906 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/cert_manager.py
+-rw-------   0 runner     (501) staff       (20)    20850 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/cluster.py
+-rw-------   0 runner     (501) staff       (20)    16051 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/cluster_addons.py
+-rw-------   0 runner     (501) staff       (20)     6577 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/cluster_admins.py
+-rw-------   0 runner     (501) staff       (20)     4547 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/cluster_autoscaler.py
+-rw-------   0 runner     (501) staff       (20)     4312 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/dashboard.py
+-rw-------   0 runner     (501) staff       (20)     4948 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/external_dns.py
+-rw-------   0 runner     (501) staff       (20)     7586 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/fluentbit.py
+-rw-------   0 runner     (501) staff       (20)    14509 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/iam_authenticator.py
+-rw-------   0 runner     (501) staff       (20)     8603 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/ingress_nginx.py
+-rw-------   0 runner     (501) staff       (20)    10726 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/irsa.py
+-rw-------   0 runner     (501) staff       (20)    14006 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/node_group.py
+-rw-------   0 runner     (501) staff       (20)    13051 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/project.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 10:35:48.440601 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/
+-rw-------   0 runner     (501) staff       (20)      477 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/__init__.py
+-rw-------   0 runner     (501) staff       (20)    30048 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/_inputs.py
+-rw-------   0 runner     (501) staff       (20)     5385 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/account_iam.py
+-rw-------   0 runner     (501) staff       (20)    11354 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/audit_logging.py
+-rw-------   0 runner     (501) staff       (20)     6133 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/iam_trusted_account.py
+-rw-------   0 runner     (501) staff       (20)     5578 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/iam_trusting_account.py
+-rw-------   0 runner     (501) staff       (20)     5626 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/landing_zone.py
+-rw-------   0 runner     (501) staff       (20)    11948 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/organization.py
+-rw-------   0 runner     (501) staff       (20)     9328 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/outputs.py
+-rw-------   0 runner     (501) staff       (20)     2763 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/provider.py
+-rw-------   0 runner     (501) staff       (20)      125 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/pulumi-plugin.json
+-rw-------   0 runner     (501) staff       (20)        0 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/py.typed
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 10:35:48.443335 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/
+-rw-------   0 runner     (501) staff       (20)      363 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/__init__.py
+-rw-------   0 runner     (501) staff       (20)      640 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/_enums.py
+-rw-------   0 runner     (501) staff       (20)     8840 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/_inputs.py
+-rw-------   0 runner     (501) staff       (20)     1778 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/outputs.py
+-rw-------   0 runner     (501) staff       (20)     9773 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/queue.py
+-rw-------   0 runner     (501) staff       (20)    11927 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/static_web.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 10:35:48.445220 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/storage/
+-rw-------   0 runner     (501) staff       (20)      316 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/storage/__init__.py
+-rw-------   0 runner     (501) staff       (20)      678 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/storage/_enums.py
+-rw-------   0 runner     (501) staff       (20)     2670 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/storage/_inputs.py
+-rw-------   0 runner     (501) staff       (20)    13890 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/storage/bucket.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-12 10:35:48.419953 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1533 2023-04-12 10:35:48.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2709 2023-04-12 10:35:48.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-12 10:35:48.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-12 10:35:48.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      116 2023-04-12 10:35:48.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       18 2023-04-12 10:35:48.000000 cloud_toolkit_aws-0.8.3/cloud_toolkit_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-12 10:35:48.446431 cloud_toolkit_aws-0.8.3/setup.cfg
+-rw-------   0 runner     (501) staff       (20)     2122 2023-04-12 10:35:47.000000 cloud_toolkit_aws-0.8.3/setup.py
```

### Comparing `cloud_toolkit_aws-0.8.2/PKG-INFO` & `cloud_toolkit_aws-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud_toolkit_aws
-Version: 0.8.2
+Version: 0.8.3
 License: Apache-2.0
 Keywords: pulumi aws cloud-toolkit category/cloud kind/component
 Description-Content-Type: text/markdown
 
 # Cloud Toolkit AWS
 
 The Cloud Toolkit AWS provider for Pulumi provision well-architected solutions in [AWS](https://aws.amazon.com/). With Cloud Toolkit AWS you can use your preferred programming language to manage your platform with Infrastructure as Code.
```

### Comparing `cloud_toolkit_aws-0.8.2/README.md` & `cloud_toolkit_aws-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/__init__.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/_utilities.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/_utilities.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/commons/certificate.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/commons/certificate.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/databases/_inputs.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/databases/_inputs.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/databases/aurora_mysql.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/databases/aurora_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from ._enums import *
 from ._inputs import *
 import pulumi_aws
 import pulumi_random
 
 __all__ = ['AuroraMysqlArgs', 'AuroraMysql']
 
 @pulumi.input_type
@@ -21,25 +20,25 @@
                  backup: Optional[pulumi.Input['AuroraMysqlBackupArgs']] = None,
                  database: Optional[pulumi.Input['AuroraMysqlDatabaseArgs']] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
                  instances_count: Optional[pulumi.Input[float]] = None,
                  logging: Optional[pulumi.Input['AuroraMysqlLoggingArgs']] = None,
                  monitoring: Optional[pulumi.Input['AuroraMysqlMonitoringArgs']] = None,
                  networking: Optional[pulumi.Input['AuroraMysqlNetworkingArgs']] = None,
-                 version: Optional[pulumi.Input['AuroraMysqlVersion']] = None):
+                 version: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a AuroraMysql resource.
         :param pulumi.Input['AuroraMysqlBackupArgs'] backup: Backup configuration parameters for Aurora cluster
         :param pulumi.Input['AuroraMysqlDatabaseArgs'] database: Configuration parameters for the database
         :param pulumi.Input[str] instance_type: The instance type for the cluster
         :param pulumi.Input[float] instances_count: The number of instances to be created for Aurora cluster
         :param pulumi.Input['AuroraMysqlLoggingArgs'] logging: Logging configuration parameters for Aurora cluster
         :param pulumi.Input['AuroraMysqlMonitoringArgs'] monitoring: Monitoring configuration parameters for Aurora cluster
         :param pulumi.Input['AuroraMysqlNetworkingArgs'] networking: Networking configuration parameters for Aurora cluster
-        :param pulumi.Input['AuroraMysqlVersion'] version: Version for database
+        :param pulumi.Input[str] version: Version for database
         """
         if backup is not None:
             pulumi.set(__self__, "backup", backup)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if instance_type is not None:
             pulumi.set(__self__, "instance_type", instance_type)
@@ -136,22 +135,22 @@
 
     @networking.setter
     def networking(self, value: Optional[pulumi.Input['AuroraMysqlNetworkingArgs']]):
         pulumi.set(self, "networking", value)
 
     @property
     @pulumi.getter
-    def version(self) -> Optional[pulumi.Input['AuroraMysqlVersion']]:
+    def version(self) -> Optional[pulumi.Input[str]]:
         """
         Version for database
         """
         return pulumi.get(self, "version")
 
     @version.setter
-    def version(self, value: Optional[pulumi.Input['AuroraMysqlVersion']]):
+    def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
 
 class AuroraMysql(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -159,28 +158,28 @@
                  backup: Optional[pulumi.Input[pulumi.InputType['AuroraMysqlBackupArgs']]] = None,
                  database: Optional[pulumi.Input[pulumi.InputType['AuroraMysqlDatabaseArgs']]] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
                  instances_count: Optional[pulumi.Input[float]] = None,
                  logging: Optional[pulumi.Input[pulumi.InputType['AuroraMysqlLoggingArgs']]] = None,
                  monitoring: Optional[pulumi.Input[pulumi.InputType['AuroraMysqlMonitoringArgs']]] = None,
                  networking: Optional[pulumi.Input[pulumi.InputType['AuroraMysqlNetworkingArgs']]] = None,
-                 version: Optional[pulumi.Input['AuroraMysqlVersion']] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a AuroraMysql resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['AuroraMysqlBackupArgs']] backup: Backup configuration parameters for Aurora cluster
         :param pulumi.Input[pulumi.InputType['AuroraMysqlDatabaseArgs']] database: Configuration parameters for the database
         :param pulumi.Input[str] instance_type: The instance type for the cluster
         :param pulumi.Input[float] instances_count: The number of instances to be created for Aurora cluster
         :param pulumi.Input[pulumi.InputType['AuroraMysqlLoggingArgs']] logging: Logging configuration parameters for Aurora cluster
         :param pulumi.Input[pulumi.InputType['AuroraMysqlMonitoringArgs']] monitoring: Monitoring configuration parameters for Aurora cluster
         :param pulumi.Input[pulumi.InputType['AuroraMysqlNetworkingArgs']] networking: Networking configuration parameters for Aurora cluster
-        :param pulumi.Input['AuroraMysqlVersion'] version: Version for database
+        :param pulumi.Input[str] version: Version for database
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[AuroraMysqlArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -204,15 +203,15 @@
                  backup: Optional[pulumi.Input[pulumi.InputType['AuroraMysqlBackupArgs']]] = None,
                  database: Optional[pulumi.Input[pulumi.InputType['AuroraMysqlDatabaseArgs']]] = None,
                  instance_type: Optional[pulumi.Input[str]] = None,
                  instances_count: Optional[pulumi.Input[float]] = None,
                  logging: Optional[pulumi.Input[pulumi.InputType['AuroraMysqlLoggingArgs']]] = None,
                  monitoring: Optional[pulumi.Input[pulumi.InputType['AuroraMysqlMonitoringArgs']]] = None,
                  networking: Optional[pulumi.Input[pulumi.InputType['AuroraMysqlNetworkingArgs']]] = None,
-                 version: Optional[pulumi.Input['AuroraMysqlVersion']] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
```

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/databases/mysql.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/email/_enums.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/email/_enums.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/email/_inputs.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/email/_inputs.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/email/email_sender.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/email/email_sender.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/email/outputs.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/email/outputs.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/__init__.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/_inputs.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/_inputs.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/adot_application.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/adot_application.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/adot_operator.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/adot_operator.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/application_addon.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/application_addon.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/argo_cd.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/argo_cd.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/aws_ebs_csi_driver.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/aws_ebs_csi_driver.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/aws_load_balancer_controller.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/aws_load_balancer_controller.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/calico.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/calico.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/cert_manager.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/cert_manager.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/cluster.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/cluster.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/cluster_addons.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/cluster_addons.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/cluster_admins.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/cluster_admins.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/cluster_autoscaler.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/dashboard.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/dashboard.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/external_dns.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/external_dns.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/fluentbit.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/fluentbit.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/iam_authenticator.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/iam_authenticator.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/ingress_nginx.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/ingress_nginx.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/irsa.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/irsa.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/node_group.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/node_group.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/kubernetes/project.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/kubernetes/project.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/_inputs.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/_inputs.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/account_iam.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/account_iam.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/audit_logging.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/audit_logging.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/iam_trusted_account.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/iam_trusted_account.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/iam_trusting_account.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/iam_trusting_account.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/landing_zone.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/landing_zone.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/organization.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/organization.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/landingzone/outputs.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/landingzone/outputs.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/provider.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/provider.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/_enums.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/_enums.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/_inputs.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/_inputs.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/outputs.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/outputs.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/queue.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/queue.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/serverless/static_web.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/serverless/static_web.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/storage/_enums.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/storage/_enums.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/storage/_inputs.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws/storage/bucket.py` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws.egg-info/PKG-INFO` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-toolkit-aws
-Version: 0.8.2
+Version: 0.8.3
 License: Apache-2.0
 Keywords: pulumi aws cloud-toolkit category/cloud kind/component
 Description-Content-Type: text/markdown
 
 # Cloud Toolkit AWS
 
 The Cloud Toolkit AWS provider for Pulumi provision well-architected solutions in [AWS](https://aws.amazon.com/). With Cloud Toolkit AWS you can use your preferred programming language to manage your platform with Infrastructure as Code.
```

### Comparing `cloud_toolkit_aws-0.8.2/cloud_toolkit_aws.egg-info/SOURCES.txt` & `cloud_toolkit_aws-0.8.3/cloud_toolkit_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud_toolkit_aws-0.8.2/setup.py` & `cloud_toolkit_aws-0.8.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.8.2"
-PLUGIN_VERSION = "0.8.2"
+VERSION = "0.8.3"
+PLUGIN_VERSION = "0.8.3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'cloud-toolkit-aws', PLUGIN_VERSION, '--server', 'github://api.github.com/cloud-toolkit/cloud-toolkit-aws'])
         except OSError as error:
```

