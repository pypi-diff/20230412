# Comparing `tmp/badsecrets-0.1.300.tar.gz` & `tmp/badsecrets-0.1.303.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badsecrets-0.1.300.tar", max compression
+gzip compressed data, was "badsecrets-0.1.303.tar", max compression
```

## Comparing `badsecrets-0.1.300.tar` & `badsecrets-0.1.303.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    35149 2023-04-10 15:03:34.146377 badsecrets-0.1.300/LICENSE
--rw-r--r--   0        0        0    26452 2023-04-10 15:03:34.146377 badsecrets-0.1.300/README.md
--rw-r--r--   0        0        0      711 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/__init__.py
--rw-r--r--   0        0        0     4485 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/base.py
--rw-r--r--   0        0        0      233 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/errors.py
--rw-r--r--   0        0        0     3570 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/helpers.py
--rw-r--r--   0        0        0        0 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/__init__.py
--rw-r--r--   0        0        0     5865 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/aspnet_viewstate.py
--rw-r--r--   0        0        0     1032 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/django_signedcookies.py
--rw-r--r--   0        0        0     2079 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/express_signedcookies.py
--rw-r--r--   0        0        0      856 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/flask_signedcookies.py
--rw-r--r--   0        0        0     3363 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/generic_jwt.py
--rw-r--r--   0        0        0    13573 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/jsf_viewstate.py
--rw-r--r--   0        0        0     2169 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/laravel_signedcookies.py
--rw-r--r--   0        0        0     1325 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/peoplesoft_pstoken.py
--rw-r--r--   0        0        0     3058 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/rails_secretkeybase.py
--rw-r--r--   0        0        0     2098 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/symfony_signedurl.py
--rw-r--r--   0        0        0     4943 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/telerik_encryptionkey.py
--rw-r--r--   0        0        0     2961 2023-04-10 15:03:34.146377 badsecrets-0.1.300/badsecrets/modules/telerik_hashkey.py
--rw-r--r--   0        0        0   654111 2023-04-10 15:03:34.154378 badsecrets-0.1.300/badsecrets/resources/aspnet_machinekeys.txt
--rw-r--r--   0        0        0    31178 2023-04-10 15:03:34.154378 badsecrets-0.1.300/badsecrets/resources/django_secret_keys.txt
--rw-r--r--   0        0        0    40993 2023-04-10 15:03:34.154378 badsecrets-0.1.300/badsecrets/resources/express_session_secrets.txt
--rw-r--r--   0        0        0  1777603 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/flask_secret_keys.txt
--rw-r--r--   0        0        0       87 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/jsf_viewstate_passwords.txt
--rw-r--r--   0        0        0     1257 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/jsf_viewstate_passwords_b64.txt
--rw-r--r--   0        0        0     7785 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/jwt_rsakeys_private.txt
--rw-r--r--   0        0        0     2122 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/jwt_rsakeys_public.txt
--rw-r--r--   0        0        0   113170 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/jwt_secrets.txt
--rw-r--r--   0        0        0    45086 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/laravel_app_keys.txt
--rw-r--r--   0        0        0       78 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/peoplesoft_passwords.txt
--rw-r--r--   0        0        0     6184 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/rails_secret_key_base.txt
--rw-r--r--   0        0        0     3009 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/symfony_appsecret.txt
--rw-r--r--   0        0        0    18037 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/telerik_encryption_keys.txt
--rw-r--r--   0        0        0    17990 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/telerik_hash_keys.txt
--rw-r--r--   0        0        0    76516 2023-04-10 15:03:34.174379 badsecrets-0.1.300/badsecrets/resources/top_10000_passwords.txt
--rw-r--r--   0        0        0      872 2023-04-10 15:04:00.163742 badsecrets-0.1.300/pyproject.toml
--rw-r--r--   0        0        0    27265 1970-01-01 00:00:00.000000 badsecrets-0.1.300/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 01:10:50.532161 badsecrets-0.1.303/LICENSE
+-rw-r--r--   0        0        0    26846 2023-04-12 01:10:50.532161 badsecrets-0.1.303/README.md
+-rw-r--r--   0        0        0      711 2023-04-12 01:10:50.532161 badsecrets-0.1.303/badsecrets/__init__.py
+-rw-r--r--   0        0        0     4485 2023-04-12 01:10:50.532161 badsecrets-0.1.303/badsecrets/base.py
+-rw-r--r--   0        0        0      233 2023-04-12 01:10:50.532161 badsecrets-0.1.303/badsecrets/errors.py
+-rw-r--r--   0        0        0     3570 2023-04-12 01:10:50.532161 badsecrets-0.1.303/badsecrets/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-12 01:10:50.532161 badsecrets-0.1.303/badsecrets/modules/__init__.py
+-rw-r--r--   0        0        0     5865 2023-04-12 01:10:50.532161 badsecrets-0.1.303/badsecrets/modules/aspnet_viewstate.py
+-rw-r--r--   0        0        0     1032 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/django_signedcookies.py
+-rw-r--r--   0        0        0     2079 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/express_signedcookies.py
+-rw-r--r--   0        0        0      856 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/flask_signedcookies.py
+-rw-r--r--   0        0        0     3363 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/generic_jwt.py
+-rw-r--r--   0        0        0    13573 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/jsf_viewstate.py
+-rw-r--r--   0        0        0     2169 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/laravel_signedcookies.py
+-rw-r--r--   0        0        0     1325 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/peoplesoft_pstoken.py
+-rw-r--r--   0        0        0     3058 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/rails_secretkeybase.py
+-rw-r--r--   0        0        0     2098 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/symfony_signedurl.py
+-rw-r--r--   0        0        0     4943 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/telerik_encryptionkey.py
+-rw-r--r--   0        0        0     2961 2023-04-12 01:10:50.536161 badsecrets-0.1.303/badsecrets/modules/telerik_hashkey.py
+-rw-r--r--   0        0        0   654111 2023-04-12 01:10:50.540161 badsecrets-0.1.303/badsecrets/resources/aspnet_machinekeys.txt
+-rw-r--r--   0        0        0    31178 2023-04-12 01:10:50.540161 badsecrets-0.1.303/badsecrets/resources/django_secret_keys.txt
+-rw-r--r--   0        0        0    40993 2023-04-12 01:10:50.544161 badsecrets-0.1.303/badsecrets/resources/express_session_secrets.txt
+-rw-r--r--   0        0        0  1777603 2023-04-12 01:10:50.560161 badsecrets-0.1.303/badsecrets/resources/flask_secret_keys.txt
+-rw-r--r--   0        0        0       87 2023-04-12 01:10:50.560161 badsecrets-0.1.303/badsecrets/resources/jsf_viewstate_passwords.txt
+-rw-r--r--   0        0        0     1257 2023-04-12 01:10:50.560161 badsecrets-0.1.303/badsecrets/resources/jsf_viewstate_passwords_b64.txt
+-rw-r--r--   0        0        0     7785 2023-04-12 01:10:50.560161 badsecrets-0.1.303/badsecrets/resources/jwt_rsakeys_private.txt
+-rw-r--r--   0        0        0     2122 2023-04-12 01:10:50.560161 badsecrets-0.1.303/badsecrets/resources/jwt_rsakeys_public.txt
+-rw-r--r--   0        0        0   113170 2023-04-12 01:10:50.560161 badsecrets-0.1.303/badsecrets/resources/jwt_secrets.txt
+-rw-r--r--   0        0        0    45086 2023-04-12 01:10:50.564161 badsecrets-0.1.303/badsecrets/resources/laravel_app_keys.txt
+-rw-r--r--   0        0        0       78 2023-04-12 01:10:50.564161 badsecrets-0.1.303/badsecrets/resources/peoplesoft_passwords.txt
+-rw-r--r--   0        0        0     6184 2023-04-12 01:10:50.564161 badsecrets-0.1.303/badsecrets/resources/rails_secret_key_base.txt
+-rw-r--r--   0        0        0     3009 2023-04-12 01:10:50.564161 badsecrets-0.1.303/badsecrets/resources/symfony_appsecret.txt
+-rw-r--r--   0        0        0    18037 2023-04-12 01:10:50.564161 badsecrets-0.1.303/badsecrets/resources/telerik_encryption_keys.txt
+-rw-r--r--   0        0        0    17990 2023-04-12 01:10:50.564161 badsecrets-0.1.303/badsecrets/resources/telerik_hash_keys.txt
+-rw-r--r--   0        0        0    76516 2023-04-12 01:10:50.564161 badsecrets-0.1.303/badsecrets/resources/top_10000_passwords.txt
+-rw-r--r--   0        0        0      927 2023-04-12 01:11:11.256242 badsecrets-0.1.303/pyproject.toml
+-rw-r--r--   0        0        0    27659 1970-01-01 00:00:00.000000 badsecrets-0.1.303/PKG-INFO
```

### Comparing `badsecrets-0.1.300/LICENSE` & `badsecrets-0.1.303/LICENSE`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/README.md` & `badsecrets-0.1.303/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,30 +32,42 @@
 | Express_SignedCookies | Checks express.js signed cookies and session cookies for known 'session secret' |
 | Laravel_SignedCookies | Checks 'laravel_session' cookies for known laravel 'APP_KEY' |
 
 ## Installation
 
 We have a [pypi](https://pypi.org/project/badsecrets/) package, so you can just do `pip install badsecrets` to make use of the library.
 
+## Simple Usage
+
+The absolute easiest way to use Badsecrets is by simply running `badsecrets` after doing a pip install:
+
+```
+pip install badsecrets
+badsecrets eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+```
+
+This is doing the same thing as the `cli.py` example shown below.
+
+## Examples
+
 To use the examples, after doing the pip install just `git clone` the repo and `cd` into the `badsecrets` directory:
 
 ```
 git clone https://github.com/blacklanternsecurity/badsecrets.git
 cd badsecrets
 ```
 
 The commands in the example section below assume you are in this directory.
 
 If you are using the Badsecrets [BBOT](https://github.com/blacklanternsecurity/bbot) module, you don't need to do anything else - BBOT will install the package for you.
 
-## Examples
 
 ### cli.py
 
-Bad secrets includes an [example CLI](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/blacklist3r.py) for convenience when manually checking secrets. It also has a URL mode, which will connect to a target and attempt to carve for cryptographic products and check any it finds against all modules. 
+Bad secrets includes an [example CLI](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/cli.py) for convenience when manually checking secrets. It also has a URL mode, which will connect to a target and attempt to carve for cryptographic products and check any it finds against all modules. 
 
 * Basic usage - checking a crytographic product for a known secret (against all modules):
 ```bash
 python examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
 ```
 
 * URL Mode - Connecting to a target and carving for a cryptographic product, and if found checking it for known secrets (against all modules):
```

