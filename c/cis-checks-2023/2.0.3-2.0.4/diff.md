# Comparing `tmp/cis_checks_2023-2.0.3.tar.gz` & `tmp/cis_checks_2023-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cis_checks_2023-2.0.3.tar", last modified: Wed Apr 12 07:12:29 2023, max compression
+gzip compressed data, was "cis_checks_2023-2.0.4.tar", last modified: Wed Apr 12 14:39:28 2023, max compression
```

## Comparing `cis_checks_2023-2.0.3.tar` & `cis_checks_2023-2.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:12:29.536816 cis_checks_2023-2.0.3/
--rw-rw-rw-   0        0        0      836 2023-04-12 07:12:29.534827 cis_checks_2023-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 07:12:29.518814 cis_checks_2023-2.0.3/cis_checks_2023/
--rw-rw-rw-   0        0        0     6574 2023-04-12 07:12:04.000000 cis_checks_2023-2.0.3/cis_checks_2023/__init__.py
--rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.3/cis_checks_2023/_security_control_5.py
--rw-rw-rw-   0        0        0    53781 2023-04-12 07:09:53.000000 cis_checks_2023-2.0.3/cis_checks_2023/iam_control_1.py
--rw-rw-rw-   0        0        0    23922 2023-04-12 07:12:03.000000 cis_checks_2023-2.0.3/cis_checks_2023/logging_control_3.py
--rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.3/cis_checks_2023/monitoring_control_4.py
--rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.3/cis_checks_2023/networking_control_5.py
--rw-rw-rw-   0        0        0    17716 2023-04-12 07:08:18.000000 cis_checks_2023-2.0.3/cis_checks_2023/storage_control_2.py
--rw-rw-rw-   0        0        0    20340 2023-04-10 07:28:15.000000 cis_checks_2023-2.0.3/cis_checks_2023/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:12:29.529814 cis_checks_2023-2.0.3/cis_checks_2023.egg-info/
--rw-rw-rw-   0        0        0      836 2023-04-12 07:12:29.000000 cis_checks_2023-2.0.3/cis_checks_2023.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-04-12 07:12:29.000000 cis_checks_2023-2.0.3/cis_checks_2023.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:12:29.000000 cis_checks_2023-2.0.3/cis_checks_2023.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-12 07:12:29.000000 cis_checks_2023-2.0.3/cis_checks_2023.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      557 2023-04-12 07:12:04.000000 cis_checks_2023-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 07:12:29.536816 cis_checks_2023-2.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 14:39:28.319993 cis_checks_2023-2.0.4/
+-rw-rw-rw-   0        0        0      836 2023-04-12 14:39:28.319993 cis_checks_2023-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 14:39:28.304354 cis_checks_2023-2.0.4/cis_checks_2023/
+-rw-rw-rw-   0        0        0     6690 2023-04-12 14:38:35.000000 cis_checks_2023-2.0.4/cis_checks_2023/__init__.py
+-rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.4/cis_checks_2023/_security_control_5.py
+-rw-rw-rw-   0        0        0    54565 2023-04-12 14:37:06.000000 cis_checks_2023-2.0.4/cis_checks_2023/iam_control_1.py
+-rw-rw-rw-   0        0        0    24792 2023-04-12 14:37:06.000000 cis_checks_2023-2.0.4/cis_checks_2023/logging_control_3.py
+-rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.4/cis_checks_2023/monitoring_control_4.py
+-rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.4/cis_checks_2023/networking_control_5.py
+-rw-rw-rw-   0        0        0    17716 2023-04-12 07:08:18.000000 cis_checks_2023-2.0.4/cis_checks_2023/storage_control_2.py
+-rw-rw-rw-   0        0        0    20340 2023-04-10 07:28:15.000000 cis_checks_2023-2.0.4/cis_checks_2023/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:39:28.319993 cis_checks_2023-2.0.4/cis_checks_2023.egg-info/
+-rw-rw-rw-   0        0        0      836 2023-04-12 14:39:28.000000 cis_checks_2023-2.0.4/cis_checks_2023.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-04-12 14:39:28.000000 cis_checks_2023-2.0.4/cis_checks_2023.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:39:28.000000 cis_checks_2023-2.0.4/cis_checks_2023.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-12 14:39:28.000000 cis_checks_2023-2.0.4/cis_checks_2023.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      557 2023-04-12 14:38:35.000000 cis_checks_2023-2.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:39:28.335613 cis_checks_2023-2.0.4/setup.cfg
```

### Comparing `cis_checks_2023-2.0.3/PKG-INFO` & `cis_checks_2023-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cis_checks_2023
-Version: 2.0.3
+Version: 2.0.4
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.3/cis_checks_2023/__init__.py` & `cis_checks_2023-2.0.4/cis_checks_2023/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cis_checks_2023.iam_control_1 import iam_control
 
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 
 
 class aws_client(iam_control, utils, storage_control, logging_control, monitoring_control, networking_control):
     def __init__(self, **kwargs):
         """
         @param str aws_access_key_id: AWS Access Key ID
         @param str aws_secret_access_key: AWS Secret Access Key
@@ -82,25 +82,26 @@
             self.control_2_3_2_rds_auto_minor_version_upgrade_enabled(regions),
             self.control_2_3_3_rds_publicly_accessible(regions),
             self.control_2_4_1_encryption_enabled_for_efs(),
 
             # logging control 3
             self.control_3_01_ensure_cloud_trail_all_regions(CloudTrail),
             self.control_3_02_ensure_cloudtrail_validation(CloudTrail),
+            self.control_3_03_ensure_cloudtrail_bucket_not_public(CloudTrail),
             self.control_3_04_ensure_cloudtrail_cloudwatch_logs_integration(CloudTrail),
             self.control_3_05_ensure_config_all_regions(regions),
             self.control_3_06_ensure_cloudtrail_bucket_logging(CloudTrail),
             self.control_3_07_ensure_cloudtrail_encryption_kms(CloudTrail),
             self.control_3_08_ensure_kms_cmk_rotation(regions),
             self.control_3_09_ensure_flow_logs_enabled_on_all_vpc(regions),
             self.control_3_1_ensure_logging_enabled_for_s3_write(regions),
             self.control_3_1_1_ensure_logging_enabled_for_s3_read(regions),
-
+            
             # Monitoring_control_4
-
+            
             self.control_4_0_1_ensure_log_metric_filter_unauthorized_api_calls(CloudTrail),
             self.control_4_0_2_ensure_log_metric_filter_console_signin_no_mfa(CloudTrail),
             self.control_4_0_3_ensure_log_metric_filter_root_usage(CloudTrail),
             self.control_4_0_4_ensure_log_metric_iam_policy_change(CloudTrail),
             self.control_4_0_5_ensure_log_metric_cloudtrail_configuration_changes(CloudTrail),
             self.control_4_0_6_ensure_log_metric_console_auth_failures(CloudTrail),
             self.control_4_0_7_ensure_log_metric_disabling_scheduled_delete_of_kms_cmk(CloudTrail),
@@ -109,15 +110,15 @@
             self.control_4_1_ensure_log_metric_security_group_changes(CloudTrail),
             self.control_4_11_ensure_log_metric_nacl(CloudTrail),
             self.control_4_12_ensure_log_metric_changes_to_network_gateways(CloudTrail),
             self.control_4_13_ensure_log_metric_changes_to_route_tables(CloudTrail),
             self.control_4_14_ensure_log_metric_changes_to_vpc(CloudTrail),
             self.control_4_15_ensure_log_metric_changes_to_org(CloudTrail),
             self.control_4_16_ensure_security_hub_is_enabled(regions),
-
+            
             # networking control
             self.control_5_01_no_nacl_allow_ingress(regions),
             self.control_5_02_ensure_admin_ports_open_to_world_over_ipv4(regions),
             self.control_5_03_ensure_ports_open_to_world_over_ipv6(regions),
             self.control_5_04_ensure_default_security_groups_restricts_traffic(regions),
             self.control_5_05_ensure_route_tables_are_least_access(regions)
         ]
```

### Comparing `cis_checks_2023-2.0.3/cis_checks_2023/_security_control_5.py` & `cis_checks_2023-2.0.4/cis_checks_2023/_security_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.3/cis_checks_2023/iam_control_1.py` & `cis_checks_2023-2.0.4/cis_checks_2023/iam_control_1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """iam_control_1.py"""
 import sys
 
-import botocore.errorfactory
-import botocore.exceptions
 import pytz
+from botocore.exceptions import ClientError
 from dateutil.relativedelta import relativedelta
 
 from cis_checks_2023.utils import *
 
 global logger
 logging.basicConfig(level=logging.INFO)
 
@@ -550,39 +549,46 @@
         failReason = ""
         offenders = []
         control = "1.16"
         description = "Ensure IAM policies that allow full *:* administrative privileges are not attached"
         scored = True
         # global IAM_CLIENT
 
-        paginator = self.session.client('iam').get_paginator('list_policies')
-        response_iterator = paginator.paginate(OnlyAttached=True)
-        pagedResult = []
-        for page in response_iterator:
-            for n in page['Policies']:
-                pagedResult.append(n)
-        offenders = []
-        for n in pagedResult:
-            policy = self.session.client('iam').get_policy_version(
-                PolicyArn=n["Arn"],
-                VersionId=n["DefaultVersionId"]
-            )
-            statements = policy['PolicyVersion']['Document']['Statement']
+        try:
+            paginator = self.session.client('iam').get_paginator('list_policies')
+            response_iterator = paginator.paginate(OnlyAttached=True)
+            pagedResult = []
+            for page in response_iterator:
+                for n in page['Policies']:
+                    pagedResult.append(n)
+            offenders = []
+            for n in pagedResult:
+                policy = self.session.client('iam').get_policy_version(
+                    PolicyArn=n["Arn"],
+                    VersionId=n["DefaultVersionId"]
+                )
+                statements = policy['PolicyVersion']['Document']['Statement']
+
+                for statement in statements:
+                    
+                        if statement["Effect"] == "Allow":
+                            try:
+                                if statement["Action"] == "*" and statement["Resource"] == "*":
+                                    result = "Not Compliant"
+                                    failReason = "IAM policies that allow full *:* administrative privileges are attached"
+                                    offenders.append(n["Arn"])
+                                else:
+                                    continue
+                            except KeyError:
+                                pass
+        except botocore.exceptions.ClientError as error:
+                logger.error(f" Exception while listing policies: {error}")
+                result = "Not Compliant"
+                failReason = "Client Error while listing policies "+str(error)
 
-            for statement in statements:
-                if statement["Effect"] == "Allow":
-                    try:
-                        if statement["Action"] == "*" and statement["Resource"] == "*":
-                            result = "Not Compliant"
-                            failReason = "IAM policies that allow full *:* administrative privileges are attached"
-                            offenders.append(n["Arn"])
-                        else:
-                            continue
-                    except KeyError:
-                        pass
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.17 Ensure a support role has been created to manage incidents with AWS Support (Scored)
     def control_1_17_AWS_support_role_created(self):
         logger.info(" ---Inside iam_control_1 :: control_1_17_AWS_support_role_created()--- ")
         """Summary
