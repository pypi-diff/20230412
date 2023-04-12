# Comparing `tmp/cis_checks_2023-2.0.2.tar.gz` & `tmp/cis_checks_2023-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cis_checks_2023-2.0.2.tar", last modified: Tue Apr 11 09:08:30 2023, max compression
+gzip compressed data, was "cis_checks_2023-2.0.3.tar", last modified: Wed Apr 12 07:12:29 2023, max compression
```

## Comparing `cis_checks_2023-2.0.2.tar` & `cis_checks_2023-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 09:08:30.228601 cis_checks_2023-2.0.2/
--rw-rw-rw-   0        0        0      836 2023-04-11 09:08:30.227600 cis_checks_2023-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 09:08:30.198600 cis_checks_2023-2.0.2/cis_checks_2023/
--rw-rw-rw-   0        0        0     6574 2023-04-11 09:07:38.000000 cis_checks_2023-2.0.2/cis_checks_2023/__init__.py
--rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.2/cis_checks_2023/_security_control_5.py
--rw-rw-rw-   0        0        0    52415 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.2/cis_checks_2023/iam_control_1.py
--rw-rw-rw-   0        0        0    23633 2023-04-11 09:07:38.000000 cis_checks_2023-2.0.2/cis_checks_2023/logging_control_3.py
--rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.2/cis_checks_2023/monitoring_control_4.py
--rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.2/cis_checks_2023/networking_control_5.py
--rw-rw-rw-   0        0        0    17716 2023-04-11 07:33:08.000000 cis_checks_2023-2.0.2/cis_checks_2023/storage_control_2.py
--rw-rw-rw-   0        0        0    20340 2023-04-10 07:28:15.000000 cis_checks_2023-2.0.2/cis_checks_2023/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:08:30.223603 cis_checks_2023-2.0.2/cis_checks_2023.egg-info/
--rw-rw-rw-   0        0        0      836 2023-04-11 09:08:30.000000 cis_checks_2023-2.0.2/cis_checks_2023.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-04-11 09:08:30.000000 cis_checks_2023-2.0.2/cis_checks_2023.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:08:30.000000 cis_checks_2023-2.0.2/cis_checks_2023.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-11 09:08:30.000000 cis_checks_2023-2.0.2/cis_checks_2023.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      557 2023-04-11 09:07:38.000000 cis_checks_2023-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 09:08:30.229605 cis_checks_2023-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 07:12:29.536816 cis_checks_2023-2.0.3/
+-rw-rw-rw-   0        0        0      836 2023-04-12 07:12:29.534827 cis_checks_2023-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 07:12:29.518814 cis_checks_2023-2.0.3/cis_checks_2023/
+-rw-rw-rw-   0        0        0     6574 2023-04-12 07:12:04.000000 cis_checks_2023-2.0.3/cis_checks_2023/__init__.py
+-rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.3/cis_checks_2023/_security_control_5.py
+-rw-rw-rw-   0        0        0    53781 2023-04-12 07:09:53.000000 cis_checks_2023-2.0.3/cis_checks_2023/iam_control_1.py
+-rw-rw-rw-   0        0        0    23922 2023-04-12 07:12:03.000000 cis_checks_2023-2.0.3/cis_checks_2023/logging_control_3.py
+-rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.3/cis_checks_2023/monitoring_control_4.py
+-rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.3/cis_checks_2023/networking_control_5.py
+-rw-rw-rw-   0        0        0    17716 2023-04-12 07:08:18.000000 cis_checks_2023-2.0.3/cis_checks_2023/storage_control_2.py
+-rw-rw-rw-   0        0        0    20340 2023-04-10 07:28:15.000000 cis_checks_2023-2.0.3/cis_checks_2023/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:12:29.529814 cis_checks_2023-2.0.3/cis_checks_2023.egg-info/
+-rw-rw-rw-   0        0        0      836 2023-04-12 07:12:29.000000 cis_checks_2023-2.0.3/cis_checks_2023.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-04-12 07:12:29.000000 cis_checks_2023-2.0.3/cis_checks_2023.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 07:12:29.000000 cis_checks_2023-2.0.3/cis_checks_2023.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-12 07:12:29.000000 cis_checks_2023-2.0.3/cis_checks_2023.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      557 2023-04-12 07:12:04.000000 cis_checks_2023-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 07:12:29.536816 cis_checks_2023-2.0.3/setup.cfg
```

### Comparing `cis_checks_2023-2.0.2/PKG-INFO` & `cis_checks_2023-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cis_checks_2023
-Version: 2.0.2
+Version: 2.0.3
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.2/cis_checks_2023/__init__.py` & `cis_checks_2023-2.0.3/cis_checks_2023/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cis_checks_2023.iam_control_1 import iam_control
 
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 
 
 class aws_client(iam_control, utils, storage_control, logging_control, monitoring_control, networking_control):
     def __init__(self, **kwargs):
         """
         @param str aws_access_key_id: AWS Access Key ID
         @param str aws_secret_access_key: AWS Secret Access Key
```

### Comparing `cis_checks_2023-2.0.2/cis_checks_2023/_security_control_5.py` & `cis_checks_2023-2.0.3/cis_checks_2023/_security_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.2/cis_checks_2023/iam_control_1.py` & `cis_checks_2023-2.0.3/cis_checks_2023/iam_control_1.py`

 * *Files 8% similar despite different names*

```diff
@@ -566,19 +566,23 @@
                 PolicyArn=n["Arn"],
                 VersionId=n["DefaultVersionId"]
             )
             statements = policy['PolicyVersion']['Document']['Statement']
 
             for statement in statements:
                 if statement["Effect"] == "Allow":
-                    if statement["Action"] == "*" and statement["Resource"] == "*":
-                        result = "Not Compliant"
-                        failReason = "IAM policies that allow full *:* administrative privileges are attached"
-                        offenders.append(n["Arn"])
-
+                    try:
+                        if statement["Action"] == "*" and statement["Resource"] == "*":
+                            result = "Not Compliant"
+                            failReason = "IAM policies that allow full *:* administrative privileges are attached"
+                            offenders.append(n["Arn"])
+                        else:
+                            continue
+                    except KeyError:
+                        pass
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.17 Ensure a support role has been created to manage incidents with AWS Support (Scored)
     def control_1_17_AWS_support_role_created(self):
         logger.info(" ---Inside iam_control_1 :: control_1_17_AWS_support_role_created()--- ")
         """Summary
