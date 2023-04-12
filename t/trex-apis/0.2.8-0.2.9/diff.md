# Comparing `tmp/trex-apis-0.2.8.tar.gz` & `tmp/trex-apis-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-0.2.8.tar", last modified: Mon Feb 27 05:28:15 2023, max compression
+gzip compressed data, was "trex-apis-0.2.9.tar", last modified: Fri Mar  3 04:50:47 2023, max compression
```

## Comparing `trex-apis-0.2.8.tar` & `trex-apis-0.2.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-27 05:28:15.328812 trex-apis-0.2.8/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-02-27 05:28:15.329007 trex-apis-0.2.8/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-0.2.8/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-02-27 05:28:15.329717 trex-apis-0.2.8/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-02-27 05:26:30.000000 trex-apis-0.2.8/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-27 05:28:15.309160 trex-apis-0.2.8/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-02-27 05:28:15.000000 trex-apis-0.2.8/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1110 2023-02-27 05:28:15.000000 trex-apis-0.2.8/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-02-27 05:28:15.000000 trex-apis-0.2.8/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-02-27 05:28:15.000000 trex-apis-0.2.8/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-02-27 05:28:15.000000 trex-apis-0.2.8/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-27 05:28:15.309831 trex-apis-0.2.8/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-0.2.8/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      728 2023-01-03 04:03:16.000000 trex-apis-0.2.8/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-27 05:28:15.321571 trex-apis-0.2.8/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-0.2.8/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7390 2023-01-25 07:12:41.000000 trex-apis-0.2.8/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-0.2.8/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    31457 2023-02-26 09:27:48.000000 trex-apis-0.2.8/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-0.2.8/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8300 2023-01-13 04:35:13.000000 trex-apis-0.2.8/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    10939 2023-02-24 02:08:38.000000 trex-apis-0.2.8/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-0.2.8/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-0.2.8/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27309 2023-02-22 08:31:07.000000 trex-apis-0.2.8/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36302 2023-01-30 04:44:34.000000 trex-apis-0.2.8/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-0.2.8/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14802 2023-02-27 02:58:10.000000 trex-apis-0.2.8/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-27 05:28:15.322528 trex-apis-0.2.8/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-0.2.8/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4454 2023-01-18 15:02:20.000000 trex-apis-0.2.8/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-27 05:28:15.324964 trex-apis-0.2.8/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-0.2.8/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-0.2.8/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7220 2023-02-20 04:25:05.000000 trex-apis-0.2.8/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3344 2023-01-18 01:16:56.000000 trex-apis-0.2.8/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-27 05:28:15.325985 trex-apis-0.2.8/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-0.2.8/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-0.2.8/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-02-27 05:28:15.327643 trex-apis-0.2.8/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-0.2.8/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-0.2.8/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    61188 2023-02-27 03:03:26.000000 trex-apis-0.2.8/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.898113 trex-apis-0.2.9/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-03-03 04:50:47.898234 trex-apis-0.2.9/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-0.2.9/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-03-03 04:50:47.898656 trex-apis-0.2.9/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-03-03 04:45:38.000000 trex-apis-0.2.9/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.881320 trex-apis-0.2.9/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-03-03 04:50:47.000000 trex-apis-0.2.9/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1110 2023-03-03 04:50:47.000000 trex-apis-0.2.9/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-03-03 04:50:47.000000 trex-apis-0.2.9/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-03-03 04:50:47.000000 trex-apis-0.2.9/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-03-03 04:50:47.000000 trex-apis-0.2.9/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.882144 trex-apis-0.2.9/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-0.2.9/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      728 2023-01-03 04:03:16.000000 trex-apis-0.2.9/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.892379 trex-apis-0.2.9/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-0.2.9/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7390 2023-01-25 07:12:41.000000 trex-apis-0.2.9/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-0.2.9/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    31457 2023-02-26 09:27:48.000000 trex-apis-0.2.9/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-0.2.9/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8300 2023-01-13 04:35:13.000000 trex-apis-0.2.9/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    10939 2023-02-24 02:08:38.000000 trex-apis-0.2.9/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-0.2.9/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-0.2.9/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27309 2023-02-22 08:31:07.000000 trex-apis-0.2.9/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36302 2023-01-30 04:44:34.000000 trex-apis-0.2.9/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-0.2.9/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14802 2023-02-27 02:58:10.000000 trex-apis-0.2.9/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.893265 trex-apis-0.2.9/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-0.2.9/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4454 2023-01-18 15:02:20.000000 trex-apis-0.2.9/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.895073 trex-apis-0.2.9/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-0.2.9/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-0.2.9/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7220 2023-02-20 04:25:05.000000 trex-apis-0.2.9/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3344 2023-01-18 01:16:56.000000 trex-apis-0.2.9/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.895877 trex-apis-0.2.9/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-0.2.9/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-0.2.9/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-03-03 04:50:47.897144 trex-apis-0.2.9/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-0.2.9/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-0.2.9/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    61210 2023-03-03 04:45:00.000000 trex-apis-0.2.9/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-0.2.8/setup.py` & `trex-apis-0.2.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='0.2.8',
+     version='0.2.9',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-0.2.8/trex_apis.egg-info/SOURCES.txt` & `trex-apis-0.2.9/trex_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/conf.py` & `trex-apis-0.2.9/trexapi/conf.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/app_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/app_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/customer_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/customer_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/loyalty_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/outlet_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/outlet_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/payment_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/pos_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/reward_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/user_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/user_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/controllers/voucher_api_routes.py` & `trex-apis-0.2.9/trexapi/controllers/voucher_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/decorators/api_decorators.py` & `trex-apis-0.2.9/trexapi/decorators/api_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/forms/customer_api_forms.py` & `trex-apis-0.2.9/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/forms/reward_api_forms.py` & `trex-apis-0.2.9/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/forms/user_api_forms.py` & `trex-apis-0.2.9/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-0.2.9/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/utils/api_helpers.py` & `trex-apis-0.2.9/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-0.2.8/trexapi/utils/reward_transaction_helper.py` & `trex-apis-0.2.9/trexapi/utils/reward_transaction_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1090,22 +1090,22 @@
                     key: "ag50cmV4LWFkbWluLWRldnJGCxIEVXNlchiAgIC4y6nFCAwLEghDdXN0b21lchiAgICE3I-JCQwLEhNDdXN0b21lclN0YW1wUmV3YXJkGICAgNjfrZAJDA",
                     redeemed_amount: 2
                     }
                 ]
             }
         },
         '''
-        redeemed_details_list   = redeemed_summary.get(conf.REWARD_TYPE_STAMP).get('customer_stamp_rewards')
+        redeemed_details_list   = redeemed_summary.get(program_conf.REWARD_FORMAT_STAMP).get('customer_stamp_rewards')
         
         for redeemed_details in redeemed_details_list:
             customer_stamp_reward = CustomerStampReward.fetch(redeemed_details.get('key'))
             redeemed_amount = redeemed_details.get('amount')
             customer_stamp_reward.update_used_reward_amount( -redeemed_amount )
             
-            customer.reward_summary[conf.REWARD_TYPE_STAMP]['amount'] += redeemed_amount
+            customer.reward_summary[program_conf.REWARD_FORMAT_STAMP]['amount'] += redeemed_amount
         
         customer.put()
         
     if program_conf.REWARD_FORMAT_PREPAID in redeemed_summary.keys(): 
         #found voucher have been redeem in the transaction
         '''
         Example of prepaid redeemed_summary
@@ -1117,15 +1117,15 @@
                     key: "ag50cmV4LWFkbWluLWRldnJICxIEVXNlchiAgIC4y6nFCAwLEghDdXN0b21lchiAgICE3I-JCQwLEhVDdXN0b21lclByZXBhaWRSZXdhcmQYgICAmP-6lAoM",
                     redeemed_amount: 25,
                     }
                 ]
             }
         },
         '''
-        redeemed_details_list   = redeemed_summary.get(program_conf.REWARD_TYPE_PREPAID).get('customer_prepaid_rewards')
+        redeemed_details_list   = redeemed_summary.get(program_conf.REWARD_FORMAT_PREPAID).get('customer_prepaid_rewards')
         
         for redeemed_details in redeemed_details_list:
             customer_prepaid_reward = CustomerPrepaidReward.fetch(redeemed_details.get('key'))
             if customer_prepaid_reward:
                 redeemed_amount = redeemed_details.get('amount')
                 customer_prepaid_reward.update_used_reward_amount( -redeemed_amount )
```