@@ -704,34 +710,41 @@
         offenders = []
         control = "1.2"
         description = "Ensure that IAM Access analyzer is enabled for all regions"
         scored = True
 
         for region in regions:
             client = self.session.client('accessanalyzer', region_name=region)
-            response = client.list_analyzers()
-            # print(response)
             try:
-                if response['analyzers'] == []:
-                    result = "Not Compliant"
-                    failReason = "IAM Access analyzer is not enabled for all regions"
-                    offenders.append(region)
-                else:
-                    continue
-            except KeyError:
-                pass
+
+                response = client.list_analyzers()
+                #print(response)
+                try:
+                    if response['analyzers'] == []:
+                        result = "Not Compliant"
+                        failReason = "IAM Access analyzer is not enabled for all regions"
+                        offenders.append(region)
+                    else:
+                        continue
+                except KeyError:
+                    pass
+            except botocore.exceptions.ClientError as error:
+                logger.error(f" Exception while listing analyzers: {error}")
+                result = "Not Compliant"
+                failReason = "Exception while listing analyzers "+str(error)
+                offenders.append(region)
 
         return {
             'Result': result,
             'failReason': failReason,
             'Offenders': offenders,
             'ScoredControl': scored,
             'Description': description,
             'ControlId': control
-        }
+        } 
 
     # 1.21 Ensure IAM users are managed centrally via identity federation or AWS Organizations for multi-account
     # environments
     def control_1_21_iam_user_managed_centrally(self):
         logger.info(" ---Inside iam_control_1 :: control_1_21_iam_user_managed_centrally()--- ")
         """Summary
```

### Comparing `cis_checks_2023-2.0.3/cis_checks_2023/logging_control_3.py` & `cis_checks_2023-2.0.4/cis_checks_2023/logging_control_3.py`

 * *Files 3% similar despite different names*

```diff
@@ -405,15 +405,15 @@
                 if not str(m['VpcId']) in str(activeLogs):
                     result = "Not Compliant"
                     failReason = "VPC without active VPC Flow Logs found"
                     offenders.append(str(n) + " : " + str(m['VpcId']))
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
-    # 3.1 Ensure that Object-level logging for write events is enabled for S3 bucket
+   # 3.1 Ensure that Object-level logging for write events is enabled for S3 bucket
 
     def control_3_1_ensure_logging_enabled_for_s3_write(self, regions):
         logger.info(" ---Inside networking_control_3 :: control_3_1_ensure_logging_enabled_for_s3_write()--- ")
         """Summary
     
         Returns:
             TYPE: Description