@@ -701,18 +705,24 @@
         control = "1.2"
         description = "Ensure that IAM Access analyzer is enabled for all regions"
         scored = True
 
         for region in regions:
             client = self.session.client('accessanalyzer', region_name=region)
             response = client.list_analyzers()
-            if not response['analyzers']:
-                result = "Not Compliant"
-                failReason = "IAM Access analyzer is not enabled for all regions"
-                offenders.append(region)
+            # print(response)
+            try:
+                if response['analyzers'] == []:
+                    result = "Not Compliant"
+                    failReason = "IAM Access analyzer is not enabled for all regions"
+                    offenders.append(region)
+                else:
+                    continue
+            except KeyError:
+                pass
 
         return {
             'Result': result,
             'failReason': failReason,
             'Offenders': offenders,
             'ScoredControl': scored,
             'Description': description,
@@ -736,489 +746,489 @@
         scored = True
         failReason = "Control not implemented using API, please verify manually"
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     '''****************************************************************************'''
 
-    # 1.5 Ensure IAM password policy requires at least one uppercase letter (Scored)
-    def control_1_5_password_policy_uppercase(self, passwordpolicy):
-        logger.info(" ---Inside iam_control_1 :: control_1_5_password_policy_uppercase()--- ")
-        """Summary
-    
-        Args:
-            passwordpolicy (TYPE): Description
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "1.5"
-        description = "Ensure IAM password policy requires at least one uppercase letter"
-        scored = True
-        if passwordpolicy is False:
-            result = "Not Compliant"
-            failReason = "Account does not have a IAM password policy."
-        else:
-            if passwordpolicy['RequireUppercaseCharacters'] is False:
-                result = "Not Compliant"
-                failReason = "Password policy does not require at least one uppercase letter"
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.6 Ensure IAM password policy requires at least one lowercase letter (Scored)
-    def control_1_6_password_policy_lowercase(self, passwordpolicy):
-        logger.info(" ---Inside iam_control_1 :: control_1_6_password_policy_lowercase()--- ")
-        """Summary
-    
-        Args:
-            passwordpolicy (TYPE): Description
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "1.6"
-        description = "Ensure IAM password policy requires at least one lowercase letter"
-        scored = True
-        if passwordpolicy is False:
-            result = "Not Compliant"
-            failReason = "Account does not have a IAM password policy."
-        else:
-            if passwordpolicy['RequireLowercaseCharacters'] is False:
-                result = "Not Compliant"
-                failReason = "Password policy does not require at least one uppercase letter"
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.7 Ensure IAM password policy requires at least one symbol (Scored)
-    def control_1_7_password_policy_symbol(self, passwordpolicy):
-        logger.info(" ---Inside iam_control_1 :: control_1_7_password_policy_symbol()--- ")
-        """Summary
-    
-        Args:
-            passwordpolicy (TYPE): Description
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "1.7"
-        description = "Ensure IAM password policy requires at least one symbol"
-        scored = True
-        if passwordpolicy is False:
-            result = "Not Compliant"
-            failReason = "Account does not have a IAM password policy."
-        else:
-            if passwordpolicy['RequireSymbols'] is False:
-                result = "Not Compliant"
-                failReason = "Password policy does not require at least one symbol"
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.8 Ensure IAM password policy requires at least one number (Scored)
-    def control_1_8_password_policy_number(self, passwordpolicy):
-        logger.info(" ---Inside iam_control_1 :: control_1_8_password_policy_number()--- ")
-        """Summary
-    
-        Args:
-            passwordpolicy (TYPE): Description
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "1.8"
-        description = "Ensure IAM password policy requires at least one number"
-        scored = True
-        if passwordpolicy is False:
-            result = "Not Compliant"
-            failReason = "Account does not have a IAM password policy."
-        else:
-            if passwordpolicy['RequireNumbers'] is False:
-                result = "Not Compliant"
-                failReason = "Password policy does not require at least one number"
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.11 Ensure IAM password policy expires passwords within 90 days or less (Scored)
-    def control_1_11_password_policy_expire(self, passwordpolicy):
-        logger.info(" ---Inside iam_control_1 :: control_1_11_password_policy_expire()--- ")
-        """Summary
-    
-        Args:
-            passwordpolicy (TYPE): Description
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "1.11"
-        description = "Ensure IAM password policy expires passwords within 90 days or less"
-        scored = True
-        if passwordpolicy is False:
-            result = "Not Compliant"
-            failReason = "Account does not have a IAM password policy."
-        else:
-            if passwordpolicy['ExpirePasswords'] is True:
-                if 0 < passwordpolicy['MaxPasswordAge'] > 90:
-                    result = "Not Compliant"
-                    failReason = "Password policy does not expire passwords after 90 days or less"
-            else:
-                result = "Not Compliant"
-                failReason = "Password policy does not expire passwords after 90 days or less"
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.16 Ensure IAM policies are attached only to groups or roles (Scored)
-    def control_1_16_no_policies_on_iam_users(self):
-        logger.info(" ---Inside iam_control_1 :: control_1_16_no_policies_on_iam_users()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "1.16"
-        description = "Ensure IAM policies are attached only to groups or roles"
-        scored = True
-        # global IAM_CLIENT
-        paginator = self.session.client('iam').get_paginator('list_users')
-        response_iterator = paginator.paginate()
-        pagedResult = []
-        for page in response_iterator:
-            for n in page['Users']:
-                pagedResult.append(n)
-        for n in pagedResult:
-            policies = self.session.client('iam').list_user_policies(
-                UserName=n['UserName'],
-                MaxItems=1
-            )
-            if policies['PolicyNames']:
-                result = "Not Compliant"
-                failReason = "IAM user have inline policy attached"
-                offenders.append(str(n['Arn']))
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.17 Enable detailed billing (Scored)
-    def control_1_17_detailed_billing_enabled(self):
-        logger.info(" ---Inside iam_control_1 :: control_1_17_detailed_billing_enabled()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Manual"
-        offenders = []
-        control = "1.17"
-        description = "Enable detailed billing, please verify manually"
-        scored = True
-        failReason = "Control not implemented using API, please verify manually"
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.18 Ensure IAM Master and IAM Manager roles are active (Scored)
-    def control_1_18_ensure_iam_master_and_manager_roles(self):
-        logger.info(" ---Inside iam_control_1 :: control_1_18_ensure_iam_master_and_manager_roles()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = "No IAM Master or IAM Manager role created"
-        offenders = []
-        control = "1.18"
-        description = "Ensure IAM Master and IAM Manager roles are active. Control under review/investigation"
-        scored = True
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.19 Maintain current contact details (Scored)
-    def control_1_19_maintain_current_contact_details(self):
-        logger.info(" ---Inside iam_control_1 :: control_1_19_maintain_current_contact_details()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Manual"
-        offenders = []
-        control = "1.19"
-        description = "Maintain current contact details, please verify manually"
-        scored = True
-        failReason = "Control not implemented using API, please verify manually"
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.21 Ensure IAM instance roles are used for AWS resource access from instances (Scored)
-    def control_1_21_ensure_iam_instance_roles_used(self):
-        logger.info(" ---Inside iam_control_1 :: control_1_21_ensure_iam_instance_roles_used()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-
-        control = "1.21"
-        description = "Ensure IAM instance roles are used for AWS resource access from instances, " \
-                      "application code is not audited"
-        scored = True
-        failReason = "Instance not assigned IAM role for EC2"
-        client = self.session.client('ec2', region_name='us-east-1')
-        response = client.describe_instances()
-        offenders = []
-        for n, _ in enumerate(response['Reservations']):
-            try:
-                if response['Reservations'][n]['Instances'][0]['IamInstanceProfile']:
-                    pass
-            except:
-                result = "Not Compliant"
-                offenders.append(str(response['Reservations'][n]['Instances'][0]['InstanceId']))
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.22 Ensure a support role has been created to manage incidents with AWS Support (Scored)
-    def control_1_22_ensure_incident_management_roles(self):
-        logger.info(" ---Inside iam_control_1 :: control_1_22_ensure_incident_management_roles()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        control = "1.22"
-        description = "Ensure a support role has been created to manage incidents with AWS Support"
-        scored = True
-        offenders = []
-        # global IAM_CLIENT
-        try:
-            response = self.session.client('iam').list_entities_for_policy(
-                PolicyArn='arn:aws:iam::aws:policy/AWSSupportAccess'
-            )
-            if (len(response['PolicyGroups']) + len(response['PolicyUsers']) + len(response['PolicyRoles'])) == 0:
-                result = "Not Compliant"
-                failReason = "No user, group or role assigned AWSSupportAccess"
-        except:
-            result = "Not Compliant"
-            failReason = "AWSSupportAccess policy not created"
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.23 Do not set up access keys during initial user setup for all IAM users that have a console password (Not
-    # Scored)
-    def control_1_23_no_active_initial_access_keys_with_iam_user(self, credreport):
-        logger.info(" ---Inside iam_control_1 :: control_1_23_no_active_initial_access_keys_with_iam_user()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        control = "1.23"
-        description = "Do not setup access keys during initial user setup for all IAM users that have a console " \
-                      "password"
-        scored = False
-        offenders = []
-        # global IAM_CLIENT
-        for n, _ in enumerate(credreport):
-            if (credreport[n]['access_key_1_active'] or credreport[n]['access_key_2_active'] == 'true') and n > 0:
-                try:
-                    response = self.session.client('iam').list_access_keys(UserName=str(credreport[n]['user']))
-                    for m in response['AccessKeyMetadata']:
-                        if re.sub(r"\s", "T", str(m['CreateDate'])) == credreport[n]['user_creation_time']:
-                            result = "Not Compliant"
-                            failReason = "Users with keys created at user creation time found"
-                            offenders.append(str(credreport[n]['arn']) + ":" + str(m['AccessKeyId']))
-                except botocore.exceptions.ClientError as error:
-                    if error.response['Error']['Code'] == 'NoSuchEntityException':
-                        logger.error(f" AccessKey credentails not found for user: {str(credreport[n]['user'])}")
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.24  Ensure IAM policies that allow full "*:*" administrative privileges are not created (Scored)
-    def control_1_24_no_overly_permissive_policies(self):
-        logger.info(" ---Inside iam_control_1 :: control_1_24_no_overly_permissive_policies()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "1.24"
-        description = "Ensure IAM policies that allow full administrative privileges are not created"
-        scored = True
-        offenders = []
-        # global IAM_CLIENT
-        paginator = self.session.client('iam').get_paginator('list_policies')
-        response_iterator = paginator.paginate(
-            Scope='Local',
-            OnlyAttached=False,
-        )
-        pagedResult = []
-        for page in response_iterator:
-            for n in page['Policies']:
-                pagedResult.append(n)
-        for m in pagedResult:
-            policy = self.session.client('iam').get_policy_version(
-                PolicyArn=m['Arn'],
-                VersionId=m['DefaultVersionId']
-            )
-
-            statements = []
-            # a policy may contain a single statement, a single statement in an array, or multiple statements in an
-            # array
-            if isinstance(policy['PolicyVersion']['Document']['Statement'], list):
-                for statement in policy['PolicyVersion']['Document']['Statement']:
-                    statements.append(statement)
-            else:
-                statements.append(policy['PolicyVersion']['Document']['Statement'])
-
-            for n in statements:
-                # a policy statement has to contain either an Action or a NotAction
-                if 'Action' in n.keys() and n['Effect'] == 'Allow':
-                    if ("'*'" in str(n['Action']) or str(n['Action']) == "*") and (
-                            "'*'" in str(n['Resource']) or str(n['Resource']) == "*"):
-                        result = "Not Compliant"
-                        failReason = "Found full administrative policy"
-                        offenders.append(str(m['Arn']))
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 1.25 Ensure MFA is enable to delete cloudtrail buckets
-    def control_1_25_require_mfa_to_delete_cloudtrail_buckets(self, regions: list) -> dict:
-        # returns the list trails
-        def list_trails(region) -> dict:
-            # trails_lst = []
-            trails_lst_with_bucket = {}
-            client = self.session.client('cloudtrail', region_name=region)
-
-            response = client.describe_trails(
-                trailNameList=[],
-                includeShadowTrails=False
-            )
-            for trail in response['trailList']:
-                trails_lst_with_bucket[trail['Name']] = trail['S3BucketName']
-
-            return trails_lst_with_bucket
-
-        logger.info(" ---Inside iam_control_1 :: control_1_25_require_mfa_to_delete_cloudtrail_buckets")
-
-        """Summary
-        
-        Returns:
-            TYPE: dict
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "1.25"
-        description = "Require MFA to delete cloudtrail buckets"
-        scored = True
-        for n in regions:
-            trails = list_trails(n)
-            client = self.session.client('s3')
-            for trail, bucket in trails.items():
-                try:
-                    response = client.get_bucket_versioning(
-                        Bucket=bucket
-                    )
-                    try:
-                        if response['MFADelete'] == 'Disabled':
-                            result = "Not Compliant"
-                            failReason = "Found cloudtrail s3 bucket with MFA delete disabled"
-                            offenders.append(trail)
-                    except KeyError:
-                        result = "Not Compliant"
-                        failReason = "Found cloudtrail s3 bucket with MFA delete disabled"
-                        offenders.append(trail)
-                except botocore.exceptions.ClientError as e:
-                    if e.response['Error']['Code'] == 'AccessDenied':
-                        result = "Not Compliant"
-                        failReason = "S3 access denied"
-                        offenders.append(trail)
-                    elif e.response['Error']['Code'] == 'NoSuchBucket':
-                        result = "Not Compliant"
-                        failReason = "Cloudtrail bucket {} not found".format(bucket)
-                        offenders.append(trail)
-
-        return {
-            'Result': result,
-            'failReason': failReason,
-            'Offenders': offenders,
-            'ScoredControl': scored,
-            'Description': description,
-            'ControlId': control
-        }
-
-    # 1.26 Ensure expired ssl and tls certificate are not in use
-    def control_1_26_dont_use_expired_ssl_tls_certificate(self, regions: list) -> dict:
-        logger.info(" ---Inside iam_control_1 :: control_1_26_dont_use_expired_ssl_tls_certificate")
-
-        """Summary
-        
-        Returns:
-            TYPE: dict
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "1.26"
-        description = "Don't use expired ssl/tls certificate"
-        scored = True
-
-        for region in regions:
-            client = self.session.client('acm', region_name=region)
-            marker = ''
-            while True:
-                if marker == '' or marker is None:
-                    response = client.list_certificates(
-                        CertificateStatuses=['EXPIRED']
-                    )
-                else:
-                    response = client.list_certificates(
-                        CertificateStatuses=['EXPIRED'],
-                        NextToken=marker
-                    )
-
-                for certificate in response['CertificateSummaryList']:
-                    try:
-                        if certificate['InUse']:
-                            result = "Not Compliant"
-                            failReason = "Found expired SSL/TLS certificate which is in use"
-                            offenders.append(certificate['CertificateArn'])
-                    except KeyError:
-                        pass
-
-                try:
-                    marker = response['NextToken']
-                    if marker == '':
-                        break
-                except:
-                    break
-
-        return {
-            'Result': result,
-            'failReason': failReason,
-            'Offenders': offenders,
-            'ScoredControl': scored,
-            'Description': description,
-            'ControlId': control
-        }
+    # # 1.5 Ensure IAM password policy requires at least one uppercase letter (Scored)
+    # def control_1_5_password_policy_uppercase(self, passwordpolicy):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_5_password_policy_uppercase()--- ")
+    #     """Summary
+    #
+    #     Args:
+    #         passwordpolicy (TYPE): Description
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "1.5"
+    #     description = "Ensure IAM password policy requires at least one uppercase letter"
+    #     scored = True
+    #     if passwordpolicy is False:
+    #         result = "Not Compliant"
+    #         failReason = "Account does not have a IAM password policy."
+    #     else:
+    #         if passwordpolicy['RequireUppercaseCharacters'] is False:
+    #             result = "Not Compliant"
+    #             failReason = "Password policy does not require at least one uppercase letter"
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.6 Ensure IAM password policy requires at least one lowercase letter (Scored)
+    # def control_1_6_password_policy_lowercase(self, passwordpolicy):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_6_password_policy_lowercase()--- ")
+    #     """Summary
+    #
+    #     Args:
+    #         passwordpolicy (TYPE): Description
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "1.6"
+    #     description = "Ensure IAM password policy requires at least one lowercase letter"
+    #     scored = True
+    #     if passwordpolicy is False:
+    #         result = "Not Compliant"
+    #         failReason = "Account does not have a IAM password policy."
+    #     else:
+    #         if passwordpolicy['RequireLowercaseCharacters'] is False:
+    #             result = "Not Compliant"
+    #             failReason = "Password policy does not require at least one uppercase letter"
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.7 Ensure IAM password policy requires at least one symbol (Scored)
+    # def control_1_7_password_policy_symbol(self, passwordpolicy):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_7_password_policy_symbol()--- ")
+    #     """Summary
+    #
+    #     Args:
+    #         passwordpolicy (TYPE): Description
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "1.7"
+    #     description = "Ensure IAM password policy requires at least one symbol"
+    #     scored = True
+    #     if passwordpolicy is False:
+    #         result = "Not Compliant"
+    #         failReason = "Account does not have a IAM password policy."
+    #     else:
+    #         if passwordpolicy['RequireSymbols'] is False:
+    #             result = "Not Compliant"
+    #             failReason = "Password policy does not require at least one symbol"
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.8 Ensure IAM password policy requires at least one number (Scored)
+    # def control_1_8_password_policy_number(self, passwordpolicy):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_8_password_policy_number()--- ")
+    #     """Summary
+    #
+    #     Args:
+    #         passwordpolicy (TYPE): Description
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "1.8"
+    #     description = "Ensure IAM password policy requires at least one number"
+    #     scored = True
+    #     if passwordpolicy is False:
+    #         result = "Not Compliant"
+    #         failReason = "Account does not have a IAM password policy."
+    #     else:
+    #         if passwordpolicy['RequireNumbers'] is False:
+    #             result = "Not Compliant"
+    #             failReason = "Password policy does not require at least one number"
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.11 Ensure IAM password policy expires passwords within 90 days or less (Scored)
+    # def control_1_11_password_policy_expire(self, passwordpolicy):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_11_password_policy_expire()--- ")
+    #     """Summary
+    #
+    #     Args:
+    #         passwordpolicy (TYPE): Description
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "1.11"
+    #     description = "Ensure IAM password policy expires passwords within 90 days or less"
+    #     scored = True
+    #     if passwordpolicy is False:
+    #         result = "Not Compliant"
+    #         failReason = "Account does not have a IAM password policy."
+    #     else:
+    #         if passwordpolicy['ExpirePasswords'] is True:
+    #             if 0 < passwordpolicy['MaxPasswordAge'] > 90:
+    #                 result = "Not Compliant"
+    #                 failReason = "Password policy does not expire passwords after 90 days or less"
+    #         else:
+    #             result = "Not Compliant"
+    #             failReason = "Password policy does not expire passwords after 90 days or less"
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.16 Ensure IAM policies are attached only to groups or roles (Scored)
+    # def control_1_16_no_policies_on_iam_users(self):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_16_no_policies_on_iam_users()--- ")
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "1.16"
+    #     description = "Ensure IAM policies are attached only to groups or roles"
+    #     scored = True
+    #     # global IAM_CLIENT
+    #     paginator = self.session.client('iam').get_paginator('list_users')
+    #     response_iterator = paginator.paginate()
+    #     pagedResult = []
+    #     for page in response_iterator:
+    #         for n in page['Users']:
+    #             pagedResult.append(n)
+    #     for n in pagedResult:
+    #         policies = self.session.client('iam').list_user_policies(
+    #             UserName=n['UserName'],
+    #             MaxItems=1
+    #         )
+    #         if policies['PolicyNames']:
+    #             result = "Not Compliant"
+    #             failReason = "IAM user have inline policy attached"
+    #             offenders.append(str(n['Arn']))
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.17 Enable detailed billing (Scored)
+    # def control_1_17_detailed_billing_enabled(self):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_17_detailed_billing_enabled()--- ")
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Manual"
+    #     offenders = []
+    #     control = "1.17"
+    #     description = "Enable detailed billing, please verify manually"
+    #     scored = True
+    #     failReason = "Control not implemented using API, please verify manually"
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.18 Ensure IAM Master and IAM Manager roles are active (Scored)
+    # def control_1_18_ensure_iam_master_and_manager_roles(self):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_18_ensure_iam_master_and_manager_roles()--- ")
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = "No IAM Master or IAM Manager role created"
+    #     offenders = []
+    #     control = "1.18"
+    #     description = "Ensure IAM Master and IAM Manager roles are active. Control under review/investigation"
+    #     scored = True
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.19 Maintain current contact details (Scored)
+    # def control_1_19_maintain_current_contact_details(self):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_19_maintain_current_contact_details()--- ")
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Manual"
+    #     offenders = []
+    #     control = "1.19"
+    #     description = "Maintain current contact details, please verify manually"
+    #     scored = True
+    #     failReason = "Control not implemented using API, please verify manually"
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.21 Ensure IAM instance roles are used for AWS resource access from instances (Scored)
+    # def control_1_21_ensure_iam_instance_roles_used(self):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_21_ensure_iam_instance_roles_used()--- ")
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #
+    #     control = "1.21"
+    #     description = "Ensure IAM instance roles are used for AWS resource access from instances, " \
+    #                   "application code is not audited"
+    #     scored = True
+    #     failReason = "Instance not assigned IAM role for EC2"
+    #     client = self.session.client('ec2', region_name='us-east-1')
+    #     response = client.describe_instances()
+    #     offenders = []
+    #     for n, _ in enumerate(response['Reservations']):
+    #         try:
+    #             if response['Reservations'][n]['Instances'][0]['IamInstanceProfile']:
+    #                 pass
+    #         except:
+    #             result = "Not Compliant"
+    #             offenders.append(str(response['Reservations'][n]['Instances'][0]['InstanceId']))
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.22 Ensure a support role has been created to manage incidents with AWS Support (Scored)
+    # def control_1_22_ensure_incident_management_roles(self):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_22_ensure_incident_management_roles()--- ")
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     control = "1.22"
+    #     description = "Ensure a support role has been created to manage incidents with AWS Support"
+    #     scored = True
+    #     offenders = []
+    #     # global IAM_CLIENT
+    #     try:
+    #         response = self.session.client('iam').list_entities_for_policy(
+    #             PolicyArn='arn:aws:iam::aws:policy/AWSSupportAccess'
+    #         )
+    #         if (len(response['PolicyGroups']) + len(response['PolicyUsers']) + len(response['PolicyRoles'])) == 0:
+    #             result = "Not Compliant"
+    #             failReason = "No user, group or role assigned AWSSupportAccess"
+    #     except:
+    #         result = "Not Compliant"
+    #         failReason = "AWSSupportAccess policy not created"
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.23 Do not set up access keys during initial user setup for all IAM users that have a console password (Not
+    # # Scored)
+    # def control_1_23_no_active_initial_access_keys_with_iam_user(self, credreport):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_23_no_active_initial_access_keys_with_iam_user()--- ")
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     control = "1.23"
+    #     description = "Do not setup access keys during initial user setup for all IAM users that have a console " \
+    #                   "password"
+    #     scored = False
+    #     offenders = []
+    #     # global IAM_CLIENT
+    #     for n, _ in enumerate(credreport):
+    #         if (credreport[n]['access_key_1_active'] or credreport[n]['access_key_2_active'] == 'true') and n > 0:
+    #             try:
+    #                 response = self.session.client('iam').list_access_keys(UserName=str(credreport[n]['user']))
+    #                 for m in response['AccessKeyMetadata']:
+    #                     if re.sub(r"\s", "T", str(m['CreateDate'])) == credreport[n]['user_creation_time']:
+    #                         result = "Not Compliant"
+    #                         failReason = "Users with keys created at user creation time found"
+    #                         offenders.append(str(credreport[n]['arn']) + ":" + str(m['AccessKeyId']))
+    #             except botocore.exceptions.ClientError as error:
+    #                 if error.response['Error']['Code'] == 'NoSuchEntityException':
+    #                     logger.error(f" AccessKey credentails not found for user: {str(credreport[n]['user'])}")
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.24  Ensure IAM policies that allow full "*:*" administrative privileges are not created (Scored)
+    # def control_1_24_no_overly_permissive_policies(self):
+    #     logger.info(" ---Inside iam_control_1 :: control_1_24_no_overly_permissive_policies()--- ")
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "1.24"
+    #     description = "Ensure IAM policies that allow full administrative privileges are not created"
+    #     scored = True
+    #     offenders = []
+    #     # global IAM_CLIENT
+    #     paginator = self.session.client('iam').get_paginator('list_policies')
+    #     response_iterator = paginator.paginate(
+    #         Scope='Local',
+    #         OnlyAttached=False,
+    #     )
+    #     pagedResult = []
+    #     for page in response_iterator:
+    #         for n in page['Policies']:
+    #             pagedResult.append(n)
+    #     for m in pagedResult:
+    #         policy = self.session.client('iam').get_policy_version(
+    #             PolicyArn=m['Arn'],
+    #             VersionId=m['DefaultVersionId']
+    #         )
+    #
+    #         statements = []
+    #         # a policy may contain a single statement, a single statement in an array, or multiple statements in an
+    #         # array
+    #         if isinstance(policy['PolicyVersion']['Document']['Statement'], list):
+    #             for statement in policy['PolicyVersion']['Document']['Statement']:
+    #                 statements.append(statement)
+    #         else:
+    #             statements.append(policy['PolicyVersion']['Document']['Statement'])
+    #
+    #         for n in statements:
+    #             # a policy statement has to contain either an Action or a NotAction
+    #             if 'Action' in n.keys() and n['Effect'] == 'Allow':
+    #                 if ("'*'" in str(n['Action']) or str(n['Action']) == "*") and (
+    #                         "'*'" in str(n['Resource']) or str(n['Resource']) == "*"):
+    #                     result = "Not Compliant"
+    #                     failReason = "Found full administrative policy"
+    #                     offenders.append(str(m['Arn']))
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 1.25 Ensure MFA is enable to delete cloudtrail buckets
+    # def control_1_25_require_mfa_to_delete_cloudtrail_buckets(self, regions: list) -> dict:
+    #     # returns the list trails
+    #     def list_trails(region) -> dict:
+    #         # trails_lst = []
+    #         trails_lst_with_bucket = {}
+    #         client = self.session.client('cloudtrail', region_name=region)
+    #
+    #         response = client.describe_trails(
+    #             trailNameList=[],
+    #             includeShadowTrails=False
+    #         )
+    #         for trail in response['trailList']:
+    #             trails_lst_with_bucket[trail['Name']] = trail['S3BucketName']
+    #
+    #         return trails_lst_with_bucket
+    #
+    #     logger.info(" ---Inside iam_control_1 :: control_1_25_require_mfa_to_delete_cloudtrail_buckets")
+    #
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: dict
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "1.25"
+    #     description = "Require MFA to delete cloudtrail buckets"
+    #     scored = True
+    #     for n in regions:
+    #         trails = list_trails(n)
+    #         client = self.session.client('s3')
+    #         for trail, bucket in trails.items():
+    #             try:
+    #                 response = client.get_bucket_versioning(
+    #                     Bucket=bucket
+    #                 )
+    #                 try:
+    #                     if response['MFADelete'] == 'Disabled':
+    #                         result = "Not Compliant"
+    #                         failReason = "Found cloudtrail s3 bucket with MFA delete disabled"
+    #                         offenders.append(trail)
+    #                 except KeyError:
+    #                     result = "Not Compliant"
+    #                     failReason = "Found cloudtrail s3 bucket with MFA delete disabled"
+    #                     offenders.append(trail)
+    #             except botocore.exceptions.ClientError as e:
+    #                 if e.response['Error']['Code'] == 'AccessDenied':
+    #                     result = "Not Compliant"
+    #                     failReason = "S3 access denied"
+    #                     offenders.append(trail)
+    #                 elif e.response['Error']['Code'] == 'NoSuchBucket':
+    #                     result = "Not Compliant"
+    #                     failReason = "Cloudtrail bucket {} not found".format(bucket)
+    #                     offenders.append(trail)
+    #
+    #     return {
+    #         'Result': result,
+    #         'failReason': failReason,
+    #         'Offenders': offenders,
+    #         'ScoredControl': scored,
+    #         'Description': description,
+    #         'ControlId': control
+    #     }
+    #
+    # # 1.26 Ensure expired ssl and tls certificate are not in use
+    # def control_1_26_dont_use_expired_ssl_tls_certificate(self, regions: list) -> dict:
+    #     logger.info(" ---Inside iam_control_1 :: control_1_26_dont_use_expired_ssl_tls_certificate")
+    #
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: dict
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "1.26"
+    #     description = "Don't use expired ssl/tls certificate"
+    #     scored = True
+    #
+    #     for region in regions:
+    #         client = self.session.client('acm', region_name=region)
+    #         marker = ''
+    #         while True:
+    #             if marker == '' or marker is None:
+    #                 response = client.list_certificates(
+    #                     CertificateStatuses=['EXPIRED']
+    #                 )
+    #             else:
+    #                 response = client.list_certificates(
+    #                     CertificateStatuses=['EXPIRED'],
+    #                     NextToken=marker
+    #                 )
+    #
+    #             for certificate in response['CertificateSummaryList']:
+    #                 try:
+    #                     if certificate['InUse']:
+    #                         result = "Not Compliant"
+    #                         failReason = "Found expired SSL/TLS certificate which is in use"
+    #                         offenders.append(certificate['CertificateArn'])
+    #                 except KeyError:
+    #                     pass
+    #
+    #             try:
+    #                 marker = response['NextToken']
+    #                 if marker == '':
+    #                     break
+    #             except:
+    #                 break
+    #
+    #     return {
+    #         'Result': result,
+    #         'failReason': failReason,
+    #         'Offenders': offenders,
+    #         'ScoredControl': scored,
+    #         'Description': description,
+    #         'ControlId': control
+    #     }
```

### Comparing `cis_checks_2023-2.0.2/cis_checks_2023/logging_control_3.py` & `cis_checks_2023-2.0.3/cis_checks_2023/logging_control_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,28 +433,30 @@
                 for n in page['Trails']:
                     pagedResult.append(n)
 
             for n in pagedResult:
                 event_selectors = self.session.client('cloudtrail', region_name=region).get_event_selectors(
                     TrailName=n['Name']
                 )
-
-                if 'EventSelectors' in event_selectors:
-                    for i in event_selectors["EventSelectors"]:
-                        if not i["DataResources"]:
-                            result = 'Not Compliant'
-                            failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
-                            offenders.append(event_selectors['TrailARN'])
-                        else:
-                            continue
-                else:
-                    result = 'Not Compliant'
-                    failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
-                    offenders.append(event_selectors['TrailARN'])
-
+                #print(event_selectors)
+                try:
+                    if 'EventSelectors' in event_selectors:
+                        for i in event_selectors["EventSelectors"]:
+                            if i["DataResources"] == []:
+                                result = 'Not Compliant'
+                                failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
+                                offenders.append(event_selectors['TrailARN'])
+                            else:
+                                continue
+                    else:
+                        result = 'Not Compliant'
+                        failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
+                        offenders.append(event_selectors['TrailARN'])
+                except:
+                    KeyError
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.11 Ensure that Object-level logging for read events is enabled for S3 bucket
 
     def control_3_1_1_ensure_logging_enabled_for_s3_read(self, regions):
         logger.info(" ---Inside networking_control_3 :: control_3_1_1_ensure_logging_enabled_for_s3_read()--- ")
@@ -477,23 +479,25 @@
                 for n in page['Trails']:
                     pagedResult.append(n)
 
             for n in pagedResult:
                 event_selectors = self.session.client('cloudtrail', region_name=region).get_event_selectors(
                     TrailName=n['Name']
                 )
+                try:
 
-                if 'EventSelectors' in event_selectors:
-                    for i in event_selectors["EventSelectors"]:
-                        if not i["DataResources"]:
-                            result = 'Not Compliant'
-                            failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
-                            offenders.append(event_selectors['TrailARN'])
-                        else:
-                            continue
-                else:
-                    result = 'Not Compliant'
-                    failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
-                    offenders.append(event_selectors['TrailARN'])
-
+                    if 'EventSelectors' in event_selectors:
+                        for i in event_selectors["EventSelectors"]:
+                            if i["DataResources"] == []:
+                                result = 'Not Compliant'
+                                failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
+                                offenders.append(event_selectors['TrailARN'])
+                            else:
+                                continue
+                    else:
+                        result = 'Not Compliant'
+                        failReason = 'Object-level logging for read/write events is not enabled for S3 bucket'
+                        offenders.append(event_selectors['TrailARN'])
+                except:
+                    KeyError
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
```

### Comparing `cis_checks_2023-2.0.2/cis_checks_2023/monitoring_control_4.py` & `cis_checks_2023-2.0.3/cis_checks_2023/monitoring_control_4.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.2/cis_checks_2023/networking_control_5.py` & `cis_checks_2023-2.0.3/cis_checks_2023/networking_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.2/cis_checks_2023/storage_control_2.py` & `cis_checks_2023-2.0.3/cis_checks_2023/storage_control_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
         offenders = []
-        control = "2.1.2"
+        control = "2.1.3"
         description = "Ensure MFA Delete is enabled on S3 buckets"
         scored = True
 
         client = self.session.client('s3')
         response = client.list_buckets()
 
         for bucket in response['Buckets']:
```

### Comparing `cis_checks_2023-2.0.2/cis_checks_2023/utils.py` & `cis_checks_2023-2.0.3/cis_checks_2023/utils.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.2/cis_checks_2023.egg-info/PKG-INFO` & `cis_checks_2023-2.0.3/cis_checks_2023.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cis-checks-2023
-Version: 2.0.2
+Version: 2.0.3
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.2/pyproject.toml` & `cis_checks_2023-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "cis_checks_2023"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name="Dheeraj Banodha", email="dheeraj.banodha@impetus.com" },
   { name="Ravish Sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

