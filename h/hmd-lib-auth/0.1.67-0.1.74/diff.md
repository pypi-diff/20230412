# Comparing `tmp/hmd_lib_auth-0.1.67-py3-none-any.whl.zip` & `tmp/hmd_lib_auth-0.1.74-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5511 bytes, number of entries: 8
--rw-rw-rw-  2.0 unx        0 b- defN 23-Feb-28 20:05 hmd_lib_auth/__init__.py
--rw-rw-rw-  2.0 unx     3170 b- defN 23-Feb-28 20:05 hmd_lib_auth/hmd_lib_auth.py
--rw-rw-rw-  2.0 unx     4437 b- defN 23-Feb-28 20:05 hmd_lib_auth/lambda_helper.py
--rw-rw-rw-  2.0 unx     1473 b- defN 23-Feb-28 20:05 hmd_lib_auth/open_policy_agent.py
--rw-rw-rw-  2.0 unx     1790 b- defN 23-Feb-28 20:05 hmd_lib_auth-0.1.67.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Feb-28 20:05 hmd_lib_auth-0.1.67.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       13 b- defN 23-Feb-28 20:05 hmd_lib_auth-0.1.67.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      661 b- defN 23-Feb-28 20:05 hmd_lib_auth-0.1.67.dist-info/RECORD
-8 files, 11636 bytes uncompressed, 4349 bytes compressed:  62.6%
+Zip file size: 5573 bytes, number of entries: 8
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Apr-11 14:13 hmd_lib_auth/__init__.py
+-rw-rw-rw-  2.0 unx     3170 b- defN 23-Apr-11 14:13 hmd_lib_auth/hmd_lib_auth.py
+-rw-rw-rw-  2.0 unx     4711 b- defN 23-Apr-11 14:13 hmd_lib_auth/lambda_helper.py
+-rw-rw-rw-  2.0 unx     1434 b- defN 23-Apr-11 14:13 hmd_lib_auth/open_policy_agent.py
+-rw-rw-rw-  2.0 unx     1790 b- defN 23-Apr-11 14:13 hmd_lib_auth-0.1.74.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-11 14:13 hmd_lib_auth-0.1.74.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       13 b- defN 23-Apr-11 14:13 hmd_lib_auth-0.1.74.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      661 b- defN 23-Apr-11 14:13 hmd_lib_auth-0.1.74.dist-info/RECORD
+8 files, 11871 bytes uncompressed, 4411 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: hmd_lib_auth/lambda_helper.py
 Comment: 
 
 Filename: hmd_lib_auth/open_policy_agent.py
 Comment: 
 
-Filename: hmd_lib_auth-0.1.67.dist-info/METADATA
+Filename: hmd_lib_auth-0.1.74.dist-info/METADATA
 Comment: 
 
-Filename: hmd_lib_auth-0.1.67.dist-info/WHEEL
+Filename: hmd_lib_auth-0.1.74.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_lib_auth-0.1.67.dist-info/top_level.txt
+Filename: hmd_lib_auth-0.1.74.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_lib_auth-0.1.67.dist-info/RECORD
+Filename: hmd_lib_auth-0.1.74.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_lib_auth/lambda_helper.py

```diff
@@ -40,21 +40,28 @@
     return claims
 
 
 def _get_issuer_and_audience(
     token: str, session: Session, additional_clients: Dict
 ) -> Tuple[str, str]:
     okta_secrets = get_secret(session, "okta", use_cache=True)
+    trusted_human_clients = []
+    human_clients_param = os.environ.get("TRUSTED_HUMAN_CLIENTS")
+
+    if human_clients_param is not None:
+        clients_param = get_param_store_parameter(human_clients_param, session=session)
+        human_clients = loads(clients_param)
+        if "trusted_clients" in human_clients:
+            trusted_human_clients.extend(human_clients["trusted_clients"])
 
     _, claims, _, _ = JWTUtils.parse_token(token)
     client_id = claims.get("cid", "")
     is_human_user = client_id in [
-        okta_secrets.get("studio_client_id"),  # TODO: Remove: Deprecated
-        okta_secrets.get("login_cli_client_id"),  # TODO: Remove: Deprecated
         okta_secrets.get("ns_client_id"),
+        *trusted_human_clients,
     ]
 
     audience = "api://neuronsphere"
     issuer = okta_secrets["services_issuer"]
 
     if is_human_user:
         issuer = okta_secrets["ns_issuer"]
```

## hmd_lib_auth/open_policy_agent.py

