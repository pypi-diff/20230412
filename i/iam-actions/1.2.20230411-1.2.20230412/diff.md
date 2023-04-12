# Comparing `tmp/iam_actions-1.2.20230411.tar.gz` & `tmp/iam_actions-1.2.20230412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230411.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230412.tar", max compression
```

## Comparing `iam_actions-1.2.20230411.tar` & `iam_actions-1.2.20230412.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/README.md
--rw-r--r--   0        0        0      228 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/__init__.py
--rw-r--r--   0        0        0  4203173 2023-04-11 02:26:38.531502 iam_actions-1.2.20230411/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-11 02:24:31.840985 iam_actions-1.2.20230411/iam_actions/generate/services.py
--rw-r--r--   0        0        0   539591 2023-04-11 02:26:38.531502 iam_actions-1.2.20230411/iam_actions/policies.json
--rw-r--r--   0        0        0   190147 2023-04-11 02:26:38.531502 iam_actions-1.2.20230411/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   523243 2023-04-11 02:26:38.531502 iam_actions-1.2.20230411/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-11 02:26:39.519521 iam_actions-1.2.20230411/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230411/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230411/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/README.md
+-rw-r--r--   0        0        0      228 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4204979 2023-04-12 02:26:50.055398 iam_actions-1.2.20230412/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-12 02:25:13.443376 iam_actions-1.2.20230412/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   539591 2023-04-12 02:26:50.055398 iam_actions-1.2.20230412/iam_actions/policies.json
+-rw-r--r--   0        0        0   190147 2023-04-12 02:26:50.055398 iam_actions-1.2.20230412/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   523243 2023-04-12 02:26:50.055398 iam_actions-1.2.20230412/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-12 02:26:50.851400 iam_actions-1.2.20230412/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230412/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230412/PKG-INFO
```

### Comparing `iam_actions-1.2.20230411/LICENSE` & `iam_actions-1.2.20230412/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/README.md` & `iam_actions-1.2.20230412/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/iam_actions/actions.json` & `iam_actions-1.2.20230412/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998798776242118%*

 * *Differences: {"'aws-portal'": "{'UpdateConsoleActionSetEnforced': {'access_level': 'Write', 'description': "*

 * *                 "'Grants permission to change whether existing or fine-grained IAM actions will "*

 * *                 'be used to control authorization to Billing, Cost Management, and Account '*

 * *                 "consoles'}, 'GetConsoleActionSetEnforced': {'access_level': 'Read', "*

 * *                 "'description': 'Grants permission to view whether existing or fine-grained IAM "*

 * *                 'actions are being  […]*

```diff
@@ -10387,18 +10387,18 @@
             "description": "Allows access to the Customer Support Eligibility page inside the AWS Marketplace Management Portal.",
             "orphan": false,
             "resources": []
         }
     },
     "aws-portal": {
         "GetConsoleActionSetEnforced": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetConsoleActionSetEnforced",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view whether existing or fine-grained IAM actions are being used to control authorization to Billing, Cost Management, and Account consoles",
             "orphan": false,
             "resources": []
         },
         "ModifyAccount": {
             "access_level": "Write",
             "action": "ModifyAccount",
             "condition_keys": [],
@@ -10419,18 +10419,18 @@
             "action": "ModifyPaymentMethods",
             "condition_keys": [],
             "description": "Allow or deny IAM users permission to modify payment methods",
             "orphan": false,
             "resources": []
         },
         "UpdateConsoleActionSetEnforced": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateConsoleActionSetEnforced",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to change whether existing or fine-grained IAM actions will be used to control authorization to Billing, Cost Management, and Account consoles",
             "orphan": false,
             "resources": []
         },
         "ViewAccount": {
             "access_level": "Read",
             "action": "ViewAccount",
             "condition_keys": [],
@@ -106211,87 +106211,87 @@
         }
     },
     "purchase-orders": {
         "AddPurchaseOrder": {
             "access_level": "Write",
             "action": "AddPurchaseOrder",
             "condition_keys": [],
-            "description": "Allow or deny IAM users permission to add a new purchase order",
+            "description": "Grants permission to add a new purchase order",
             "orphan": false,
             "resources": []
         },
         "DeletePurchaseOrder": {
             "access_level": "Write",
             "action": "DeletePurchaseOrder",
             "condition_keys": [],
-            "description": "Allow or deny IAM users permission to delete a purchase order",
+            "description": "Grants permission to delete a purchase order",
             "orphan": false,
             "resources": []
         },
         "GetConsoleActionSetEnforced": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetConsoleActionSetEnforced",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view whether existing or fine-grained IAM actions are being used to control authorization to Billing, Cost Management, and Account consoles",
             "orphan": false,
             "resources": []
         },
         "GetPurchaseOrder": {
             "access_level": "Read",
             "action": "GetPurchaseOrder",
             "condition_keys": [],
-            "description": "Allow or deny IAM users permission to get a purchase order",
+            "description": "Grants permission to get a purchase order",
             "orphan": false,
             "resources": []
         },
         "ListPurchaseOrderInvoices": {
             "access_level": "List",
             "action": "ListPurchaseOrderInvoices",
             "condition_keys": [],
-            "description": "Allow or deny IAM users permission to list purchase order invoices",
+            "description": "Grants permission to list purchase order invoices",
             "orphan": false,
             "resources": []
         },
         "ListPurchaseOrders": {
             "access_level": "List",
             "action": "ListPurchaseOrders",
             "condition_keys": [],
-            "description": "Allow or deny IAM users permission to get all available purchase orders",
+            "description": "Grants permission to get all available purchase orders",
             "orphan": false,
             "resources": []
         },
         "ModifyPurchaseOrders": {
             "access_level": "Write",
             "action": "ModifyPurchaseOrders",
             "condition_keys": [],
             "description": "Grants permission to modify purchase orders and details",
             "orphan": false,
             "resources": []
         },
         "UpdateConsoleActionSetEnforced": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateConsoleActionSetEnforced",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to change whether existing or fine-grained IAM actions will be used to control authorization to Billing, Cost Management, and Account consoles",
             "orphan": false,
             "resources": []
         },
         "UpdatePurchaseOrder": {
             "access_level": "Write",
             "action": "UpdatePurchaseOrder",
             "condition_keys": [],
-            "description": "Allow or deny IAM users permission to update an existing purchase order",
+            "description": "Grants permission to update an existing purchase order",
             "orphan": false,
             "resources": []
         },
         "UpdatePurchaseOrderStatus": {
             "access_level": "Write",
             "action": "UpdatePurchaseOrderStatus",
             "condition_keys": [],
-            "description": "Allow or deny IAM users permission to set purchase order status",
+            "description": "Grants permission to set purchase order status",
             "orphan": false,
             "resources": []
         },
         "ViewPurchaseOrders": {
             "access_level": "Read",
             "action": "ViewPurchaseOrders",
             "condition_keys": [],
@@ -112744,18 +112744,18 @@
             "description": "Grants permission to create a new Amazon Rekognition Custom Labels dataset",
             "orphan": false,
             "resources": [
                 "project"
             ]
         },
         "CreateFaceLivenessSession": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateFaceLivenessSession",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a face liveness session",
             "orphan": false,
             "resources": []
         },
         "CreateProject": {
             "access_level": "Write",
             "action": "CreateProject",
             "condition_keys": [],
@@ -112998,18 +112998,18 @@
             "action": "GetFaceDetection",
             "condition_keys": [],
             "description": "Grants permission to read the faces detection results found in a stored video by an asynchronous face detection job",
             "orphan": false,
             "resources": []
         },
         "GetFaceLivenessSessionResults": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetFaceLivenessSessionResults",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get results of a face liveness session",
             "orphan": false,
             "resources": []
         },
         "GetFaceSearch": {
             "access_level": "Read",
             "action": "GetFaceSearch",
             "condition_keys": [],
@@ -113188,18 +113188,18 @@
             "action": "StartFaceDetection",
             "condition_keys": [],
             "description": "Grants permission to start asynchronous detection of faces in a stored video",
             "orphan": false,
             "resources": []
         },
         "StartFaceLivenessSession": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartFaceLivenessSession",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start streaming video for a face liveness session",
             "orphan": false,
             "resources": []
         },
         "StartFaceSearch": {
             "access_level": "Write",
             "action": "StartFaceSearch",
             "condition_keys": [],
@@ -120760,20 +120760,27 @@
             "description": "Grants permission to retrieve a specific version of an object",
             "orphan": false,
             "resources": [
                 "object"
             ]
         },
         "GetObjectVersionForReplication": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetObjectVersionForReplication",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "s3-outposts:authType",
+                "s3-outposts:signatureAge",
+                "s3-outposts:signatureversion",
+                "s3-outposts:x-amz-content-sha256"
+            ],
+            "description": "Grants permission to replicate both unencrypted objects and objects encrypted with SSE-KMS",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "object"
+            ]
         },
         "GetObjectVersionTagging": {
             "access_level": "Read",
             "action": "GetObjectVersionTagging",
             "condition_keys": [
                 "s3-outposts:AccessPointNetworkOrigin",
                 "s3-outposts:DataAccessPointAccount",
@@ -120788,20 +120795,27 @@
             "description": "Grants permission to return the tag set for a specific version of the object",
             "orphan": false,
             "resources": [
                 "object"
             ]
         },
         "GetReplicationConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetReplicationConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "s3-outposts:authType",
+                "s3-outposts:signatureAge",
+                "s3-outposts:signatureversion",
+                "s3-outposts:x-amz-content-sha256"
+            ],
+            "description": "Grants permission to get the replication configuration information set on an Amazon S3 bucket",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "bucket"
+            ]
         },
         "ListAccessPoints": {
             "access_level": "List",
             "action": "ListAccessPoints",
             "condition_keys": [
                 "s3-outposts:authType",
                 "s3-outposts:signatureAge",
@@ -121093,44 +121107,73 @@
             "description": "Grants permission to set the supplied tag-set for a specific version of an object",
             "orphan": false,
             "resources": [
                 "object"
             ]
         },
         "PutReplicationConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutReplicationConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "s3-outposts:authType",
+                "s3-outposts:signatureAge",
+                "s3-outposts:signatureversion",
+                "s3-outposts:x-amz-content-sha256"
+            ],
+            "description": "Grants permission to create a new replication configuration or replace an existing one",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "bucket"
+            ]
         },
         "ReplicateDelete": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReplicateDelete",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "s3-outposts:authType",
+                "s3-outposts:signatureAge",
+                "s3-outposts:signatureversion",
+                "s3-outposts:x-amz-content-sha256"
+            ],
+            "description": "Grants permission to replicate delete markers to the destination bucket",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "object"
+            ]
         },
         "ReplicateObject": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReplicateObject",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "s3-outposts:authType",
+                "s3-outposts:signatureAge",
+                "s3-outposts:signatureversion",
+                "s3-outposts:x-amz-content-sha256",
+                "s3-outposts:x-amz-server-side-encryption"
+            ],
+            "description": "Grants permission to replicate objects and object tags to the destination bucket",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "object"
+            ]
         },
         "ReplicateTags": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "ReplicateTags",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "s3-outposts:authType",
+                "s3-outposts:signatureAge",
+                "s3-outposts:signatureversion",
+                "s3-outposts:x-amz-content-sha256"
+            ],
+            "description": "Grants permission to replicate object tags to the destination bucket",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "object"
+            ]
         }
     },
     "sagemaker": {
         "AddAssociation": {
             "access_level": "Write",
             "action": "AddAssociation",
             "condition_keys": [
```

### Comparing `iam_actions-1.2.20230411/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230412/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230412/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/iam_actions/generate/generate.py` & `iam_actions-1.2.20230412/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230412/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230412/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/iam_actions/generate/services.py` & `iam_actions-1.2.20230412/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/iam_actions/policies.json` & `iam_actions-1.2.20230412/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230412/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/iam_actions/services.json` & `iam_actions-1.2.20230412/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230411/pyproject.toml` & `iam_actions-1.2.20230412/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230411"
+version = "1.2.20230412"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230411/setup.py` & `iam_actions-1.2.20230412/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230411',
+    'version': '1.2.20230412',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230411/PKG-INFO` & `iam_actions-1.2.20230412/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230411
+Version: 1.2.20230412
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

