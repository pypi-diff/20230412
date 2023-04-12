# Comparing `tmp/getsmarter-api-clients-0.4.0.tar.gz` & `tmp/getsmarter-api-clients-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getsmarter-api-clients-0.4.0.tar", last modified: Thu Sep 15 16:50:15 2022, max compression
+gzip compressed data, was "getsmarter-api-clients-0.5.0.tar", last modified: Wed Apr 12 07:52:01 2023, max compression
```

## Comparing `getsmarter-api-clients-0.4.0.tar` & `getsmarter-api-clients-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:50:15.654910 getsmarter-api-clients-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-09-15 16:50:11.000000 getsmarter-api-clients-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35139 2022-09-15 16:50:11.000000 getsmarter-api-clients-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-09-15 16:50:11.000000 getsmarter-api-clients-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2022-09-15 16:50:15.654910 getsmarter-api-clients-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4599 2022-09-15 16:50:11.000000 getsmarter-api-clients-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:50:15.650910 getsmarter-api-clients-0.4.0/getsmarter_api_clients/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-15 16:50:11.000000 getsmarter-api-clients-0.4.0/getsmarter_api_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9378 2022-09-15 16:50:11.000000 getsmarter-api-clients-0.4.0/getsmarter_api_clients/geag.py
--rw-r--r--   0 runner    (1001) docker     (121)     3184 2022-09-15 16:50:11.000000 getsmarter-api-clients-0.4.0/getsmarter_api_clients/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:50:15.650910 getsmarter-api-clients-0.4.0/getsmarter_api_clients.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2022-09-15 16:50:15.000000 getsmarter-api-clients-0.4.0/getsmarter_api_clients.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-15 16:50:15.000000 getsmarter-api-clients-0.4.0/getsmarter_api_clients.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 16:50:15.000000 getsmarter-api-clients-0.4.0/getsmarter_api_clients.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 16:50:15.000000 getsmarter-api-clients-0.4.0/getsmarter_api_clients.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-15 16:50:15.000000 getsmarter-api-clients-0.4.0/getsmarter_api_clients.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-15 16:50:15.000000 getsmarter-api-clients-0.4.0/getsmarter_api_clients.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 16:50:15.654910 getsmarter-api-clients-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-09-15 16:50:11.000000 getsmarter-api-clients-0.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-09-15 16:50:11.000000 getsmarter-api-clients-0.4.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-09-15 16:50:15.654910 getsmarter-api-clients-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     4952 2022-09-15 16:50:11.000000 getsmarter-api-clients-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 07:52:01.888938 getsmarter-api-clients-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-04-12 07:51:55.000000 getsmarter-api-clients-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-12 07:51:55.000000 getsmarter-api-clients-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-04-12 07:51:55.000000 getsmarter-api-clients-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-04-12 07:52:01.888938 getsmarter-api-clients-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-04-12 07:51:55.000000 getsmarter-api-clients-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 07:52:01.888938 getsmarter-api-clients-0.5.0/getsmarter_api_clients/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-12 07:51:55.000000 getsmarter-api-clients-0.5.0/getsmarter_api_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9532 2023-04-12 07:51:55.000000 getsmarter-api-clients-0.5.0/getsmarter_api_clients/geag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-04-12 07:51:55.000000 getsmarter-api-clients-0.5.0/getsmarter_api_clients/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 07:52:01.888938 getsmarter-api-clients-0.5.0/getsmarter_api_clients.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-04-12 07:52:01.000000 getsmarter-api-clients-0.5.0/getsmarter_api_clients.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-04-12 07:52:01.000000 getsmarter-api-clients-0.5.0/getsmarter_api_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 07:52:01.000000 getsmarter-api-clients-0.5.0/getsmarter_api_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 07:52:01.000000 getsmarter-api-clients-0.5.0/getsmarter_api_clients.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-12 07:52:01.000000 getsmarter-api-clients-0.5.0/getsmarter_api_clients.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-12 07:52:01.000000 getsmarter-api-clients-0.5.0/getsmarter_api_clients.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 07:52:01.888938 getsmarter-api-clients-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-04-12 07:51:55.000000 getsmarter-api-clients-0.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-12 07:51:55.000000 getsmarter-api-clients-0.5.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-12 07:52:01.888938 getsmarter-api-clients-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4952 2023-04-12 07:51:55.000000 getsmarter-api-clients-0.5.0/setup.py
```

### Comparing `getsmarter-api-clients-0.4.0/CHANGELOG.rst` & `getsmarter-api-clients-0.5.0/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[0.5.0] - 2023-04-12
+~~~~~~~~~~~~~~~~~~~~
+
+* Added new field for data_share_consent in enterprise_allocations
+
 [0.4.0] - 2022-09-12
 ~~~~~~~~~~~~~~~~~~~~
 
 * Add enterprise_allocations endpoint functionality to client
 
 [0.1.0] - 2022-08-01
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `getsmarter-api-clients-0.4.0/LICENSE.txt` & `getsmarter-api-clients-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.4.0/PKG-INFO` & `getsmarter-api-clients-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsmarter-api-clients
-Version: 0.4.0
+Version: 0.5.0
 Summary: Clients to interact with GetSmarter APIs.
 Home-page: https://github.com/edx/getsmarter-api-clients
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -169,14 +169,19 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[0.5.0] - 2023-04-12
+~~~~~~~~~~~~~~~~~~~~
+
+* Added new field for data_share_consent in enterprise_allocations
+
 [0.4.0] - 2022-09-12
 ~~~~~~~~~~~~~~~~~~~~
 
 * Add enterprise_allocations endpoint functionality to client
 
 [0.1.0] - 2022-08-01
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `getsmarter-api-clients-0.4.0/README.rst` & `getsmarter-api-clients-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.4.0/getsmarter_api_clients/geag.py` & `getsmarter-api-clients-0.5.0/getsmarter_api_clients/geag.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         payment_reference,
         enterprise_customer_uuid,
         first_name,
         last_name,
         email,
         date_of_birth,
         terms_accepted_at,
