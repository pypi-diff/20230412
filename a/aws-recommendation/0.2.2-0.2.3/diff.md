# Comparing `tmp/aws_recommendation-0.2.2.tar.gz` & `tmp/aws_recommendation-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_recommendation-0.2.2.tar", last modified: Wed Apr  5 08:41:16 2023, max compression
+gzip compressed data, was "aws_recommendation-0.2.3.tar", last modified: Wed Apr 12 12:11:30 2023, max compression
```

## Comparing `aws_recommendation-0.2.2.tar` & `aws_recommendation-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 08:41:16.613756 aws_recommendation-0.2.2/
--rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 aws_recommendation-0.2.2/LICENCE
--rw-rw-rw-   0        0        0     1220 2023-04-05 08:41:16.612755 aws_recommendation-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-04-04 11:43:43.000000 aws_recommendation-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 08:41:16.601757 aws_recommendation-0.2.2/aws_recommendation/
--rw-rw-rw-   0        0        0     1579 2023-04-05 08:40:52.000000 aws_recommendation-0.2.2/aws_recommendation/__init__.py
--rw-rw-rw-   0        0        0     4633 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/cloudwatch.py
--rw-rw-rw-   0        0        0    11840 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/cost_estimations.py
--rw-rw-rw-   0        0        0     3636 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/dynamodb.py
--rw-rw-rw-   0        0        0    16652 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/ebs.py
--rw-rw-rw-   0        0        0    23966 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/ec2.py
--rw-rw-rw-   0        0        0     7927 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/elb.py
--rw-rw-rw-   0        0        0     3571 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/kms.py
--rw-rw-rw-   0        0        0    10666 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/rds.py
--rw-rw-rw-   0        0        0     3334 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/recommendation.py
--rw-rw-rw-   0        0        0     5257 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/redshift.py
--rw-rw-rw-   0        0        0    13828 2023-04-04 11:43:43.000000 aws_recommendation-0.2.2/aws_recommendation/s3.py
--rw-rw-rw-   0        0        0     1564 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/truted_advisor.py
--rw-rw-rw-   0        0        0     3711 2023-04-04 10:14:19.000000 aws_recommendation-0.2.2/aws_recommendation/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 08:41:16.610757 aws_recommendation-0.2.2/aws_recommendation.egg-info/
--rw-rw-rw-   0        0        0     1220 2023-04-05 08:41:16.000000 aws_recommendation-0.2.2/aws_recommendation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-04-05 08:41:16.000000 aws_recommendation-0.2.2/aws_recommendation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 08:41:16.000000 aws_recommendation-0.2.2/aws_recommendation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-05 08:41:16.000000 aws_recommendation-0.2.2/aws_recommendation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      491 2023-04-05 08:40:52.000000 aws_recommendation-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 08:41:16.614756 aws_recommendation-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 12:11:30.018588 aws_recommendation-0.2.3/
+-rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 aws_recommendation-0.2.3/LICENCE
+-rw-rw-rw-   0        0        0     1220 2023-04-12 12:11:30.017590 aws_recommendation-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-04-04 11:43:43.000000 aws_recommendation-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 12:11:30.003589 aws_recommendation-0.2.3/aws_recommendation/
+-rw-rw-rw-   0        0        0     2333 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/__init__.py
+-rw-rw-rw-   0        0        0     5487 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/cloudwatch.py
+-rw-rw-rw-   0        0        0    11769 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/cost_estimations.py
+-rw-rw-rw-   0        0        0     4287 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/dynamodb.py
+-rw-rw-rw-   0        0        0    15213 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/ebs.py
+-rw-rw-rw-   0        0        0    26661 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/ec2.py
+-rw-rw-rw-   0        0        0     8961 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/elb.py
+-rw-rw-rw-   0        0        0     4208 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/kms.py
+-rw-rw-rw-   0        0        0    11638 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/rds.py
+-rw-rw-rw-   0        0        0     5955 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/redshift.py
+-rw-rw-rw-   0        0        0    11003 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/s3.py
+-rw-rw-rw-   0        0        0     1726 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/truted_advisor.py
+-rw-rw-rw-   0        0        0     5821 2023-04-12 12:09:37.000000 aws_recommendation-0.2.3/aws_recommendation/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:11:30.013590 aws_recommendation-0.2.3/aws_recommendation.egg-info/
+-rw-rw-rw-   0        0        0     1220 2023-04-12 12:11:29.000000 aws_recommendation-0.2.3/aws_recommendation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-04-12 12:11:29.000000 aws_recommendation-0.2.3/aws_recommendation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 12:11:29.000000 aws_recommendation-0.2.3/aws_recommendation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-12 12:11:29.000000 aws_recommendation-0.2.3/aws_recommendation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      491 2023-04-12 12:11:07.000000 aws_recommendation-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 12:11:30.018588 aws_recommendation-0.2.3/setup.cfg
```

### Comparing `aws_recommendation-0.2.2/PKG-INFO` & `aws_recommendation-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_recommendation
-Version: 0.2.2
+Version: 0.2.3
 Summary: Provides AWS recommendations
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `aws_recommendation-0.2.2/README.md` & `aws_recommendation-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.2/aws_recommendation/cloudwatch.py` & `aws_recommendation-0.2.3/aws_recommendation/cloudwatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,75 @@
 from botocore.exceptions import ClientError
 
+from aws_recommendation import utils
 from aws_recommendation.utils import *
 
+import logging
+r_logger = logging.getLogger('Recommender')
+r_logger.setLevel(logging.DEBUG)
+
+logger = logging.getLogger()
+
+class cloudwatch:
+    # returns aggregated cloudwatch recommendations
+    def get_cw_recommendations(self, regions) -> list:
+        """
+        :return:
+        """
+        logger.info(" ---Inside cloudwatch.cloudwatch :: get_cw_recommendations()--- ")
+
+        return self.__log_group_retention_period_check(regions)
+
+    #Generate the recommendation for log groups with no retention period
+    def __log_group_retention_period_check(self, regions: list) -> list:
+        """
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside log_group_retention_period_check()")
+
+        recommendation = []
+
+        for region in regions:
+            try:
+                client = self.session.client('logs', region_name=region)
 
-#Generate the recommendation for log groups with no retention period
-def log_group_retention_period_check(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside log_group_retention_period_check()")
-
-    recommendation = []
-
-    regions = self.regions
-
-    for region in regions:
-        try:
-            client = self.session.client('logs', region_name=region)
-
-            marker = ''
-            while True:
-                if marker == '':
-                    response = client.describe_log_groups()
-                else:
-                    response = client.describe_log_groups(
-                        nextToken=marker
-                    )
-                for group in response['logGroups']:
-                    try:
-                        retention_period = group['retentionInDays']
-                        if retention_period <= 0:
+                marker = ''
+                while True:
+                    if marker == '':
+                        response = client.describe_log_groups()
+                    else:
+                        response = client.describe_log_groups(
+                            nextToken=marker
+                        )
+                    for group in response['logGroups']:
+                        try:
+                            retention_period = group['retentionInDays']
+                            if retention_period <= 0:
+                                temp = {
+                                    'Service Name': 'CloudWatch',
+                                    'Id': group['logGroupName'],
+                                    'Recommendation': 'Add retention period in log group',
+                                    'Description': 'Enabling the retention period will reduce the aws costs',
+                                    'Metadata': {
+                                        'Region': region,
+                                        'creation time': group['creationTime'],
+                                        'arn': group['arn'],
+                                        'storedBytes': group['storedBytes']
+                                    },
+                                    'Recommendation Reason': {
+                                        'reason': 'Retention period is not set on the log group'
+                                    },
+                                    'Risk': 'Medium',
+                                    'Savings': None,
+                                    'Source': 'Klera',
+                                    'Category': 'Cost Optimization'
+                                }
+                                recommendation.append(temp)
+                        except KeyError:
                             temp = {
                                 'Service Name': 'CloudWatch',
                                 'Id': group['logGroupName'],
                                 'Recommendation': 'Add retention period in log group',
                                 'Description': 'Enabling the retention period will reduce the aws costs',
                                 'Metadata': {
                                     'Region': region,
@@ -47,60 +82,39 @@
                                 },
                                 'Risk': 'Medium',
                                 'Savings': None,
                                 'Source': 'Klera',
                                 'Category': 'Cost Optimization'
                             }
                             recommendation.append(temp)
-                    except KeyError:
-                        temp = {
-                            'Service Name': 'CloudWatch',
-                            'Id': group['logGroupName'],
-                            'Recommendation': 'Add retention period in log group',
-                            'Description': 'Enabling the retention period will reduce the aws costs',
-                            'Metadata': {
-                                'Region': region,
-                                'creation time': group['creationTime'],
-                                'arn': group['arn'],
-                                'storedBytes': group['storedBytes']
-                            },
-                            'Recommendation Reason': {
-                                'reason': 'Retention period is not set on the log group'
-                            },
-                            'Risk': 'Medium',
-                            'Savings': None,
-                            'Source': 'Klera',
-                            'Category': 'Cost Optimization'
-                        }
-                        recommendation.append(temp)
 
-                try:
-                    marker = response['nextToken']
-                    if marker == '':
+                    try:
+                        marker = response['nextToken']
+                        if marker == '':
+                            break
+                    except KeyError:
                         break
-                except KeyError:
-                    break
 
-        except ClientError as e:
-            if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
-                logger.info('---------Cloudwatch read access denied----------')
-                temp = {
-                    'Service Name': 'CloudWatch',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'Medium',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.warning("Something went wrong with the region {}: {}".format(region, e))
+            except ClientError as e:
+                if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
+                    logger.info('---------Cloudwatch read access denied----------')
+                    temp = {
+                        'Service Name': 'CloudWatch',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Access Denied'
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'Medium',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+                    return recommendation
+                logger.warning("Something went wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/cost_estimations.py` & `aws_recommendation-0.2.3/aws_recommendation/cost_estimations.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,17 +111,18 @@
     d1['Number of Instances'] = d1['Number of Instances']+d2['Number of Instances']
     # print('after addition'+str(d1['Number of Instances']))
 
     return d1
 
 
 # Generates the cost estimations for different upgrades
-def estimated_savings(self) -> list:
+def estimated_savings(self, regions, ec2_instances) -> list:
     """
-
+    :param ec2_instances:
+    :param regions:
     :param self:
     :return list: details of estimated savings
     """
     logger.info(" ---Inside cost_estimations :: estimated_savings()")
 
     possible_upgrade = [
             ('t1.micro', 't2.micro'),
@@ -175,43 +176,43 @@
             # ('t2.2xlarge', 't2.xlarge'),
             # ('t2.xlarge', 't2.large'),
             # ('t2.large', 't2.medium')
         ]
 
     recommendations = []
 
-    regions = self.regions
+
     available_instance_types = {}
-    for region in regions:
-        try:
-            instance_list = list_instances(self, region)
-            for instance in instance_list:
+
+    try:
+        for region, instances in ec2_instances.items():
+            for instance in instances:
                 # available_instance_types.add(instance['InstanceType'])
                 available_instance_types.setdefault(instance['InstanceType'], []).append(region)
 
-        except botocore.exceptions.ClientError as e:
-            if e.response['Error']['Code'] == 'UnauthorizedOperation':
-                logger.info('---------EC2 read access denied----------')
-                temp = {
-                    'Service Name': 'RDS',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'Low',
-                    'Savings': None
-                }
-                recommendations.append(temp)
-                return recommendations
-            logger.error("Something went wrong with region {}: {}".format(region, e))
+    except botocore.exceptions.ClientError as e:
+        if e.response['Error']['Code'] == 'UnauthorizedOperation':
+            logger.info('---------EC2 read access denied----------')
+            temp = {
+                'Service Name': 'RDS',
+                'Id': 'Access Denied',
+                'Recommendation': 'Access Denied',
+                'Description': 'Access Denied',
+                'Metadata': {
+                    'Access Denied'
+                },
+                'Recommendation Reason': {
+                    'Access Denied'
+                },
+                'Risk': 'Low',
+                'Savings': None
+            }
+            recommendations.append(temp)
+            return recommendations
+        logger.error("Something went wrong with region {}: {}".format(region, e))
 
     # print('available_instance_types'+str(available_instance_types.items()))
 
     for instance_type, regions in available_instance_types.items():
         blacklist = []
         for up in possible_upgrade:
             if up[0] == instance_type and not up[1] in blacklist:
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/dynamodb.py` & `aws_recommendation-0.2.3/aws_recommendation/dynamodb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,95 @@
 from botocore.exceptions import ClientError
 
 from aws_recommendation.utils import *
 
 
-# generated the recommendations for unused dynamodb tables
-def unused_dynamodb_tables(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside dynamodb :: unused_dynamodb_tables()")
-
-    recommendation = []
-    regions = self.regions
-
-    for region in regions:
-        try:
-            client = self.session.client('dynamodb', region_name=region)
-
-            marker=''
-            while True:
-                if marker == '':
-                    response = client.list_tables()
-                else:
-                    response = client.list_tables(
-                        ExclusiveStartTableName=marker
-                    )
-                for table in response['TableNames']:
-                    table_desc = client.describe_table(
-                        TableName=table
-                    )
-                    if table_desc['Table']['ItemCount'] == 0:
-                        temp = {
-                            'Service Name': 'DynamoDB',
-                            'Id': table,
-                            'Recommendation': 'Remove Dynamodb table',
-                            'Description': 'Identify any unused Amazon DynamoDB tables available within your AWS account and remove them to help lower the cost of your monthly AWS bill. A DynamoDB table is considered unused if it’s ItemCount parameter, which describes the number of items in the table, is equal to 0 (zero)',
-                            'Metadata': {
-                                'Region': region,
-                                'TableStatus': table_desc['TableStatus']
-                            },
-                            'Recommendation Reason': {
-                                'reason': "The ItemCount parameter value is 0, therefore the selected amazon dynamodb table is not currently in use and can be safely removed from your AWS Account"
-                            },
-                            'Risk': 'Medium',
-                            'Savings': None,
-                            'Source': 'Klera',
-                            'Category': 'Cost Optimization'
-                        }
-                        recommendation.append(temp)
-                try:
-                    marker = response['LastEvaluatedTableName']
+class dynamodb:
+    def get_dynamodb_recommendations(self, regions=None):
+        """
+        :param regions:
+        :return:
+        """
+        logger.info(" ---Inside dynamodb :: get_dynamodb_recommendations()--- ")
+
+        if regions is None:
+            regions = self.get_regions()
+
+        return self.unused_dynamodb_tables(regions)
+
+    # generated the recommendations for unused dynamodb tables
+    def unused_dynamodb_tables(self, regions) -> list:
+        """
+        :param regions:
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside dynamodb :: unused_dynamodb_tables()")
+
+        recommendation = []
+
+        for region in regions:
+            try:
+                client = self.session.client('dynamodb', region_name=region)
+
+                marker=''
+                while True:
                     if marker == '':
+                        response = client.list_tables()
+                    else:
+                        response = client.list_tables(
+                            ExclusiveStartTableName=marker
+                        )
+                    for table in response['TableNames']:
+                        table_desc = client.describe_table(
+                            TableName=table
+                        )
+                        if table_desc['Table']['ItemCount'] == 0:
+                            temp = {
+                                'Service Name': 'DynamoDB',
+                                'Id': table,
+                                'Recommendation': 'Remove Dynamodb table',
+                                'Description': 'Identify any unused Amazon DynamoDB tables available within your AWS account and remove them to help lower the cost of your monthly AWS bill. A DynamoDB table is considered unused if it’s ItemCount parameter, which describes the number of items in the table, is equal to 0 (zero)',
+                                'Metadata': {
+                                    'Region': region,
+                                    'TableStatus': table_desc['TableStatus']
+                                },
+                                'Recommendation Reason': {
+                                    'reason': "The ItemCount parameter value is 0, therefore the selected amazon dynamodb table is not currently in use and can be safely removed from your AWS Account"
+                                },
+                                'Risk': 'Medium',
+                                'Savings': None,
+                                'Source': 'Klera',
+                                'Category': 'Cost Optimization'
+                            }
+                            recommendation.append(temp)
+                    try:
+                        marker = response['LastEvaluatedTableName']
+                        if marker == '':
+                            break
+                    except KeyError:
                         break
-                except KeyError:
-                    break
-        except ClientError as e:
-            if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
-                logger.warning(e)
-                logger.info('---------Dynamodb read access denied----------')
-                temp = {
-                    'Service Name': 'DynamoDB',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'Medium',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.warning("Something went wrong with the region {}: {}".format(region, e))
+            except ClientError as e:
+                if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
+                    logger.warning(e)
+                    logger.info('---------Dynamodb read access denied----------')
+                    temp = {
+                        'Service Name': 'DynamoDB',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Access Denied'
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'Medium',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+                    return recommendation
+                logger.warning("Something went wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/ebs.py` & `aws_recommendation-0.2.3/aws_recommendation/ebs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 from botocore.exceptions import ClientError
 
 from aws_recommendation.utils import *
 
 
-# Generated the recommendation for unused EBS volumes
-def idle_ebs_volumes(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside ebs :: unused_ebs_volumes")
+class ebs:
+    def get_ebs_recommendations(self, regions=None, ebs_volumes=None)-> list:
+        """
+        :param regions:
+        :param ebs_volumes:
+        :return:
+        """
+        logger.info(" ---Inside ebs :: get_ebs_recommendations()--- ")
+
+        if regions is None:
+            regions = self.get_regions()
+        if ebs_volumes is None:
+            ebs_volumes = self.list_ebs_volumes(regions)
+
+        return self.idle_ebs_volumes(ebs_volumes) + self.ebs_general_purpose_ssd(ebs_volumes) + \
+            self.unused_ebs_volume(ebs_volumes) + self.gp2_to_gp3(ebs_volumes)
+
+    # Generated the recommendation for unused EBS volumes
+    def idle_ebs_volumes(self, ebs_volumes) -> list:
+        """
+        :param ebs_volumes:
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside ebs :: idle_ebs_volumes")
 
-    recommendation = []
-    regions = self.regions
+        recommendation = []
 
-    for region in regions:
         try:
-            client = self.session.client('ec2', region_name=region)
-            marker = ''
-            while True:
-                response = client.describe_volumes(
-                    Filters=[
-                        {
-                            'Name': 'status',
-                            'Values': [
-                                'in-use'
-                            ]
-                        },
-                    ],
-                    MaxResults=500,
-                    NextToken=marker
-                )
-                for volume in response['Volumes']:
+            for region, volumes in ebs_volumes.items():
+                for volume in volumes:
                     # device = volume['Attachments']['Device']
                     if '/dev/xvda' not in [x['Device'] for x in volume['Attachments']]:
-                        read_datapoints = get_metrics_stats(
-                            self=self,
+                        read_datapoints = self.get_metrics_stats(
                             region=region,
                             namespace='AWS/EBS',
                             dimensions= [
                                 {
                                     'Name':'VolumeId',
                                     'Value': volume['VolumeId']
                                 }
@@ -56,16 +57,15 @@
 
                         flag = True
 
                         if sum_read_ops > 1:
                             flag = False
 
                         if flag:
-                            write_datapoints = get_metrics_stats(
-                                self=self,
+                            write_datapoints = self.get_metrics_stats(
                                 region=region,
                                 namespace='AWS/EBS',
                                 dimensions=[
                                     {
                                         'Name': 'VolumeId',
                                         'Value': volume['VolumeId']
                                     }
@@ -111,20 +111,15 @@
                                     },
                                     'Risk': 'Medium',
                                     'Savings': None,
                                     'Source': 'Klera',
                                     'Category': 'Cost Optimization'
                                 }
                                 recommendation.append(temp)
-                try:
-                    marker = response['NextToken']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
+
         except ClientError as e:
             if e.response['Error']['Code'] == 'UnauthorizedOperation':
                 logger.info('---------EBS read access denied----------')
                 temp = {
                     'Service Name': 'EC2 (EBS)',
                     'Id': 'Access Denied',
                     'Recommendation': 'Access Denied',
@@ -140,38 +135,31 @@
                     'Source': 'Klera',
                     'Category': 'Cost Optimization'
                 }
                 recommendation.append(temp)
                 return recommendation
             logger.info("Something went wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
 
 
-# Generated the recommendation for general purpose ssd
-def ebs_general_purpose_ssd(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside ebs :: ebs_general_purpose_ssd()")
+    # Generated the recommendation for general purpose ssd
+    def ebs_general_purpose_ssd(self, ebs_volumes) -> list:
+        """
+        :param ebs_volumes:
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside ebs :: ebs_general_purpose_ssd()")
 
-    recommendation = []
-    regions = self.regions
+        recommendation = []
 
-    for region in regions:
         try:
-            client = self.session.client('ec2', region_name=region)
-            marker = ''
-            while True:
-                response = client.describe_volumes(
-                    MaxResults=500,
-                    NextToken=marker
-                )
-                for volume in response['Volumes']:
+            for region, volumes in ebs_volumes.items():
+                for volume in volumes:
                     storage_type = volume['VolumeType']
                     if storage_type == 'io1' or storage_type == 'io2':
                         try:
                             tags = volume['Tags']
                         except KeyError:
                             tags = None
 
@@ -193,20 +181,14 @@
                             'Risk': 'Medium',
                             'Savings': None,
                             'Source': 'Klera',
                             'Category': 'Cost Optimization'
                         }
                         recommendation.append(temp)
 
-                try:
-                    marker = response['NextToken']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
         except ClientError as e:
             if e.response['Error']['Code'] == 'UnauthorizedOperation':
                 logger.info('---------EBS read access denied----------')
                 temp = {
                     'Service Name': 'EC2 (EBS)',
                     'Id': 'Access Denied',
                     'Recommendation': 'Access Denied',
@@ -222,38 +204,31 @@
                     'Source': 'Klera',
                     'Category': 'Cost Optimization'
                 }
                 recommendation.append(temp)
                 return recommendation
             logger.warning("Something went wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
 
 
-# Generate the recommendation for upgrade volume from GP2 to gp3 to save cost
-def gp2_to_gp3(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside ebs :: gp2_to_gp3()")
+    # Generate the recommendation for upgrade volume from GP2 to gp3 to save cost
+    def gp2_to_gp3(self, ebs_volumes) -> list:
+        """
+        :param ebs_volumes:
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside ebs :: gp2_to_gp3()")
 
-    recommendation = []
-    regions = self.regions
+        recommendation = []
 
-    for region in regions:
         try:
-            client = self.session.client('ec2', region_name=region)
-            marker = ''
-            while True:
-                response = client.describe_volumes(
-                    MaxResults=500,
-                    NextToken=marker
-                )
-                for volume in response['Volumes']:
+            for region, volumes in ebs_volumes.items():
+                for volume in volumes:
                     storage_type = volume['VolumeType']
                     if storage_type == 'gp2':
                         try:
                             tags = volume['Tags']
                         except KeyError:
                             tags = None
 
@@ -276,20 +251,15 @@
                             },
                             'Risk': 'High',
                             'Savings': str(savings),
                             'Source': 'Klera',
                             'Category': 'Cost Optimization'
                         }
                         recommendation.append(temp)
-                try:
-                    marker = response['NextToken']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
+
         except ClientError as e:
             if e.response['Error']['Code'] == 'UnauthorizedOperation':
                 logger.info('---------EBS read access denied----------')
                 temp = {
                     'Service Name': 'EC2 (EBS)',
                     'Id': 'Access Denied',
                     'Recommendation': 'Access Denied',
@@ -305,40 +275,31 @@
                     'Source': 'Klera',
                     'Category': 'Cost Optimization'
                 }
                 recommendation.append(temp)
                 return recommendation
             logger.warning("Something went wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
 
 
-# Generate recommendation for unused ebs volume
-def unused_ebs_volume(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside ebs :: unused_ebs_volume()")
+    # Generate recommendation for unused ebs volume
+    def unused_ebs_volume(self, ebs_volumes) -> list:
+        """
+        :param ebs_volumes:
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside ebs :: unused_ebs_volume()")
 
-    recommendation = []
-    regions = self.regions
+        recommendation = []
 
-    for region in regions:
         try:
-            client = self.session.client('ec2', region_name=region)
-            marker = ''
-            while True:
-                if marker == '':
-                    response = client.describe_volumes()
-                else:
-                    response = client.describe_volumes(
-                        NextToken=marker
-                    )
-                for volume in response['Volumes']:
+            for region, volumes in ebs_volumes.items():
+                for volume in volumes:
                     state = volume['State']
                     if state == 'available':
                         try:
                             tags = volume['Tags']
                         except KeyError:
                             tags = None
 
@@ -359,21 +320,14 @@
                             'Risk': 'Medium',
                             'Savings': '100%',
                             'Source': 'Klera',
                             'Category': 'Cost Optimization'
                         }
                         recommendation.append(temp)
 
-                try:
-                    marker = response['NextToken']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
-
         except ClientError as e:
             if e.response['Error']['Code'] == 'UnauthorizedOperation':
                 logger.info('---------EBS read access denied----------')
                 temp = {
                     'Service Name': 'EC2 (EBS)',
                     'Id': 'Access Denied',
                     'Recommendation': 'Access Denied',
@@ -389,8 +343,8 @@
                     'Source': 'Klera',
                     'Category': 'Cost Optimization'
                 }
                 recommendation.append(temp)
                 return recommendation
             logger.warning("Something went wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/ec2.py` & `aws_recommendation-0.2.3/aws_recommendation/ec2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,104 +1,129 @@
 import botocore
 import pytz
 from botocore.exceptions import ClientError
 
 from aws_recommendation.utils import *
 
-logging.basicConfig(level=logging.INFO)
+import logging
+r_logger = logging.getLogger('Recommender')
+r_logger.setLevel(logging.DEBUG)
+
 logger = logging.getLogger()
 
+class ec2:
+    # returns ec2 recommendations
+    def get_ec2_recommendations(self, regions=None, ec2_instances=None):
+        """
+        :param ec2_instances:
+        :param regions:
+        :return:
+        """
+        logger.info(" ---Inside ec2 :: get_ec2_recommendations()--- ")
+        if regions is None:
+            regions = self.get_regions()
+        if ec2_instances is None:
+            ec2_instances = self.list_instances(regions)
+            r_logger.debug(ec2_instances)
+
+        response = []
+        response.extend(self.delete_or_downsize_instance_recommendation(ec2_instances))
+        response.extend(self.purge_unattached_vol_recommendation(regions))
+        response.extend(self.purge_8_weeks_older_snapshots(regions))
+        response.extend(self.unused_ami(regions))
+        response.extend(self.unassociated_elastic_ip_addresses(regions))
+        response.extend(self.reserved_instance_lease_expiration(regions))
+
+        return response
+
+
+    # Generates recommendation to delete idle instances
+    def delete_or_downsize_instance_recommendation(self, ec2_instances) -> list:
+        logger.info(" ---Inside delete_or_downsize_instance_recommendation()")
 
-# Generates recommendation to delete idle instances
-def delete_or_downsize_instance_recommendation(self) -> list:
-    logger.info(" ---Inside delete_or_downsize_instance_recommendation()")
+        recommendation = []
 
-    recommendation = []
-    regions = self.regions
 
-    # iterating through all the available regions
-    for region in regions:
         try:
-            instance_lst = list_instances(self, region)
-
-            for instance in instance_lst:
-                response_cpu = get_metrics_stats(self, region, "AWS/EC2", [{'Name': 'InstanceId', 'Value': instance['InstanceId']}])
-                # response_mem = get_metics_stats(session, region, "AWS/EC2", {'Name': 'InstanceId', 'Value': instance},
-                # metric_name=) response_net_in = get_metrics_stats(region, "AWS/EC2", [{'Name': 'InstanceId',
-                # 'Value': instance}], metric_name='NetworkIn') response_net_out = get_metrics_stats(region, "AWS/EC2",
-                # [{'Name': 'InstanceId', 'Value': instance}], metric_name='NetworkOut') # print(response_net_in) print(
-                # response_net_out) for r in response_net_in['Datapoints']: print(r['Average'])
+            for region, instances in ec2_instances.items():
+                for instance in instances:
+                    response_cpu = self.get_metrics_stats(region, "AWS/EC2", [{'Name': 'InstanceId', 'Value': instance['InstanceId']}])
+                    # response_mem = get_metics_stats(session, region, "AWS/EC2", {'Name': 'InstanceId', 'Value': instance},
+                    # metric_name=) response_net_in = get_metrics_stats(region, "AWS/EC2", [{'Name': 'InstanceId',
+                    # 'Value': instance}], metric_name='NetworkIn') response_net_out = get_metrics_stats(region, "AWS/EC2",
+                    # [{'Name': 'InstanceId', 'Value': instance}], metric_name='NetworkOut') # print(response_net_in) print(
+                    # response_net_out) for r in response_net_in['Datapoints']: print(r['Average'])
 
-                tmp_lst_cpu = []
+                    tmp_lst_cpu = []
 
-                for r in response_cpu['Datapoints']:
-                    tmp_lst_cpu.append(r['Average'])
+                    for r in response_cpu['Datapoints']:
+                        tmp_lst_cpu.append(r['Average'])
 
-                if len(tmp_lst_cpu) >= 7:
-                    if max(tmp_lst_cpu) < 3:
-                        try:
-                            tags = instance['Tags']
-                        except KeyError:
-                            tags = None
-                        try:
-                            platform = instance['Platform']
-                        except KeyError:
-                            platform = None
-                        temp = {
-                            'Service Name': 'EC2 (Instance)',
-                            'Id': instance['InstanceId'],
-                            'Recommendation': 'Delete idle compute instance',
-                            'Description': 'The Delete idle compute instances recommendation indicates that some compute instances are unused. Deleting unused compute instances saves you from paying for instances that you are not using.',
-                            'Metadata': {
-                                'Region': region,
-                                'Instance Type': instance['InstanceType'],
-                                'Tags': tags,
-                                'LaunchTime': instance['LaunchTime'],
-                                'Platform': platform
-                            },
-                            'Recommendation Reason': {
-                                'Average CPU Datapoints(7 days)': [float('{:.2f}'.format(x)) for x in tmp_lst_cpu]
-                            },
-                            'Risk': 'High',
-                            'Savings': None,
-                            'Source': 'Klera',
-                            'Category': 'Cost Optimization'
-                        }
-                        recommendation.append(temp)
-                    else:
-                        avg = 0
-                        for v in tmp_lst_cpu:
-                            avg = avg + v
-                        avg = avg / len(tmp_lst_cpu)
-
-                        if avg < 5:
+                    if len(tmp_lst_cpu) >= 7:
+                        if max(tmp_lst_cpu) < 3:
                             try:
                                 tags = instance['Tags']
                             except KeyError:
                                 tags = None
+                            try:
+                                platform = instance['Platform']
+                            except KeyError:
+                                platform = None
                             temp = {
-                                'Service Name': 'EC2 Instance',
+                                'Service Name': 'EC2 (Instance)',
                                 'Id': instance['InstanceId'],
-                                'Recommendation': 'Downsize underutilized compute instances',
-                                'Description': 'The Downsize underutilized compute instances recommendation indicates that some compute instances are bigger than needed. Implementing this recommendation saves you money without degrading performance.',
+                                'Recommendation': 'Delete idle compute instance',
+                                'Description': 'The Delete idle compute instances recommendation indicates that some compute instances are unused. Deleting unused compute instances saves you from paying for instances that you are not using.',
                                 'Metadata': {
                                     'Region': region,
                                     'Instance Type': instance['InstanceType'],
                                     'Tags': tags,
-                                    'LaunchTime': instance['LaunchTime']
+                                    'LaunchTime': instance['LaunchTime'],
+                                    'Platform': platform
                                 },
                                 'Recommendation Reason': {
                                     'Average CPU Datapoints(7 days)': [float('{:.2f}'.format(x)) for x in tmp_lst_cpu]
                                 },
                                 'Risk': 'High',
                                 'Savings': None,
                                 'Source': 'Klera',
                                 'Category': 'Cost Optimization'
                             }
                             recommendation.append(temp)
+                        else:
+                            avg = 0
+                            for v in tmp_lst_cpu:
+                                avg = avg + v
+                            avg = avg / len(tmp_lst_cpu)
+
+                            if avg < 5:
+                                try:
+                                    tags = instance['Tags']
+                                except KeyError:
+                                    tags = None
+                                temp = {
+                                    'Service Name': 'EC2 Instance',
+                                    'Id': instance['InstanceId'],
+                                    'Recommendation': 'Downsize underutilized compute instances',
+                                    'Description': 'The Downsize underutilized compute instances recommendation indicates that some compute instances are bigger than needed. Implementing this recommendation saves you money without degrading performance.',
+                                    'Metadata': {
+                                        'Region': region,
+                                        'Instance Type': instance['InstanceType'],
+                                        'Tags': tags,
+                                        'LaunchTime': instance['LaunchTime']
+                                    },
+                                    'Recommendation Reason': {
+                                        'Average CPU Datapoints(7 days)': [float('{:.2f}'.format(x)) for x in tmp_lst_cpu]
+                                    },
+                                    'Risk': 'High',
+                                    'Savings': None,
+                                    'Source': 'Klera',
+                                    'Category': 'Cost Optimization'
+                                }
+                                recommendation.append(temp)
 
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == 'UnauthorizedOperation':
                 logger.info('---------Ec2 read access denied----------')
                 temp = {
                     'Service Name': 'EC2',
                     'Id': 'Access Denied',
@@ -115,425 +140,423 @@
                     'Source': 'Klera',
                     'Category': 'Cost Optimization'
                 }
                 recommendation.append(temp)
                 return recommendation
             logger.info("Something wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
 
 
-# generates the recommendation to delete unattached volumes
-def purge_unattached_vol_recommendation(self) -> list:
-    logger.info(" ---Inside purge_unattached_vol_recommendation()")
+    # generates the recommendation to delete unattached volumes
+    def purge_unattached_vol_recommendation(self, regions) -> list:
+        logger.info(" ---Inside purge_unattached_vol_recommendation()")
+
+        recommendation = []
+
+        # iterating through all the available regions
+        for region in regions:
+            try:
+                vol_data = {}
+                client = self.session.client('ec2', region_name=region)
+                marker = ''
+                while True:
+                    response = client.describe_volumes(
+                        MaxResults=500,
+                        NextToken=marker
+                    )
+                    for item in response['Volumes']:
+                        create_time = item['CreateTime']
+                        datetime_4_weeks_ago = dt.datetime.now() - dt.timedelta(weeks=4)
+                        timezone = pytz.timezone("UTC")
+                        datetime_4_weeks_ago = timezone.localize(datetime_4_weeks_ago)
+
+                        older = create_time <= datetime_4_weeks_ago
+                        if older:
+                            # vol_data[item['VolumeId']] = item['Attachments']
+                            if len(item['Attachments']) == 0:
+                                try:
+                                    tags = item['Tags']
+                                except KeyError:
+                                    tags = None
+                                temp = {
+                                    'Service Name': 'EC2 (EBS)',
+                                    'Id': item['VolumeId'],
+                                    'Recommendation': 'Purge unattached volume',
+                                    'Description': 'The Delete unattached volumes recommendation indicates that unattached volumes exists. Attaching or deleting unattached volumes reduces costs.',
+                                    'Metadata': {
+                                        'Region': region,
+                                        'Instance Type': item['VolumeType'],
+                                        'Tags': tags,
+                                        'CreateTime': item['CreateTime']
+                                    },
+                                    'Recommendation Reason': {
+                                        'reason': 'This Volume is 4 weeks older and is not attached to any instance'
+                                    },
+                                    'Risk': 'Medium',
+                                    'Savings': None,
+                                    'Source': 'Klera',
+                                    'Category': 'Cost Optimization'
+                                }
+                                recommendation.append(temp)
+                    try:
+                        marker = response['NextToken']
+                        if marker == '':
+                            break
+                    except KeyError:
+                        break
 
-    recommendation = []
-    regions = self.regions
+            except botocore.exceptions.ClientError as e:
+                if e.response['Error']['Code'] == 'UnauthorizedOperation':
+                    logger.info('---------Ec2 read access denied----------')
+                    temp = {
+                        'Service Name': 'EC2 (EBS)',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Access Denied'
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'Medium',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+                    return recommendation
+                logger.info("Something wrong with the region {}: {}".format(region, e))
+
+        return recommendation
+
+
+    # Generates the recommendation to purge the snapshots which are older than 8 weeks
+    def purge_8_weeks_older_snapshots(self, regions) -> list:
+        logger.info(" ---Inside purge_8_weeks_older_snapshots()")
+
+        recommendation = []
+
+        datetime_8_weeks_ago = dt.datetime.now() - dt.timedelta(weeks=8)
+        timezone = pytz.timezone("UTC")
+        datetime_8_weeks_ago = timezone.localize(datetime_8_weeks_ago)
+
+        for region in regions:
+            try:
+                client = self.session.client('ec2', region_name=region)
+                marker = ''
+                while True:
+                    response = client.describe_snapshots(
+                        MaxResults=1000,
+                        OwnerIds=['self'],
+                        NextToken=marker
+                    )
+                    for snapshot in response['Snapshots']:
+                        start_time = snapshot['StartTime']
+                        older = start_time <= datetime_8_weeks_ago
+
+                        if older:
+                            service_name = 'EC2 (EBS)'
+                            r_id =  snapshot['SnapshotId']
+                            recom = 'Purge 8 week older snapshot'
+                            desc = 'The Delete 8 weeks older snapshot recommendation indicates that snapshots is older than 8 weeks exists. Deleting older snapshots reduces costs.'
 
-    # iterating through all the available regions
-    for region in regions:
-        try:
-            vol_data = {}
-            client = self.session.client('ec2', region_name=region)
-            marker = ''
-            while True:
-                response = client.describe_volumes(
-                    MaxResults=500,
-                    NextToken=marker
-                )
-                for item in response['Volumes']:
-                    create_time = item['CreateTime']
-                    datetime_4_weeks_ago = dt.datetime.now() - dt.timedelta(weeks=4)
-                    timezone = pytz.timezone("UTC")
-                    datetime_4_weeks_ago = timezone.localize(datetime_4_weeks_ago)
-
-                    older = create_time <= datetime_4_weeks_ago
-                    if older:
-                        # vol_data[item['VolumeId']] = item['Attachments']
-                        if len(item['Attachments']) == 0:
                             try:
-                                tags = item['Tags']
+                                tags = snapshot['Tags']
                             except KeyError:
                                 tags = None
+
+                            metadata = {
+                                'Region': region,
+                                # 'StorageTier': snapshot['StorageTier'],
+                                'Tags': tags,
+                                'CreateTime': snapshot['StartTime']
+                            }
+                            reason = {
+                                'This snapshot is 8 weeks older'
+                            }
                             temp = {
-                                'Service Name': 'EC2 (EBS)',
-                                'Id': item['VolumeId'],
-                                'Recommendation': 'Purge unattached volume',
-                                'Description': 'The Delete unattached volumes recommendation indicates that unattached volumes exists. Attaching or deleting unattached volumes reduces costs.',
-                                'Metadata': {
-                                    'Region': region,
-                                    'Instance Type': item['VolumeType'],
-                                    'Tags': tags,
-                                    'CreateTime': item['CreateTime']
-                                },
-                                'Recommendation Reason': {
-                                    'reason': 'This Volume is 4 weeks older and is not attached to any instance'
-                                },
-                                'Risk': 'Medium',
+                                'Service Name': service_name,
+                                'Id': r_id,
+                                'Recommendation': recom,
+                                'Description': desc,
+                                'Metadata': metadata,
+                                'Recommendation Reason': reason,
+                                'Risk': 'Low',
                                 'Savings': None,
                                 'Source': 'Klera',
                                 'Category': 'Cost Optimization'
                             }
                             recommendation.append(temp)
-                try:
-                    marker = response['NextToken']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
-
-        except botocore.exceptions.ClientError as e:
-            if e.response['Error']['Code'] == 'UnauthorizedOperation':
-                logger.info('---------Ec2 read access denied----------')
-                temp = {
-                    'Service Name': 'EC2 (EBS)',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'Medium',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.info("Something wrong with the region {}: {}".format(region, e))
-
-    return recommendation
-
-
-# Generates the recommendation to purge the snapshots which are older than 8 weeks
-def purge_8_weeks_older_snapshots(self) -> list:
-    logger.info(" ---Inside purge_8_weeks_older_snapshots()")
-
-    recommendation = []
-    regions = self.regions
-
-    datetime_8_weeks_ago = dt.datetime.now() - dt.timedelta(weeks=8)
-    timezone = pytz.timezone("UTC")
-    datetime_8_weeks_ago = timezone.localize(datetime_8_weeks_ago)
-
-    for region in regions:
-        try:
-            client = self.session.client('ec2', region_name=region)
-            marker = ''
-            while True:
-                response = client.describe_snapshots(
-                    MaxResults=1000,
-                    OwnerIds=['self'],
-                    NextToken=marker
-                )
-                for snapshot in response['Snapshots']:
-                    start_time = snapshot['StartTime']
-                    older = start_time <= datetime_8_weeks_ago
-
-                    if older:
-                        service_name = 'EC2 (EBS)'
-                        r_id =  snapshot['SnapshotId']
-                        recom = 'Purge 8 week older snapshot'
-                        desc = 'The Delete 8 weeks older snapshot recommendation indicates that snapshots is older than 8 weeks exists. Deleting older snapshots reduces costs.'
 
+                    try:
+                        marker = response['NextToken']
+                        if marker == '':
+                            break
+                    except KeyError:
+                        break
+            except botocore.exceptions.ClientError as e:
+                if e.response['Error']['Code'] == 'UnauthorizedOperation':
+                    logger.info('---------Ec2 read access denied----------')
+                    temp = {
+                        'Service Name': 'EC2 (EBS)',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Access Denied'
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'Low',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+                    return recommendation
+                logger.info("Something wrong with the region {}: {}".format(region, e))
+        return recommendation
+
+
+    # Generates the recommendations fot amazon ec2 reserved instance lease expiration
+    def reserved_instance_lease_expiration(self, regions) -> list:
+        """
+        :param regions:
+        :param self:
+        :return list: list of recommendations for reserved instances for lease expiration
+        """
+        logger.info(' ---Inside ec2 :: reserved_instance_lease_expiration()')
+
+        recommendation = []
+
+        datetime_now = dt.datetime.utcnow()
+        timezone = pytz.timezone("UTC")
+        datetime_30_days_ago = timezone.localize(datetime_now - dt.timedelta(days=30))
+
+        datetime_30_days_after = timezone.localize(datetime_now + dt.timedelta(days=30))
+
+        for region in regions:
+            try:
+                client = self.session.client('ec2', region_name=region)
+                response = client.describe_reserved_instances()
+
+                for instance in response['ReservedInstances']:
+                    expiry_date = instance['End']
+                    if datetime_30_days_ago <= expiry_date <= datetime_30_days_after:
                         try:
-                            tags = snapshot['Tags']
+                            tags = instance['Tags']
                         except KeyError:
                             tags = None
-
-                        metadata = {
-                            'Region': region,
-                            # 'StorageTier': snapshot['StorageTier'],
-                            'Tags': tags,
-                            'CreateTime': snapshot['StartTime']
-                        }
-                        reason = {
-                            'This snapshot is 8 weeks older'
-                        }
                         temp = {
-                            'Service Name': service_name,
-                            'Id': r_id,
-                            'Recommendation': recom,
-                            'Description': desc,
-                            'Metadata': metadata,
-                            'Recommendation Reason': reason,
-                            'Risk': 'Low',
+                            'Service Name': 'EC2 (Instance)',
+                            'Id': instance['ReservedInstancesId'],
+                            'Recommendation': 'Consider purchasing a new reserved instance',
+                            'Description': 'Checks for Amazon EC2 Reserved Instances that are scheduled to expire within the next 30 days, or have expired in the preceding 30 days.',
+                            'Metadata': {
+                                'Region': region,
+                                'Zone': instance['AvailabilityZone'],
+                                'Status': instance['State'],
+                                'Instance Type': instance['InstanceType'],
+                                'Tags': tags,
+                                'Expiration Date': expiry_date
+                            },
+                            'Recommendation Reason': {
+                                'Reason': 'The Instance is either expired within 30 days or will be expiring in next 30 days'
+                            },
+                            'Risk': 'High',
                             'Savings': None,
                             'Source': 'Klera',
                             'Category': 'Cost Optimization'
                         }
                         recommendation.append(temp)
 
-                try:
-                    marker = response['NextToken']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
-        except botocore.exceptions.ClientError as e:
-            if e.response['Error']['Code'] == 'UnauthorizedOperation':
-                logger.info('---------Ec2 read access denied----------')
-                temp = {
-                    'Service Name': 'EC2 (EBS)',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'Low',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.info("Something wrong with the region {}: {}".format(region, e))
-    return recommendation
-
-
-# Generates the recommendations fot amazon ec2 reserved instance lease expiration
-def reserved_instance_lease_expiration(self) -> list:
-    """
-    :param self:
-    :return list: list of recommendations for reserved instances for lease expiration
-    """
-    logger.info(' ---Inside ec2 :: reserved_instance_lease_expiration()')
-
-    recommendation = []
-    regions = self.regions
-
-    datetime_now = dt.datetime.utcnow()
-    timezone = pytz.timezone("UTC")
-    datetime_30_days_ago = timezone.localize(datetime_now - dt.timedelta(days=30))
-
-    datetime_30_days_after = timezone.localize(datetime_now + dt.timedelta(days=30))
-
-    for region in regions:
-        try:
-            client = self.session.client('ec2', region_name=region)
-            response = client.describe_reserved_instances()
-
-            for instance in response['ReservedInstances']:
-                expiry_date = instance['End']
-                if datetime_30_days_ago <= expiry_date <= datetime_30_days_after:
-                    try:
-                        tags = instance['Tags']
-                    except KeyError:
-                        tags = None
+            except botocore.exceptions.ClientError as e:
+                if e.response['Error']['Code'] == 'UnauthorizedOperation':
+                    logger.info('---------Ec2 read access denied----------')
                     temp = {
                         'Service Name': 'EC2 (Instance)',
-                        'Id': instance['ReservedInstancesId'],
-                        'Recommendation': 'Consider purchasing a new reserved instance',
-                        'Description': 'Checks for Amazon EC2 Reserved Instances that are scheduled to expire within the next 30 days, or have expired in the preceding 30 days.',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
                         'Metadata': {
-                            'Region': region,
-                            'Zone': instance['AvailabilityZone'],
-                            'Status': instance['State'],
-                            'Instance Type': instance['InstanceType'],
-                            'Tags': tags,
-                            'Expiration Date': expiry_date
+                            'Access Denied'
                         },
                         'Recommendation Reason': {
-                            'Reason': 'The Instance is either expired within 30 days or will be expiring in next 30 days'
+                            'Access Denied'
                         },
                         'Risk': 'High',
                         'Savings': None,
                         'Source': 'Klera',
                         'Category': 'Cost Optimization'
                     }
                     recommendation.append(temp)
+                    return recommendation
+                logger.error("Something went wrong with the region {}: {}".format(region, e))
 
-        except botocore.exceptions.ClientError as e:
-            if e.response['Error']['Code'] == 'UnauthorizedOperation':
-                logger.info('---------Ec2 read access denied----------')
-                temp = {
-                    'Service Name': 'EC2 (Instance)',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'High',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.error("Something went wrong with the region {}: {}".format(region, e))
-
-    return recommendation
+        return recommendation
 
 
-# Generated recommendations for unassociated elastic IP addresses
-def unassociated_elastic_ip_addresses(self) -> list:
-    """
-    :param self:
-    :return list: list of recommendations for unassociated elastic ip addresses
-    """
-    logger.info(" ---Inside ec2 :: unassociated_elastic_ip_addresses()")
+    # Generated recommendations for unassociated elastic IP addresses
+    def unassociated_elastic_ip_addresses(self, regions) -> list:
+        """
+        :param regions:
+        :param self:
+        :return list: list of recommendations for unassociated elastic ip addresses
+        """
+        logger.info(" ---Inside ec2 :: unassociated_elastic_ip_addresses()")
 
-    recommendation = []
-    regions = self.regions
+        recommendation = []
 
-    for region in regions:
-        try:
-            client = self.session.client('ec2', region_name=region)
-            response = client.describe_addresses()
+        for region in regions:
+            try:
+                client = self.session.client('ec2', region_name=region)
+                response = client.describe_addresses()
 
-            for eip in response['Addresses']:
-                try:
-                    association = eip['AssociationId']
-                except KeyError:
+                for eip in response['Addresses']:
                     try:
-                        tags = eip['Tags']
+                        association = eip['AssociationId']
                     except KeyError:
-                        tags = None
+                        try:
+                            tags = eip['Tags']
+                        except KeyError:
+                            tags = None
+                        temp = {
+                            'Service Name': 'EC2 (EIP)',
+                            'Id': eip['AllocationId'],
+                            'Recommendation': 'Associate the EIP with a running active instance, or release the unassociated EIP',
+                            'Description': 'Checks for Elastic IP addresses (EIPs) that are not associated with a running Amazon Elastic Compute Cloud (Amazon EC2) instance.',
+                            'Metadata': {
+                                'Region': region,
+                                'IP address': eip['PublicIp'],
+                                'Tags': tags
+                            },
+                            'Recommendation Reason': {
+                                'Reason': 'An allocated Elastic IP address (EIP) is not associated with a running Amazon EC2 instance'
+                            },
+                            'Risk': 'Low',
+                            'Savings': '$3.65',
+                            'Source': 'Klera',
+                            'Category': 'Cost Optimization'
+                        }
+                        recommendation.append(temp)
+
+            except botocore.exceptions.ClientError as e:
+                if e.response['Error']['Code'] == 'UnauthorizedOperation':
+                    logger.info('---------Ec2 read access denied----------')
                     temp = {
                         'Service Name': 'EC2 (EIP)',
-                        'Id': eip['AllocationId'],
-                        'Recommendation': 'Associate the EIP with a running active instance, or release the unassociated EIP',
-                        'Description': 'Checks for Elastic IP addresses (EIPs) that are not associated with a running Amazon Elastic Compute Cloud (Amazon EC2) instance.',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
                         'Metadata': {
-                            'Region': region,
-                            'IP address': eip['PublicIp'],
-                            'Tags': tags
+                            'Access Denied'
                         },
                         'Recommendation Reason': {
-                            'Reason': 'An allocated Elastic IP address (EIP) is not associated with a running Amazon EC2 instance'
+                            'Access Denied'
                         },
                         'Risk': 'Low',
-                        'Savings': '$3.65',
+                        'Savings': None,
                         'Source': 'Klera',
                         'Category': 'Cost Optimization'
                     }
                     recommendation.append(temp)
+                    return recommendation
+                logger.error("Something went wrong with the region {}: {}".format(region, e))
 
-        except botocore.exceptions.ClientError as e:
-            if e.response['Error']['Code'] == 'UnauthorizedOperation':
-                logger.info('---------Ec2 read access denied----------')
-                temp = {
-                    'Service Name': 'EC2 (EIP)',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'Low',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.error("Something went wrong with the region {}: {}".format(region, e))
-
-    return recommendation
+        return recommendation
 
 
-# Generates the recommendations for unused AMI
-def unused_ami(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(' ---Inside ec2 :: unused_ami()')
+    # Generates the recommendations for unused AMI
+    def unused_ami(self, regions) -> list:
+        """
+        :param regions:
+        :param self:
+        :return:
+        """
+        logger.info(' ---Inside ec2 :: unused_ami()')
 
-    recommendation = []
-    regions = self.regions
+        recommendation = []
 
-    for region in regions:
-        try:
-            client = self.session.client('ec2', region_name=region)
+        for region in regions:
+            try:
+                client = self.session.client('ec2', region_name=region)
 
-            marker = ''
-            while True:
-                if marker == '':
-                    response_ami = client.describe_images(
-                        Owners=['self']
-                    )
-                else:
-                    response_ami = client.describe_images(
-                        Owners=['self'],
-                        NextToken=marker
-                    )
+                marker = ''
+                while True:
+                    if marker == '':
+                        response_ami = client.describe_images(
+                            Owners=['self']
+                        )
+                    else:
+                        response_ami = client.describe_images(
+                            Owners=['self'],
+                            NextToken=marker
+                        )
+
+                    for image in response_ami['Images']:
+                        response_ec2 = client.describe_instances(
+                            Filters=[
+                                {
+                                    'Name': 'image-id',
+                                    'Values': [image['ImageId']]
+                                }
+                            ]
+                        )
+                        if len(response_ec2['Reservations']) == 0:
+                            try:
+                                tags = image['Tags']
+                            except KeyError:
+                                tags = None
 
-                for image in response_ami['Images']:
-                    response_ec2 = client.describe_instances(
-                        Filters=[
-                            {
-                                'Name': 'image-id',
-                                'Values': [image['ImageId']]
+                            temp = {
+                                'Service Name': 'EC2 (AMI)',
+                                'Id': image['ImageId'],
+                                'Recommendation': 'Remove AMI',
+                                'Description': 'Find any unused Amazon Machine Images available in your AWS account and remove them in order to lower the cost of your monthly AWS bill',
+                                'Metadata': {
+                                    'Region': region,
+                                    'Public': image['Public'],
+                                    'ImageType': image['ImageType'],
+                                    'Tags': tags,
+                                },
+                                'Recommendation Reason': {
+                                    'Reason': 'AMI is not used anymore and can be safely removed'
+                                },
+                                'Risk': 'Low',
+                                'Savings': None,
+                                'Source': 'Klera',
+                                'Category': 'Cost Optimization'
                             }
-                        ]
-                    )
-                    if len(response_ec2['Reservations']) == 0:
-                        try:
-                            tags = image['Tags']
-                        except KeyError:
-                            tags = None
-                            
-                        temp = {
-                            'Service Name': 'EC2 (AMI)',
-                            'Id': image['ImageId'],
-                            'Recommendation': 'Remove AMI',
-                            'Description': 'Find any unused Amazon Machine Images available in your AWS account and remove them in order to lower the cost of your monthly AWS bill',
-                            'Metadata': {
-                                'Region': region,
-                                'Public': image['Public'],
-                                'ImageType': image['ImageType'],
-                                'Tags': tags,
-                            },
-                            'Recommendation Reason': {
-                                'Reason': 'AMI is not used anymore and can be safely removed'
-                            },
-                            'Risk': 'Low',
-                            'Savings': None,
-                            'Source': 'Klera',
-                            'Category': 'Cost Optimization'
-                        }
-                try:
-                    marker = response_ami['NextToken']
-                    if marker == '':
+                    try:
+                        marker = response_ami['NextToken']
+                        if marker == '':
+                            break
+                    except KeyError:
                         break
-                except KeyError:
-                    break
 
-        except ClientError as e:
-            if e.response['Error']['Code'] == 'UnauthorizedOperation':
-                logger.info('---------EC2 read access denied----------')
-                temp = {
-                    'Service Name': 'EC2 (AMI)',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'Low',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.warning("Something went wrong with the region {}: {}".format(region, e))
+            except ClientError as e:
+                if e.response['Error']['Code'] == 'UnauthorizedOperation':
+                    logger.info('---------EC2 read access denied----------')
+                    temp = {
+                        'Service Name': 'EC2 (AMI)',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Access Denied'
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'Low',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+                    return recommendation
+                logger.warning("Something went wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/elb.py` & `aws_recommendation-0.2.3/aws_recommendation/elb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,192 +1,204 @@
 from botocore.exceptions import ClientError
 
 from aws_recommendation.utils import *
 
 
-# Generate the recommendation for idle elastic load balancer
-def idle_elastic_load_balancer(self):
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside elb :: idle_elastic_load_balancer()")
-
-    recommendation = []
-    regions = self.regions
-
-    for region in regions:
-        try:
-            client = self.session.client('elbv2', region_name=region)
-            marker = ''
-            while True:
-                if marker == '':
-                    response = client.describe_load_balancers()
-                else:
-                    response = client.describe_load_balancers(
-                        Marker=marker
-                    )
-                for lb in response['LoadBalancers']:
-                    datapoints = get_metrics_stats(
-                        self,
-                        region=region,
-                        namespace='AWS/EC2',
-                        dimensions=[
-                            {
-                                'Name': 'LoadBalancerName',
-                                'Value': lb['LoadBalancerName']
-                            }
-                        ],
-                        metric_name='RequestCount',
-                        stats=['Sum'],
-                        unit=None
-                    )
-                    sum_request_count = 0
-                    for datapoint in datapoints['Datapoints']:
-                        sum_request_count = sum_request_count + datapoint['Sum']
-
-                    recommend_flag = True
-                    if sum_request_count >= 100:
-                        recommend_flag = False
-
-                    if recommend_flag:
-                        tags_response = client.describe_tags(
-                            ResourceArns=[
-                                lb['LoadBalancerArn']
-                            ]
+class elb:
+    def get_elb_recommendations(self, regions=None):
+        """
+        :param regions:
+        :return:
+        """
+        logger.info(" ---Inside elb :: get_elb_recommendations()--- ")
+
+        if regions is None:
+            regions = self.get_regions()
+
+        return self.idle_elastic_load_balancer(regions) + self.unused_elb(regions)
+
+    # Generate the recommendation for idle elastic load balancer
+    def idle_elastic_load_balancer(self, regions):
+        """
+        :param regions:
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside elb :: idle_elastic_load_balancer()")
+
+        recommendation = []
+
+        for region in regions:
+            try:
+                client = self.session.client('elbv2', region_name=region)
+                marker = ''
+                while True:
+                    if marker == '':
+                        response = client.describe_load_balancers()
+                    else:
+                        response = client.describe_load_balancers(
+                            Marker=marker
                         )
-                        try:
-                            for tag in tags_response['TagDescriptions'][0]['Tags']:
-                                if 'Role' in tag['Key']:
-                                    recommend_flag = False
-                        except TypeError:
-                            pass
+                    for lb in response['LoadBalancers']:
+                        datapoints = self.get_metrics_stats(
+                            region=region,
+                            namespace='AWS/EC2',
+                            dimensions=[
+                                {
+                                    'Name': 'LoadBalancerName',
+                                    'Value': lb['LoadBalancerName']
+                                }
+                            ],
+                            metric_name='RequestCount',
+                            stats=['Sum'],
+                            unit=None
+                        )
+                        sum_request_count = 0
+                        for datapoint in datapoints['Datapoints']:
+                            sum_request_count = sum_request_count + datapoint['Sum']
+
+                        recommend_flag = True
+                        if sum_request_count >= 100:
+                            recommend_flag = False
+
                         if recommend_flag:
+                            tags_response = client.describe_tags(
+                                ResourceArns=[
+                                    lb['LoadBalancerArn']
+                                ]
+                            )
+                            try:
+                                for tag in tags_response['TagDescriptions'][0]['Tags']:
+                                    if 'Role' in tag['Key']:
+                                        recommend_flag = False
+                            except TypeError:
+                                pass
+                            if recommend_flag:
+                                temp = {
+                                    'Service Name': 'EC2 (ELB)',
+                                    'Id': lb['LoadBalancerName'],
+                                    'Recommendation': 'Terminate Elastic Load Balancer',
+                                    'Description': 'The selected Elastic Load Balancer can be safely removed from the AWS account to reduce the ELB monthly costs.',
+                                    'Metadata': {
+                                        'Region': region,
+                                        'Type': lb['Type'],
+                                        'Tags': tags_response['TagDescriptions'][0]['Tags'],
+                                    },
+                                    'Recommendation Reason': {
+                                        'reason': "Load balancer is idle"
+                                    },
+                                    'Risk': 'High',
+                                    'Savings': None,
+                                    'Source': 'Klera',
+                                    'Category': 'Cost Optimization'
+                                }
+                                recommendation.append(temp)
+
+                    try:
+                        marker = response['NextMarker']
+                        if marker == '':
+                            break
+                    except KeyError:
+                        break
+
+            except ClientError as e:
+                if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
+                    logger.info('---------ELB read access denied----------')
+                    temp = {
+                        'Service Name': 'EC2 (ELB)',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Access Denied'
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'High',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+                    return recommendation
+                logger.error("Something went wrong with the region {}: {}".format(region, e))
+
+        return recommendation
+
+
+    # Generates the recommendation for unused elastic load balancer
+    def unused_elb(self, regions) -> list:
+        """
+        :param regions:
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside elb :: unused_elb()")
+
+        recommendation = []
+
+        for region in regions:
+            try:
+                client = self.session.client('elb', region_name=region)
+                marker = ''
+                while True:
+                    if marker == '':
+                        response = client.describe_load_balancers()
+                    else:
+                        response = client.describe_load_balancers(
+                            Marker=marker
+                        )
+                    for lb in response['LoadBalancerDescriptions']:
+                        try:
+                            instances = response['Instances']
+                        except KeyError:
                             temp = {
                                 'Service Name': 'EC2 (ELB)',
                                 'Id': lb['LoadBalancerName'],
-                                'Recommendation': 'Terminate Elastic Load Balancer',
-                                'Description': 'The selected Elastic Load Balancer can be safely removed from the AWS account to reduce the ELB monthly costs.',
+                                'Recommendation': 'Remove Unused ELB',
+                                'Description': 'Identify unused Elastic Load Balancers, and delete them to help lower the cost of your monthly AWS bill.',
                                 'Metadata': {
                                     'Region': region,
-                                    'Type': lb['Type'],
-                                    'Tags': tags_response['TagDescriptions'][0]['Tags'],
+                                    # 'Type': lb['Type'],
                                 },
                                 'Recommendation Reason': {
-                                    'reason': "Load balancer is idle"
+                                    'reason': 'The load balancer has 0 instances behind it'
                                 },
                                 'Risk': 'High',
                                 'Savings': None,
                                 'Source': 'Klera',
                                 'Category': 'Cost Optimization'
                             }
                             recommendation.append(temp)
 
-                try:
-                    marker = response['NextMarker']
-                    if marker == '':
-                        break
-                except KeyError:
-                    break
-
-        except ClientError as e:
-            if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
-                logger.info('---------ELB read access denied----------')
-                temp = {
-                    'Service Name': 'EC2 (ELB)',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'High',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.error("Something went wrong with the region {}: {}".format(region, e))
-
-    return recommendation
-
-
-# Generates the recommendation for unused elastic load balancer
-def unused_elb(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside elb :: unused_elb()")
-
-    recommendation = []
-    regions = self.regions
-
-    for region in regions:
-        try:
-            client = self.session.client('elb', region_name=region)
-            marker = ''
-            while True:
-                if marker == '':
-                    response = client.describe_load_balancers()
-                else:
-                    response = client.describe_load_balancers(
-                        Marker=marker
-                    )
-                for lb in response['LoadBalancerDescriptions']:
                     try:
-                        instances = response['Instances']
+                        marker = response['NextMarker']
+                        if marker == '':
+                            break
                     except KeyError:
-                        temp = {
-                            'Service Name': 'EC2 (ELB)',
-                            'Id': lb['LoadBalancerName'],
-                            'Recommendation': 'Remove Unused ELB',
-                            'Description': 'Identify unused Elastic Load Balancers, and delete them to help lower the cost of your monthly AWS bill.',
-                            'Metadata': {
-                                'Region': region,
-                                # 'Type': lb['Type'],
-                            },
-                            'Recommendation Reason': {
-                                'reason': 'The load balancer has 0 instances behind it'
-                            },
-                            'Risk': 'High',
-                            'Savings': None,
-                            'Source': 'Klera',
-                            'Category': 'Cost Optimization'
-                        }
-                        recommendation.append(temp)
-
-                try:
-                    marker = response['NextMarker']
-                    if marker == '':
                         break
-                except KeyError:
-                    break
 
-        except ClientError as e:
-            if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
-                logger.info('---------ELB read access denied----------')
-                temp = {
-                    'Service Name': 'EC2 (ELB)',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'High',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.warning("Something went wrong with the region {}: {}".format(region, e))
+            except ClientError as e:
+                if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
+                    logger.info('---------ELB read access denied----------')
+                    temp = {
+                        'Service Name': 'EC2 (ELB)',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Access Denied'
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'High',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+                    return recommendation
+                logger.warning("Something went wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/kms.py` & `aws_recommendation-0.2.3/aws_recommendation/kms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,98 @@
 from botocore.exceptions import ClientError
 
 from aws_recommendation.utils import *
 
+class kms:
+    def get_kms_recommendations(self, regions=None):
+        """
+        :param regions:
+        :return:
+        """
+        logger.info(" ---Inside kms :: get_kms_recommendations()--- ")
+
+        if regions is None:
+            regions = self.get_regions()
+
+        return self.unused_cmk(regions)
+
+    # generate the recommendations for unused cmk
+    def unused_cmk(self, regions: list) -> list:
+        """
+        :param regions:
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside kms :: unused_cmk()")
+
+        recommendation = []
+
+        for region in regions:
+            try:
+                client = self.session.client('kms', region_name=region)
 
-# generate the recommendations for unused cmk
-def unused_cmk(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside kms :: unused_cmk()")
-
-    recommendation = []
-
-    regions = self.regions
-
-    for region in regions:
-        try:
-            client = self.session.client('kms', region_name=region)
-
-            marker = ''
-            while True:
-                if marker == '':
-                    response = client.list_keys(
-                        Limit=1000
-                    )
-                else:
-                    response = client.list_keys(
-                        Limit=1000,
-                        Marker=marker
-                    )
-                for key in response['Keys']:
-                    key_desc = client.describe_key(
-                        KeyId=key['KeyId']
-                    )
-                    if not key_desc['KeyMetadata']['Enabled']:
-                        temp = {
-                            'Service Name': 'Key Management Service',
-                            'Id': key['KeyId'],
-                            'Recommendation': 'Remove Customer Master Key',
-                            'Description': 'Check for any disabled KMS Customer Master Keys in your AWS account and remove them in order to lower the cost of your monthly AWS bill',
-                            'Metadata': {
-                                'Region': region,
-                                'CreationDate': key_desc['KeyMetadata']['CreationDate'],
-                                'Enabled': key_desc['KeyMetadata']['Enabled'],
-                                'MultiRegion': key_desc['KeyMetadata']['MultiRegion']
-                            },
-                            'Recommendation Reason': {
-                                'reason': "Customer Master key is not in enabled state"
-                            },
-                            'Risk': 'Low',
-                            'Savings': None,
-                            'Source': 'Klera',
-                            'Category': 'Cost Optimization'
-                        }
-                        recommendation.append(temp)
-                try:
-                    marker = response['NextMarker']
+                marker = ''
+                while True:
                     if marker == '':
+                        response = client.list_keys(
+                            Limit=1000
+                        )
+                    else:
+                        response = client.list_keys(
+                            Limit=1000,
+                            Marker=marker
+                        )
+                    for key in response['Keys']:
+                        key_desc = client.describe_key(
+                            KeyId=key['KeyId']
+                        )
+                        if not key_desc['KeyMetadata']['Enabled']:
+                            temp = {
+                                'Service Name': 'Key Management Service',
+                                'Id': key['KeyId'],
+                                'Recommendation': 'Remove Customer Master Key',
+                                'Description': 'Check for any disabled KMS Customer Master Keys in your AWS account and remove them in order to lower the cost of your monthly AWS bill',
+                                'Metadata': {
+                                    'Region': region,
+                                    'CreationDate': key_desc['KeyMetadata']['CreationDate'],
+                                    'Enabled': key_desc['KeyMetadata']['Enabled'],
+                                    'MultiRegion': key_desc['KeyMetadata']['MultiRegion']
+                                },
+                                'Recommendation Reason': {
+                                    'reason': "Customer Master key is not in enabled state"
+                                },
+                                'Risk': 'Low',
+                                'Savings': None,
+                                'Source': 'Klera',
+                                'Category': 'Cost Optimization'
+                            }
+                            recommendation.append(temp)
+                    try:
+                        marker = response['NextMarker']
+                        if marker == '':
+                            break
+                    except KeyError:
                         break
-                except KeyError:
-                    break
-        except ClientError as e:
-            if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
-                logger.info('---------KMS read access denied----------')
-                temp = {
-                    'Service Name': 'Key Management Service',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'Low',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.warning("Something went wrong with the region {}: {}".format(region, e))
+            except ClientError as e:
+                if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
+                    logger.info('---------KMS read access denied----------')
+                    temp = {
+                        'Service Name': 'Key Management Service',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Access Denied'
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'Low',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+                    return recommendation
+                logger.warning("Something went wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/rds.py` & `aws_recommendation-0.2.3/aws_recommendation/rds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,82 @@
 import logging
 
 import botocore
 from botocore.exceptions import ClientError
 
+from aws_recommendation import utils
 from aws_recommendation.utils import *
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
-# Generates the recommendation to downsize underutilized rds instance
-def downsize_underutilized_rds_recommendation(self) -> list:
-    logger.info(" ---Inside downsize_underutilized_rds_recommendation()")
+class rds:
+    def get_rds_recommendations(self, regions):
+        """
+        :return:
+        """
+        logger.info(" ---Inside rds :: get_rds_recommendations()--- ")
+
+        rds_instances = self.list_rds_instances(regions)
+        response = []
+        # r_logger.debug(str(rds_instances))
+
+        response.extend(self.downsize_underutilized_rds_recommendation(rds_instances))
+        response.extend(self.rds_idle_db_instances(rds_instances))
+        response.extend(self.rds_general_purpose_ssd(rds_instances))
+
+        return response
+
+    # Generates the recommendation to downsize underutilized rds instance
+    def downsize_underutilized_rds_recommendation(self, rds_instances) -> list:
+        logger.info(" ---Inside downsize_underutilized_rds_recommendation()")
 
-    recommendation = []
-    regions = self.regions
+        recommendation = []
 
-    for region in regions:
         try:
-            rds_instance_lst = list_rds_instances(self, region)
-
-            for instance in rds_instance_lst:
-                cpu_stats = get_metrics_stats(
-                    self, region, namespace='AWS/RDS',
-                    dimensions=[{'Name': 'DBInstanceIdentifier', 'Value': instance['DBInstanceIdentifier']}]
-                )
-
-                if len(cpu_stats['Datapoints']) >= 7:
-                    flag = True
-                    for points in cpu_stats['Datapoints']:
-                        if points['Average'] > 30:
-                            flag = False
-                            break
-
-                    if flag:
-                        try:
-                            Tags = instance['TagList']
-                        except KeyError:
-                            Tags = None
-                        temp = {
-                            'Service Name': 'RDS',
-                            'Id': instance['DBInstanceIdentifier'],
-                            'Recommendation': 'Downsize underutilized rds instance',
-                            'Description': 'The Downsize underutilized rds databases recommendation indicates that more CPUs are allocated to autonomous databases than you need. Reducing the number of CPUs allocated to your databases saves you money.',
-                            'Metadata': {
-                                'Region': region,
-                                'DBInstanceClass': instance['DBInstanceClass'],
-                                'Engine': instance['Engine'],
-                                'Tags': Tags,
-                                'InstanceCreateTime': instance['InstanceCreateTime']
-                            },
-                            'Recommendation Reason': {
-                                'Average CPU Datapoints(7 days)': [float('{:.2f}'.format(item['Average'])) for item in cpu_stats['Datapoints']]
-                            },
-                            'Risk': 'High',
-                            'Savings': None,
-                            'Source': 'Klera',
-                            'Category': 'Cost Optimization'
-                        }
-                        recommendation.append(temp)
+            for region, instances in rds_instances.items():
+                for instance in instances:
+                    cpu_stats = self.get_metrics_stats(
+                        region, namespace='AWS/RDS',
+                        dimensions=[{'Name': 'DBInstanceIdentifier', 'Value': instance['DBInstanceIdentifier']}]
+                    )
+
+                    if len(cpu_stats['Datapoints']) >= 7:
+                        flag = True
+                        for points in cpu_stats['Datapoints']:
+                            if points['Average'] > 30:
+                                flag = False
+                                break
+
+                        if flag:
+                            try:
+                                Tags = instance['TagList']
+                            except KeyError:
+                                Tags = None
+                            temp = {
+                                'Service Name': 'RDS',
+                                'Id': instance['DBInstanceIdentifier'],
+                                'Recommendation': 'Downsize underutilized rds instance',
+                                'Description': 'The Downsize underutilized rds databases recommendation indicates that more CPUs are allocated to autonomous databases than you need. Reducing the number of CPUs allocated to your databases saves you money.',
+                                'Metadata': {
+                                    'Region': region,
+                                    'DBInstanceClass': instance['DBInstanceClass'],
+                                    'Engine': instance['Engine'],
+                                    'Tags': Tags,
+                                    'InstanceCreateTime': instance['InstanceCreateTime']
+                                },
+                                'Recommendation Reason': {
+                                    'Average CPU Datapoints(7 days)': [float('{:.2f}'.format(item['Average'])) for item in cpu_stats['Datapoints']]
+                                },
+                                'Risk': 'High',
+                                'Savings': None,
+                                'Source': 'Klera',
+                                'Category': 'Cost Optimization'
+                            }
+                            recommendation.append(temp)
 
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
                 logger.info('---------RDS read access denied----------')
                 temp = {
                     'Service Name': 'RDS',
                     'Id': 'Access Denied',
@@ -78,70 +93,68 @@
                     'Source': 'Klera',
                     'Category': 'Cost Optimization'
                 }
                 recommendation.append(temp)
                 return recommendation
             logger.info("Something wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
 
 
-# Generates the recommendation Amazon RDS Idle DB Instances
-def rds_idle_db_instances(self) -> list:
-    """
+    # Generates the recommendation Amazon RDS Idle DB Instances
+    def rds_idle_db_instances(self, rds_instances) -> list:
+        """
 
-    :param self:
-    :return list: recommendation list for rds idle db instances
-    """
-    logger.info(' ---Inside rds :: rds_idle_db_instances()')
+        :param self:
+        :return list: recommendation list for rds idle db instances
+        """
+        logger.info(' ---Inside rds :: rds_idle_db_instances()')
 
-    recommendation = []
-    regions = self.regions
+        recommendation = []
 
-    for region in regions:
         try:
-            rds_instance_lst = list_rds_instances(self, region)
-            for instance in rds_instance_lst:
-                datapoints = get_metrics_stats(
-                    self, region, namespace='AWS/RDS',
-                    dimensions=[{'Name': 'DBInstanceIdentifier', 'Value': instance['DBInstanceIdentifier']}], metric_name='DatabaseConnections', stats=['Maximum'], unit='Count'
-                )
-                flag = True
-                for points in datapoints['Datapoints']:
-                    if points['Maximum'] > 0:
-                        flag = False
-                        break
-
-                if flag:
-                    try:
-                        Tags = instance['TagList']
-                    except KeyError:
-                        Tags = None
-                    temp = {
-                        'Service Name': 'RDS',
-                        'Id': instance['DBInstanceIdentifier'],
-                        'Recommendation': 'Delete idle rds instance',
-                        'Description': 'Consider taking a snapshot of the idle DB instance and then either stopping it or deleting it. Stopping the DB instance removes some of the costs for it, but does not remove storage costs. A stopped instance keeps all automated backups based upon the configured retention period. Stopping a DB instance usually incurs additional costs when compared to deleting the instance and then retaining only the final snapshot',
-                        'Metadata': {
-                            'Region': region,
-                            'DBInstanceClass': instance['DBInstanceClass'],
-                            'MultiAZ': instance['MultiAZ'],
-                            'Engine': instance['Engine'],
-                            'Tags': Tags,
-                            'InstanceCreateTime': instance['InstanceCreateTime']
-                        },
-                        'Recommendation Reason': {
-                            'Reason': 'An active DB instance has not had a connection in the last 7 days.'
-                        },
-                        'Risk': 'High',
-                        'Savings': None,
-                        'Source': 'Klera',
-                        'Category': 'Cost Optimization'
-                    }
-                    recommendation.append(temp)
+            for region, instances in rds_instances.items():
+                for instance in instances:
+                    datapoints = self.get_metrics_stats(
+                        region, namespace='AWS/RDS',
+                        dimensions=[{'Name': 'DBInstanceIdentifier', 'Value': instance['DBInstanceIdentifier']}], metric_name='DatabaseConnections', stats=['Maximum'], unit='Count'
+                    )
+                    flag = True
+                    for points in datapoints['Datapoints']:
+                        if points['Maximum'] > 0:
+                            flag = False
+                            break
+
+                    if flag:
+                        try:
+                            Tags = instance['TagList']
+                        except KeyError:
+                            Tags = None
+                        temp = {
+                            'Service Name': 'RDS',
+                            'Id': instance['DBInstanceIdentifier'],
+                            'Recommendation': 'Delete idle rds instance',
+                            'Description': 'Consider taking a snapshot of the idle DB instance and then either stopping it or deleting it. Stopping the DB instance removes some of the costs for it, but does not remove storage costs. A stopped instance keeps all automated backups based upon the configured retention period. Stopping a DB instance usually incurs additional costs when compared to deleting the instance and then retaining only the final snapshot',
+                            'Metadata': {
+                                'Region': region,
+                                'DBInstanceClass': instance['DBInstanceClass'],
+                                'MultiAZ': instance['MultiAZ'],
+                                'Engine': instance['Engine'],
+                                'Tags': Tags,
+                                'InstanceCreateTime': instance['InstanceCreateTime']
+                            },
+                            'Recommendation Reason': {
+                                'Reason': 'An active DB instance has not had a connection in the last 7 days.'
+                            },
+                            'Risk': 'High',
+                            'Savings': None,
+                            'Source': 'Klera',
+                            'Category': 'Cost Optimization'
+                        }
+                        recommendation.append(temp)
 
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
                 logger.info('---------RDS read access denied----------')
                 temp = {
                     'Service Name': 'RDS',
                     'Id': 'Access Denied',
@@ -158,59 +171,58 @@
                     'Source': 'Klera',
                     'Category': 'Cost Optimization'
                 }
                 recommendation.append(temp)
                 return recommendation
             logger.info("Something wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
 
 
-#Generated the recommendation for rds general purpose ssd
-def rds_general_purpose_ssd(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(' ---Inside rds :: rds_general_purpose_ssd()')
+    #Generated the recommendation for rds general purpose ssd
+    def rds_general_purpose_ssd(self, rds_instances) -> list:
+        """
+        :param rds_instances:
+        :param self:
+        :return:
+        """
+        logger.info(' ---Inside rds :: rds_general_purpose_ssd()')
 
-    recommendation = []
-    regions = self.regions
+        recommendation = []
 
-    for region in regions:
         try:
-            rds_instance_lst = list_rds_instances(self, region)
-            for instance in rds_instance_lst:
-                storage = instance['StorageType']
-                if storage == 'io1':
-                    try:
-                        Tags = instance['TagList']
-                    except KeyError:
-                        Tags = None
-                    temp = {
-                        'Service Name': 'RDS',
-                        'Id': instance['DBInstanceIdentifier'],
-                        'Recommendation': 'Upgrade to General Purpose SSD',
-                        'Description': 'Using General Purpose (GP) SSD database storage instead of Provisioned IOPS (PIOPS) SSD storage represents a good strategy to cut down on AWS RDS costs because for GP SSDs you only pay for the storage compared to PIOPS SSDs where you pay for both storage and IOPS',
-                        'Metadata': {
-                            'Region': region,
-                            'DBInstanceClass': instance['DBInstanceClass'],
-                            'Engine': instance['Engine'],
-                            'Tags': Tags,
-                            'InstanceCreateTime': instance['InstanceCreateTime']
-                        },
-                        'Recommendation Reason': {
-                            'Reason': 'the storage type used is Provisioned IOPS SSD'
-                        },
-                        'Risk': 'Medium',
-                        'Savings': None,
-                        'Source': 'Klera',
-                        'Category': 'Cost Optimization'
-                    }
-                    recommendation.append(temp)
+            for region, instances in rds_instances.items():
+                for instance in instances:
+                    storage = instance['StorageType']
+                    if storage == 'io1':
+                        try:
+                            Tags = instance['TagList']
+                        except KeyError:
+                            Tags = None
+                        temp = {
+                            'Service Name': 'RDS',
+                            'Id': instance['DBInstanceIdentifier'],
+                            'Recommendation': 'Upgrade to General Purpose SSD',
+                            'Description': 'Using General Purpose (GP) SSD database storage instead of Provisioned IOPS (PIOPS) SSD storage represents a good strategy to cut down on AWS RDS costs because for GP SSDs you only pay for the storage compared to PIOPS SSDs where you pay for both storage and IOPS',
+                            'Metadata': {
+                                'Region': region,
+                                'DBInstanceClass': instance['DBInstanceClass'],
+                                'Engine': instance['Engine'],
+                                'Tags': Tags,
+                                'InstanceCreateTime': instance['InstanceCreateTime']
+                            },
+                            'Recommendation Reason': {
+                                'Reason': 'the storage type used is Provisioned IOPS SSD'
+                            },
+                            'Risk': 'Medium',
+                            'Savings': None,
+                            'Source': 'Klera',
+                            'Category': 'Cost Optimization'
+                        }
+                        recommendation.append(temp)
         except ClientError as e:
             if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
                 logger.info('---------RDS read access denied----------')
                 temp = {
                     'Service Name': 'RDS',
                     'Id': 'Access Denied',
                     'Recommendation': 'Access Denied',
@@ -226,8 +238,8 @@
                     'Source': 'Klera',
                     'Category': 'Cost Optimization'
                 }
                 recommendation.append(temp)
                 return recommendation
             logger.info("Something went wrong with the region {}: {}".format(region, e))
 
-    return recommendation
+        return recommendation
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/redshift.py` & `aws_recommendation-0.2.3/aws_recommendation/redshift.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,125 +3,134 @@
 from botocore.exceptions import ClientError
 
 from aws_recommendation.utils import *
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
+class redshift:
+    def get_redshift_recommendations(self, regions=None):
+        """
+        :param regions:
+        :return:
+        """
+        logger.info(" ---Inside redshift :: get_redshift_recommendations()--- ")
+
+        if regions is None:
+            regions = self.get_regions()
+
+        return self.under_utilized_redshift_cluster(regions)
+
+    # Generated recommendation for under utilized redshift cluster
+    def under_utilized_redshift_cluster(self, regions) -> list:
+        """
+        :param regions:
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside redshift :: under_utilized_redshift_cluster()")
+
+        recommendation = []
+
+        for region in regions:
+            try:
+                client = self.session.client('redshift', region_name=region)
+                clusters = self.list_redshift_clusters(client)
 
-# Generated recommendation for under utilized redshift cluster
-def under_utilized_redshift_cluster(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside redshift :: under_utilized_redshift_cluster()")
-
-    recommendation = []
-    regions = self.regions
-
-    for region in regions:
-        try:
-            client = self.session.client('redshift', region_name=region)
-            clusters = list_redshift_clusters(client)
-
-            for cluster in clusters:
-                cpu_datapoints = get_metrics_stats(
-                    self=self,
-                    region=region,
-                    namespace='AWS/Redshift',
-                    dimensions=[{'Name': 'ClusterIdentifier', 'Value': cluster['ClusterIdentifier']}],
-                    metric_name='CPUUtilization',
-                    period=3600,
-                    stats=["Average"]
-                )
-                flag = True
-                for datapoint in cpu_datapoints['Datapoints']:
-                    if datapoint['Average'] > 60:
-                        flag = False
-                        break
-
-                if flag:
-                    read_datapoints = get_metrics_stats(
-                        self=self,
+                for cluster in clusters:
+                    cpu_datapoints = self.get_metrics_stats(
                         region=region,
                         namespace='AWS/Redshift',
                         dimensions=[{'Name': 'ClusterIdentifier', 'Value': cluster['ClusterIdentifier']}],
-                        metric_name='ReadIOPS',
+                        metric_name='CPUUtilization',
                         period=3600,
-                        stats=["Sum"]
+                        stats=["Average"]
                     )
-                    readOps_sum = 0
-                    for datapoint in read_datapoints['Datapoints']:
-                        readOps_sum = readOps_sum +  datapoint['Sum']
-
-                    if readOps_sum > 100:
-                        flag = False
-
-                if flag:
-                    write_datapoints = get_metrics_stats(
-                        self=self,
-                        region=region,
-                        namespace='AWS/Redshift',
-                        dimensions=[{'Name': 'ClusterIdentifier', 'Value': cluster['ClusterIdentifier']}],
-                        metric_name='WriteIOPS',
-                        period=3600,
-                        stats=["Sum"]
-                    )
-                    writeOps_sum = 0
-                    for datapoint in write_datapoints['Datapoints']:
-                        writeOps_sum = writeOps_sum + datapoint['Sum']
-
-                    if writeOps_sum > 100:
-                        flag = False
-
-                if flag:
-                    try:
-                        tags = cluster['Tags']
-                    except KeyError:
-                        tags = None
+                    flag = True
+                    for datapoint in cpu_datapoints['Datapoints']:
+                        if datapoint['Average'] > 60:
+                            flag = False
+                            break
+
+                    if flag:
+                        read_datapoints = self.get_metrics_stats(
+                            region=region,
+                            namespace='AWS/Redshift',
+                            dimensions=[{'Name': 'ClusterIdentifier', 'Value': cluster['ClusterIdentifier']}],
+                            metric_name='ReadIOPS',
+                            period=3600,
+                            stats=["Sum"]
+                        )
+                        readOps_sum = 0
+                        for datapoint in read_datapoints['Datapoints']:
+                            readOps_sum = readOps_sum +  datapoint['Sum']
+
+                        if readOps_sum > 100:
+                            flag = False
+
+                    if flag:
+                        write_datapoints = self.get_metrics_stats(
+                            region=region,
+                            namespace='AWS/Redshift',
+                            dimensions=[{'Name': 'ClusterIdentifier', 'Value': cluster['ClusterIdentifier']}],
+                            metric_name='WriteIOPS',
+                            period=3600,
+                            stats=["Sum"]
+                        )
+                        writeOps_sum = 0
+                        for datapoint in write_datapoints['Datapoints']:
+                            writeOps_sum = writeOps_sum + datapoint['Sum']
+
+                        if writeOps_sum > 100:
+                            flag = False
+
+                    if flag:
+                        try:
+                            tags = cluster['Tags']
+                        except KeyError:
+                            tags = None
+                        temp = {
+                            'Service Name': 'Redshift',
+                            'Id': cluster['ClusterIdentifier'],
+                            'Recommendation': 'Consider shutting down the cluster and taking a final snapshot, or downsizing the cluster',
+                            'Description': 'TChecks your Amazon Redshift configuration for clusters that appear to be underutilized',
+                            'Metadata': {
+                                'Region': region,
+                                'Node Type': cluster['NodeType'],
+                                'Tags': tags,
+                            },
+                            'Recommendation Reason': {
+                                'Average CPU Datapoints(7 days)': [float('{:.2f}'.format(x['Average'])) for x in cpu_datapoints['Datapoints']],
+                                'Total ReadOps': readOps_sum,
+                                'Total WriteOps': writeOps_sum
+                            },
+                            'Risk': 'High',
+                            'Savings': None,
+                            'Source': 'Klera',
+                            'Category': 'Cost Optimization'
+                        }
+                        recommendation.append(temp)
+
+            except ClientError as e:
+                if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
+                    logger.info('---------Redshift read access denied----------')
                     temp = {
                         'Service Name': 'Redshift',
-                        'Id': cluster['ClusterIdentifier'],
-                        'Recommendation': 'Consider shutting down the cluster and taking a final snapshot, or downsizing the cluster',
-                        'Description': 'TChecks your Amazon Redshift configuration for clusters that appear to be underutilized',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
                         'Metadata': {
-                            'Region': region,
-                            'Node Type': cluster['NodeType'],
-                            'Tags': tags,
+                            'Access Denied'
                         },
                         'Recommendation Reason': {
-                            'Average CPU Datapoints(7 days)': [float('{:.2f}'.format(x['Average'])) for x in cpu_datapoints['Datapoints']],
-                            'Total ReadOps': readOps_sum,
-                            'Total WriteOps': writeOps_sum
+                            'Access Denied'
                         },
                         'Risk': 'High',
                         'Savings': None,
                         'Source': 'Klera',
                         'Category': 'Cost Optimization'
                     }
                     recommendation.append(temp)
+                    return recommendation
+                logger.error("Something went wrong with the region {}: {}".format(region, e))
 
-        except ClientError as e:
-            if e.response['Error']['Code'] == 'AccessDenied' or e.response['Error']['Code'] == 'AccessDeniedException':
-                logger.info('---------Redshift read access denied----------')
-                temp = {
-                    'Service Name': 'Redshift',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Access Denied'
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'High',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            logger.error("Something went wrong with the region {}: {}".format(region, e))
-
-    return recommendation
+        return recommendation
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/s3.py` & `aws_recommendation-0.2.3/aws_recommendation/s3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,329 +1,270 @@
-from botocore.exceptions import ClientError
 import traceback
-from aws_recommendation.utils import *
 
+from botocore.exceptions import ClientError
+
+from aws_recommendation.utils import *
 
-# Generate the recommendation for enable s3 bucket keys
-def enable_s3_bucket_keys(self) -> list:
-    """
-    :param self:
-    :return:
-    """
-    logger.info(" ---Inside s3 :: enable_s3_bucket_keys()")
-
-    recommendation = []
-
-    client = self.session.client('s3')
-
-    try:
-        response = client.list_buckets()
-    except ClientError as e:
-        if e.response['Error']['Code'] == 'AccessDenied':
-            logger.info('---------S3 read access denied----------')
-            temp = {
-                'Service Name': 'S3',
-                'Id': 'Access Denied',
-                'Recommendation': 'Access Denied',
-                'Description': 'Access Denied',
-                'Metadata': {
-                    'Exception': str(traceback.format_exc())
-                },
-                'Recommendation Reason': {
-                    'Access Denied'
-                },
-                'Risk': 'Low',
-                'Savings': None,
-                'Source': 'Klera',
-                'Category': 'Cost Optimization'
-            }
-            recommendation.append(temp)
-        else:
-            temp = {
-                'Service Name': 'S3',
-                'Id': e.response['Error']['Code'],
-                'Recommendation': e.response['Error']['Code'],
-                'Description': e.response['Error']['Code'],
-                'Metadata': {
-                    'Exception': str(traceback.format_exc())
-                },
-                'Recommendation Reason': {
-                    e.response['Error']['Code']
-                },
-                'Risk': 'Low',
-                'Savings': None,
-                'Source': 'Klera',
-                'Category': 'Cost Optimization'
-            }
-            recommendation.append(temp)
-        return recommendation
+import logging
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger()
+
+class s3:
+    def get_s3_recommendations(self) -> list:
+        """
+        :return: list of s3 recommendations
+        """
+        bucket_list = self.__list_s3_buckets()
+        return self.__enable_s3_bucket_keys(bucket_list) + self.__s3_bucket_versioning_enabled(bucket_list) + self.__s3_bucket_lifecycle_configuration(bucket_list)
+
+    # returns the list of s3 buckets
+    def __list_s3_buckets(self):
+        """
+        :return:
+        """
+        logger.info(" ---Inside utils :: list_s3_buckets()--- ")
+        client = self.session.client('s3')
 
-    for bucket in response['Buckets']:
         try:
-            res = client.get_bucket_encryption(
-                Bucket=bucket['Name']
-            )
+            response = client.list_buckets()
+            return response['Buckets']
         except ClientError as e:
-            if e.response['Error']['Code'] == 'AccessDenied':
-                logger.info('---------S3 read access denied----------')
+            return e.response['Error']['Code']
+
+    # Generate the recommendation for enable s3 bucket keys
+    def __enable_s3_bucket_keys(self, bucket_list: list) -> list:
+        """
+        :param bucket_list:
+        :param self:
+        :return:
+        """
+        logger.info(" ---Inside s3 :: enable_s3_bucket_keys()")
+
+        recommendation = []
+
+        client = self.session.client('s3')
+
+        for bucket in bucket_list:
+            try:
+                res = client.get_bucket_encryption(
+                    Bucket=bucket['Name']
+                )
+            except ClientError as e:
+                if e.response['Error']['Code'] == 'AccessDenied':
+                    logger.info('---------S3 read access denied----------')
+                    temp = {
+                        'Service Name': 'S3',
+                        'Id': bucket['Name'],
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Exception': str(traceback.format_exc())
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'Low',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+                continue
+            for rule in res['ServerSideEncryptionConfiguration']['Rules']:
+                if rule['ApplyServerSideEncryptionByDefault']['SSEAlgorithm'] == 'aws:kms' and rule['BucketKeyEnabled']:
+                    temp = {
+                        'Service Name': 'S3',
+                        'Id': bucket['Name'],
+                        'Recommendation': 'Enable s3 bucket keys',
+                        'Description': 'Enable s3 bucket keys instead of KMS keys to optimize the aws cost',
+                        'Metadata':{
+
+                        },
+                        'Recommendation Reason': {
+                            # 'Average CPU Datapoints(7 days)': [float('{:.2f}'.format(x)) for x in tmp_lst_cpu]
+                            'reason': 'KMS keys are used for encryption'
+                        },
+                        'Risk': 'Low',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+
+        return recommendation
+
+    # Generate the recommendation for bucket versioning enabled
+    def __s3_bucket_versioning_enabled(self, bucket_list: list):
+        """
+        :param bucket_list:
+        :param self:
+        :return dict: details of s3 bucket versioning enabled compliance.py
+        """
+        logger.info(" ---Inside s3 :: s3_bucket_versioning_enabled()")
+
+        recommendation = []
+
+        client = self.session.client('s3')
+
+        for bucket in bucket_list:
+            bucket_name = bucket['Name']
+
+            try:
+                resp = client.get_bucket_versioning(
+                    Bucket=bucket_name,
+                )
+                status = resp['Status']
+            except ClientError as e:
+                if e.response['Error']['Code'] == 'AccessDenied':
+                    logger.info('---------S3 read access denied----------')
+                    temp = {
+                        'Service Name': 'S3',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Exception': str(traceback.format_exc())
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'Low',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Operational Best Practice'
+                    }
+                    recommendation.append(temp)
+                    return recommendation
                 temp = {
                     'Service Name': 'S3',
                     'Id': bucket['Name'],
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
+                    'Recommendation': 'Enable S3 bucket versioning',
+                    'Description': 'Enable s3 bucket versioning',
                     'Metadata': {
-                        'Exception': str(traceback.format_exc())
+
                     },
                     'Recommendation Reason': {
-                        'Access Denied'
+                        'reason': 'Bucket versioning is not enabled'
                     },
                     'Risk': 'Low',
                     'Savings': None,
                     'Source': 'Klera',
-                    'Category': 'Cost Optimization'
+                    'Category': 'Operational Best Practice'
                 }
                 recommendation.append(temp)
-            continue
-        for rule in res['ServerSideEncryptionConfiguration']['Rules']:
-            if rule['ApplyServerSideEncryptionByDefault']['SSEAlgorithm'] == 'aws:kms' and rule['BucketKeyEnabled']:
+                continue
+            except KeyError:
                 temp = {
                     'Service Name': 'S3',
                     'Id': bucket['Name'],
-                    'Recommendation': 'Enable s3 bucket keys',
-                    'Description': 'Enable s3 bucket keys instead of KMS keys to optimize the aws cost',
-                    'Metadata':{
+                    'Recommendation': 'Enable S3 bucket versioning',
+                    'Description': 'Enable s3 bucket versioning',
+                    'Metadata': {
 
                     },
                     'Recommendation Reason': {
-                        # 'Average CPU Datapoints(7 days)': [float('{:.2f}'.format(x)) for x in tmp_lst_cpu]
-                        'reason': 'KMS keys are used for encryption'
+                        'reason': 'Bucket versioning is not enabled'
                     },
                     'Risk': 'Low',
                     'Savings': None,
                     'Source': 'Klera',
-                    'Category': 'Cost Optimization'
+                    'Category': 'Operational Best Practice'
                 }
                 recommendation.append(temp)
+                continue
 
-    return recommendation
-
-
-# Generate the recommendation for bucket versioning enabled
-def s3_bucket_versioning_enabled(self):
-    """
-    :param self:
-    :return dict: details of s3 bucket versioning enabled compliance.py
-    """
-    logger.info(" ---Inside s3 :: s3_bucket_versioning_enabled()")
-
-    recommendation = []
-
-    client = self.session.client('s3')
-    try:
-        response = client.list_buckets()
-    except ClientError as e:
-        if e.response['Error']['Code'] == 'AccessDenied':
-            logger.info('---------S3 read access denied----------')
-            temp = {
-                'Service Name': 'S3',
-                'Id': 'Access Denied',
-                'Recommendation': 'Access Denied',
-                'Description': 'Access Denied',
-                'Metadata': {
-                    'Exception': str(traceback.format_exc())
-                },
-                'Recommendation Reason': {
-                    'Access Denied'
-                },
-                'Risk': 'Low',
-                'Savings': None,
-                'Source': 'Klera',
-                'Category': 'Operational Best Practice'
-            }
-            recommendation.append(temp)
-        else:
-            temp = {
-                'Service Name': 'S3',
-                'Id': e.response['Error']['Code'],
-                'Recommendation': e.response['Error']['Code'],
-                'Description': e.response['Error']['Code'],
-                'Metadata': {
-                    'Exception': str(traceback.format_exc())
-                },
-                'Recommendation Reason': {
-                    e.response['Error']['Code']
-                },
-                'Risk': 'Low',
-                'Savings': None,
-                'Source': 'Klera',
-                'Category': 'Operational Best Practice'
-            }
-            recommendation.append(temp)
-        return recommendation
-
-    for bucket in response['Buckets']:
-        bucket_name = bucket['Name']
-
-        try:
-            resp = client.get_bucket_versioning(
-                Bucket=bucket_name,
-            )
-            status = resp['Status']
-        except ClientError as e:
-            if e.response['Error']['Code'] == 'AccessDenied':
-                logger.info('---------S3 read access denied----------')
+            if not status == 'Enabled':
                 temp = {
                     'Service Name': 'S3',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
+                    'Id': bucket['Name'],
+                    'Recommendation': 'Enable S3 bucket versioning',
+                    'Description': 'Enable s3 bucket versioning',
                     'Metadata': {
-                        'Exception': str(traceback.format_exc())
+
                     },
                     'Recommendation Reason': {
-                        'Access Denied'
+                        'reason': 'Bucket versioning is not enabled'
                     },
                     'Risk': 'Low',
                     'Savings': None,
                     'Source': 'Klera',
                     'Category': 'Operational Best Practice'
                 }
                 recommendation.append(temp)
-                return recommendation
-            temp = {
-                'Service Name': 'S3',
-                'Id': bucket['Name'],
-                'Recommendation': 'Enable S3 bucket versioning',
-                'Description': 'Enable s3 bucket versioning',
-                'Metadata': {
-
-                },
-                'Recommendation Reason': {
-                    'reason': 'Bucket versioning is not enabled'
-                },
-                'Risk': 'Low',
-                'Savings': None,
-                'Source': 'Klera',
-                'Category': 'Operational Best Practice'
-            }
-            recommendation.append(temp)
-            continue
-        except KeyError:
-            temp = {
-                'Service Name': 'S3',
-                'Id': bucket['Name'],
-                'Recommendation': 'Enable S3 bucket versioning',
-                'Description': 'Enable s3 bucket versioning',
-                'Metadata': {
-
-                },
-                'Recommendation Reason': {
-                    'reason': 'Bucket versioning is not enabled'
-                },
-                'Risk': 'Low',
-                'Savings': None,
-                'Source': 'Klera',
-                'Category': 'Operational Best Practice'
-            }
-            recommendation.append(temp)
-            continue
-
-        if not status == 'Enabled':
-            temp = {
-                'Service Name': 'S3',
-                'Id': bucket['Name'],
-                'Recommendation': 'Enable S3 bucket versioning',
-                'Description': 'Enable s3 bucket versioning',
-                'Metadata': {
-
-                },
-                'Recommendation Reason': {
-                    'reason': 'Bucket versioning is not enabled'
-                },
-                'Risk': 'Low',
-                'Savings': None,
-                'Source': 'Klera',
-                'Category': 'Operational Best Practice'
-            }
-            recommendation.append(temp)
-
-    return recommendation
-
-
-#Generate the recommendation for s3 lifecycle enabled
-def s3_bucket_lifecycle_configuration(self)-> list:
-    """
-    :param self:
-    :return dict: details of s3 bucket versioning enabled compliance.py
-    """
-    logger.info(" ---Inside s3 :: s3_bucket_lifecycle_configuration()")
-
-    recommendation = []
-
-    client = self.session.client('s3')
-    try:
-        response = client.list_buckets()
-
-    except ClientError as e:
-        print(e)
-        if e.response['Error']['Code'] == 'AccessDenied':
-            logger.info('---------S3 read access denied----------')
-            temp = {
-                'Service Name': 'S3',
-                'Id': 'Access Denied',
-                'Recommendation': 'Access Denied',
-                'Description': 'Access Denied',
-                'Metadata': {
-                    'Exception': str(traceback.format_exc())
-                },
-                'Recommendation Reason': {
-                    'Access Denied'
-                },
-                'Risk': 'Low',
-                'Savings': None,
-                'Source': 'Klera',
-                'Category': 'Cost Optimization'
-            }
-            recommendation.append(temp)
-        else:
-            temp = {
-                'Service Name': 'S3',
-                'Id': e.response['Error']['Code'],
-                'Recommendation': e.response['Error']['Code'],
-                'Description': e.response['Error']['Code'],
-                'Metadata': {
-                    'Exception': str(traceback.format_exc())
-                },
-                'Recommendation Reason': {
-                    e.response['Error']['Code']
-                },
-                'Risk': 'Low',
-                'Savings': None,
-                'Source': 'Klera',
-                'Category': 'Cost Optimization'
-            }
-            recommendation.append(temp)
-        return recommendation
 
-    for bucket in response['Buckets']:
-        bucket_name = bucket['Name']
-        # print(bucket_name)
-        try:
-            resp = client.get_bucket_lifecycle_configuration(
-                Bucket=bucket_name,
-            )
-            # print(resp)
-            flag = False
-            for rule in resp['Rules']:
-                if rule['Status'] == 'Enabled':
-                    flag = flag or True
-                else:
-                    flag = flag or False
+        return recommendation
 
-            if not flag:
+    #Generate the recommendation for s3 lifecycle enabled
+    def __s3_bucket_lifecycle_configuration(self, bucket_list: list)-> list:
+        """
+        :param bucket_list:
+        :param self:
+        :return dict: details of s3 bucket versioning enabled compliance.py
+        """
+        logger.info(" ---Inside s3 :: s3_bucket_lifecycle_configuration()")
+
+        recommendation = []
+
+        client = self.session.client('s3')
+
+        for bucket in bucket_list:
+            bucket_name = bucket['Name']
+            # print(bucket_name)
+            try:
+                resp = client.get_bucket_lifecycle_configuration(
+                    Bucket=bucket_name,
+                )
+                # print(resp)
+                flag = False
+                for rule in resp['Rules']:
+                    if rule['Status'] == 'Enabled':
+                        flag = flag or True
+                    else:
+                        flag = flag or False
+
+                if not flag:
+                    temp = {
+                        'Service Name': 'S3',
+                        'Id': bucket['Name'],
+                        'Recommendation': 'Add lifecycle rules to the bucket',
+                        'Description': 'Add lifecycle rules to the bucket',
+                        'Metadata': {
+
+                        },
+                        'Recommendation Reason': {
+                            'reason': 'lifecycle rules are not there for s3 bucket'
+                        },
+                        'Risk': 'Low',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+
+            except ClientError as e:
+                if e.response['Error']['Code'] == 'AccessDenied':
+                    logger.info('---------S3 read access denied----------')
+                    temp = {
+                        'Service Name': 'S3',
+                        'Id': 'Access Denied',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Access Denied',
+                        'Metadata': {
+                            'Exception': str(traceback.format_exc())
+                        },
+                        'Recommendation Reason': {
+                            'Access Denied'
+                        },
+                        'Risk': 'Low',
+                        'Savings': None,
+                        'Source': 'Klera',
+                        'Category': 'Cost Optimization'
+                    }
+                    recommendation.append(temp)
+                    return recommendation
                 temp = {
                     'Service Name': 'S3',
                     'Id': bucket['Name'],
                     'Recommendation': 'Add lifecycle rules to the bucket',
                     'Description': 'Add lifecycle rules to the bucket',
                     'Metadata': {
 
@@ -334,47 +275,8 @@
                     'Risk': 'Low',
                     'Savings': None,
                     'Source': 'Klera',
                     'Category': 'Cost Optimization'
                 }
                 recommendation.append(temp)
 
-        except ClientError as e:
-            if e.response['Error']['Code'] == 'AccessDenied':
-                logger.info('---------S3 read access denied----------')
-                temp = {
-                    'Service Name': 'S3',
-                    'Id': 'Access Denied',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Access Denied',
-                    'Metadata': {
-                        'Exception': str(traceback.format_exc())
-                    },
-                    'Recommendation Reason': {
-                        'Access Denied'
-                    },
-                    'Risk': 'Low',
-                    'Savings': None,
-                    'Source': 'Klera',
-                    'Category': 'Cost Optimization'
-                }
-                recommendation.append(temp)
-                return recommendation
-            temp = {
-                'Service Name': 'S3',
-                'Id': bucket['Name'],
-                'Recommendation': 'Add lifecycle rules to the bucket',
-                'Description': 'Add lifecycle rules to the bucket',
-                'Metadata': {
-
-                },
-                'Recommendation Reason': {
-                    'reason': 'lifecycle rules are not there for s3 bucket'
-                },
-                'Risk': 'Low',
-                'Savings': None,
-                'Source': 'Klera',
-                'Category': 'Cost Optimization'
-            }
-            recommendation.append(temp)
-
-    return recommendation
+        return recommendation
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/truted_advisor.py` & `aws_recommendation-0.2.3/aws_recommendation/truted_advisor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import logging
 
 from botocore.exceptions import ClientError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
-
-# Generates recommendation from trusted advisor
-def get_trusted_advisor_recommendations(self) -> list:
-    """
-    :param self:
-    :return: list of
-    """
-    logger.info(" ---Inside get_trusted_advisor_recommendations")
-
-    recommendation = []
-    client = self.session.client('support')
-    try:
-        response = client.describe_trusted_advisor_checks(
-            language='en'
-        )
-        for check in response['checks']:
-            check_description = client.describe_trusted_advisor_check_result(
-                checkId=check['id'],
+class trusted_advisor:
+    # Generates recommendation from trusted advisor
+    def get_trusted_advisor_recommendations(self) -> list:
+        """
+        :param self:
+        :return: list of
+        """
+        logger.info(" ---Inside get_trusted_advisor_recommendations")
+
+        recommendation = []
+        client = self.session.client('support')
+        try:
+            response = client.describe_trusted_advisor_checks(
                 language='en'
             )
-            print(check_description)
-
-    except ClientError as e:
-        logger.info('Exception caught: ' + (e.response['Error']['Code']))
-        if e.response['Error']['Code'] == 'SubscriptionRequiredException':
-            return [{
-                    'Service Name': 'CloudWatch',
-                    'Id': 'Subscription Required',
-                    'Recommendation': 'Access Denied',
-                    'Description': 'Amazon Web Services Premium Support Subscription is required to use this service.',
-                    'Metadata': {},
-                    'Recommendation Reason': {},
-                    'Risk': 'Medium',
-                    'Savings': None,
-                    'Source': 'AWS',
-                    'Category': ''
-                }]
+            for check in response['checks']:
+                check_description = client.describe_trusted_advisor_check_result(
+                    checkId=check['id'],
+                    language='en'
+                )
+                print(check_description)
+
+        except ClientError as e:
+            logger.info('Exception caught: ' + (e.response['Error']['Code']))
+            if e.response['Error']['Code'] == 'SubscriptionRequiredException':
+                return [{
+                        'Service Name': 'CloudWatch',
+                        'Id': 'Subscription Required',
+                        'Recommendation': 'Access Denied',
+                        'Description': 'Amazon Web Services Premium Support Subscription is required to use this service.',
+                        'Metadata': {},
+                        'Recommendation Reason': {},
+                        'Risk': 'Medium',
+                        'Savings': None,
+                        'Source': 'AWS',
+                        'Category': ''
+                    }]
 
-    return recommendation
+        return recommendation
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation/utils.py` & `aws_recommendation-0.2.3/aws_recommendation/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,131 +1,182 @@
-from dateutil.relativedelta import relativedelta
 import datetime as dt
 import logging
 
-logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger()
-
-
-# returns the list of instances
-def list_instances(self, region) -> list:
-    client = self.session.client('ec2', region_name=region)
-    instance_lst = []
-    marker = ''
-    while True:
-        response = client.describe_instances(
-            MaxResults=1000,
-            NextToken=marker
-        )
-        for i in response['Reservations']:
-            for instance in i['Instances']:
-                state = instance['State']['Name']
-                if not state == 'terminated':
-                    instance_lst.append(instance)
-
-        try:
-            marker = response['NextToken']
-            if marker == '':
-                break
-        except KeyError:
-            break
+from dateutil.relativedelta import relativedelta
 
-    return instance_lst
+r_logger = logging.getLogger('Recommender')
+r_logger.setLevel(logging.DEBUG)
 
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger()
 
-# returns the list of rds instances
-def list_rds_instances(self, region) -> list:
-    client = self.session.client('rds', region_name=region)
-
-    rds_instance_lst = []
-    marker = ''
-    while True:
-        response = client.describe_db_instances(
-            MaxRecords=100,
-            Marker=marker
-        )
-        rds_instance_lst.extend(response['DBInstances'])
-
-        try:
-            marker = response['Marker']
-            if marker == '':
-                break
-        except KeyError:
-            break
-    return rds_instance_lst
-
-
-# returns the metrics data
-def get_metrics_stats(self, region: str, namespace: str, dimensions: list,
-                      metric_name='CPUUtilization', start_time=dt.datetime.utcnow() - relativedelta(days=7),
-                      end_time=dt.datetime.utcnow(), period=86400, stats=None, unit='Percent'):
-    if stats is None:
-        stats = ["Average"]
-
-    client = self.session.client('cloudwatch', region_name=region)
-
-    if unit is None:
-        response_cpu = client.get_metric_statistics(
-            Namespace=namespace,
-            MetricName=metric_name,
-            StartTime=start_time,
-            EndTime=end_time,
-            Period=period,
-            Statistics=stats,
-            Dimensions=dimensions
-        )
-    else:
-        response_cpu = client.get_metric_statistics(
-            Namespace=namespace,
-            MetricName=metric_name,
-            StartTime=start_time,
-            EndTime=end_time,
-            Period=period,
-            Statistics=stats,
-            Unit=unit,
-            Dimensions=dimensions
-        )
-    return response_cpu
-
-
-# returns the list of redshift clusters
-def list_redshift_clusters(client) -> list:
-    """
-    :param client:
-    :return:
-    """
-    logger.info(" ---Inside utils() :: list_redshift_clusters()")
-
-    cluster_list = []
-
-    marker = ''
-    while True:
-        if marker == '' or marker is None:
-            response = client.describe_clusters()
+class utils:
+    # returns the list of instances
+    def list_instances(self, regions) -> dict:
+        logger.info(" ---Inside utils :: list_instances()--- ")
+
+        instance_lst = {}
+
+        for region in regions:
+            client = self.session.client('ec2', region_name=region)
+
+            marker = ''
+            while True:
+                response = client.describe_instances(
+                    MaxResults=1000,
+                    NextToken=marker
+                )
+                for i in response['Reservations']:
+                    for instance in i['Instances']:
+                        state = instance['State']['Name']
+                        if not state == 'terminated':
+                            instance_lst.setdefault(region, []).append(instance)
+
+                try:
+                    marker = response['NextToken']
+                    if marker == '':
+                        break
+                except KeyError:
+                    break
+
+        return instance_lst
+
+
+    # returns the list of rds instances
+    def list_rds_instances(self, regions) -> dict:
+        """
+        :param regions:
+        :return:
+        """
+        logger.info(" ---Inside utils :: list_rds_instances()--- ")
+        rds_instance_lst = {}
+
+        for region in regions:
+            client = self.session.client('rds', region_name=region)
+            marker = ''
+            while True:
+                response = client.describe_db_instances(
+                    MaxRecords=100,
+                    Marker=marker
+                )
+                rds_instance_lst.setdefault(region, []).extend(response['DBInstances'])
+
+                try:
+                    marker = response['Marker']
+                    if marker == '':
+                        break
+                except KeyError:
+                    break
+        return rds_instance_lst
+
+
+    # returns the metrics data
+    def get_metrics_stats(self, region, namespace: str, dimensions: list,
+                          metric_name='CPUUtilization', start_time=dt.datetime.utcnow() - relativedelta(days=7),
+                          end_time=dt.datetime.utcnow(), period=86400, stats=None, unit='Percent'):
+        if stats is None:
+            stats = ["Average"]
+
+        client = self.session.client('cloudwatch', region_name=region)
+
+        if unit is None:
+            response_cpu = client.get_metric_statistics(
+                Namespace=namespace,
+                MetricName=metric_name,
+                StartTime=start_time,
+                EndTime=end_time,
+                Period=period,
+                Statistics=stats,
+                Dimensions=dimensions
+            )
         else:
-            response = client.describe_clusters(
-                Marker = marker
+            response_cpu = client.get_metric_statistics(
+                Namespace=namespace,
+                MetricName=metric_name,
+                StartTime=start_time,
+                EndTime=end_time,
+                Period=period,
+                Statistics=stats,
+                Unit=unit,
+                Dimensions=dimensions
             )
-        cluster_list.extend(response['Clusters'])
+        return response_cpu
+
 
-        try:
-            marker = response['Marker']
-            if marker == '':
+    # returns the list of redshift clusters
+    def list_redshift_clusters(self, client) -> list:
+        """
+        :param client:
+        :return:
+        """
+        logger.info(" ---Inside utils() :: list_redshift_clusters()")
+
+        cluster_list = []
+
+        marker = ''
+        while True:
+            if marker == '' or marker is None:
+                response = client.describe_clusters()
+            else:
+                response = client.describe_clusters(
+                    Marker = marker
+                )
+            cluster_list.extend(response['Clusters'])
+
+            try:
+                marker = response['Marker']
+                if marker == '':
+                    break
+            except KeyError:
                 break
-        except KeyError:
-            break
 
-    return cluster_list
+        return cluster_list
 
 
-# returns the list of aws regions
-def get_regions(session):
-    """
-    :session: aws session object
-    :return: list of regions
-    """
-    logger.info(" ---Inside utils :: get_regions()--- ")
-    client = session.client('ec2', region_name='us-east-1')
-    region_response = client.describe_regions()
+    # returns the list of aws regions
+    def get_regions(self):
+        """
+        :session: aws session object
+        :return: list of regions
+        """
+        logger.info(" ---Inside utils :: get_regions()--- ")
+        client = self.session.client('ec2', region_name='us-east-1')
+        region_response = client.describe_regions()
+
+        regions = [region['RegionName'] for region in region_response['Regions']]
+        return regions
+
+#     returns the list of ebs volumes
+    def list_ebs_volumes(self, regions: list) -> dict:
+        """
+        :param regions:
+        :return:
+        """
+        logger.info("---Inside utils :: list_ebs_volumes()--- ")
+
+        ebs_volumes = {}
+
+        for region in regions:
+            client = self.session.client('ec2', region_name=region)
+            marker = ''
+            while True:
+                response = client.describe_volumes(
+                    Filters=[
+                        {
+                            'Name': 'status',
+                            'Values': [
+                                'in-use'
+                            ]
+                        },
+                    ],
+                    MaxResults=500,
+                    NextToken=marker
+                )
+                ebs_volumes.setdefault(region, []).extend(response['Volumes'])
+                try:
+                    marker = response['NextToken']
+                    if marker == '':
+                        break
+                except KeyError:
+                    break
 
-    regions = [region['RegionName'] for region in region_response['Regions']]
-    return regions
+        return ebs_volumes
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation.egg-info/PKG-INFO` & `aws_recommendation-0.2.3/aws_recommendation.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-recommendation
-Version: 0.2.2
+Version: 0.2.3
 Summary: Provides AWS recommendations
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `aws_recommendation-0.2.2/aws_recommendation.egg-info/SOURCES.txt` & `aws_recommendation-0.2.3/aws_recommendation.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 aws_recommendation/cost_estimations.py
 aws_recommendation/dynamodb.py
 aws_recommendation/ebs.py
 aws_recommendation/ec2.py
 aws_recommendation/elb.py
 aws_recommendation/kms.py
 aws_recommendation/rds.py
-aws_recommendation/recommendation.py
 aws_recommendation/redshift.py
 aws_recommendation/s3.py
 aws_recommendation/truted_advisor.py
 aws_recommendation/utils.py
 aws_recommendation.egg-info/PKG-INFO
 aws_recommendation.egg-info/SOURCES.txt
 aws_recommendation.egg-info/dependency_links.txt
```

