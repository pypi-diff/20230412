# Comparing `tmp/python-mcs-sdk-0.2.12.tar.gz` & `tmp/python-mcs-sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mcs-sdk-0.2.12.tar", last modified: Thu Mar  9 00:30:19 2023, max compression
+gzip compressed data, was "python-mcs-sdk-0.3.0.tar", last modified: Wed Apr 12 15:25:57 2023, max compression
```

## Comparing `python-mcs-sdk-0.2.12.tar` & `python-mcs-sdk-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,64 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-09 00:30:19.386448 python-mcs-sdk-0.2.12/
--rw-r--r--   0 daniel     (501) staff       (20)     1064 2022-07-01 06:58:03.000000 python-mcs-sdk-0.2.12/LICENSE
--rw-r--r--   0 daniel     (501) staff       (20)       31 2022-08-10 05:11:25.000000 python-mcs-sdk-0.2.12/MANIFEST.in
--rw-r--r--   0 daniel     (501) staff       (20)     1815 2023-03-09 00:30:19.386336 python-mcs-sdk-0.2.12/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)     3881 2023-02-01 21:22:37.000000 python-mcs-sdk-0.2.12/README.md
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-09 00:30:19.381611 python-mcs-sdk-0.2.12/mcs/
--rw-r--r--   0 daniel     (501) staff       (20)       97 2023-03-07 21:01:28.000000 python-mcs-sdk-0.2.12/mcs/__init__.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-09 00:30:19.382290 python-mcs-sdk-0.2.12/mcs/api/
--rw-r--r--   0 daniel     (501) staff       (20)       84 2023-01-23 15:15:38.000000 python-mcs-sdk-0.2.12/mcs/api/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    13992 2023-03-09 00:00:47.000000 python-mcs-sdk-0.2.12/mcs/api/bucket_api.py
--rw-r--r--   0 daniel     (501) staff       (20)    11250 2023-03-08 23:59:52.000000 python-mcs-sdk-0.2.12/mcs/api/onchain_api.py
--rw-r--r--   0 daniel     (501) staff       (20)     6332 2023-03-08 23:59:52.000000 python-mcs-sdk-0.2.12/mcs/api_client.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-09 00:30:19.383234 python-mcs-sdk-0.2.12/mcs/common/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2022-07-01 07:09:06.000000 python-mcs-sdk-0.2.12/mcs/common/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1620 2023-03-09 00:04:34.000000 python-mcs-sdk-0.2.12/mcs/common/constants.py
--rw-r--r--   0 daniel     (501) staff       (20)     1284 2022-07-01 09:17:05.000000 python-mcs-sdk-0.2.12/mcs/common/exceptions.py
--rw-r--r--   0 daniel     (501) staff       (20)      880 2023-01-23 15:15:38.000000 python-mcs-sdk-0.2.12/mcs/common/params.py
--rw-r--r--   0 daniel     (501) staff       (20)     1185 2023-03-08 23:59:52.000000 python-mcs-sdk-0.2.12/mcs/common/utils.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-09 00:30:19.383427 python-mcs-sdk-0.2.12/mcs/contract/
--rw-r--r--   0 daniel     (501) staff       (20)       53 2023-01-23 15:15:38.000000 python-mcs-sdk-0.2.12/mcs/contract/__init__.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-09 00:30:19.384100 python-mcs-sdk-0.2.12/mcs/contract/abi/
--rw-r--r--   0 daniel     (501) staff       (20)     4860 2023-03-07 21:01:28.000000 python-mcs-sdk-0.2.12/mcs/contract/abi/CollectionFactory.json
--rw-r--r--   0 daniel     (501) staff       (20)     5704 2022-06-11 13:28:00.000000 python-mcs-sdk-0.2.12/mcs/contract/abi/ERC20.json
--rw-r--r--   0 daniel     (501) staff       (20)     1276 2022-06-11 13:28:00.000000 python-mcs-sdk-0.2.12/mcs/contract/abi/SwanPayment.json
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-09 00:30:19.384568 python-mcs-sdk-0.2.12/mcs/object/
--rw-r--r--   0 daniel     (501) staff       (20)     1850 2023-03-09 00:03:04.000000 python-mcs-sdk-0.2.12/mcs/object/bucket_storage.py
--rw-r--r--   0 daniel     (501) staff       (20)     4597 2023-03-07 21:01:28.000000 python-mcs-sdk-0.2.12/mcs/object/onchain_storage.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-09 00:30:19.385162 python-mcs-sdk-0.2.12/python_mcs_sdk.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)     1815 2023-03-09 00:30:19.000000 python-mcs-sdk-0.2.12/python_mcs_sdk.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      732 2023-03-09 00:30:19.000000 python-mcs-sdk-0.2.12/python_mcs_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-03-09 00:30:19.000000 python-mcs-sdk-0.2.12/python_mcs_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       69 2023-03-09 00:30:19.000000 python-mcs-sdk-0.2.12/python_mcs_sdk.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        4 2023-03-09 00:30:19.000000 python-mcs-sdk-0.2.12/python_mcs_sdk.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-03-09 00:30:19.386483 python-mcs-sdk-0.2.12/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      732 2023-03-09 00:30:15.000000 python-mcs-sdk-0.2.12/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-03-09 00:30:19.386045 python-mcs-sdk-0.2.12/test/
--rw-r--r--   0 daniel     (501) staff       (20)     2121 2023-03-08 23:59:52.000000 python-mcs-sdk-0.2.12/test/test_bucket_api.py
--rw-r--r--   0 daniel     (501) staff       (20)     1697 2023-03-08 23:59:52.000000 python-mcs-sdk-0.2.12/test/test_onchain_api.py
--rw-r--r--   0 daniel     (501) staff       (20)      482 2023-02-10 18:43:03.000000 python-mcs-sdk-0.2.12/test/test_point.py
--rw-r--r--   0 daniel     (501) staff       (20)        0 2022-10-09 10:25:58.000000 python-mcs-sdk-0.2.12/test/test_upload.py
--rw-r--r--   0 daniel     (501) staff       (20)      153 2023-02-01 21:00:37.000000 python-mcs-sdk-0.2.12/test/test_utils.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.455010 python-mcs-sdk-0.3.0/
+-rw-r--r--   0 daniel     (501) staff       (20)     1064 2022-07-01 06:58:03.000000 python-mcs-sdk-0.3.0/LICENSE
+-rw-r--r--   0 daniel     (501) staff       (20)       31 2022-08-10 05:11:25.000000 python-mcs-sdk-0.3.0/MANIFEST.in
+-rw-r--r--   0 daniel     (501) staff       (20)     1677 2023-04-12 15:25:57.454860 python-mcs-sdk-0.3.0/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     3896 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.447331 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     1677 2023-04-12 15:25:57.000000 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     1599 2023-04-12 15:25:57.000000 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-04-12 15:25:57.000000 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       69 2023-04-12 15:25:57.000000 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        9 2023-04-12 15:25:57.000000 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-04-12 15:25:57.455060 python-mcs-sdk-0.3.0/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      878 2023-04-12 15:25:40.000000 python-mcs-sdk-0.3.0/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.447543 python-mcs-sdk-0.3.0/swan_mcs/
+-rw-r--r--   0 daniel     (501) staff       (20)      230 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.0/swan_mcs/__init__.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.447861 python-mcs-sdk-0.3.0/swan_mcs/api/
+-rw-r--r--   0 daniel     (501) staff       (20)       94 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.0/swan_mcs/api/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    18026 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.0/swan_mcs/api/bucket_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)    11270 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.0/swan_mcs/api/onchain_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6443 2023-04-11 16:14:34.000000 python-mcs-sdk-0.3.0/swan_mcs/api_client.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.448325 python-mcs-sdk-0.3.0/swan_mcs/common/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2022-07-01 07:09:06.000000 python-mcs-sdk-0.3.0/swan_mcs/common/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1639 2023-04-11 15:42:48.000000 python-mcs-sdk-0.3.0/swan_mcs/common/constants.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1289 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/swan_mcs/common/exceptions.py
+-rw-r--r--   0 daniel     (501) staff       (20)      923 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.0/swan_mcs/common/params.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1190 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.0/swan_mcs/common/utils.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.448426 python-mcs-sdk-0.3.0/swan_mcs/contract/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-04-11 14:55:17.000000 python-mcs-sdk-0.3.0/swan_mcs/contract/__init__.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.448603 python-mcs-sdk-0.3.0/swan_mcs/object/
+-rw-r--r--   0 daniel     (501) staff       (20)     1850 2023-03-09 00:03:04.000000 python-mcs-sdk-0.3.0/swan_mcs/object/bucket_storage.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4597 2023-03-07 21:01:28.000000 python-mcs-sdk-0.3.0/swan_mcs/object/onchain_storage.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.454616 python-mcs-sdk-0.3.0/test/
+-rw-r--r--   0 daniel     (501) staff       (20)     2545 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_bucket_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2082 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_api_key_login.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1489 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_create_bucket_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2432 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_create_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1534 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_delete_bucket.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1636 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_delete_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2884 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_mock_download_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2942 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_mock_download_ipfs_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2325 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_get_bucket.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1291 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_get_bucket_list.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1975 2023-04-11 15:06:12.000000 python-mcs-sdk-0.3.0/test/test_mock_get_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)      698 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_get_gateway.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1233 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_mock_list_files.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4451 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_upload_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3185 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.0/test/test_mock_upload_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2272 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_mock_upload_ipfs_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1955 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_onchain_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1266 2023-04-11 16:14:34.000000 python-mcs-sdk-0.3.0/test/test_real_api_key_login.py
+-rw-r--r--   0 daniel     (501) staff       (20)      979 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_create_bucket_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1219 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_create_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1041 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_delete_bucket.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1300 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_delete_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1889 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_download_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1853 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.0/test/test_real_download_ipfs_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1685 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_get_bucket.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1186 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_get_bucket_list.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1335 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_real_get_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)      179 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_get_gateway.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2258 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_list_files.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2097 2023-04-11 17:28:02.000000 python-mcs-sdk-0.3.0/test/test_real_upload_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1864 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_upload_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2627 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.0/test/test_real_upload_ipfs_folder.py
```

### Comparing `python-mcs-sdk-0.2.12/LICENSE` & `python-mcs-sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.2.12/PKG-INFO` & `python-mcs-sdk-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: python-mcs-sdk
-Version: 0.2.12
+Version: 0.3.0
 Summary: A python software development kit for the Multi-Chain Storage
 Author: daniel8088
 Author-email: danilew8088@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Made by FilSwan](https://img.shields.io/badge/made%20by-FilSwan-green.svg)](https://www.filswan.com/) [![Chat on discord](https://img.shields.io/badge/join%20-discord-brightgreen.svg)](https://discord.com/invite/KKGhy8ZqzK)
 
 Python-MCS-SDK is a python software development kit for the [Multi-Chain Storage(MCS)](https://www.multichain.storage) service. It provides a convenient interface for working with the MCS API.
 
 Please take a look at our documentation for how to install and use Python-MCS-SDK:
-
-- [Prerequisites](https://docs.filswan.com/multichain.storage/developer-quickstart/sdk/python-mcs-sdk/prerequisite)
-- [Get Started](https://docs.filswan.com/multichain.storage/developer-quickstart/sdk/python-mcs-sdk/get-started)
+- [Get Started](https://docs.filswan.com/multichain.storage/developer-quickstart/sdk/python-mcs-sdk/quickstart)
 
 If you find bugs, need help, or want to talk to the developers, please use our mailing lists or chat rooms:
 
 - [Discord channel](https://discord.com/invite/KKGhy8ZqzK)
 - [Issue tracking](https://github.com/filswan/python-mcs-sdk/issues)
 
 If you want to get involved, head over to GitHub to get the source code, look at our developer documentation and feel free to jump on the developer mailing lists and chat rooms:
 
 - [GitHub Page](https://github.com/filswan/python-mcs-sdk)
 - [Development documentation](https://docs.filswan.com/multichain.storage/developer-quickstart/sdk/python-mcs-sdk)
 
 ## Code of Conduct
 
 Everyone interacting in the pip project’s codebases, issue trackers, chat rooms, and mailing lists is expected to follow the [PSF Code of Conduct](https://www.python.org/psf/conduct/).
-
```

### Comparing `python-mcs-sdk-0.2.12/README.md` & `python-mcs-sdk-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,30 +43,30 @@
 rpc_endpoint="<RPC_ENDPOINT>"# e.g https://polygon-rpc.com
 
 ```
 
 **Authentication**
 
  ```python
-from mcs import APIClient
+from swan_mcs import APIClient
 if __name__ == '__main__':
     api_key="<API_KEY>"
     access_token="<ACCESS_TOKEN>"
     mcs_api = APIClient(api_key, access_token, chain_name)
     # polygon.mainnet for mainnet, polygon.mumbai for testnet
  ```
 
 ## 👨‍💻 Examples
 
 ### Bucket Storage
 
 - Create a bucket
 
 ```python
-from mcs import BucketAPI
+from swan_mcs import BucketAPI
     bucket_client = BucketAPI(mcs_api)
     bucket_data = bucket_client.create_bucket('YOUR_BUCKET_NAME')
     print(bucket_data)
 ```
 
 -  Upload a file to the bucket
 
@@ -80,15 +80,15 @@
 ### Onchain Storage
 
 Onchain storage is designed for stored file information in smart contract.It requires payment for each file
 
 * Upload File to Onchain storage
 
  ```python
-from mcs import OnchainAPI
+from swan_mcs import OnchainAPI
     onchain = OnchainAPI(mcs_api)
     print(onchain.upload_file('<File Path>'))
  ```
 
 * Pay for the storage contract
 
 Please move forward for [How to pay for the storage](https://docs.filswan.com/multichain.storage/developer-quickstart/sdk/python-mcs-sdk/onchain-storage/advanced-usage)
```

### Comparing `python-mcs-sdk-0.2.12/mcs/api/onchain_api.py` & `python-mcs-sdk-0.3.0/swan_mcs/api/onchain_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from mcs.api_client import APIClient
-from mcs.common.constants import *
-from mcs.common.utils import get_contract_abi, get_amount
+from swan_mcs.api_client import APIClient
+from swan_mcs.common.constants import *
+from swan_mcs.common.utils import get_contract_abi, get_amount
 from web3 import Web3
 from web3.middleware import geth_poa_middleware
 from web3.logs import DISCARD
 from eth_account import Account
 import json
 import logging
 
-from mcs.object.onchain_storage import *
+from swan_mcs.object.onchain_storage import *
 
 
 class OnchainAPI(object):
     def __init__(self, api_client=None, private_key=None, rpc_url='https://polygon-rpc.com/'):
         if private_key is None:
             logging.error("Please provide private_key to use MCS Onchain Storage.")
         if api_client is None:
```

### Comparing `python-mcs-sdk-0.2.12/mcs/api_client.py` & `python-mcs-sdk-0.3.0/swan_mcs/api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from mcs.common.constants import *
-from mcs.common.params import Params
+from swan_mcs.common.constants import *
+from swan_mcs.common.params import Params
 import requests
 import json
 import logging
-from mcs.common import utils, exceptions
-from mcs.common import constants as c
+from swan_mcs.common import utils, exceptions
+from swan_mcs.common import constants as c
 from requests_toolbelt.multipart.encoder import MultipartEncoder, MultipartEncoderMonitor
 from tqdm import tqdm
 from pathlib import Path
 
 
 class APIClient(object):
     def __init__(self, api_key, access_token, chain_name=None, login=True):
@@ -23,33 +23,37 @@
             self.api_key_login()
 
     def get_params(self):
         return self._request_without_params(GET, MCS_PARAMS, self.MCS_API, self.token)
 
     def get_price_rate(self):
         return self._request_without_params(GET, PRICE_RATE, self.MCS_API, self.token)
-    
+
     def get_gateway(self):
         res = self._request_without_params(GET, GET_GATEWAY, self.MCS_API, self.token)
-        gateway = res["data"][0]
-        return gateway
+        if res:
+            gateway = res["data"][0]
+            return gateway
+        else:
+            logging.error("\033[31m Get Gateway error\033[0m")
+            return
 
     def api_key_login(self):
         params = {'apikey': self.api_key, 'access_token': self.access_token, 'network': self.chain_name}
         # if params.get('apikey') == '' or params.get('access_token') == '' or params.get('chain_name') == '':
         #     logging.error("\033[31mAPIkey, access token, or chain name does not exist\033[0m")
         #     return
         try:
             result = self._request_with_params(POST, APIKEY_LOGIN, self.MCS_API, params, None, None)
             self.token = result['data']['jwt_token']
             logging.info("\033[32mLogin successful\033[0m")
             return self.token
         except:
             logging.error("\033[31m Please check your APIkey and access token, or "
-                                                  "check whether the current network environment corresponds to the APIkey.\033[0m")
+                          "check whether the current network environment corresponds to the APIkey.\033[0m")
             return
 
     def _request(self, method, request_path, mcs_api, params, token, files=False):
         if method == c.GET:
             request_path = request_path + utils.parse_params_to_str(params)
         url = mcs_api + request_path
         header = {}
@@ -81,15 +85,14 @@
             json_res = response.json()
             # print(json_res['message'])
             return None
         #     raise exceptions.McsAPIException(response)
         #
         # if str(json_res['status']) == 'error':
         #     raise exceptions.McsRequestException(json_res['message'])
-
         return response.json()
 
     def _request_stream_upload(self, request_path, mcs_api, params, token):
         url = mcs_api + request_path
         header = {}
         if token:
             header["Authorization"] = "Bearer " + token
```

### Comparing `python-mcs-sdk-0.2.12/mcs/common/constants.py` & `python-mcs-sdk-0.3.0/swan_mcs/common/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 MCS_POLYGON_MAIN_API = "https://api.multichain.storage"
-MCS_POLYGON_MUMBAI_API = "http://192.168.88.41:8889"
+MCS_POLYGON_MUMBAI_API = "https://calibration-mcs-api.filswan.com"
 MCS_BSC_API = 'https://calibration-mcs-bsc.filswan.com'
 GET = "GET"
 POST = "POST"
 PUT = "PUT"
 DELETE = "DELETE"
 FIL_PRICE_API = "https://api.filswan.com/stats/storage"
-# mcs api
+# swan_mcs api
 MCS_PARAMS = "/api/v1/common/system/params"
 PRICE_RATE = "/api/v1/billing/price/filecoin"
 PAYMENT_INFO = "/api/v1/billing/deal/lockpayment/info"
 TASKS_DEALS = "/api/v1/storage/tasks/deals"
 MINT_INFO = "/api/v1/storage/mint/info"
 UPLOAD_FILE = "/api/v1/storage/ipfs/upload"
 DEAL_DETAIL = "/api/v1/storage/deal/detail/"
```

### Comparing `python-mcs-sdk-0.2.12/mcs/common/exceptions.py` & `python-mcs-sdk-0.3.0/swan_mcs/common/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     def __init__(self, response):
         print(response.text + ', ' + str(response.status_code))
         self.code = 0
         try:
             json_res = response.json()
         except ValueError:
-            self.message = 'Invalid JSON error message from Mcs: {}'.format(response.text)
+            self.message = 'Invalid JSON error message from swan_mcs: {}'.format(response.text)
         else:
             if "error_code" in json_res.keys() and "error_message" in json_res.keys():
                 self.code = json_res['error_code']
                 self.message = json_res['error_message']
             else:
                 self.code = 'None'
                 self.message = 'System error'
```

### Comparing `python-mcs-sdk-0.2.12/mcs/common/params.py` & `python-mcs-sdk-0.3.0/swan_mcs/common/params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from mcs.common.constants import MCS_POLYGON_MUMBAI_API, MCS_BSC_API, MCS_POLYGON_MAIN_API
+from swan_mcs.common.constants import MCS_POLYGON_MUMBAI_API, MCS_BSC_API, MCS_POLYGON_MAIN_API
+import logging
 
 class Params:
     def __init__(self, chain_name='polygon.mainnet'):
         if chain_name == 'polygon.mainnet' or chain_name == 'main':
             self.MCS_API = MCS_POLYGON_MAIN_API
         elif chain_name == 'polygon.mumbai' or chain_name == 'mumbai':
             self.MCS_API = MCS_POLYGON_MUMBAI_API
         elif chain_name == 'bsc.testnet' or chain_name == 'bsc':
             self.MCS_API = MCS_BSC_API
         else:
-            print('unknown chain name')
+            logging.error("\033[31munknown chain name\033[0m")
 
     def get_params(self):
 
         param_vars = [attr for attr in dir(self) if not callable(getattr(self, attr)) and not attr.startswith("__")]
         param_dict = {}
         for i in param_vars:
             param_dict[i] = getattr(self, i)
```

### Comparing `python-mcs-sdk-0.2.12/mcs/common/utils.py` & `python-mcs-sdk-0.3.0/swan_mcs/common/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from mcs.common.constants import FIL_PRICE_API
+from swan_mcs.common.constants import FIL_PRICE_API
 import json
 import os
 
 
 def get_fil_price():
     response = requests.request("GET", FIL_PRICE_API)
     price = response.json()["data"]['historical_average_price_verified']
```

### Comparing `python-mcs-sdk-0.2.12/mcs/object/bucket_storage.py` & `python-mcs-sdk-0.3.0/swan_mcs/object/bucket_storage.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.2.12/mcs/object/onchain_storage.py` & `python-mcs-sdk-0.3.0/swan_mcs/object/onchain_storage.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.2.12/python_mcs_sdk.egg-info/PKG-INFO` & `python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: python-mcs-sdk
-Version: 0.2.12
+Version: 0.3.0
 Summary: A python software development kit for the Multi-Chain Storage
 Author: daniel8088
 Author-email: danilew8088@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Made by FilSwan](https://img.shields.io/badge/made%20by-FilSwan-green.svg)](https://www.filswan.com/) [![Chat on discord](https://img.shields.io/badge/join%20-discord-brightgreen.svg)](https://discord.com/invite/KKGhy8ZqzK)
 
 Python-MCS-SDK is a python software development kit for the [Multi-Chain Storage(MCS)](https://www.multichain.storage) service. It provides a convenient interface for working with the MCS API.
 
 Please take a look at our documentation for how to install and use Python-MCS-SDK:
-
-- [Prerequisites](https://docs.filswan.com/multichain.storage/developer-quickstart/sdk/python-mcs-sdk/prerequisite)
-- [Get Started](https://docs.filswan.com/multichain.storage/developer-quickstart/sdk/python-mcs-sdk/get-started)
+- [Get Started](https://docs.filswan.com/multichain.storage/developer-quickstart/sdk/python-mcs-sdk/quickstart)
 
 If you find bugs, need help, or want to talk to the developers, please use our mailing lists or chat rooms:
 
 - [Discord channel](https://discord.com/invite/KKGhy8ZqzK)
 - [Issue tracking](https://github.com/filswan/python-mcs-sdk/issues)
 
 If you want to get involved, head over to GitHub to get the source code, look at our developer documentation and feel free to jump on the developer mailing lists and chat rooms:
 
 - [GitHub Page](https://github.com/filswan/python-mcs-sdk)
 - [Development documentation](https://docs.filswan.com/multichain.storage/developer-quickstart/sdk/python-mcs-sdk)
 
 ## Code of Conduct
 
 Everyone interacting in the pip project’s codebases, issue trackers, chat rooms, and mailing lists is expected to follow the [PSF Code of Conduct](https://www.python.org/psf/conduct/).
-
```

### Comparing `python-mcs-sdk-0.2.12/test/test_bucket_api.py` & `python-mcs-sdk-0.3.0/test/test_bucket_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,85 @@
 import pytest
 import os
 from dotenv import load_dotenv
-from mcs.common.params import Params
-from mcs import BucketAPI, APIClient
-import time
-
-def login():
-    load_dotenv(".env_test")
-    api_key = os.getenv('api_key')
-    access_token = os.getenv('access_token')
-    chain_name = os.getenv("chain_name")
-    api = BucketAPI(APIClient(api_key, access_token, chain_name))
-    
-    assert api
-    return api
-
-def test_delete_bucket():
-    api = login()
-    print(api.delete_bucket('test-bucket'))
-
-def test_list_buckets():
-    api = login()
-    assert api.list_buckets() is not None
-
-def test_create_bucket():
-    api = login()
-    create = api.create_bucket('test-bucket')
-    assert create == True
-
-def test_get_bucket():
-    api = login()
-    bucket = api.get_bucket('test-bucket')
-    assert bucket.bucket_name == 'test-bucket'
-
-
-def test_create_folder():
-    api = login()
-    create = api.create_folder('test-bucket', 'folder1')
-
-    assert create == True
-
-# def test_create_folder_with_same_name():
-#     api = login()
-#     create = api.create_folder('test-bucket', 'folder1')
-#     print(create)
-
-def test_upload_file():
-    api = login()
-    filepath = "/images/log_mcs.png"
-    parentpath = os.path.abspath(os.path.dirname(__file__))
-    file = api.upload_file('test-bucket', "folder1/mcs-logo.png", parentpath + filepath)
-    assert file.name == "mcs-logo.png"
-
-def test_get_file():
-    api = login()
-    file = api.get_file('test-bucket', 'folder1/mcs-logo.png')
-
-    assert file.name == "mcs-logo.png"
-
-
-def test_get_file_list():
-    api = login()
-    list = api.list_files('test-bucket', 'folder1')
-    
-    assert len(list) == 1
-    assert list[0].name == 'mcs-logo.png'
-
-
-def test_download_file():
-    api = login()
-    result = api.download_file('test-bucket', 'folder1/mcs-logo.png', "aaaa.png")
-    
-    assert result == True
-
-
-def test_delete_file():
-    api = login()
-    delete = api.delete_file('test-bucket', 'folder1/mcs-logo.png')
-
-    assert delete == True
-
-def test_upload_ipfs_folder():
-    api = login()
-    res = api.upload_ipfs_folder('test-bucket', 'ipfs-folder', 'images')
+from swan_mcs import BucketAPI, APIClient
 
-    print(res)
+
+@pytest.mark.skip(reason="no way of currently testing this")
+class TestBucketAPI:
+    def login(self):
+        load_dotenv(".env_test")
+        api_key = os.getenv('api_key')
+        access_token = os.getenv('access_token')
+        chain_name = os.getenv("chain_name")
+        api = BucketAPI(APIClient(api_key, access_token, chain_name))
+
+        assert api
+        return api
+
+    def test_delete_bucket(self):
+        api = self.login()
+        print(api.delete_bucket('test-bucket'))
+
+    def test_list_buckets(self):
+        api = self.login()
+        print(api.list_buckets())
+        assert api.list_buckets() is not None
+
+    def test_create_bucket(self):
+        api = self.login()
+        create = api.create_bucket('test-bucket')
+        assert create is True
+
+    def test_get_bucket(self):
+        api = self.login()
+        bucket = api.get_bucket('test-bucket')
+        assert bucket.bucket_name == 'test-bucket'
+
+    def test_create_folder(self):
+        api = self.login()
+        create = api.create_folder('test-bucket', 'folder1')
+
+        assert create is True
+
+    # def test_create_folder_with_same_name():
+    #     api = login()
+    #     create = api.create_folder('test-bucket', 'folder1')
+    #     print(create)
+
+    def test_upload_file(self):
+        api = self.login()
+        filepath = "/images/log_mcs.png"
+        parentpath = os.path.abspath(os.path.dirname(__file__))
+        file = api.upload_file('test-bucket', "folder1/swan_mcs-logo.png", parentpath + filepath)
+        assert file.name == "swan_mcs-logo.png"
+
+    def test_get_file(self):
+        api = self.login()
+        file = api.get_file('test-bucket', 'folder1/swan_mcs-logo.png')
+
+        assert file.name == "swan_mcs-logo.png"
+
+    def test_get_file_list(self):
+        api = self.login()
+        list = api.list_files('test-bucket', 'folder1')
+
+        assert len(list) == 1
+        assert list[0].name == 'swan_mcs-logo.png'
+
+    def test_download_file(self):
+        api = self.login()
+        result = api.download_file('test-bucket', 'folder1/swan_mcs-logo.png', "aaaa.png")
+
+        assert result is True
+
+    def test_delete_file(self):
+        api = self.login()
+        delete = api.delete_file('test-bucket', 'folder1/swan_mcs-logo.png')
+
+        assert delete is True
+
+    def test_upload_ipfs_folder(self):
+        api = self.login()
+        res = api.upload_ipfs_folder('test-bucket', 'ipfs-folder', 'images')
+
+        print(res)
```

### Comparing `python-mcs-sdk-0.2.12/test/test_onchain_api.py` & `python-mcs-sdk-0.3.0/test/test_onchain_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 import pytest
 import os
 from dotenv import load_dotenv
-from mcs.common.params import Params
-from mcs import OnchainAPI, APIClient
+from swan_mcs import OnchainAPI, APIClient
 
 
-def login():
-    load_dotenv(".env_test")
-    api_key = os.getenv('api_key')
-    access_token = os.getenv('access_token')
-    chain_name = os.getenv("chain_name")
+@pytest.mark.skip(reason="no way of currently testing this")
+class TestOnchainAPI:
+    def login(self):
+        load_dotenv(".env_test")
+        api_key = os.getenv('api_key')
+        access_token = os.getenv('access_token')
+        chain_name = os.getenv("chain_name")
 
-    private_key = os.getenv("private_key")
-    rpc_endpoint = os.getenv("rpc_endpoint")
+        private_key = os.getenv("private_key")
+        rpc_endpoint = os.getenv("rpc_endpoint")
 
-    api = OnchainAPI(APIClient(api_key, access_token, chain_name), private_key, rpc_endpoint)
-    # print(api.token)
+        api = OnchainAPI(APIClient(api_key, access_token, chain_name), private_key, rpc_endpoint)
+        # print(api.token)
 
-    assert api
-    return api
+        assert api
+        return api
 
-def test_upload_file():
-    api = login()
-    filepath = "/images/log_mcs.png"
-    parentpath = os.path.abspath(os.path.dirname(__file__))
-    file = api.upload(parentpath + filepath)
+    def test_upload_file(self):
+        api = self.login()
+        filepath = "/images/log_mcs.png"
+        parentpath = os.path.abspath(os.path.dirname(__file__))
+        file = api.upload(parentpath + filepath)
 
-    pytest.file = file
-    assert file
+        pytest.file = file
+        assert file
 
-def test_pay_file():
-    api = login()
-    payment = api.pay(pytest.file.source_file_upload_id, pytest.file.file_size)
-    print(payment)
+    def test_pay_file(self):
+        api = self.login()
+        payment = api.pay(pytest.file.source_file_upload_id, pytest.file.file_size)
+        print(payment)
 
-def test_create_collection():
-    api = login()
+    def test_create_collection(self):
+        api = self.login()
 
-    num_collections = len(api.get_collections())
-    collection = api.create_collection({"name": 'test-collection-'+str(num_collections)})
+        num_collections = len(api.get_collections())
+        collection = api.create_collection({"name": 'test-collection-' + str(num_collections)})
 
-    assert len(api.get_collections()) == num_collections + 1
+        assert len(api.get_collections()) == num_collections + 1
 
-# def test_mint():
-#     api = login()
+    # def test_mint():
+    #     api = login()
 
-#     mint = api.mint(pytest.file.source_file_upload_id, {"name": 'test-nft', 'image': pytest.file.ipfs_url}, pytest.collection_address)
+    #     mint = api.mint(pytest.file.source_file_upload_id, {"name": 'test-nft', 'image': pytest.file.ipfs_url}, pytest.collection_address)
 
-#     assert mint["id"] == 1
+    #     assert mint["id"] == 1
 
-def test_get_uploads():
-    api = login()
-    deals = api.get_user_tasks_deals()
+    def test_get_uploads(self):
+        api = self.login()
+        deals = api.get_user_tasks_deals()
 
-    file_ids = [deal.source_file_upload_id for deal in deals]
-    
-    assert pytest.file.source_file_upload_id in file_ids
+        file_ids = [deal.source_file_upload_id for deal in deals]
 
-def test_get_deal_detail():
-    api = login()
-    detail = api.get_deal_detail(pytest.file.source_file_upload_id)
+        assert pytest.file.source_file_upload_id in file_ids
 
-    assert detail
+    def test_get_deal_detail(self):
+        api = self.login()
+        detail = api.get_deal_detail(pytest.file.source_file_upload_id)
+
+        assert detail
```