### Comparing `badsecrets-0.1.300/badsecrets/__init__.py` & `badsecrets-0.1.303/badsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/base.py` & `badsecrets-0.1.303/badsecrets/base.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/helpers.py` & `badsecrets-0.1.303/badsecrets/helpers.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/aspnet_viewstate.py` & `badsecrets-0.1.303/badsecrets/modules/aspnet_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/django_signedcookies.py` & `badsecrets-0.1.303/badsecrets/modules/django_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/express_signedcookies.py` & `badsecrets-0.1.303/badsecrets/modules/express_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/flask_signedcookies.py` & `badsecrets-0.1.303/badsecrets/modules/flask_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/generic_jwt.py` & `badsecrets-0.1.303/badsecrets/modules/generic_jwt.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/jsf_viewstate.py` & `badsecrets-0.1.303/badsecrets/modules/jsf_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/laravel_signedcookies.py` & `badsecrets-0.1.303/badsecrets/modules/laravel_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/peoplesoft_pstoken.py` & `badsecrets-0.1.303/badsecrets/modules/peoplesoft_pstoken.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/rails_secretkeybase.py` & `badsecrets-0.1.303/badsecrets/modules/rails_secretkeybase.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/symfony_signedurl.py` & `badsecrets-0.1.303/badsecrets/modules/symfony_signedurl.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/telerik_encryptionkey.py` & `badsecrets-0.1.303/badsecrets/modules/telerik_encryptionkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/modules/telerik_hashkey.py` & `badsecrets-0.1.303/badsecrets/modules/telerik_hashkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/aspnet_machinekeys.txt` & `badsecrets-0.1.303/badsecrets/resources/aspnet_machinekeys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/django_secret_keys.txt` & `badsecrets-0.1.303/badsecrets/resources/django_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/express_session_secrets.txt` & `badsecrets-0.1.303/badsecrets/resources/express_session_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/flask_secret_keys.txt` & `badsecrets-0.1.303/badsecrets/resources/flask_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/jsf_viewstate_passwords_b64.txt` & `badsecrets-0.1.303/badsecrets/resources/jsf_viewstate_passwords_b64.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/jwt_rsakeys_private.txt` & `badsecrets-0.1.303/badsecrets/resources/jwt_rsakeys_private.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/jwt_rsakeys_public.txt` & `badsecrets-0.1.303/badsecrets/resources/jwt_rsakeys_public.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/jwt_secrets.txt` & `badsecrets-0.1.303/badsecrets/resources/jwt_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/laravel_app_keys.txt` & `badsecrets-0.1.303/badsecrets/resources/laravel_app_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/rails_secret_key_base.txt` & `badsecrets-0.1.303/badsecrets/resources/rails_secret_key_base.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/symfony_appsecret.txt` & `badsecrets-0.1.303/badsecrets/resources/symfony_appsecret.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/telerik_encryption_keys.txt` & `badsecrets-0.1.303/badsecrets/resources/telerik_encryption_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/telerik_hash_keys.txt` & `badsecrets-0.1.303/badsecrets/resources/telerik_hash_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/badsecrets/resources/top_10000_passwords.txt` & `badsecrets-0.1.303/badsecrets/resources/top_10000_passwords.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.300/pyproject.toml` & `badsecrets-0.1.303/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "badsecrets"
-version = "v0.1.300"
+version = "v0.1.303"
 description = "About"
 authors = ["A library for detecting known or weak secrets on across many platforms"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dev-dependencies]
 requests-mock = "^1.10.0"