@@ -422,41 +422,50 @@
         failReason = ""
         offenders = []
         control = "3.1"
         description = "Ensure that Object-level logging for write events is enabled for S3 bucket"
         scored = True
 
         for region in regions:
-            paginator = self.session.client('cloudtrail', region_name=region).get_paginator('list_trails')
-            response_iterator = paginator.paginate()
-            pagedResult = []
-            for page in response_iterator:
-                for n in page['Trails']:
-                    pagedResult.append(n)
-
-            for n in pagedResult:
-                event_selectors = self.session.client('cloudtrail', region_name=region).get_event_selectors(
-                    TrailName=n['Name']
-                )
-                #print(event_selectors)
-                try:
-                    if 'EventSelectors' in event_selectors:
-                        for i in event_selectors["EventSelectors"]:
-                            if i["DataResources"] == []:
-                                result = 'Not Compliant'
-                                failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
-                                offenders.append(event_selectors['TrailARN'])
-                            else:
-                                continue
-                    else:
-                        result = 'Not Compliant'
-                        failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
-                        offenders.append(event_selectors['TrailARN'])
-                except:
-                    KeyError
+            try:
+
+                paginator = self.session.client('cloudtrail', region_name=region).get_paginator('list_trails')
+                response_iterator = paginator.paginate()
+                pagedResult = []
+                for page in response_iterator:
+                    for n in page['Trails']:
+                        pagedResult.append(n)
+
+                for n in pagedResult:
+                    event_selectors = self.session.client('cloudtrail', region_name=region).get_event_selectors(
+                        TrailName=n['Name']
+                    )
+                    #print(event_selectors)
+                    try:
+                        if 'EventSelectors' in event_selectors:
+                            for i in event_selectors["EventSelectors"]:
+
+                                if i["DataResources"] == []:
+                                    result = 'Not Compliant'
+                                    failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
+                                    offenders.append(event_selectors['TrailARN'])
+                                else:
+                                    continue
+                        else:
+                            result = 'Not Compliant'
+                            failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
+                            offenders.append(event_selectors['TrailARN'])
+                    except:
+                        KeyError
+            except botocore.exceptions.ClientError as error:
+                logger.error(f" Exception while listing trails: {error}")
+                result = "Not Compliant"
+                failReason = "Exception while listing trails "+str(error)
+                offenders.append(region)
+            
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.11 Ensure that Object-level logging for read events is enabled for S3 bucket
 
     def control_3_1_1_ensure_logging_enabled_for_s3_read(self, regions):
         logger.info(" ---Inside networking_control_3 :: control_3_1_1_ensure_logging_enabled_for_s3_read()--- ")
