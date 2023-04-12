# Comparing `tmp/stytch-6.7.0.tar.gz` & `tmp/stytch-6.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-6.7.0.tar", last modified: Fri Mar 31 17:10:42 2023, max compression
+gzip compressed data, was "stytch-6.7.1.tar", last modified: Wed Apr 12 19:53:52 2023, max compression
```

## Comparing `stytch-6.7.0.tar` & `stytch-6.7.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.565709 stytch-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-31 17:10:22.000000 stytch-6.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-03-31 17:10:42.565709 stytch-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-03-31 17:10:22.000000 stytch-6.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-31 17:10:42.569709 stytch-6.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-31 17:10:22.000000 stytch-6.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.557710 stytch-6.7.0/stytch/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.561710 stytch-6.7.0/stytch/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/api/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.561710 stytch-6.7.0/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.561710 stytch-6.7.0/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    33269 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.561710 stytch-6.7.0/stytch/b2b/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.565709 stytch-6.7.0/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.565709 stytch-6.7.0/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/core/api_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.565709 stytch-6.7.0/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.565709 stytch-6.7.0/stytch/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/models/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 17:10:22.000000 stytch-6.7.0/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.557710 stytch-6.7.0/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-03-31 17:10:42.000000 stytch-6.7.0/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-03-31 17:10:42.000000 stytch-6.7.0/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:10:42.000000 stytch-6.7.0/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 17:10:42.000000 stytch-6.7.0/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 17:10:42.000000 stytch-6.7.0/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:10:42.565709 stytch-6.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-03-31 17:10:22.000000 stytch-6.7.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-03-31 17:10:22.000000 stytch-6.7.0/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.769403 stytch-6.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 19:53:38.000000 stytch-6.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-12 19:53:52.769403 stytch-6.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-12 19:53:38.000000 stytch-6.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 19:53:52.769403 stytch-6.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-12 19:53:38.000000 stytch-6.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.757403 stytch-6.7.1/stytch/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.761403 stytch-6.7.1/stytch/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/api/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.761403 stytch-6.7.1/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.765403 stytch-6.7.1/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49021 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17130 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.765403 stytch-6.7.1/stytch/b2b/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.765403 stytch-6.7.1/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.765403 stytch-6.7.1/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/core/api_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.765403 stytch-6.7.1/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.769403 stytch-6.7.1/stytch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/models/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 19:53:38.000000 stytch-6.7.1/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.761403 stytch-6.7.1/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-12 19:53:52.000000 stytch-6.7.1/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-12 19:53:52.000000 stytch-6.7.1/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:53:52.000000 stytch-6.7.1/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 19:53:52.000000 stytch-6.7.1/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 19:53:52.000000 stytch-6.7.1/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:53:52.769403 stytch-6.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-04-12 19:53:38.000000 stytch-6.7.1/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-12 19:53:38.000000 stytch-6.7.1/test/test_integration_async.py
```

### Comparing `stytch-6.7.0/LICENSE.txt` & `stytch-6.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/PKG-INFO` & `stytch-6.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 6.7.0
+Version: 6.7.1
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
@@ -48,15 +48,15 @@
 - [x] [SMS passcodes](https://stytch.com/docs/api/send-otp-by-sms)
 - [x] [WhatsApp passcodes](https://stytch.com/docs/api/whatsapp-send)
 - [x] [Email passcodes](https://stytch.com/docs/api/send-otp-by-email)
 - [x] [Session Management](https://stytch.com/docs/api/sessions-overview)
 - [x] [WebAuthn](https://stytch.com/docs/api/webauthn-overview)
 - [x] [Time-based one-time passcodes (TOTPs)](https://stytch.com/docs/api/totps-overview)
 - [x] [Crypto wallets](https://stytch.com/docs/api/crypto-wallet-overview)
-- [x] [Passwords (Beta)](https://stytch.com/docs/api/password-overview)
+- [x] [Passwords](https://stytch.com/docs/api/password-overview)
 
 ### Example usage
 
 Create an API client:
 
 ```python
 import stytch
```

### Comparing `stytch-6.7.0/README.md` & `stytch-6.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 - [x] [SMS passcodes](https://stytch.com/docs/api/send-otp-by-sms)
 - [x] [WhatsApp passcodes](https://stytch.com/docs/api/whatsapp-send)
 - [x] [Email passcodes](https://stytch.com/docs/api/send-otp-by-email)
 - [x] [Session Management](https://stytch.com/docs/api/sessions-overview)
 - [x] [WebAuthn](https://stytch.com/docs/api/webauthn-overview)
 - [x] [Time-based one-time passcodes (TOTPs)](https://stytch.com/docs/api/totps-overview)
 - [x] [Crypto wallets](https://stytch.com/docs/api/crypto-wallet-overview)
-- [x] [Passwords (Beta)](https://stytch.com/docs/api/password-overview)
+- [x] [Passwords](https://stytch.com/docs/api/password-overview)
 
 ### Example usage
 
 Create an API client:
 
 ```python
 import stytch
```

### Comparing `stytch-6.7.0/setup.py` & `stytch-6.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/crypto_wallets.py` & `stytch-6.7.1/stytch/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/magic_links.py` & `stytch-6.7.1/stytch/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/magic_links_email.py` & `stytch-6.7.1/stytch/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/oauth.py` & `stytch-6.7.1/stytch/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/otp.py` & `stytch-6.7.1/stytch/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/otp_email.py` & `stytch-6.7.1/stytch/api/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/otp_sms.py` & `stytch-6.7.1/stytch/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/otp_whatsapp.py` & `stytch-6.7.1/stytch/api/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/passwords.py` & `stytch-6.7.1/stytch/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/passwords_email.py` & `stytch-6.7.1/stytch/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/passwords_existing_password.py` & `stytch-6.7.1/stytch/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/passwords_session.py` & `stytch-6.7.1/stytch/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/sessions.py` & `stytch-6.7.1/stytch/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/totps.py` & `stytch-6.7.1/stytch/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/users.py` & `stytch-6.7.1/stytch/api/users.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/api/webauthn.py` & `stytch-6.7.1/stytch/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/b2b/api/magic_links.py` & `stytch-6.7.1/stytch/b2b/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/b2b/api/magic_links_email.py` & `stytch-6.7.1/stytch/b2b/api/magic_links_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,222 +26,248 @@
     def sub_url(self) -> str:
         return "magic_links/email"
 
     def login_or_signup(
         self,
         organization_id: str,
         email_address: str,
-        create_member_as_pending: Optional[bool] = None,
         login_redirect_url: Optional[str] = None,
         signup_redirect_url: Optional[str] = None,
         pkce_code_challenge: Optional[str] = None,
         login_template_id: Optional[str] = None,
         signup_template_id: Optional[str] = None,
+        locale: Optional[str] = None,
     ) -> LoginOrSignupResponse:
         """Send either a login or signup magic link to a Member. A new or pending Member will receive a signup Email Magic Link. An active Member will receive a login Email Magic Link.
 
         Parameters:
 
         - `organization_id`: Globally unique UUID that identifies a specific Organization. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
 
         - `email_address`: The email of the Member who will receive the Email Magic Link for login or signup.
 
-        - `create_member_as_pending`: Flag for whether or not to save a Member as pending vs active in Stytch. Defaults to false. If true, new Members will be created with status pending in Stytch's backend. Their status will remain pending and they will continue to receive sign-up magic links until a magic link is authenticated for that Member. If false, new Members will be created with status active. They will receive a sign-up magic link for their first magic link but subsequent magic links will use the login email template, even if the Member never authenticated their initial magic link.
-
         - `login_redirect_url`: The URL that Member clicks from the login email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default login redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
 
         - `signup_redirect_url`: The url the Member clicks from the sign-up email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default sign-up redirect URL that you set in your Dashboard is used. If you have not set a default sign-up redirect URL, an error is returned.
 
         - `pkce_code_challenge`: A base64url encoded SHA256 hash of a one time secret used to validate that the request starts and ends on the same device. See the PKCE OAuth guide for usage instructions.
 
         - `login_template_id`: Use a custom template for login emails. By default, it will use your default email template The template must be a template using our built-in customizations or a custom HTML email for Magic links - Login.
 
         - `signup_template_id`: Use a custom template for sign-up emails. By default, it will use your default email template. The template must be a template using our built-in customizations or a custom HTML email for Magic links - Sign-up.
+
+        - `locale`: Used to determine which language to use when sending the user this delivery method. Parameter is a two character [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"` or `"es"`.
+
+          Currently supported languages are English (en) and Spanish (es); if no value is provided, the copy defaults to English.
+
+          Request more languages for support [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link)!
         """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
 
-        if create_member_as_pending is not None:
-            payload["create_member_as_pending"] = create_member_as_pending
         if login_redirect_url is not None:
             payload["login_redirect_url"] = login_redirect_url
         if signup_redirect_url is not None:
             payload["signup_redirect_url"] = signup_redirect_url
         if pkce_code_challenge is not None:
             payload["pkce_code_challenge"] = pkce_code_challenge
         if login_template_id is not None:
             payload["login_template_id"] = login_template_id
         if signup_template_id is not None:
             payload["signup_template_id"] = signup_template_id
+        if locale is not None:
+            payload["locale"] = locale
 
         url = self.api_base.route_with_sub_url(self.sub_url, "login_or_signup")
 
         res = self.sync_client.post(url, json=payload)
         return LoginOrSignupResponse.from_json(res.response.status_code, res.json)
 
     async def login_or_signup_async(
         self,
         organization_id: str,
         email_address: str,
-        create_member_as_pending: Optional[bool] = None,
         login_redirect_url: Optional[str] = None,
         signup_redirect_url: Optional[str] = None,
         pkce_code_challenge: Optional[str] = None,
         login_template_id: Optional[str] = None,
         signup_template_id: Optional[str] = None,
+        locale: Optional[str] = None,
     ) -> LoginOrSignupResponse:
         """Send either a login or signup magic link to a Member. A new or pending Member will receive a signup Email Magic Link. An active Member will receive a login Email Magic Link.
 
         Parameters:
 
         - `organization_id`: Globally unique UUID that identifies a specific Organization. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
 
         - `email_address`: The email of the Member who will receive the Email Magic Link for login or signup.
 
-        - `create_member_as_pending`: Flag for whether or not to save a Member as pending vs active in Stytch. Defaults to false. If true, new Members will be created with status pending in Stytch's backend. Their status will remain pending and they will continue to receive sign-up magic links until a magic link is authenticated for that Member. If false, new Members will be created with status active. They will receive a sign-up magic link for their first magic link but subsequent magic links will use the login email template, even if the Member never authenticated their initial magic link.
-
         - `login_redirect_url`: The URL that Member clicks from the login email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default login redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
 
         - `signup_redirect_url`: The url the Member clicks from the sign-up email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default sign-up redirect URL that you set in your Dashboard is used. If you have not set a default sign-up redirect URL, an error is returned.
 
         - `pkce_code_challenge`: A base64url encoded SHA256 hash of a one time secret used to validate that the request starts and ends on the same device. See the PKCE OAuth guide for usage instructions.
 
         - `login_template_id`: Use a custom template for login emails. By default, it will use your default email template The template must be a template using our built-in customizations or a custom HTML email for Magic links - Login.
 
         - `signup_template_id`: Use a custom template for sign-up emails. By default, it will use your default email template. The template must be a template using our built-in customizations or a custom HTML email for Magic links - Sign-up.
+
+        - `locale`: Used to determine which language to use when sending the user this delivery method. Parameter is a two character [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"` or `"es"`.
+
+          Currently supported languages are English (en) and Spanish (es); if no value is provided, the copy defaults to English.
+
+          Request more languages for support [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link)!
         """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
 
-        if create_member_as_pending is not None:
-            payload["create_member_as_pending"] = create_member_as_pending
         if login_redirect_url is not None:
             payload["login_redirect_url"] = login_redirect_url
         if signup_redirect_url is not None:
             payload["signup_redirect_url"] = signup_redirect_url
         if pkce_code_challenge is not None:
             payload["pkce_code_challenge"] = pkce_code_challenge
         if login_template_id is not None:
             payload["login_template_id"] = login_template_id
         if signup_template_id is not None:
             payload["signup_template_id"] = signup_template_id
+        if locale is not None:
+            payload["locale"] = locale
 
         url = self.api_base.route_with_sub_url(self.sub_url, "login_or_signup")
 
         res = await self.async_client.post(url, json=payload)
         return LoginOrSignupResponse.from_json(res.response.status, res.json)
 
     def invite(
         self,
         organization_id: str,
         email_address: str,
         invite_redirect_url: Optional[str] = None,
-        invite_by_member_id: Optional[str] = None,
+        invited_by_member_id: Optional[str] = None,
         name: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
         invite_template_id: Optional[str] = None,
+        locale: Optional[str] = None,
     ) -> InviteResponse:
         """Send an invite email to a new Member to join an Organization. The Member will be created with a pending status until they successfully authenticate.
 
         Parameters:
 
         - `organization_id`: Globally unique UUID that identifies a specific Organization in the Stytch API. The organization_id is critical to perform operations on an Organization so be sure to preserve this value.
 
         - `email_address`: The email address of the Member.
 
         - `invite_redirect_url`: The URL that Members click from the login email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default login redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
 
-        - `invite_by_member_id`: The member_id of the Member who sent the invite.
+        - `invited_by_member_id`: The member_id of the Member who sent the invite.
 
         - `name`: The name of the invited Member.
 
         - `trusted_metadata`: An arbitrary JSON object for storing application-specific or identity-provider-specific data.
 
-        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the Metadata reference for complete field behavior details.
+        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for complete field behavior details.
 
         - `invite_template_id`: Use a custom template for invite emails. By default, it will use your default email template. The template must be a template using our built-in customizations or a custom HTML email for Magic links - Invite.
+
+        - `locale`: Used to determine which language to use when sending the user this delivery method. Parameter is a two character [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"` or `"es"`.
+
+          Currently supported languages are English (en) and Spanish (es); if no value is provided, the copy defaults to English.
+
+          Request more languages for support [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link)!
         """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
 
         if invite_redirect_url is not None:
             payload["invite_redirect_url"] = invite_redirect_url
-        if invite_by_member_id is not None:
-            payload["invite_by_member_id"] = invite_by_member_id
+        if invited_by_member_id is not None:
+            payload["invited_by_member_id"] = invited_by_member_id
         if name is not None:
             payload["name"] = name
         if trusted_metadata is not None:
             payload["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             payload["untrusted_metadata"] = untrusted_metadata
         if invite_template_id is not None:
             payload["invite_template_id"] = invite_template_id
+        if locale is not None:
+            payload["locale"] = locale
 
         url = self.api_base.route_with_sub_url(self.sub_url, "invite")
 
         res = self.sync_client.post(url, json=payload)
         return InviteResponse.from_json(res.response.status_code, res.json)
 
     async def invite_async(
         self,
         organization_id: str,
         email_address: str,
         invite_redirect_url: Optional[str] = None,
-        invite_by_member_id: Optional[str] = None,
+        invited_by_member_id: Optional[str] = None,
         name: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
         invite_template_id: Optional[str] = None,
+        locale: Optional[str] = None,
     ) -> InviteResponse:
         """Send an invite email to a new Member to join an Organization. The Member will be created with a pending status until they successfully authenticate.
 
         Parameters:
 
         - `organization_id`: Globally unique UUID that identifies a specific Organization in the Stytch API. The organization_id is critical to perform operations on an Organization so be sure to preserve this value.
 
         - `email_address`: The email address of the Member.
 
         - `invite_redirect_url`: The URL that Members click from the login email magic link. This URL should be an endpoint in the backend server that verifies the request by querying Stytch's authenticate endpoint and finishes the login. If this value is not passed, the default login redirect URL that you set in your Dashboard is used. If you have not set a default login redirect URL, an error is returned.
 
-        - `invite_by_member_id`: The member_id of the Member who sent the invite.
+        - `invited_by_member_id`: The member_id of the Member who sent the invite.
 
         - `name`: The name of the invited Member.
 
         - `trusted_metadata`: An arbitrary JSON object for storing application-specific or identity-provider-specific data.
 
-        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the Metadata reference for complete field behavior details.
+        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for complete field behavior details.
 
         - `invite_template_id`: Use a custom template for invite emails. By default, it will use your default email template. The template must be a template using our built-in customizations or a custom HTML email for Magic links - Invite.
+
+        - `locale`: Used to determine which language to use when sending the user this delivery method. Parameter is a two character [IETF BCP 47 language tag](https://www.w3.org/International/articles/language-tags/), e.g. `"en"` or `"es"`.
+
+          Currently supported languages are English (en) and Spanish (es); if no value is provided, the copy defaults to English.
+
+          Request more languages for support [here](https://docs.google.com/forms/d/e/1FAIpQLScZSpAu_m2AmLXRT3F3kap-s_mcV6UTBitYn6CdyWP0-o7YjQ/viewform?usp=sf_link)!
         """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
 
         if invite_redirect_url is not None:
             payload["invite_redirect_url"] = invite_redirect_url
-        if invite_by_member_id is not None:
-            payload["invite_by_member_id"] = invite_by_member_id
+        if invited_by_member_id is not None:
+            payload["invited_by_member_id"] = invited_by_member_id
         if name is not None:
             payload["name"] = name
         if trusted_metadata is not None:
             payload["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             payload["untrusted_metadata"] = untrusted_metadata
         if invite_template_id is not None:
             payload["invite_template_id"] = invite_template_id
+        if locale is not None:
+            payload["locale"] = locale
 
         url = self.api_base.route_with_sub_url(self.sub_url, "invite")
 
         res = await self.async_client.post(url, json=payload)
         return InviteResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-6.7.0/stytch/b2b/api/organizations.py` & `stytch-6.7.1/stytch/b2b/api/organizations.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 # !!!
 
 from typing import Any, Dict, List, Optional
 
 import pydantic
 
 from stytch.b2b.models.organizations import (
+    CreateMemberResponse,
     CreateResponse,
     DeleteMemberPasswordResponse,
     DeleteMemberResponse,
     DeleteResponse,
     GetMemberResponse,
     GetResponse,
     SearchMembersResponse,
     SearchResponse,
+    UpdateMemberResponse,
     UpdateResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 from stytch.core.models import SearchQuery
 
 
@@ -39,132 +41,162 @@
     def sub_url(self) -> str:
         return "organizations"
 
     def create(
         self,
         organization_name: str,
         organization_slug: str,
+        organization_logo_url: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         email_allowed_domains: Optional[List[str]] = None,
         sso_jit_provisioning: Optional[str] = None,
+        auth_methods: Optional[str] = None,
+        allowed_auth_methods: Optional[List[str]] = None,
     ) -> CreateResponse:
         """Creates a new Organization. It requires a name and a unique slug.
 
-        See the Organization authentication settings resource to learn more about fields like email_jit_provisioning, email_allowed_domains, sso_jit_provisioning, etc., and their behaviors.
+        See the [Organization authentication settings resource](https://stytch.com/docs/b2b/api/org-auth-settings) to learn more about fields like `email_jit_provisioning`, `email_allowed_domains`, `sso_jit_provisioning`, etc., and their behaviors.
 
         Parameters:
 
         - `organization_name`: The name of the Organization.
 
         - `organization_slug`: The unique URL slug of the Organization.
 
-        - `organzation_logo_url`: The image URL of the Organization’s logo.
+        - `organization_logo_url`: The image URL of the Organization’s logo.
 
         - `trusted_metadata`: An arbitrary JSON object for storing application-specific data.
 
         - `email_jit_provisioning`: The setting that controls the JIT provisioning of new Members when authenticating via email. The accepted values are:
 
-          - RESTRICTED – only new Members with verified emails that comply with email_allowed_domains can be provisioned upon authentication.
+          - RESTRICTED – only new Members with verified emails that comply with `email_allowed_domains` can be provisioned upon authentication.
           - NOT_ALLOWED – disable JIT provisioning.
 
         - `email_invites`: The setting that controls how a new Member can be invited to an organization by email. The accepted values are:
 
           - ALL_ALLOWED – any new Member can be invited to join
-          - RESTRICTED – only new Members with verified emails that comply with email_allowed_domains can be invited
+          - RESTRICTED – only new Members with verified emails that comply with `email_allowed_domains` can be invited
           - NOT_ALLOWED – disable invites
 
         - `email_allowed_domains`: An array of email domains that allow invitations or JIT provisioning for new Members. This list is enforced when either email_invites or email_jit_provisioning is set to RESTRICTED.
 
         - `sso_jit_provisioning`: The setting that controls the JIT provisioning of Members when authenticating via SSO. The accepted values are:
           - ALL_ALLOWED – any new Member can be provisioned upon authentication
-          - RESTRICTED – only new Members with SSO logins that comply with sso_jit_provisioning_allowed_connections can be provisioned upon authentication
+          - RESTRICTED – only new Members with SSO logins that comply with `sso_jit_provisioning_allowed_connections` can be provisioned upon authentication
           - NOT_ALLOWED – disable JIT provisioning
+
+        - `auth_methods`: The setting that controls which authentication methods can be used by Members of an Organization. The accepted values are:
+          - ALL_ALLOWED – the default setting which allows all authentication methods to be used.
+          - RESTRICTED - only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
+
+        - `allowed_auth_methods`: An array of allowed authentication methods. This list is enforced when auth_methods is set to RESTRICTED. The list's accepted values are: `sso`, `magic_link`, and `password`.
         """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_name": organization_name,
             "organization_slug": organization_slug,
         }
 
+        if organization_logo_url is not None:
+            payload["organization_logo_url"] = organization_logo_url
         if trusted_metadata is not None:
             payload["trusted_metadata"] = trusted_metadata
         if email_jit_provisioning is not None:
             payload["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
             payload["email_invites"] = email_invites
         if email_allowed_domains is not None:
             payload["email_allowed_domains"] = email_allowed_domains
         if sso_jit_provisioning is not None:
             payload["sso_jit_provisioning"] = sso_jit_provisioning
+        if auth_methods is not None:
+            payload["auth_methods"] = auth_methods
+        if allowed_auth_methods is not None:
+            payload["allowed_auth_methods"] = allowed_auth_methods
 
         url = self.api_base.route_with_sub_url(self.sub_url, None)
 
         res = self.sync_client.post(url, json=payload)
         return CreateResponse.from_json(res.response.status_code, res.json)
 
     async def create_async(
         self,
         organization_name: str,
         organization_slug: str,
+        organization_logo_url: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         email_allowed_domains: Optional[List[str]] = None,
         sso_jit_provisioning: Optional[str] = None,
+        auth_methods: Optional[str] = None,
+        allowed_auth_methods: Optional[List[str]] = None,
     ) -> CreateResponse:
         """Creates a new Organization. It requires a name and a unique slug.
 
-        See the Organization authentication settings resource to learn more about fields like email_jit_provisioning, email_allowed_domains, sso_jit_provisioning, etc., and their behaviors.
+        See the [Organization authentication settings resource](https://stytch.com/docs/b2b/api/org-auth-settings) to learn more about fields like `email_jit_provisioning`, `email_allowed_domains`, `sso_jit_provisioning`, etc., and their behaviors.
 
         Parameters:
 
         - `organization_name`: The name of the Organization.
 
         - `organization_slug`: The unique URL slug of the Organization.
 
-        - `organzation_logo_url`: The image URL of the Organization’s logo.
+        - `organization_logo_url`: The image URL of the Organization’s logo.
 
         - `trusted_metadata`: An arbitrary JSON object for storing application-specific data.
 
         - `email_jit_provisioning`: The setting that controls the JIT provisioning of new Members when authenticating via email. The accepted values are:
 
-          - RESTRICTED – only new Members with verified emails that comply with email_allowed_domains can be provisioned upon authentication.
+          - RESTRICTED – only new Members with verified emails that comply with `email_allowed_domains` can be provisioned upon authentication.
           - NOT_ALLOWED – disable JIT provisioning.
 
         - `email_invites`: The setting that controls how a new Member can be invited to an organization by email. The accepted values are:
 
           - ALL_ALLOWED – any new Member can be invited to join
-          - RESTRICTED – only new Members with verified emails that comply with email_allowed_domains can be invited
+          - RESTRICTED – only new Members with verified emails that comply with `email_allowed_domains` can be invited
           - NOT_ALLOWED – disable invites
 
         - `email_allowed_domains`: An array of email domains that allow invitations or JIT provisioning for new Members. This list is enforced when either email_invites or email_jit_provisioning is set to RESTRICTED.
 
         - `sso_jit_provisioning`: The setting that controls the JIT provisioning of Members when authenticating via SSO. The accepted values are:
           - ALL_ALLOWED – any new Member can be provisioned upon authentication
-          - RESTRICTED – only new Members with SSO logins that comply with sso_jit_provisioning_allowed_connections can be provisioned upon authentication
+          - RESTRICTED – only new Members with SSO logins that comply with `sso_jit_provisioning_allowed_connections` can be provisioned upon authentication
           - NOT_ALLOWED – disable JIT provisioning
+
+        - `auth_methods`: The setting that controls which authentication methods can be used by Members of an Organization. The accepted values are:
+          - ALL_ALLOWED – the default setting which allows all authentication methods to be used.
+          - RESTRICTED - only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
+
+        - `allowed_auth_methods`: An array of allowed authentication methods. This list is enforced when auth_methods is set to RESTRICTED. The list's accepted values are: `sso`, `magic_link`, and `password`.
         """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_name": organization_name,
             "organization_slug": organization_slug,
         }
 
+        if organization_logo_url is not None:
+            payload["organization_logo_url"] = organization_logo_url
         if trusted_metadata is not None:
             payload["trusted_metadata"] = trusted_metadata
         if email_jit_provisioning is not None:
             payload["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
             payload["email_invites"] = email_invites
         if email_allowed_domains is not None:
             payload["email_allowed_domains"] = email_allowed_domains
         if sso_jit_provisioning is not None:
             payload["sso_jit_provisioning"] = sso_jit_provisioning
+        if auth_methods is not None:
+            payload["auth_methods"] = auth_methods
+        if allowed_auth_methods is not None:
+            payload["allowed_auth_methods"] = allowed_auth_methods
 
         url = self.api_base.route_with_sub_url(self.sub_url, None)
 
         res = await self.async_client.post(url, json=payload)
         return CreateResponse.from_json(res.response.status, res.json)
 
     def get(
@@ -216,18 +248,20 @@
         trusted_metadata: Optional[Dict[str, Any]] = None,
         sso_default_connection_id: Optional[str] = None,
         sso_jit_provisioning_allowed_connections: Optional[List[str]] = None,
         sso_jit_provisioning: Optional[str] = None,
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
+        auth_methods: Optional[str] = None,
+        allowed_auth_methods: Optional[List[str]] = None,
     ) -> UpdateResponse:
-        """Updates an Organization specified by organization_id.
+        """Updates an Organization specified by `organization_id`.
 
-        See the Organization authentication settings resource to learn more about fields like email_jit_provisioning, email_allowed_domains, sso_jit_provisioning, etc., and their behaviors.
+        See the [Organization authentication settings resource](https://stytch.com/docs/b2b/api/org-auth-settings) to learn more about fields like `email_jit_provisioning`, `email_allowed_domains`, `sso_jit_provisioning`, etc., and their behaviors.
 
         Parameters:
 
         - `organization_id`: Globally unique UUID that identifies a specific Organization. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
 
         - `organization_name`: The name of the Organization.
 
@@ -235,15 +269,15 @@
 
         - `organization_logo_url`: The image URL of the Organization’s logo.
 
         - `trusted_metadata`: An arbitrary JSON object for storing application-specific data.
 
         - `sso_default_connection_id`: The default connection used for SSO when there are multiple active connections.
 
-        - `sso_jit_provisioning_allowed_connections`: An array of connections used for SSO when sso_jit_provisiniong is set to RESTRICTED.
+        - `sso_jit_provisioning_allowed_connections`: An array of connections used for SSO when `sso_jit_provisioniong` is set to RESTRICTED.
 
         - `sso_jit_provisioning`: The setting that controls the JIT provisioning of Members when authenticating via SSO. The accepted values are:
 
           - ALL_ALLOWED – any new Member can be provisioned upon authentication
           - RESTRICTED – only new Members with SSO logins that comply with sso_jit_provisioning_allowed_connections can be provisioned upon authentication
           - NOT_ALLOWED – disable JIT provisioning
 
@@ -254,14 +288,20 @@
           - RESTRICTED – only new Members with verified emails that comply with email_allowed_domains can be provisioned upon authentication
           - NOT_ALLOWED – disable JIT provisioning
 
         - `email_invites`: The setting that controls how a new Member can be invited to an Organization by email. The three accepted values are:
           - ALL_ALLOWED – any new Member can be invited to join
           - RESTRICTED – only new Members with verified emails that comply with email_allowed_domains can be invited
           - NOT_ALLOWED – disable invites
+
+        - `auth_methods`: The setting that controls which authentication methods can be used by Members of an Organization. The accepted values are:
+          - ALL_ALLOWED – the default setting which allows all authentication methods to be used.
+          - RESTRICTED - only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
+
+        - `allowed_auth_methods`: An array of allowed authentication methods. This list is enforced when auth_methods is set to RESTRICTED. The list's accepted values are: `sso`, `magic_link`, and `password`.
         """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_id": organization_id,
         }
 
         if organization_name is not None:
@@ -282,14 +322,18 @@
             payload["sso_jit_provisioning"] = sso_jit_provisioning
         if email_allowed_domains is not None:
             payload["email_allowed_domains"] = email_allowed_domains
         if email_jit_provisioning is not None:
             payload["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
             payload["email_invites"] = email_invites
+        if auth_methods is not None:
+            payload["auth_methods"] = auth_methods
+        if allowed_auth_methods is not None:
+            payload["allowed_auth_methods"] = allowed_auth_methods
 
         url = self.api_base.route_with_sub_url(self.sub_url, organization_id)
 
         res = self.sync_client.put(url, json=payload)
         return UpdateResponse.from_json(res.response.status_code, res.json)
 
     async def update_async(
@@ -301,18 +345,20 @@
         trusted_metadata: Optional[Dict[str, Any]] = None,
         sso_default_connection_id: Optional[str] = None,
         sso_jit_provisioning_allowed_connections: Optional[List[str]] = None,
         sso_jit_provisioning: Optional[str] = None,
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
+        auth_methods: Optional[str] = None,
+        allowed_auth_methods: Optional[List[str]] = None,
     ) -> UpdateResponse:
-        """Updates an Organization specified by organization_id.
+        """Updates an Organization specified by `organization_id`.
 
-        See the Organization authentication settings resource to learn more about fields like email_jit_provisioning, email_allowed_domains, sso_jit_provisioning, etc., and their behaviors.
+        See the [Organization authentication settings resource](https://stytch.com/docs/b2b/api/org-auth-settings) to learn more about fields like `email_jit_provisioning`, `email_allowed_domains`, `sso_jit_provisioning`, etc., and their behaviors.
 
         Parameters:
 
         - `organization_id`: Globally unique UUID that identifies a specific Organization. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
 
         - `organization_name`: The name of the Organization.
 
@@ -320,15 +366,15 @@
 
         - `organization_logo_url`: The image URL of the Organization’s logo.
 
         - `trusted_metadata`: An arbitrary JSON object for storing application-specific data.
 
         - `sso_default_connection_id`: The default connection used for SSO when there are multiple active connections.
 
-        - `sso_jit_provisioning_allowed_connections`: An array of connections used for SSO when sso_jit_provisiniong is set to RESTRICTED.
+        - `sso_jit_provisioning_allowed_connections`: An array of connections used for SSO when `sso_jit_provisioniong` is set to RESTRICTED.
 
         - `sso_jit_provisioning`: The setting that controls the JIT provisioning of Members when authenticating via SSO. The accepted values are:
 
           - ALL_ALLOWED – any new Member can be provisioned upon authentication
           - RESTRICTED – only new Members with SSO logins that comply with sso_jit_provisioning_allowed_connections can be provisioned upon authentication
           - NOT_ALLOWED – disable JIT provisioning
 
@@ -339,14 +385,20 @@
           - RESTRICTED – only new Members with verified emails that comply with email_allowed_domains can be provisioned upon authentication
           - NOT_ALLOWED – disable JIT provisioning
 
         - `email_invites`: The setting that controls how a new Member can be invited to an Organization by email. The three accepted values are:
           - ALL_ALLOWED – any new Member can be invited to join
           - RESTRICTED – only new Members with verified emails that comply with email_allowed_domains can be invited
           - NOT_ALLOWED – disable invites
+
+        - `auth_methods`: The setting that controls which authentication methods can be used by Members of an Organization. The accepted values are:
+          - ALL_ALLOWED – the default setting which allows all authentication methods to be used.
+          - RESTRICTED - only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
+
+        - `allowed_auth_methods`: An array of allowed authentication methods. This list is enforced when auth_methods is set to RESTRICTED. The list's accepted values are: `sso`, `magic_link`, and `password`.
         """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_id": organization_id,
         }
 
         if organization_name is not None:
@@ -367,14 +419,18 @@
             payload["sso_jit_provisioning"] = sso_jit_provisioning
         if email_allowed_domains is not None:
             payload["email_allowed_domains"] = email_allowed_domains
         if email_jit_provisioning is not None:
             payload["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
             payload["email_invites"] = email_invites
+        if auth_methods is not None:
+            payload["auth_methods"] = auth_methods
+        if allowed_auth_methods is not None:
+            payload["allowed_auth_methods"] = allowed_auth_methods
 
         url = self.api_base.route_with_sub_url(self.sub_url, organization_id)
 
         res = await self.async_client.put(url, json=payload)
         return UpdateResponse.from_json(res.response.status, res.json)
 
     def delete(
@@ -411,14 +467,24 @@
 
     def get_member(
         self,
         organization_id: str,
         member_id: Optional[str] = None,
         email_address: Optional[str] = None,
     ) -> GetMemberResponse:
+        """Gets a Member by `member_id` or `email_address`.
+
+        Parameters:
+
+        - `organization_id`: The UUID of the Organization that the Member belongs to.
+
+        - `member_id`: The UUID of the Member.
+
+        - `email_address`: The email address of the Member.
+        """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_id": organization_id,
         }
 
         if member_id is not None:
             payload["member_id"] = member_id
@@ -434,14 +500,24 @@
 
     async def get_member_async(
         self,
         organization_id: str,
         member_id: Optional[str] = None,
         email_address: Optional[str] = None,
     ) -> GetMemberResponse:
+        """Gets a Member by `member_id` or `email_address`.
+
+        Parameters:
+
+        - `organization_id`: The UUID of the Organization that the Member belongs to.
+
+        - `member_id`: The UUID of the Member.
+
+        - `email_address`: The email address of the Member.
+        """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_id": organization_id,
         }
 
         if member_id is not None:
             payload["member_id"] = member_id
@@ -451,14 +527,212 @@
         url = self.api_base.route_with_sub_url(
             self.sub_url, f"{organization_id}/member"
         )
 
         res = await self.async_client.get(url, params=payload)
         return GetMemberResponse.from_json(res.response.status, res.json)
 
+    def create_member(
+        self,
+        organization_id: str,
+        email_address: str,
+        name: Optional[str] = None,
+        trusted_metadata: Optional[Dict[str, Any]] = None,
+        untrusted_metadata: Optional[Dict[str, Any]] = None,
+        create_member_as_pending: Optional[bool] = None,
+        is_breakglass: Optional[bool] = None,
+    ) -> CreateMemberResponse:
+        """Creates a Member. An `organization_id` and `email_address` are required.
+
+        Parameters:
+
+        - `organization_id`: The UUID of the Organization that the Member should be created within.
+
+        - `email_address`: The email address of the Member.
+
+        - `name`: The name of the Member.
+
+        - `trusted_metadata`: An arbitrary JSON object for storing application-specific or identity-provider-specific data.
+
+        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for complete field behavior details.
+
+        - `create_member_as_pending`: Flag for whether to save a Member as `pending` or `active` in Stytch. It defaults to false. If true, new Members will be created with status `pending` in Stytch's backend. Their status will remain `pending` and they will continue to receive signup email templates for every Email Magic Link until that Member authenticates and becomes `active`. If false, new Members will be created with status `active`.
+
+        - `is_breakglass`: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](https://stytch.com/docs/b2b/api/organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
+        """  # noqa
+
+        payload: Dict[str, Any] = {
+            "organization_id": organization_id,
+            "email_address": email_address,
+        }
+
+        if name is not None:
+            payload["name"] = name
+        if trusted_metadata is not None:
+            payload["trusted_metadata"] = trusted_metadata
+        if untrusted_metadata is not None:
+            payload["untrusted_metadata"] = untrusted_metadata
+        if create_member_as_pending is not None:
+            payload["create_member_as_pending"] = create_member_as_pending
+        if is_breakglass is not None:
+            payload["is_breakglass"] = is_breakglass
+
+        url = self.api_base.route_with_sub_url(
+            self.sub_url, f"{organization_id}/members"
+        )
+
+        res = self.sync_client.post(url, json=payload)
+        return CreateMemberResponse.from_json(res.response.status_code, res.json)
+
+    async def create_member_async(
+        self,
+        organization_id: str,
+        email_address: str,
+        name: Optional[str] = None,
+        trusted_metadata: Optional[Dict[str, Any]] = None,
+        untrusted_metadata: Optional[Dict[str, Any]] = None,
+        create_member_as_pending: Optional[bool] = None,
+        is_breakglass: Optional[bool] = None,
+    ) -> CreateMemberResponse:
+        """Creates a Member. An `organization_id` and `email_address` are required.
+
+        Parameters:
+
+        - `organization_id`: The UUID of the Organization that the Member should be created within.
+
+        - `email_address`: The email address of the Member.
+
+        - `name`: The name of the Member.
+
+        - `trusted_metadata`: An arbitrary JSON object for storing application-specific or identity-provider-specific data.
+
+        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for complete field behavior details.
+
+        - `create_member_as_pending`: Flag for whether to save a Member as `pending` or `active` in Stytch. It defaults to false. If true, new Members will be created with status `pending` in Stytch's backend. Their status will remain `pending` and they will continue to receive signup email templates for every Email Magic Link until that Member authenticates and becomes `active`. If false, new Members will be created with status `active`.
+
+        - `is_breakglass`: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](https://stytch.com/docs/b2b/api/organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
+        """  # noqa
+
+        payload: Dict[str, Any] = {
+            "organization_id": organization_id,
+            "email_address": email_address,
+        }
+
+        if name is not None:
+            payload["name"] = name
+        if trusted_metadata is not None:
+            payload["trusted_metadata"] = trusted_metadata
+        if untrusted_metadata is not None:
+            payload["untrusted_metadata"] = untrusted_metadata
+        if create_member_as_pending is not None:
+            payload["create_member_as_pending"] = create_member_as_pending
+        if is_breakglass is not None:
+            payload["is_breakglass"] = is_breakglass
+
+        url = self.api_base.route_with_sub_url(
+            self.sub_url, f"{organization_id}/members"
+        )
+
+        res = await self.async_client.post(url, json=payload)
+        return CreateMemberResponse.from_json(res.response.status, res.json)
+
+    def update_member(
+        self,
+        organization_id: str,
+        member_id: str,
+        name: Optional[str] = None,
+        trusted_metadata: Optional[Dict[str, Any]] = None,
+        untrusted_metadata: Optional[Dict[str, Any]] = None,
+        is_breakglass: Optional[bool] = None,
+    ) -> UpdateMemberResponse:
+        """Updates a member specified by `organization_id` and `member_id`.
+
+        Parameters:
+
+        - `organization_id`: The UUID of the Organization that the Member belongs to.
+
+        - `member_id`: The UUID of the Member.
+
+        - `name`: The new name of the Member.
+
+        - `trusted_metadata`: An arbitrary JSON object for storing application-specific or identity-provider-specific data. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for information on how metadata updates are handled.
+
+        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for complete field behavior details.
+
+        - `is_breakglass`: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](https://stytch.com/docs/b2b/api/organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
+        """  # noqa
+
+        payload: Dict[str, Any] = {
+            "organization_id": organization_id,
+            "member_id": member_id,
+        }
+
+        if name is not None:
+            payload["name"] = name
+        if trusted_metadata is not None:
+            payload["trusted_metadata"] = trusted_metadata
+        if untrusted_metadata is not None:
+            payload["untrusted_metadata"] = untrusted_metadata
+        if is_breakglass is not None:
+            payload["is_breakglass"] = is_breakglass
+
+        url = self.api_base.route_with_sub_url(
+            self.sub_url, f"{organization_id}/members/{member_id}"
+        )
+
+        res = self.sync_client.put(url, json=payload)
+        return UpdateMemberResponse.from_json(res.response.status_code, res.json)
+
+    async def update_member_async(
+        self,
+        organization_id: str,
+        member_id: str,
+        name: Optional[str] = None,
+        trusted_metadata: Optional[Dict[str, Any]] = None,
+        untrusted_metadata: Optional[Dict[str, Any]] = None,
+        is_breakglass: Optional[bool] = None,
+    ) -> UpdateMemberResponse:
+        """Updates a member specified by `organization_id` and `member_id`.
+
+        Parameters:
+
+        - `organization_id`: The UUID of the Organization that the Member belongs to.
+
+        - `member_id`: The UUID of the Member.
+
+        - `name`: The new name of the Member.
+
+        - `trusted_metadata`: An arbitrary JSON object for storing application-specific or identity-provider-specific data. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for information on how metadata updates are handled.
+
+        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for complete field behavior details.
+
+        - `is_breakglass`: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](https://stytch.com/docs/b2b/api/organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
+        """  # noqa
+
+        payload: Dict[str, Any] = {
+            "organization_id": organization_id,
+            "member_id": member_id,
+        }
+
+        if name is not None:
+            payload["name"] = name
+        if trusted_metadata is not None:
+            payload["trusted_metadata"] = trusted_metadata
+        if untrusted_metadata is not None:
+            payload["untrusted_metadata"] = untrusted_metadata
+        if is_breakglass is not None:
+            payload["is_breakglass"] = is_breakglass
+
+        url = self.api_base.route_with_sub_url(
+            self.sub_url, f"{organization_id}/members/{member_id}"
+        )
+
+        res = await self.async_client.put(url, json=payload)
+        return UpdateMemberResponse.from_json(res.response.status, res.json)
+
     def delete_member(
         self,
         organization_id: str,
         member_id: str,
     ) -> DeleteMemberResponse:
         """Deletes a Member from an Organization.
 
@@ -614,15 +888,15 @@
         limit: Optional[int] = None,
         query: Optional[SearchQuery] = None,
     ) -> SearchMembersResponse:
         """Search for members within an Organization. It requires an organization_id. Submitting an empty query returns all Members of an Organization.
 
         Parameters:
 
-        - `organization_ids`: List of globally unique UUIDs that identify specific Organizations. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
+        - `organization_ids`: List of organization IDs to search Members by. You must specify at least one Organization.
 
         - `cursor`: The cursor field allows you to paginate through your results. Each result array is limited to 1000 results, if your query returns more than 1000 results, you will need to paginate the responses using the cursor. If you receive a response that includes a non-null next_cursor in the results_metadata object, you should repeat the call, being sure to include all of the original fields, but pass in the next_cursor in the cursor field. Continue to make calls until the next_cursor in the response is null.
 
         - `limit`: The number of Organizations to return per page, the default is 100. A maximum of 1000 Members can be returned by a single request. If the total size of your result is greater than one page size, you must paginate the response. See the cursor field above.
 
         - `query`: The optional query object contains the operator, e.g. AND or OR, and the operands that will filter your Members. Only an operator is required, if you include no operands, no filtering will be applied. Similarly if you include no query object, no filtering is applied and we'll return all of your Members with no filtering applied.
         """  # noqa
@@ -652,15 +926,15 @@
         limit: Optional[int] = None,
         query: Optional[SearchQuery] = None,
     ) -> SearchMembersResponse:
         """Search for members within an Organization. It requires an organization_id. Submitting an empty query returns all Members of an Organization.
 
         Parameters:
 
-        - `organization_ids`: List of globally unique UUIDs that identify specific Organizations. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
+        - `organization_ids`: List of organization IDs to search Members by. You must specify at least one Organization.
 
         - `cursor`: The cursor field allows you to paginate through your results. Each result array is limited to 1000 results, if your query returns more than 1000 results, you will need to paginate the responses using the cursor. If you receive a response that includes a non-null next_cursor in the results_metadata object, you should repeat the call, being sure to include all of the original fields, but pass in the next_cursor in the cursor field. Continue to make calls until the next_cursor in the response is null.
 
         - `limit`: The number of Organizations to return per page, the default is 100. A maximum of 1000 Members can be returned by a single request. If the total size of your result is greater than one page size, you must paginate the response. See the cursor field above.
 
         - `query`: The optional query object contains the operator, e.g. AND or OR, and the operands that will filter your Members. Only an operator is required, if you include no operands, no filtering will be applied. Similarly if you include no query object, no filtering is applied and we'll return all of your Members with no filtering applied.
         """  # noqa
```

### Comparing `stytch-6.7.0/stytch/b2b/api/passwords.py` & `stytch-6.7.1/stytch/b2b/api/passwords.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,14 @@
         return AuthenticateResponse.from_json(res.response.status, res.json)
 
     def strength_check(
         self,
         password: str,
         email_address: Optional[str] = None,
     ) -> StrengthCheckResponse:
-
         payload: Dict[str, Any] = {
             "password": password,
         }
 
         if email_address is not None:
             payload["email_address"] = email_address
 
@@ -176,15 +175,14 @@
         return StrengthCheckResponse.from_json(res.response.status_code, res.json)
 
     async def strength_check_async(
         self,
         password: str,
         email_address: Optional[str] = None,
     ) -> StrengthCheckResponse:
-
         payload: Dict[str, Any] = {
             "password": password,
         }
 
         if email_address is not None:
             payload["email_address"] = email_address
 
@@ -227,15 +225,15 @@
 
         - `sha_1_config`: Optional parameters for SHA-1 hash types.
 
         - `name`: The name of the user. Each field in the name object is optional.
 
         - `trusted_metadata`: An arbitrary JSON object for storing application-specific or identity-provider-specific data.
 
-        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the Metadata reference for complete field behavior details.
+        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for complete field behavior details.
         """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
             "hash": hash,
             "hash_type": hash_type,
@@ -295,15 +293,15 @@
 
         - `sha_1_config`: Optional parameters for SHA-1 hash types.
 
         - `name`: The name of the user. Each field in the name object is optional.
 
         - `trusted_metadata`: An arbitrary JSON object for storing application-specific or identity-provider-specific data.
 
-        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the Metadata reference for complete field behavior details.
+        - `untrusted_metadata`: The untrusted_metadata field contains an arbitrary JSON object of application-specific data. Untrusted metadata can be edited by end Members directly via the SDK, and cannot be used to store critical information. See the [Metadata reference](https://stytch.com/docs/b2b/api/metadata) for complete field behavior details.
         """  # noqa
 
         payload: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
             "hash": hash,
             "hash_type": hash_type,
```

### Comparing `stytch-6.7.0/stytch/b2b/api/passwords_email.py` & `stytch-6.7.1/stytch/b2b/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/b2b/api/passwords_existing_password.py` & `stytch-6.7.1/stytch/b2b/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/b2b/api/passwords_session.py` & `stytch-6.7.1/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/b2b/api/sessions.py` & `stytch-6.7.1/stytch/b2b/api/sessions.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,17 +77,17 @@
     def authenticate(
         self,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
-        """Authenticates a Session. You may provide a JWT that needs to be refreshed and is expired according to its exp claim. A new JWT will be returned If both the signature and the underlying Session are still valid.
+        """Authenticates a Session. You may provide a JWT that needs to be refreshed and is expired according to its exp claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
 
-        This endpoint requires only one of either the session_jwt or session_token be included in the request. It will return an error if both are present.
+        This endpoint requires only one of either the `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
 
         Parameters:
 
         - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our session management guide.
 
         - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session Management guide.
 
@@ -115,17 +115,17 @@
     async def authenticate_async(
         self,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
     ) -> AuthenticateResponse:
-        """Authenticates a Session. You may provide a JWT that needs to be refreshed and is expired according to its exp claim. A new JWT will be returned If both the signature and the underlying Session are still valid.
+        """Authenticates a Session. You may provide a JWT that needs to be refreshed and is expired according to its exp claim. A new JWT will be returned if both the signature and the underlying Session are still valid.
 
-        This endpoint requires only one of either the session_jwt or session_token be included in the request. It will return an error if both are present.
+        This endpoint requires only one of either the `session_jwt` or `session_token` be included in the request. It will return an error if both are present.
 
         Parameters:
 
         - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our session management guide.
 
         - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session Management guide.
 
@@ -153,25 +153,25 @@
     def revoke(
         self,
         member_session_id: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         member_id: Optional[str] = None,
     ) -> RevokeResponse:
-        """Revoke a Session and immediately invalidate all its tokens. To revoke a specific Session, pass either the member_session_id, session_token, or session_jwt. To revoke all Sessions for a Member, pass the member_id. This endpoint requires exactly one body param to be included in the request. It will return an error if multiple are present.
+        """Revoke a Session and immediately invalidate all its tokens. To revoke a specific Session, pass either the `member_session_id`, `session_token`, or `session_jwt`. To revoke all Sessions for a Member, pass the `member_id`. This endpoint requires exactly one body param to be included in the request. It will return an error if multiple are present.
 
         Parameters:
 
-        - `member_session_id`: Globally unique UUID that identifies a specific Member’s Session.
+        - `member_session_id`: The UUID of the specific Member Session to revoke.
 
-        - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session Management guide.
+        - `session_token`: The `session_token` of the specific Member Session to revoke.
 
-        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
+        - `session_jwt`: The JSON Web Token (JWT) of the specific Member Session to revoke.
 
-        - `member_id`: Globally unique UUID that identifies a specific Member. The member_id is critical to perform operations on a Member, so be sure to preserve this value.
+        - `member_id`: The UUID of the Member to revoke all sessions for.
         """  # noqa
 
         payload: Dict[str, Any] = {}
 
         if member_session_id is not None:
             payload["member_session_id"] = member_session_id
         if session_token is not None:
@@ -189,25 +189,25 @@
     async def revoke_async(
         self,
         member_session_id: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         member_id: Optional[str] = None,
     ) -> RevokeResponse:
-        """Revoke a Session and immediately invalidate all its tokens. To revoke a specific Session, pass either the member_session_id, session_token, or session_jwt. To revoke all Sessions for a Member, pass the member_id. This endpoint requires exactly one body param to be included in the request. It will return an error if multiple are present.
+        """Revoke a Session and immediately invalidate all its tokens. To revoke a specific Session, pass either the `member_session_id`, `session_token`, or `session_jwt`. To revoke all Sessions for a Member, pass the `member_id`. This endpoint requires exactly one body param to be included in the request. It will return an error if multiple are present.
 
         Parameters:
 
-        - `member_session_id`: Globally unique UUID that identifies a specific Member’s Session.
+        - `member_session_id`: The UUID of the specific Member Session to revoke.
 
-        - `session_token`: A secret token for a given Stytch Session. Read more about session_token in our Session Management guide.
+        - `session_token`: The `session_token` of the specific Member Session to revoke.
 
-        - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our Session management guide.
+        - `session_jwt`: The JSON Web Token (JWT) of the specific Member Session to revoke.
 
-        - `member_id`: Globally unique UUID that identifies a specific Member. The member_id is critical to perform operations on a Member, so be sure to preserve this value.
+        - `member_id`: The UUID of the Member to revoke all sessions for.
         """  # noqa
 
         payload: Dict[str, Any] = {}
 
         if member_session_id is not None:
             payload["member_session_id"] = member_session_id
         if session_token is not None:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stytch-6.7.0/stytch/b2b/client.py` & `stytch-6.7.1/stytch/b2b/client.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/b2b/core/models.py` & `stytch-6.7.1/stytch/b2b/core/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,34 @@
 
 import datetime
 from typing import Any, Dict, List, Optional
 
 import pydantic
 
 
+class ActiveSSOConnection(pydantic.BaseModel):
+    connection_id: str
+    display_name: str
+
+
 class Organization(pydantic.BaseModel):
     organization_id: str
     organization_name: str
     organization_slug: str
     organization_logo_url: str
     trusted_metadata: Dict[str, Any]
     sso_default_connection_id: Optional[str]
     sso_jit_provisioning_allowed_connections: List[str]
+    sso_active_connections: List[ActiveSSOConnection]
     sso_jit_provisioning: str
     email_allowed_domains: List[str]
     email_jit_provisioning: str
     email_invites: str
+    auth_methods: str
+    allowed_auth_methods: List[str]
 
 
 class SSORegistration(pydantic.BaseModel):
     connection_id: str
     identity_provider: str
     external_id: str
     registration_id: str
@@ -33,14 +41,18 @@
 class Member(pydantic.BaseModel):
     organization_id: str
     member_id: str
     email_address: str
     status: str
     name: str
     sso_registrations: List[SSORegistration]
+    trusted_metadata: Dict[str, Any]
+    untrusted_metadata: Dict[str, Any]
+    is_breakglass: bool
+    member_password_id: str
 
 
 class B2BStytchSession(pydantic.BaseModel):
     member_session_id: str
     member_id: str
     started_at: datetime.datetime
     last_accessed_at: datetime.datetime
```

### Comparing `stytch-6.7.0/stytch/b2b/models/magic_links.py` & `stytch-6.7.1/stytch/b2b/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/b2b/models/magic_links_email.py` & `stytch-6.7.1/stytch/b2b/models/magic_links_email.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 #!/usr/bin/env python3
 
 
-from stytch.b2b.core.models import Member
+from stytch.b2b.core.models import Member, Organization
 from stytch.core.models import ResponseBase
 
 
 class LoginOrSignupResponse(ResponseBase):
     """Response fields beyond those defined in `ResponseBase`:
 
     - `member_id`: Globally unique UUID that identifies a specific Member in the Stytch API. The member_id is critical to perform operations on a Member, so be sure to preserve this value.
 
-    - `member_created`: Boolean if a Member already exists with that email.
+    - `member_created`: A flag indicating `true` if a new Member object was created and `false` if the Member object already existed.
 
     - `member`: The Member object.
+
+    - `organization`: The Organization object.
     """  # noqa
 
     member_id: str
     member_created: bool
     member: Member
+    organization: Organization
 
 
 class InviteResponse(ResponseBase):
     """Response fields beyond those defined in `ResponseBase`:
 
     - `member_id`: Globally unique UUID that identifies a specific Member. The member_id is critical to perform operations on a Member, so be sure to preserve this value.
     - `member`: The Member object.
+    - `organization`: The Organization object.
     """  # noqa
 
     member_id: str
     member: Member
+    organization: Organization
```

### Comparing `stytch-6.7.0/stytch/b2b/models/organizations.py` & `stytch-6.7.1/stytch/b2b/models/organizations.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,52 @@
     - `organization_id`: Globally unique UUID that identifies a specific Organization. The organization_id is critical to perform operations on an Organization, so be sure to preserve this value.
     """  # noqa
 
     organization_id: str
 
 
 class GetMemberResponse(ResponseBase):
+    """Response fields beyond those defined in `ResponseBase`:
+
+    - `member_id`: The UUID of the Member.
+
+    - `member`: The Member object.
+
+    - `organization`: The Organization object.
+    """  # noqa
+
+    member_id: str
+    member: Member
+    organization: Organization
+
+
+class CreateMemberResponse(ResponseBase):
+    """Response fields beyond those defined in `ResponseBase`:
+
+    - `member_id`: The UUID of the Member.
+
+    - `member`: The Member object.
+
+    - `organization`: The Organization object.
+    """  # noqa
+
+    member_id: str
+    member: Member
+    organization: Organization
+
+
+class UpdateMemberResponse(ResponseBase):
+    """Response fields beyond those defined in `ResponseBase`:
+
+    - `member_id`: The UUID of the Member.
+
+    - `member`: The Member object.
+
+    - `organization`: The Organization object.
+    """  # noqa
 
     member_id: str
     member: Member
     organization: Organization
 
 
 class DeleteMemberResponse(ResponseBase):
```

### Comparing `stytch-6.7.0/stytch/b2b/models/passwords.py` & `stytch-6.7.1/stytch/b2b/models/passwords.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     organization: Organization
     session_token: str
     session_jwt: str
     member_session: Optional[B2BStytchSession]
 
 
 class StrengthCheckResponse(ResponseBase):
-
     breach_detection_on_create: bool
     breached_password: bool
     luds_feedback: dict
     request_id: str
     score: int
     status_code: int
     strength_policy: str
```

### Comparing `stytch-6.7.0/stytch/b2b/models/passwords_email.py` & `stytch-6.7.1/stytch/b2b/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/b2b/models/passwords_existing_password.py` & `stytch-6.7.1/stytch/b2b/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/b2b/models/passwords_session.py` & `stytch-6.7.1/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/b2b/models/sessions.py` & `stytch-6.7.1/stytch/b2b/models/sessions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 from typing import List
 
-from stytch.b2b.core.models import B2BStytchSession, Member
+from stytch.b2b.core.models import B2BStytchSession, Member, Organization
 from stytch.core.models import ResponseBase
 
 
 class GetResponse(ResponseBase):
     """Response fields beyond those defined in `ResponseBase`:
 
     - `sessions`: An array of B2BStytchSession objects
@@ -21,20 +21,23 @@
     - `member_session`: The Session object.
 
     - `session_token`: A secret token for a given Stytch Session. Read more about Session_token in our Session management guide.
 
     - `session_jwt`: The JSON Web Token (JWT) for a given Stytch Session. Read more about session_token in our session management guide.
 
     - `member`: The Member object.
+
+    - `organization`: The Organization object.
     """  # noqa
 
     member_session: B2BStytchSession
     session_token: str
     session_jwt: str
     member: Member
+    organization: Organization
 
 
 class RevokeResponse(ResponseBase):
     """Response fields beyond those defined in `ResponseBase`:
 
     (None)
     """  # noqa
```

### Comparing `stytch-6.7.0/stytch/client.py` & `stytch-6.7.1/stytch/client.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/core/http/client.py` & `stytch-6.7.1/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/core/models.py` & `stytch-6.7.1/stytch/core/models.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/models/crypto_wallets.py` & `stytch-6.7.1/stytch/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/models/magic_links.py` & `stytch-6.7.1/stytch/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/models/magic_links_email.py` & `stytch-6.7.1/stytch/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/models/oauth.py` & `stytch-6.7.1/stytch/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/models/passwords.py` & `stytch-6.7.1/stytch/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/models/sessions.py` & `stytch-6.7.1/stytch/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/models/totps.py` & `stytch-6.7.1/stytch/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/models/users.py` & `stytch-6.7.1/stytch/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch/models/webauthn.py` & `stytch-6.7.1/stytch/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/stytch.egg-info/PKG-INFO` & `stytch-6.7.1/stytch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 6.7.0
+Version: 6.7.1
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
@@ -48,15 +48,15 @@
 - [x] [SMS passcodes](https://stytch.com/docs/api/send-otp-by-sms)
 - [x] [WhatsApp passcodes](https://stytch.com/docs/api/whatsapp-send)
 - [x] [Email passcodes](https://stytch.com/docs/api/send-otp-by-email)
 - [x] [Session Management](https://stytch.com/docs/api/sessions-overview)
 - [x] [WebAuthn](https://stytch.com/docs/api/webauthn-overview)
 - [x] [Time-based one-time passcodes (TOTPs)](https://stytch.com/docs/api/totps-overview)
 - [x] [Crypto wallets](https://stytch.com/docs/api/crypto-wallet-overview)
-- [x] [Passwords (Beta)](https://stytch.com/docs/api/password-overview)
+- [x] [Passwords](https://stytch.com/docs/api/password-overview)
 
 ### Example usage
 
 Create an API client:
 
 ```python
 import stytch
```

### Comparing `stytch-6.7.0/stytch.egg-info/SOURCES.txt` & `stytch-6.7.1/stytch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/test/test_integration.py` & `stytch-6.7.1/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-6.7.0/test/test_integration_async.py` & `stytch-6.7.1/test/test_integration_async.py`

 * *Files identical despite different names*