@@ -19,14 +19,16 @@
 viewstate = "^0.5.3"
 pytest = "^7.1.3"
 flask-unsign = "^1.2.0"
 Django = "^4.1.2"
 pyjwt = {extras = ["crypto"], version = "^2.6.0"}
 requests = "^2.28.1"
 
+[tool.poetry.scripts]
+badsecrets = 'examples.cli:main'
 
 [tool.black]
 line-length = 119
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `badsecrets-0.1.300/PKG-INFO` & `badsecrets-0.1.303/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badsecrets
-Version: 0.1.300
+Version: 0.1.303
 Summary: About
 License: GPL-3.0
 Author: A library for detecting known or weak secrets on across many platforms
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -53,30 +53,42 @@
 | Express_SignedCookies | Checks express.js signed cookies and session cookies for known 'session secret' |
 | Laravel_SignedCookies | Checks 'laravel_session' cookies for known laravel 'APP_KEY' |
 
 ## Installation
 
 We have a [pypi](https://pypi.org/project/badsecrets/) package, so you can just do `pip install badsecrets` to make use of the library.
 
+## Simple Usage
+
+The absolute easiest way to use Badsecrets is by simply running `badsecrets` after doing a pip install:
+
+```
+pip install badsecrets
+badsecrets eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+```
+
+This is doing the same thing as the `cli.py` example shown below.
+
+## Examples
+
 To use the examples, after doing the pip install just `git clone` the repo and `cd` into the `badsecrets` directory:
 
 ```
 git clone https://github.com/blacklanternsecurity/badsecrets.git
 cd badsecrets
 ```
 
 The commands in the example section below assume you are in this directory.
 
 If you are using the Badsecrets [BBOT](https://github.com/blacklanternsecurity/bbot) module, you don't need to do anything else - BBOT will install the package for you.
 
-## Examples
 
 ### cli.py
 
-Bad secrets includes an [example CLI](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/blacklist3r.py) for convenience when manually checking secrets. It also has a URL mode, which will connect to a target and attempt to carve for cryptographic products and check any it finds against all modules. 
+Bad secrets includes an [example CLI](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/cli.py) for convenience when manually checking secrets. It also has a URL mode, which will connect to a target and attempt to carve for cryptographic products and check any it finds against all modules. 
 
 * Basic usage - checking a crytographic product for a known secret (against all modules):
 ```bash
 python examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
 ```
 
 * URL Mode - Connecting to a target and carving for a cryptographic product, and if found checking it for known secrets (against all modules):
```

