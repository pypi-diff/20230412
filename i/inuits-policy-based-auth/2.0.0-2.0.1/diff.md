# Comparing `tmp/inuits_policy_based_auth-2.0.0.tar.gz` & `tmp/inuits_policy_based_auth-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inuits_policy_based_auth-2.0.0.tar", last modified: Tue Mar 21 19:22:14 2023, max compression
+gzip compressed data, was "inuits_policy_based_auth-2.0.1.tar", last modified: Wed Apr 12 16:39:45 2023, max compression
```

## Comparing `inuits_policy_based_auth-2.0.0.tar` & `inuits_policy_based_auth-2.0.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.733482 inuits_policy_based_auth-2.0.0/
--rw-r--r--   0 eray      (1000) eray      (1000)    18092 2023-01-11 09:40:36.000000 inuits_policy_based_auth-2.0.0/LICENSE
--rw-r--r--   0 eray      (1000) eray      (1000)     7015 2023-03-21 19:22:14.732483 inuits_policy_based_auth-2.0.0/PKG-INFO
--rw-r--r--   0 eray      (1000) eray      (1000)     6553 2023-03-20 13:40:00.000000 inuits_policy_based_auth-2.0.0/README.md
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.729483 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/
--rw-r--r--   0 eray      (1000) eray      (1000)     1100 2023-03-17 17:05:37.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/__init__.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.729483 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authentication/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 15:56:53.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authentication/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1856 2023-01-11 09:40:36.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authentication/base_authentication_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.729483 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authentication/policies/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 15:56:58.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authentication/policies/__init__.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.729483 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 17:27:12.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     6291 2023-03-21 17:46:54.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.730482 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authorization/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 15:57:41.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authorization/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     2665 2023-01-11 10:41:17.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authorization/base_authorization_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.730482 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authorization/policies/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 17:27:18.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authorization/policies/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)      470 2023-01-11 11:28:59.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authorization/policies/open_data_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)      530 2023-03-20 10:09:51.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)      488 2023-01-11 13:46:35.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.730482 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/contexts/
--rw-r--r--   0 eray      (1000) eray      (1000)      223 2023-01-10 14:21:54.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/contexts/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)      851 2023-01-10 13:08:56.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/contexts/policy_context.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1388 2023-03-20 10:01:52.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/contexts/request_context.py
--rw-r--r--   0 eray      (1000) eray      (1000)     2863 2023-03-21 08:18:14.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/contexts/user_context.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1193 2023-01-10 13:40:55.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/exceptions.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.730482 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/helpers/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-21 08:11:53.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/helpers/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     4767 2023-03-21 18:25:35.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/helpers/immutable_dict.py
--rw-r--r--   0 eray      (1000) eray      (1000)     6187 2023-03-20 12:35:18.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/policy_factory.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.729483 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth.egg-info/
--rw-r--r--   0 eray      (1000) eray      (1000)     7015 2023-03-21 19:22:14.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth.egg-info/PKG-INFO
--rw-r--r--   0 eray      (1000) eray      (1000)     2621 2023-03-21 19:22:14.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth.egg-info/SOURCES.txt
--rw-r--r--   0 eray      (1000) eray      (1000)        1 2023-03-21 19:22:14.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth.egg-info/dependency_links.txt
--rw-r--r--   0 eray      (1000) eray      (1000)      129 2023-03-21 19:22:14.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth.egg-info/requires.txt
--rw-r--r--   0 eray      (1000) eray      (1000)       31 2023-03-21 19:22:14.000000 inuits_policy_based_auth-2.0.0/inuits_policy_based_auth.egg-info/top_level.txt
--rw-r--r--   0 eray      (1000) eray      (1000)       38 2023-03-21 19:22:14.733482 inuits_policy_based_auth-2.0.0/setup.cfg
--rw-r--r--   0 eray      (1000) eray      (1000)      959 2023-03-21 19:21:46.000000 inuits_policy_based_auth-2.0.0/setup.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.728483 inuits_policy_based_auth-2.0.0/tests/
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.731483 inuits_policy_based_auth-2.0.0/tests/integration/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 15:47:05.000000 inuits_policy_based_auth-2.0.0/tests/integration/__init__.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.731483 inuits_policy_based_auth-2.0.0/tests/integration/authentication/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-19 13:52:33.000000 inuits_policy_based_auth-2.0.0/tests/integration/authentication/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1201 2023-01-19 15:47:59.000000 inuits_policy_based_auth-2.0.0/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.731483 inuits_policy_based_auth-2.0.0/tests/integration/authorization/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-20 08:59:06.000000 inuits_policy_based_auth-2.0.0/tests/integration/authorization/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1093 2023-03-20 10:42:01.000000 inuits_policy_based_auth-2.0.0/tests/integration/authorization/test_open_data_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1317 2023-03-21 17:11:07.000000 inuits_policy_based_auth-2.0.0/tests/integration/authorization/test_scope_based_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1952 2023-03-21 08:25:37.000000 inuits_policy_based_auth-2.0.0/tests/integration/authorization/test_super_admin_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)      656 2023-01-19 15:19:28.000000 inuits_policy_based_auth-2.0.0/tests/integration/custom_token.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1490 2023-03-20 10:41:06.000000 inuits_policy_based_auth-2.0.0/tests/integration/flask_process.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.731483 inuits_policy_based_auth-2.0.0/tests/integration/test_api/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 15:47:05.000000 inuits_policy_based_auth-2.0.0/tests/integration/test_api/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1791 2023-03-21 18:23:06.000000 inuits_policy_based_auth-2.0.0/tests/integration/test_api/app.py
--rw-r--r--   0 eray      (1000) eray      (1000)     2341 2023-01-20 13:51:13.000000 inuits_policy_based_auth-2.0.0/tests/integration/test_api/policy_loader.py
--rw-r--r--   0 eray      (1000) eray      (1000)     3485 2023-03-20 14:35:23.000000 inuits_policy_based_auth-2.0.0/tests/integration/test_policy_factory.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.732483 inuits_policy_based_auth-2.0.0/tests/unit/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 14:32:25.000000 inuits_policy_based_auth-2.0.0/tests/unit/__init__.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.732483 inuits_policy_based_auth-2.0.0/tests/unit/authentication/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 14:32:11.000000 inuits_policy_based_auth-2.0.0/tests/unit/authentication/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1345 2023-01-11 15:24:33.000000 inuits_policy_based_auth-2.0.0/tests/unit/authentication/test_base_authentication_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.732483 inuits_policy_based_auth-2.0.0/tests/unit/authorization/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-11 10:19:57.000000 inuits_policy_based_auth-2.0.0/tests/unit/authorization/__init__.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.732483 inuits_policy_based_auth-2.0.0/tests/unit/authorization/policies/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-11 11:40:35.000000 inuits_policy_based_auth-2.0.0/tests/unit/authorization/policies/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)      150 2023-01-11 11:37:14.000000 inuits_policy_based_auth-2.0.0/tests/unit/authorization/policies/dummies.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1138 2023-01-11 14:27:27.000000 inuits_policy_based_auth-2.0.0/tests/unit/authorization/policies/test_open_data_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1105 2023-03-20 10:20:57.000000 inuits_policy_based_auth-2.0.0/tests/unit/authorization/policies/test_scope_based_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)     1045 2023-01-11 14:28:13.000000 inuits_policy_based_auth-2.0.0/tests/unit/authorization/policies/test_super_admin_policy.py
--rw-r--r--   0 eray      (1000) eray      (1000)     2024 2023-01-11 15:24:03.000000 inuits_policy_based_auth-2.0.0/tests/unit/authorization/test_base_authorization_policy.py
-drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-03-21 19:22:14.732483 inuits_policy_based_auth-2.0.0/tests/unit/helpers/
--rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-21 13:26:01.000000 inuits_policy_based_auth-2.0.0/tests/unit/helpers/__init__.py
--rw-r--r--   0 eray      (1000) eray      (1000)     3524 2023-03-21 18:25:06.000000 inuits_policy_based_auth-2.0.0/tests/unit/helpers/test_immutable_dict.py
--rw-r--r--   0 eray      (1000) eray      (1000)     6509 2023-03-20 13:21:30.000000 inuits_policy_based_auth-2.0.0/tests/unit/test_policy_factory.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)    18092 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/LICENSE
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     7015 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/PKG-INFO
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     6553 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/README.md
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1100 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1856 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/base_authentication_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     6291 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2665 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/base_authorization_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      470 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/open_data_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      530 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      576 2023-04-12 16:37:24.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      223 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      851 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/policy_context.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1388 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/request_context.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2863 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/user_context.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1193 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/exceptions.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/helpers/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/helpers/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     4768 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/helpers/immutable_dict.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     6187 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/policy_factory.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     7015 2023-04-12 16:39:45.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/PKG-INFO
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2621 2023-04-12 16:39:45.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        1 2023-04-12 16:39:45.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      129 2023-04-12 16:39:45.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/requires.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)       31 2023-04-12 16:39:45.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/top_level.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)       38 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/setup.cfg
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      959 2023-04-12 16:37:24.000000 inuits_policy_based_auth-2.0.1/setup.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/tests/
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/integration/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/integration/authentication/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authentication/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1201 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/integration/authorization/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authorization/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1093 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_open_data_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1317 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_scope_based_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1952 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_super_admin_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      656 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/custom_token.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1490 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/flask_process.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/integration/test_api/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/test_api/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1791 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/test_api/app.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2341 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/test_api/policy_loader.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     3485 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/test_policy_factory.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/unit/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/unit/authentication/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authentication/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1345 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authentication/test_base_authentication_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/unit/authorization/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      150 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/dummies.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1138 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_open_data_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1105 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_scope_based_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1045 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_super_admin_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2024 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/test_base_authorization_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/unit/helpers/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/helpers/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     3524 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/helpers/test_immutable_dict.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     6509 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/test_policy_factory.py
```

### Comparing `inuits_policy_based_auth-2.0.0/LICENSE` & `inuits_policy_based_auth-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/PKG-INFO` & `inuits_policy_based_auth-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits_policy_based_auth
-Version: 2.0.0
+Version: 2.0.1
 Summary: Module for securing API endpoints based on policies.
 Author: Inuits
 Author-email: developers@inuits.eu
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inuits_policy_based_auth-2.0.0/README.md` & `inuits_policy_based_auth-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/__init__.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authentication/base_authentication_policy.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authorization/base_authorization_policy.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/authorization/policies/scope_based_policy.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/contexts/policy_context.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/policy_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/contexts/request_context.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/request_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/contexts/user_context.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/user_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/exceptions.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/helpers/immutable_dict.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/helpers/immutable_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 
+
 class ImmutableDict:
     """
     A dictionary-like object that cannot be modified after initialization.
 
     The keys and values of an ImmutableDict can be any hashable object.
     Values can also be dictionaries or lists containing hashable objects.
```

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth/policy_factory.py` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/policy_factory.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth.egg-info/PKG-INFO` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-policy-based-auth
-Version: 2.0.0
+Version: 2.0.1
 Summary: Module for securing API endpoints based on policies.
 Author: Inuits
 Author-email: developers@inuits.eu
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inuits_policy_based_auth-2.0.0/inuits_policy_based_auth.egg-info/SOURCES.txt` & `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/setup.py` & `inuits_policy_based_auth-2.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,9 +25,9 @@
     ],
     license="GPLv2",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     name="inuits_policy_based_auth",
     packages=find_packages(exclude=["tests"]),
     provides=["inuits_policy_based_auth"],
-    version="2.0.0",
+    version="2.0.1",
 )
```

### Comparing `inuits_policy_based_auth-2.0.0/tests/integration/authentication/test_authlib_flask_oauth2_policy.py` & `inuits_policy_based_auth-2.0.1/tests/integration/authentication/test_authlib_flask_oauth2_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/integration/authorization/test_open_data_policy.py` & `inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/integration/authorization/test_scope_based_policy.py` & `inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/integration/authorization/test_super_admin_policy.py` & `inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/integration/custom_token.py` & `inuits_policy_based_auth-2.0.1/tests/integration/custom_token.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/integration/flask_process.py` & `inuits_policy_based_auth-2.0.1/tests/integration/flask_process.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/integration/test_api/app.py` & `inuits_policy_based_auth-2.0.1/tests/integration/test_api/app.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/integration/test_api/policy_loader.py` & `inuits_policy_based_auth-2.0.1/tests/integration/test_api/policy_loader.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/integration/test_policy_factory.py` & `inuits_policy_based_auth-2.0.1/tests/integration/test_policy_factory.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/unit/authentication/test_base_authentication_policy.py` & `inuits_policy_based_auth-2.0.1/tests/unit/authentication/test_base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/unit/authorization/policies/test_open_data_policy.py` & `inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/unit/authorization/policies/test_scope_based_policy.py` & `inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/unit/authorization/policies/test_super_admin_policy.py` & `inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/unit/authorization/test_base_authorization_policy.py` & `inuits_policy_based_auth-2.0.1/tests/unit/authorization/test_base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/unit/helpers/test_immutable_dict.py` & `inuits_policy_based_auth-2.0.1/tests/unit/helpers/test_immutable_dict.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.0/tests/unit/test_policy_factory.py` & `inuits_policy_based_auth-2.0.1/tests/unit/test_policy_factory.py`

 * *Files identical despite different names*

