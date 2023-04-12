# Comparing `tmp/badsecrets-0.1.304.tar.gz` & `tmp/badsecrets-0.2.311.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badsecrets-0.1.304.tar", max compression
+gzip compressed data, was "badsecrets-0.2.311.tar", max compression
```

## Comparing `badsecrets-0.1.304.tar` & `badsecrets-0.2.311.tar`

### file list

```diff
@@ -1,37 +1,42 @@
--rw-r--r--   0        0        0    35149 2023-04-12 02:26:44.555471 badsecrets-0.1.304/LICENSE
--rw-r--r--   0        0        0    26846 2023-04-12 02:26:44.555471 badsecrets-0.1.304/README.md
--rw-r--r--   0        0        0      711 2023-04-12 02:26:44.555471 badsecrets-0.1.304/badsecrets/__init__.py
--rw-r--r--   0        0        0     4485 2023-04-12 02:26:44.555471 badsecrets-0.1.304/badsecrets/base.py
--rw-r--r--   0        0        0      233 2023-04-12 02:26:44.555471 badsecrets-0.1.304/badsecrets/errors.py
--rw-r--r--   0        0        0     3570 2023-04-12 02:26:44.555471 badsecrets-0.1.304/badsecrets/helpers.py
--rw-r--r--   0        0        0        0 2023-04-12 02:26:44.555471 badsecrets-0.1.304/badsecrets/modules/__init__.py
--rw-r--r--   0        0        0     5865 2023-04-12 02:26:44.555471 badsecrets-0.1.304/badsecrets/modules/aspnet_viewstate.py
--rw-r--r--   0        0        0     1032 2023-04-12 02:26:44.555471 badsecrets-0.1.304/badsecrets/modules/django_signedcookies.py
--rw-r--r--   0        0        0     2079 2023-04-12 02:26:44.555471 badsecrets-0.1.304/badsecrets/modules/express_signedcookies.py
--rw-r--r--   0        0        0      856 2023-04-12 02:26:44.559471 badsecrets-0.1.304/badsecrets/modules/flask_signedcookies.py
--rw-r--r--   0        0        0     3363 2023-04-12 02:26:44.559471 badsecrets-0.1.304/badsecrets/modules/generic_jwt.py
--rw-r--r--   0        0        0    13573 2023-04-12 02:26:44.559471 badsecrets-0.1.304/badsecrets/modules/jsf_viewstate.py
--rw-r--r--   0        0        0     2169 2023-04-12 02:26:44.559471 badsecrets-0.1.304/badsecrets/modules/laravel_signedcookies.py
--rw-r--r--   0        0        0     1325 2023-04-12 02:26:44.559471 badsecrets-0.1.304/badsecrets/modules/peoplesoft_pstoken.py
--rw-r--r--   0        0        0     3058 2023-04-12 02:26:44.559471 badsecrets-0.1.304/badsecrets/modules/rails_secretkeybase.py
--rw-r--r--   0        0        0     2098 2023-04-12 02:26:44.559471 badsecrets-0.1.304/badsecrets/modules/symfony_signedurl.py
--rw-r--r--   0        0        0     4943 2023-04-12 02:26:44.559471 badsecrets-0.1.304/badsecrets/modules/telerik_encryptionkey.py
--rw-r--r--   0        0        0     2961 2023-04-12 02:26:44.559471 badsecrets-0.1.304/badsecrets/modules/telerik_hashkey.py
--rw-r--r--   0        0        0   654111 2023-04-12 02:26:44.563470 badsecrets-0.1.304/badsecrets/resources/aspnet_machinekeys.txt
--rw-r--r--   0        0        0    31178 2023-04-12 02:26:44.563470 badsecrets-0.1.304/badsecrets/resources/django_secret_keys.txt
--rw-r--r--   0        0        0    40993 2023-04-12 02:26:44.567471 badsecrets-0.1.304/badsecrets/resources/express_session_secrets.txt
--rw-r--r--   0        0        0  1777603 2023-04-12 02:26:44.583471 badsecrets-0.1.304/badsecrets/resources/flask_secret_keys.txt
--rw-r--r--   0        0        0       87 2023-04-12 02:26:44.583471 badsecrets-0.1.304/badsecrets/resources/jsf_viewstate_passwords.txt
--rw-r--r--   0        0        0     1257 2023-04-12 02:26:44.583471 badsecrets-0.1.304/badsecrets/resources/jsf_viewstate_passwords_b64.txt
--rw-r--r--   0        0        0     7785 2023-04-12 02:26:44.583471 badsecrets-0.1.304/badsecrets/resources/jwt_rsakeys_private.txt
--rw-r--r--   0        0        0     2122 2023-04-12 02:26:44.583471 badsecrets-0.1.304/badsecrets/resources/jwt_rsakeys_public.txt
--rw-r--r--   0        0        0   113170 2023-04-12 02:26:44.583471 badsecrets-0.1.304/badsecrets/resources/jwt_secrets.txt
--rw-r--r--   0        0        0    45086 2023-04-12 02:26:44.583471 badsecrets-0.1.304/badsecrets/resources/laravel_app_keys.txt
--rw-r--r--   0        0        0       78 2023-04-12 02:26:44.583471 badsecrets-0.1.304/badsecrets/resources/peoplesoft_passwords.txt
--rw-r--r--   0        0        0     6184 2023-04-12 02:26:44.583471 badsecrets-0.1.304/badsecrets/resources/rails_secret_key_base.txt
--rw-r--r--   0        0        0     3009 2023-04-12 02:26:44.583471 badsecrets-0.1.304/badsecrets/resources/symfony_appsecret.txt
--rw-r--r--   0        0        0    18037 2023-04-12 02:26:44.587471 badsecrets-0.1.304/badsecrets/resources/telerik_encryption_keys.txt
--rw-r--r--   0        0        0    17990 2023-04-12 02:26:44.587471 badsecrets-0.1.304/badsecrets/resources/telerik_hash_keys.txt
--rw-r--r--   0        0        0    76516 2023-04-12 02:26:44.587471 badsecrets-0.1.304/badsecrets/resources/top_10000_passwords.txt
--rw-r--r--   0        0        0      927 2023-04-12 02:27:06.175518 badsecrets-0.1.304/pyproject.toml
--rw-r--r--   0        0        0    27659 1970-01-01 00:00:00.000000 badsecrets-0.1.304/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 03:22:02.947149 badsecrets-0.2.311/LICENSE
+-rw-r--r--   0        0        0    26959 2023-04-12 03:22:02.947149 badsecrets-0.2.311/README.md
+-rw-r--r--   0        0        0      711 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/__init__.py
+-rw-r--r--   0        0        0     4485 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/base.py
+-rw-r--r--   0        0        0      233 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/errors.py
+-rw-r--r--   0        0        0        0 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/examples/__init__.py
+-rwxr-xr-x   0        0        0     4220 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/examples/blacklist3r.py
+-rwxr-xr-x   0        0        0     3560 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/examples/cli.py
+-rwxr-xr-x   0        0        0     3541 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/examples/symfony_knownkey.py
+-rwxr-xr-x   0        0        0    10597 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/examples/telerik_knownkey.py
+-rw-r--r--   0        0        0     3570 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/modules/__init__.py
+-rw-r--r--   0        0        0     5865 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/modules/aspnet_viewstate.py
+-rw-r--r--   0        0        0     1032 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/modules/django_signedcookies.py
+-rw-r--r--   0        0        0     2079 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/express_signedcookies.py
+-rw-r--r--   0        0        0      856 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/flask_signedcookies.py
+-rw-r--r--   0        0        0     3363 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/generic_jwt.py
+-rw-r--r--   0        0        0    13573 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/jsf_viewstate.py
+-rw-r--r--   0        0        0     2169 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/laravel_signedcookies.py
+-rw-r--r--   0        0        0     1325 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/peoplesoft_pstoken.py
+-rw-r--r--   0        0        0     3058 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/rails_secretkeybase.py
+-rw-r--r--   0        0        0     2098 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/symfony_signedurl.py
+-rw-r--r--   0        0        0     4943 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/telerik_encryptionkey.py
+-rw-r--r--   0        0        0     2961 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/telerik_hashkey.py
+-rw-r--r--   0        0        0   654111 2023-04-12 03:22:02.955150 badsecrets-0.2.311/badsecrets/resources/aspnet_machinekeys.txt
+-rw-r--r--   0        0        0    31178 2023-04-12 03:22:02.955150 badsecrets-0.2.311/badsecrets/resources/django_secret_keys.txt
+-rw-r--r--   0        0        0    40993 2023-04-12 03:22:02.955150 badsecrets-0.2.311/badsecrets/resources/express_session_secrets.txt
+-rw-r--r--   0        0        0  1777603 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/flask_secret_keys.txt
+-rw-r--r--   0        0        0       87 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/jsf_viewstate_passwords.txt
+-rw-r--r--   0        0        0     1257 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/jsf_viewstate_passwords_b64.txt
+-rw-r--r--   0        0        0     7785 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/jwt_rsakeys_private.txt
+-rw-r--r--   0        0        0     2122 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/jwt_rsakeys_public.txt
+-rw-r--r--   0        0        0   113170 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/jwt_secrets.txt
+-rw-r--r--   0        0        0    45086 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/laravel_app_keys.txt
+-rw-r--r--   0        0        0       78 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/peoplesoft_passwords.txt
+-rw-r--r--   0        0        0     6184 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/rails_secret_key_base.txt
+-rw-r--r--   0        0        0     3009 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/symfony_appsecret.txt
+-rw-r--r--   0        0        0    18037 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/telerik_encryption_keys.txt
+-rw-r--r--   0        0        0    17990 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/telerik_hash_keys.txt
+-rw-r--r--   0        0        0    76516 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/top_10000_passwords.txt
+-rw-r--r--   0        0        0      938 2023-04-12 03:22:20.923581 badsecrets-0.2.311/pyproject.toml
+-rw-r--r--   0        0        0    27772 1970-01-01 00:00:00.000000 badsecrets-0.2.311/PKG-INFO
```

### Comparing `badsecrets-0.1.304/LICENSE` & `badsecrets-0.2.311/LICENSE`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/README.md` & `badsecrets-0.2.311/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,66 +63,66 @@
 
 ### cli.py
 
 Bad secrets includes an [example CLI](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/cli.py) for convenience when manually checking secrets. It also has a URL mode, which will connect to a target and attempt to carve for cryptographic products and check any it finds against all modules. 
 
 * Basic usage - checking a crytographic product for a known secret (against all modules):
 ```bash