```diff
@@ -4,34 +4,31 @@
 from hmd_cli_tools.hmd_cli_tools import get_neuronsphere_domain
 
 
 def validate_authorization(
     service: str,
     rules: List[str],
     input_dict: dict,
-    opa_server: str = None,
+    opa_server: str = os.environ.get("OPA_SERVER"),
     token: str = os.environ.get("OPA_TOKEN"),
 ) -> Tuple[bool, dict]:
     """
     queries OPA to determine whether the input satisfies the given policy rules
     """
 
     if not opa_server:
-        opa_server = os.environ.get(
-            "OPA_HOST",
-            f"base-opa.{get_neuronsphere_domain(os.environ['HMD_CUSTOMER_CODE'], os.environ['HMD_ENVIRONMENT'])}",
-        )
+        opa_server = f"https://base-opa.{get_neuronsphere_domain(os.environ['HMD_CUSTOMER_CODE'], os.environ['HMD_ENVIRONMENT'])}"
 
     headers = None
     if token:
         headers = {"Authorization": f"Bearer {token}"}
 
     # TODO: explore using Query API instead
     rsp = requests.post(
-        f"https://{opa_server}/v1/data/base/{service}/main",
+        f"{opa_server}/v1/data/base/{service}/main",
         json=input_dict,
         headers=headers,
     )
 
     policy = {
         rule_name: rule_value
         for (rule_name, rule_value) in rsp.json().get("result", {}).items()
```

## Comparing `hmd_lib_auth-0.1.67.dist-info/METADATA` & `hmd_lib_auth-0.1.74.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-lib-auth
-Version: 0.1.67
+Version: 0.1.74
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Michael Misshore
 Author-email: michael.misshore@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: acachecontrol (==0.3.5)
@@ -20,15 +20,15 @@
 Requires-Dist: cement (==3.0.6)
 Requires-Dist: certifi (==2022.12.7)
 Requires-Dist: charset-normalizer (==2.0.12)
 Requires-Dist: decorator (==5.1.1)
 Requires-Dist: ecdsa (==0.17.0)
 Requires-Dist: frozenlist (==1.3.0)
 Requires-Dist: google-auth (==2.9.1)
-Requires-Dist: hmd-cli-tools (~=1.1.227)
+Requires-Dist: hmd-cli-tools (~=1.1.228)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: kubernetes (==24.2.0)
 Requires-Dist: multidict (==6.0.2)
 Requires-Dist: oauthlib (==3.2.2)
 Requires-Dist: okta-jwt-verifier (==0.2.3)
```

## Comparing `hmd_lib_auth-0.1.67.dist-info/RECORD` & `hmd_lib_auth-0.1.74.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 hmd_lib_auth/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hmd_lib_auth/hmd_lib_auth.py,sha256=JA2k_bWxcCF0PZaNlr4g1b3eclM7FYqet4lKYlnXXIE,3170
-hmd_lib_auth/lambda_helper.py,sha256=0yS3Xea5aHteikjDQ1Fk_t446SjzRR1lmkxX-f6ohyQ,4437
-hmd_lib_auth/open_policy_agent.py,sha256=Ah-wlAeaaLlZFdh-M09Wx2Sf-NjMDmtfxkBOd2p7SgU,1473
-hmd_lib_auth-0.1.67.dist-info/METADATA,sha256=wF4NTrJUuva1RYPCs-8oIG-H8NfEtHFHmNDvW9z5Smg,1790
-hmd_lib_auth-0.1.67.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
-hmd_lib_auth-0.1.67.dist-info/top_level.txt,sha256=uXHFAYFljv__hxt889J42QxMsX43eDh5q-n3iJI2oe4,13
-hmd_lib_auth-0.1.67.dist-info/RECORD,,
+hmd_lib_auth/lambda_helper.py,sha256=BEisUgt0izhaPRNtSlBvrgqQC-JiU2AgSyThKeB8dEg,4711
+hmd_lib_auth/open_policy_agent.py,sha256=__NnF8laehmYJGDwSmu2JVHFmekobnnd6yrzCzoe7V8,1434
+hmd_lib_auth-0.1.74.dist-info/METADATA,sha256=erueh-tji2muuW94-z3encUo3ioyuQ__oG5HKyoHTP4,1790
+hmd_lib_auth-0.1.74.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
+hmd_lib_auth-0.1.74.dist-info/top_level.txt,sha256=uXHFAYFljv__hxt889J42QxMsX43eDh5q-n3iJI2oe4,13
+hmd_lib_auth-0.1.74.dist-info/RECORD,,
```