@@ -465,39 +474,48 @@
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
         offenders = []
         control = "3.11"
-        description = "Ensure that Object-level logging for write events is enabled for S3 bucket"
+        description = "Ensure that Object-level logging for read events is enabled for S3 bucket"
         scored = True
         for region in regions:
-            paginator = self.session.client('cloudtrail', region_name=region).get_paginator('list_trails')
-            response_iterator = paginator.paginate()
-            pagedResult = []
-            for page in response_iterator:
-                for n in page['Trails']:
-                    pagedResult.append(n)
-
-            for n in pagedResult:
-                event_selectors = self.session.client('cloudtrail', region_name=region).get_event_selectors(
-                    TrailName=n['Name']
-                )
-                try:
-
-                    if 'EventSelectors' in event_selectors:
-                        for i in event_selectors["EventSelectors"]:
-                            if i["DataResources"] == []:
-                                result = 'Not Compliant'
-                                failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
-                                offenders.append(event_selectors['TrailARN'])
-                            else:
-                                continue
-                    else:
-                        result = 'Not Compliant'
-                        failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
-                        offenders.append(event_selectors['TrailARN'])
-                except:
-                    KeyError
+
+            try:
+
+                paginator = self.session.client('cloudtrail', region_name=region).get_paginator('list_trails')
+                response_iterator = paginator.paginate()
+                pagedResult = []
+                for page in response_iterator:
+                    for n in page['Trails']:
+                        pagedResult.append(n)
+
+                for n in pagedResult:
+                    event_selectors = self.session.client('cloudtrail', region_name=region).get_event_selectors(
+                        TrailName=n['Name']
+                    )
+                    try:
+
+                        if 'EventSelectors' in event_selectors:
+                            for i in event_selectors["EventSelectors"]:
+                                if i["DataResources"] == []:
+                                    result = 'Not Compliant'
+                                    failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
+                                    offenders.append(event_selectors['TrailARN'])
+                                else:
+                                    continue
+                        else:
+                            result = 'Not Compliant'
+                            failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
+                            offenders.append(event_selectors['TrailARN'])
+                    except:
+                        KeyError
+            except botocore.exceptions.ClientError as error:
+                logger.error(f" Exception while listing trails: {error}")
+                result = "Not Compliant"
+                failReason = "Exception while listing trails "+str(error)
+                offenders.append(region)
+                
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
```

### Comparing `cis_checks_2023-2.0.3/cis_checks_2023/monitoring_control_4.py` & `cis_checks_2023-2.0.4/cis_checks_2023/monitoring_control_4.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.3/cis_checks_2023/networking_control_5.py` & `cis_checks_2023-2.0.4/cis_checks_2023/networking_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.3/cis_checks_2023/storage_control_2.py` & `cis_checks_2023-2.0.4/cis_checks_2023/storage_control_2.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.3/cis_checks_2023/utils.py` & `cis_checks_2023-2.0.4/cis_checks_2023/utils.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.3/cis_checks_2023.egg-info/PKG-INFO` & `cis_checks_2023-2.0.4/cis_checks_2023.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cis-checks-2023
-Version: 2.0.3
+Version: 2.0.4
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.3/pyproject.toml` & `cis_checks_2023-2.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "cis_checks_2023"
-version = "2.0.3"
+version = "2.0.4"
 authors = [
   { name="Dheeraj Banodha", email="dheeraj.banodha@impetus.com" },
   { name="Ravish Sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

