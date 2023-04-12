# Comparing `tmp/python-mcs-sdk-0.3.0.tar.gz` & `tmp/python-mcs-sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mcs-sdk-0.3.0.tar", last modified: Wed Apr 12 15:25:57 2023, max compression
+gzip compressed data, was "python-mcs-sdk-0.3.1.tar", last modified: Wed Apr 12 17:47:59 2023, max compression
```

## Comparing `python-mcs-sdk-0.3.0.tar` & `python-mcs-sdk-0.3.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.455010 python-mcs-sdk-0.3.0/
--rw-r--r--   0 daniel     (501) staff       (20)     1064 2022-07-01 06:58:03.000000 python-mcs-sdk-0.3.0/LICENSE
--rw-r--r--   0 daniel     (501) staff       (20)       31 2022-08-10 05:11:25.000000 python-mcs-sdk-0.3.0/MANIFEST.in
--rw-r--r--   0 daniel     (501) staff       (20)     1677 2023-04-12 15:25:57.454860 python-mcs-sdk-0.3.0/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)     3896 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/README.md
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.447331 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)     1677 2023-04-12 15:25:57.000000 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)     1599 2023-04-12 15:25:57.000000 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-04-12 15:25:57.000000 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       69 2023-04-12 15:25:57.000000 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        9 2023-04-12 15:25:57.000000 python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-04-12 15:25:57.455060 python-mcs-sdk-0.3.0/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      878 2023-04-12 15:25:40.000000 python-mcs-sdk-0.3.0/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.447543 python-mcs-sdk-0.3.0/swan_mcs/
--rw-r--r--   0 daniel     (501) staff       (20)      230 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.0/swan_mcs/__init__.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.447861 python-mcs-sdk-0.3.0/swan_mcs/api/
--rw-r--r--   0 daniel     (501) staff       (20)       94 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.0/swan_mcs/api/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    18026 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.0/swan_mcs/api/bucket_api.py
--rw-r--r--   0 daniel     (501) staff       (20)    11270 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.0/swan_mcs/api/onchain_api.py
--rw-r--r--   0 daniel     (501) staff       (20)     6443 2023-04-11 16:14:34.000000 python-mcs-sdk-0.3.0/swan_mcs/api_client.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.448325 python-mcs-sdk-0.3.0/swan_mcs/common/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2022-07-01 07:09:06.000000 python-mcs-sdk-0.3.0/swan_mcs/common/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     1639 2023-04-11 15:42:48.000000 python-mcs-sdk-0.3.0/swan_mcs/common/constants.py
--rw-r--r--   0 daniel     (501) staff       (20)     1289 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/swan_mcs/common/exceptions.py
--rw-r--r--   0 daniel     (501) staff       (20)      923 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.0/swan_mcs/common/params.py
--rw-r--r--   0 daniel     (501) staff       (20)     1190 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.0/swan_mcs/common/utils.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.448426 python-mcs-sdk-0.3.0/swan_mcs/contract/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2023-04-11 14:55:17.000000 python-mcs-sdk-0.3.0/swan_mcs/contract/__init__.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.448603 python-mcs-sdk-0.3.0/swan_mcs/object/
--rw-r--r--   0 daniel     (501) staff       (20)     1850 2023-03-09 00:03:04.000000 python-mcs-sdk-0.3.0/swan_mcs/object/bucket_storage.py
--rw-r--r--   0 daniel     (501) staff       (20)     4597 2023-03-07 21:01:28.000000 python-mcs-sdk-0.3.0/swan_mcs/object/onchain_storage.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 15:25:57.454616 python-mcs-sdk-0.3.0/test/
--rw-r--r--   0 daniel     (501) staff       (20)     2545 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_bucket_api.py
--rw-r--r--   0 daniel     (501) staff       (20)     2082 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_api_key_login.py
--rw-r--r--   0 daniel     (501) staff       (20)     1489 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_create_bucket_api.py
--rw-r--r--   0 daniel     (501) staff       (20)     2432 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_create_folder.py
--rw-r--r--   0 daniel     (501) staff       (20)     1534 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_delete_bucket.py
--rw-r--r--   0 daniel     (501) staff       (20)     1636 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_delete_file.py
--rw-r--r--   0 daniel     (501) staff       (20)     2884 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_mock_download_file.py
--rw-r--r--   0 daniel     (501) staff       (20)     2942 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_mock_download_ipfs_folder.py
--rw-r--r--   0 daniel     (501) staff       (20)     2325 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_get_bucket.py
--rw-r--r--   0 daniel     (501) staff       (20)     1291 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_get_bucket_list.py
--rw-r--r--   0 daniel     (501) staff       (20)     1975 2023-04-11 15:06:12.000000 python-mcs-sdk-0.3.0/test/test_mock_get_file.py
--rw-r--r--   0 daniel     (501) staff       (20)      698 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_get_gateway.py
--rw-r--r--   0 daniel     (501) staff       (20)     1233 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_mock_list_files.py
--rw-r--r--   0 daniel     (501) staff       (20)     4451 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.0/test/test_mock_upload_file.py
--rw-r--r--   0 daniel     (501) staff       (20)     3185 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.0/test/test_mock_upload_folder.py
--rw-r--r--   0 daniel     (501) staff       (20)     2272 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_mock_upload_ipfs_folder.py
--rw-r--r--   0 daniel     (501) staff       (20)     1955 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_onchain_api.py
--rw-r--r--   0 daniel     (501) staff       (20)     1266 2023-04-11 16:14:34.000000 python-mcs-sdk-0.3.0/test/test_real_api_key_login.py
--rw-r--r--   0 daniel     (501) staff       (20)      979 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_create_bucket_api.py
--rw-r--r--   0 daniel     (501) staff       (20)     1219 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_create_folder.py
--rw-r--r--   0 daniel     (501) staff       (20)     1041 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_delete_bucket.py
--rw-r--r--   0 daniel     (501) staff       (20)     1300 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_delete_file.py
--rw-r--r--   0 daniel     (501) staff       (20)     1889 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_download_file.py
--rw-r--r--   0 daniel     (501) staff       (20)     1853 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.0/test/test_real_download_ipfs_folder.py
--rw-r--r--   0 daniel     (501) staff       (20)     1685 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_get_bucket.py
--rw-r--r--   0 daniel     (501) staff       (20)     1186 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_get_bucket_list.py
--rw-r--r--   0 daniel     (501) staff       (20)     1335 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.0/test/test_real_get_file.py
--rw-r--r--   0 daniel     (501) staff       (20)      179 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_get_gateway.py
--rw-r--r--   0 daniel     (501) staff       (20)     2258 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_list_files.py
--rw-r--r--   0 daniel     (501) staff       (20)     2097 2023-04-11 17:28:02.000000 python-mcs-sdk-0.3.0/test/test_real_upload_file.py
--rw-r--r--   0 daniel     (501) staff       (20)     1864 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.0/test/test_real_upload_folder.py
--rw-r--r--   0 daniel     (501) staff       (20)     2627 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.0/test/test_real_upload_ipfs_folder.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 17:47:59.378903 python-mcs-sdk-0.3.1/
+-rw-r--r--   0 daniel     (501) staff       (20)     1064 2022-07-01 06:58:03.000000 python-mcs-sdk-0.3.1/LICENSE
+-rw-r--r--   0 daniel     (501) staff       (20)       31 2022-08-10 05:11:25.000000 python-mcs-sdk-0.3.1/MANIFEST.in
+-rw-r--r--   0 daniel     (501) staff       (20)     1677 2023-04-12 17:47:59.378759 python-mcs-sdk-0.3.1/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     3896 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 17:47:59.373346 python-mcs-sdk-0.3.1/python_mcs_sdk.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     1677 2023-04-12 17:47:59.000000 python-mcs-sdk-0.3.1/python_mcs_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     1599 2023-04-12 17:47:59.000000 python-mcs-sdk-0.3.1/python_mcs_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-04-12 17:47:59.000000 python-mcs-sdk-0.3.1/python_mcs_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       69 2023-04-12 17:47:59.000000 python-mcs-sdk-0.3.1/python_mcs_sdk.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        9 2023-04-12 17:47:59.000000 python-mcs-sdk-0.3.1/python_mcs_sdk.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-04-12 17:47:59.378949 python-mcs-sdk-0.3.1/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      761 2023-04-12 17:47:36.000000 python-mcs-sdk-0.3.1/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 17:47:59.373553 python-mcs-sdk-0.3.1/swan_mcs/
+-rw-r--r--   0 daniel     (501) staff       (20)      113 2023-04-12 17:45:39.000000 python-mcs-sdk-0.3.1/swan_mcs/__init__.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 17:47:59.373942 python-mcs-sdk-0.3.1/swan_mcs/api/
+-rw-r--r--   0 daniel     (501) staff       (20)       94 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.1/swan_mcs/api/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    18026 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.1/swan_mcs/api/bucket_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)    11270 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.1/swan_mcs/api/onchain_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6443 2023-04-11 16:14:34.000000 python-mcs-sdk-0.3.1/swan_mcs/api_client.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 17:47:59.374448 python-mcs-sdk-0.3.1/swan_mcs/common/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2022-07-01 07:09:06.000000 python-mcs-sdk-0.3.1/swan_mcs/common/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1639 2023-04-11 15:42:48.000000 python-mcs-sdk-0.3.1/swan_mcs/common/constants.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1289 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/swan_mcs/common/exceptions.py
+-rw-r--r--   0 daniel     (501) staff       (20)      923 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.1/swan_mcs/common/params.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1190 2023-04-11 14:54:53.000000 python-mcs-sdk-0.3.1/swan_mcs/common/utils.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 17:47:59.374549 python-mcs-sdk-0.3.1/swan_mcs/contract/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-04-11 14:55:17.000000 python-mcs-sdk-0.3.1/swan_mcs/contract/__init__.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 17:47:59.374876 python-mcs-sdk-0.3.1/swan_mcs/object/
+-rw-r--r--   0 daniel     (501) staff       (20)     1850 2023-03-09 00:03:04.000000 python-mcs-sdk-0.3.1/swan_mcs/object/bucket_storage.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4597 2023-03-07 21:01:28.000000 python-mcs-sdk-0.3.1/swan_mcs/object/onchain_storage.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-12 17:47:59.378588 python-mcs-sdk-0.3.1/test/
+-rw-r--r--   0 daniel     (501) staff       (20)     2545 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/test/test_bucket_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2082 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/test/test_mock_api_key_login.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1489 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/test/test_mock_create_bucket_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2432 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/test/test_mock_create_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1534 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/test/test_mock_delete_bucket.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1636 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/test/test_mock_delete_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2884 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.1/test/test_mock_download_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2942 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.1/test/test_mock_download_ipfs_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2325 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/test/test_mock_get_bucket.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1291 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/test/test_mock_get_bucket_list.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1975 2023-04-11 15:06:12.000000 python-mcs-sdk-0.3.1/test/test_mock_get_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)      698 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/test/test_mock_get_gateway.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1233 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.1/test/test_mock_list_files.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4451 2023-04-11 14:56:07.000000 python-mcs-sdk-0.3.1/test/test_mock_upload_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3185 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.1/test/test_mock_upload_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2272 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.1/test/test_mock_upload_ipfs_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1955 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.1/test/test_onchain_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1266 2023-04-11 16:14:34.000000 python-mcs-sdk-0.3.1/test/test_real_api_key_login.py
+-rw-r--r--   0 daniel     (501) staff       (20)      979 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.1/test/test_real_create_bucket_api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1219 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.1/test/test_real_create_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1041 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.1/test/test_real_delete_bucket.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1300 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.1/test/test_real_delete_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1889 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.1/test/test_real_download_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1853 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.1/test/test_real_download_ipfs_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1685 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.1/test/test_real_get_bucket.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1186 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.1/test/test_real_get_bucket_list.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1335 2023-04-11 15:10:02.000000 python-mcs-sdk-0.3.1/test/test_real_get_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)      179 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.1/test/test_real_get_gateway.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2258 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.1/test/test_real_list_files.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2097 2023-04-11 17:28:02.000000 python-mcs-sdk-0.3.1/test/test_real_upload_file.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1864 2023-04-11 14:50:38.000000 python-mcs-sdk-0.3.1/test/test_real_upload_folder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2627 2023-04-12 15:12:35.000000 python-mcs-sdk-0.3.1/test/test_real_upload_ipfs_folder.py
```

### Comparing `python-mcs-sdk-0.3.0/LICENSE` & `python-mcs-sdk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/PKG-INFO` & `python-mcs-sdk-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mcs-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python software development kit for the Multi-Chain Storage
 Author: daniel8088
 Author-email: danilew8088@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-mcs-sdk-0.3.0/README.md` & `python-mcs-sdk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/PKG-INFO` & `python-mcs-sdk-0.3.1/python_mcs_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mcs-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python software development kit for the Multi-Chain Storage
 Author: daniel8088
 Author-email: danilew8088@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-mcs-sdk-0.3.0/python_mcs_sdk.egg-info/SOURCES.txt` & `python-mcs-sdk-0.3.1/python_mcs_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/swan_mcs/api/bucket_api.py` & `python-mcs-sdk-0.3.1/swan_mcs/api/bucket_api.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/swan_mcs/api/onchain_api.py` & `python-mcs-sdk-0.3.1/swan_mcs/api/onchain_api.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/swan_mcs/api_client.py` & `python-mcs-sdk-0.3.1/swan_mcs/api_client.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/swan_mcs/common/constants.py` & `python-mcs-sdk-0.3.1/swan_mcs/common/constants.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/swan_mcs/common/exceptions.py` & `python-mcs-sdk-0.3.1/swan_mcs/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/swan_mcs/common/params.py` & `python-mcs-sdk-0.3.1/swan_mcs/common/params.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/swan_mcs/common/utils.py` & `python-mcs-sdk-0.3.1/swan_mcs/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/swan_mcs/object/bucket_storage.py` & `python-mcs-sdk-0.3.1/swan_mcs/object/bucket_storage.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/swan_mcs/object/onchain_storage.py` & `python-mcs-sdk-0.3.1/swan_mcs/object/onchain_storage.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_bucket_api.py` & `python-mcs-sdk-0.3.1/test/test_bucket_api.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_api_key_login.py` & `python-mcs-sdk-0.3.1/test/test_mock_api_key_login.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_create_bucket_api.py` & `python-mcs-sdk-0.3.1/test/test_mock_create_bucket_api.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_create_folder.py` & `python-mcs-sdk-0.3.1/test/test_mock_create_folder.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_delete_bucket.py` & `python-mcs-sdk-0.3.1/test/test_mock_delete_bucket.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_delete_file.py` & `python-mcs-sdk-0.3.1/test/test_mock_delete_file.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_download_file.py` & `python-mcs-sdk-0.3.1/test/test_mock_download_file.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_download_ipfs_folder.py` & `python-mcs-sdk-0.3.1/test/test_mock_download_ipfs_folder.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_get_bucket.py` & `python-mcs-sdk-0.3.1/test/test_mock_get_bucket.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_get_bucket_list.py` & `python-mcs-sdk-0.3.1/test/test_mock_get_bucket_list.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_get_file.py` & `python-mcs-sdk-0.3.1/test/test_mock_get_file.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_get_gateway.py` & `python-mcs-sdk-0.3.1/test/test_mock_get_gateway.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_list_files.py` & `python-mcs-sdk-0.3.1/test/test_mock_list_files.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_upload_file.py` & `python-mcs-sdk-0.3.1/test/test_mock_upload_file.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_upload_folder.py` & `python-mcs-sdk-0.3.1/test/test_mock_upload_folder.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_mock_upload_ipfs_folder.py` & `python-mcs-sdk-0.3.1/test/test_mock_upload_ipfs_folder.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_onchain_api.py` & `python-mcs-sdk-0.3.1/test/test_onchain_api.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_api_key_login.py` & `python-mcs-sdk-0.3.1/test/test_real_api_key_login.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_create_bucket_api.py` & `python-mcs-sdk-0.3.1/test/test_real_create_bucket_api.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_create_folder.py` & `python-mcs-sdk-0.3.1/test/test_real_create_folder.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_delete_bucket.py` & `python-mcs-sdk-0.3.1/test/test_real_delete_bucket.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_delete_file.py` & `python-mcs-sdk-0.3.1/test/test_real_delete_file.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_download_file.py` & `python-mcs-sdk-0.3.1/test/test_real_download_file.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_download_ipfs_folder.py` & `python-mcs-sdk-0.3.1/test/test_real_download_ipfs_folder.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_get_bucket.py` & `python-mcs-sdk-0.3.1/test/test_real_get_bucket.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_get_bucket_list.py` & `python-mcs-sdk-0.3.1/test/test_real_get_bucket_list.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_get_file.py` & `python-mcs-sdk-0.3.1/test/test_real_get_file.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_list_files.py` & `python-mcs-sdk-0.3.1/test/test_real_list_files.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_upload_file.py` & `python-mcs-sdk-0.3.1/test/test_real_upload_file.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_upload_folder.py` & `python-mcs-sdk-0.3.1/test/test_real_upload_folder.py`

 * *Files identical despite different names*

### Comparing `python-mcs-sdk-0.3.0/test/test_real_upload_ipfs_folder.py` & `python-mcs-sdk-0.3.1/test/test_real_upload_ipfs_folder.py`

 * *Files identical despite different names*