-python examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+python ./badsecrets/examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
 ```
 
 * URL Mode - Connecting to a target and carving for a cryptographic product, and if found checking it for known secrets (against all modules):
 
 ```bash
-python examples/cli.py --url http://example.com/contains_bad_secret.html
+python ./badsecrets/examples/cli.py --url http://example.com/contains_bad_secret.html
 ```
 
 You can also set a custom user-agent with `--user-agent "user-agent string"` or a proxy with `--proxy http://127.0.0.1` in this mode.
 
 Example output:
 
 ```bash
-$ python examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+$ python ./badsecrets/examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
 badsecrets - example command line interface
 
 ***********************
 Known Secret Found!
 
 Detecting Module: Generic_JWT
 
 Secret: 1234
 Details: {'Issuer': 'Issuer', 'Username': 'BadSecrets', 'exp': 1593133483, 'iat': 1466903083, 'jwt_headers': {'alg': 'HS256'}}
 ***********************
 ```
 
 ### Blacklist3r.py
 
-Bad secrets includes a [fully functional CLI example](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/blacklist3r.py) which replicates the functionality of [blacklist3r](https://github.com/NotSoSecure/Blacklist3r) in python examples/blacklist3r. 
+Bad secrets includes a [fully functional CLI example](https://github.com/blacklanternsecurity/badsecrets/blob/dev/badsecrets/examples/blacklist3r.py) which replicates the functionality of [blacklist3r](https://github.com/NotSoSecure/Blacklist3r) in python badsecrets/examples/blacklist3r. 
 
 ```bash
-python examples/blacklist3r.py --url http://vulnerablesite/vulnerablepage.aspx
-python examples/blacklist3r.py --viewstate /wEPDwUJODExMDE5NzY5ZGQMKS6jehX5HkJgXxrPh09vumNTKQ== --generator EDD8C9AE
+python ./badsecrets/examples/blacklist3r.py --url http://vulnerablesite/vulnerablepage.aspx
+python ./badsecrets/examples/blacklist3r.py --viewstate /wEPDwUJODExMDE5NzY5ZGQMKS6jehX5HkJgXxrPh09vumNTKQ== --generator EDD8C9AE
 ```
 
 
 ### Telerik_knownkey.py
 
 Fully functional CLI example for identifying known Telerik Hash keys and Encryption keys for Post-2017 versions (those patched for CVE-2017-9248), and brute-forcing version / generating exploitation DialogParameters values.
 
 ```bash
-python examples/telerik_knownkey.py --url http://vulnerablesite/Telerik.Web.UI.DialogHandler.aspx
+python ./badsecrets/examples/telerik_knownkey.py --url http://vulnerablesite/Telerik.Web.UI.DialogHandler.aspx
 ```
 Optionally include ASP.NET MachineKeys with --machine-keys (Will SIGNIFICANTLY increase brute-forcing time)
 
 ### Symfony_knownkey.py
 
 Brute-force detection of Symfony known secret key when "\_fragment" URLs are enabled, even when no example URL containing a hash can be located. [Relevent Blog Post](https://www.ambionics.io/blog/symfony-secret-fragment).
 
 ```bash
-python examples/symfony_knownkey.py --url https://localhost/
+python ./badsecrets/examples/symfony_knownkey.py --url https://localhost/
 ```
 
 ## BBOT Module
 
 One of the best ways to use Badsecrets, especially for the `ASPNET_Viewstate` and `Jsf_viewstate` modules is with the Badsecrets [BBOT](https://github.com/blacklanternsecurity/bbot) module. This will allow you to easily check across thousands of systems in conjunction with subdomain enummeration. 
 
 ```
```

### Comparing `badsecrets-0.1.304/badsecrets/__init__.py` & `badsecrets-0.2.311/badsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/base.py` & `badsecrets-0.2.311/badsecrets/base.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/helpers.py` & `badsecrets-0.2.311/badsecrets/helpers.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/aspnet_viewstate.py` & `badsecrets-0.2.311/badsecrets/modules/aspnet_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/django_signedcookies.py` & `badsecrets-0.2.311/badsecrets/modules/django_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/express_signedcookies.py` & `badsecrets-0.2.311/badsecrets/modules/express_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/flask_signedcookies.py` & `badsecrets-0.2.311/badsecrets/modules/flask_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/generic_jwt.py` & `badsecrets-0.2.311/badsecrets/modules/generic_jwt.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/jsf_viewstate.py` & `badsecrets-0.2.311/badsecrets/modules/jsf_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/laravel_signedcookies.py` & `badsecrets-0.2.311/badsecrets/modules/laravel_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/peoplesoft_pstoken.py` & `badsecrets-0.2.311/badsecrets/modules/peoplesoft_pstoken.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/rails_secretkeybase.py` & `badsecrets-0.2.311/badsecrets/modules/rails_secretkeybase.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/symfony_signedurl.py` & `badsecrets-0.2.311/badsecrets/modules/symfony_signedurl.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/telerik_encryptionkey.py` & `badsecrets-0.2.311/badsecrets/modules/telerik_encryptionkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/modules/telerik_hashkey.py` & `badsecrets-0.2.311/badsecrets/modules/telerik_hashkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/aspnet_machinekeys.txt` & `badsecrets-0.2.311/badsecrets/resources/aspnet_machinekeys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/django_secret_keys.txt` & `badsecrets-0.2.311/badsecrets/resources/django_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/express_session_secrets.txt` & `badsecrets-0.2.311/badsecrets/resources/express_session_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/flask_secret_keys.txt` & `badsecrets-0.2.311/badsecrets/resources/flask_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/jsf_viewstate_passwords_b64.txt` & `badsecrets-0.2.311/badsecrets/resources/jsf_viewstate_passwords_b64.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/jwt_rsakeys_private.txt` & `badsecrets-0.2.311/badsecrets/resources/jwt_rsakeys_private.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/jwt_rsakeys_public.txt` & `badsecrets-0.2.311/badsecrets/resources/jwt_rsakeys_public.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/jwt_secrets.txt` & `badsecrets-0.2.311/badsecrets/resources/jwt_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/laravel_app_keys.txt` & `badsecrets-0.2.311/badsecrets/resources/laravel_app_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/rails_secret_key_base.txt` & `badsecrets-0.2.311/badsecrets/resources/rails_secret_key_base.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/symfony_appsecret.txt` & `badsecrets-0.2.311/badsecrets/resources/symfony_appsecret.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/telerik_encryption_keys.txt` & `badsecrets-0.2.311/badsecrets/resources/telerik_encryption_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/telerik_hash_keys.txt` & `badsecrets-0.2.311/badsecrets/resources/telerik_hash_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/badsecrets/resources/top_10000_passwords.txt` & `badsecrets-0.2.311/badsecrets/resources/top_10000_passwords.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.1.304/pyproject.toml` & `badsecrets-0.2.311/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "badsecrets"
-version = "v0.1.304"
+version = "v0.2.311"
 description = "About"
 authors = ["A library for detecting known or weak secrets on across many platforms"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dev-dependencies]
 requests-mock = "^1.10.0"
@@ -20,20 +20,20 @@
 pytest = "^7.1.3"
 flask-unsign = "^1.2.0"
 Django = "^4.1.2"
 pyjwt = {extras = ["crypto"], version = "^2.6.0"}
 requests = "^2.28.1"
 
 [tool.poetry.scripts]
-badsecrets = 'examples.cli:main'
+badsecrets = 'badsecrets.examples.cli:main'
 
 [tool.black]
 line-length = 119
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 metadata = false
-format = 'v0.1.{distance}'
+format = 'v0.2.{distance}'
```

### Comparing `badsecrets-0.1.304/PKG-INFO` & `badsecrets-0.2.311/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badsecrets
-Version: 0.1.304
+Version: 0.2.311
 Summary: About
 License: GPL-3.0
 Author: A library for detecting known or weak secrets on across many platforms
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -84,66 +84,66 @@
 
 ### cli.py
 
 Bad secrets includes an [example CLI](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/cli.py) for convenience when manually checking secrets. It also has a URL mode, which will connect to a target and attempt to carve for cryptographic products and check any it finds against all modules. 
 
 * Basic usage - checking a crytographic product for a known secret (against all modules):
 ```bash
-python examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+python ./badsecrets/examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
 ```
 
 * URL Mode - Connecting to a target and carving for a cryptographic product, and if found checking it for known secrets (against all modules):
 
 ```bash
-python examples/cli.py --url http://example.com/contains_bad_secret.html
+python ./badsecrets/examples/cli.py --url http://example.com/contains_bad_secret.html
 ```
 
 You can also set a custom user-agent with `--user-agent "user-agent string"` or a proxy with `--proxy http://127.0.0.1` in this mode.
 
 Example output:
 
 ```bash
-$ python examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+$ python ./badsecrets/examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
 badsecrets - example command line interface
 
 ***********************
 Known Secret Found!
 
 Detecting Module: Generic_JWT
 
 Secret: 1234
 Details: {'Issuer': 'Issuer', 'Username': 'BadSecrets', 'exp': 1593133483, 'iat': 1466903083, 'jwt_headers': {'alg': 'HS256'}}
 ***********************
 ```
 
 ### Blacklist3r.py
 
-Bad secrets includes a [fully functional CLI example](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/blacklist3r.py) which replicates the functionality of [blacklist3r](https://github.com/NotSoSecure/Blacklist3r) in python examples/blacklist3r. 
+Bad secrets includes a [fully functional CLI example](https://github.com/blacklanternsecurity/badsecrets/blob/dev/badsecrets/examples/blacklist3r.py) which replicates the functionality of [blacklist3r](https://github.com/NotSoSecure/Blacklist3r) in python badsecrets/examples/blacklist3r. 
 
 ```bash
-python examples/blacklist3r.py --url http://vulnerablesite/vulnerablepage.aspx
-python examples/blacklist3r.py --viewstate /wEPDwUJODExMDE5NzY5ZGQMKS6jehX5HkJgXxrPh09vumNTKQ== --generator EDD8C9AE
+python ./badsecrets/examples/blacklist3r.py --url http://vulnerablesite/vulnerablepage.aspx
+python ./badsecrets/examples/blacklist3r.py --viewstate /wEPDwUJODExMDE5NzY5ZGQMKS6jehX5HkJgXxrPh09vumNTKQ== --generator EDD8C9AE
 ```
 
 
 ### Telerik_knownkey.py
 
 Fully functional CLI example for identifying known Telerik Hash keys and Encryption keys for Post-2017 versions (those patched for CVE-2017-9248), and brute-forcing version / generating exploitation DialogParameters values.
 
 ```bash
-python examples/telerik_knownkey.py --url http://vulnerablesite/Telerik.Web.UI.DialogHandler.aspx
+python ./badsecrets/examples/telerik_knownkey.py --url http://vulnerablesite/Telerik.Web.UI.DialogHandler.aspx
 ```
 Optionally include ASP.NET MachineKeys with --machine-keys (Will SIGNIFICANTLY increase brute-forcing time)
 
 ### Symfony_knownkey.py
 
 Brute-force detection of Symfony known secret key when "\_fragment" URLs are enabled, even when no example URL containing a hash can be located. [Relevent Blog Post](https://www.ambionics.io/blog/symfony-secret-fragment).
 
 ```bash
-python examples/symfony_knownkey.py --url https://localhost/
+python ./badsecrets/examples/symfony_knownkey.py --url https://localhost/
 ```
 
 ## BBOT Module
 
 One of the best ways to use Badsecrets, especially for the `ASPNET_Viewstate` and `Jsf_viewstate` modules is with the Badsecrets [BBOT](https://github.com/blacklanternsecurity/bbot) module. This will allow you to easily check across thousands of systems in conjunction with subdomain enummeration. 
 
 ```
```