+        data_share_consent,
         currency,
         order_items,
         address_line1=None,
         address_line2=None,
         city=None,
         postal_code=None,
         state=None,
@@ -179,14 +180,15 @@
              to identify which enterprise customer the order was placed for
           - `first_name (str)`: First name
           - `last_name (str)`: Last name
           - `email (str)`: Email
           - `date_of_birth (str)`: Date of birth
           - `terms_accepted_at (str)`: ISO 8601 timestamp of
             when the terms and policies were accepted
+          - `data_share_consent (bool)`: Learner consent for data sharing
           - `currency (str)`: One of ['USD', 'GBP', 'ZAR', 'EUR', 'AED',
             'SGD', 'HKD', 'SAR', 'INR', 'CAD']
           - `order_items (list of dict)`: Items ordered
           - `address_line1 (str)`: Address Line 1
           - `address_line2 (str)`: Adress Line 2
           - `city (str)`: City
           - `postal_code (str)`: Postal code
@@ -226,14 +228,15 @@
             'paymentReference': payment_reference,
             'enterpriseCustomerUuid': enterprise_customer_uuid,
             'firstName': first_name,
             'lastName': last_name,
             'email': email,
             'dateOfBirth': date_of_birth,
             'termsAcceptedAt': terms_accepted_at,
+            'dataShareConsent': data_share_consent,
             'currency': currency,
             'orderItems': order_items,
             # optional fields
             'addressLine1': address_line1,
             'addressLine2': address_line2,
             'city': city,
             'postalCode': postal_code,
```

### Comparing `getsmarter-api-clients-0.4.0/getsmarter_api_clients/oauth.py` & `getsmarter-api-clients-0.5.0/getsmarter_api_clients/oauth.py`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.4.0/getsmarter_api_clients.egg-info/PKG-INFO` & `getsmarter-api-clients-0.5.0/getsmarter_api_clients.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsmarter-api-clients
-Version: 0.4.0
+Version: 0.5.0
 Summary: Clients to interact with GetSmarter APIs.
 Home-page: https://github.com/edx/getsmarter-api-clients
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -169,14 +169,19 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[0.5.0] - 2023-04-12
+~~~~~~~~~~~~~~~~~~~~
+
+* Added new field for data_share_consent in enterprise_allocations
+
 [0.4.0] - 2022-09-12
 ~~~~~~~~~~~~~~~~~~~~
 
 * Add enterprise_allocations endpoint functionality to client
 
 [0.1.0] - 2022-08-01
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `getsmarter-api-clients-0.4.0/requirements/constraints.txt` & `getsmarter-api-clients-0.5.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `getsmarter-api-clients-0.4.0/setup.py` & `getsmarter-api-clients-0.5.0/setup.py`

 * *Files identical despite different names*

