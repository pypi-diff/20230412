# Comparing `tmp/getswish-0.1.2.tar.gz` & `tmp/getswish-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getswish-0.1.2.tar", max compression
+gzip compressed data, was "getswish-0.2.0.tar", last modified: Wed Apr 12 12:50:46 2023, max compression
```

## Comparing `getswish-0.1.2.tar` & `getswish-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,40 @@
--rw-r--r--   0        0        0     1069 2022-09-14 14:36:23.957580 getswish-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      277 2022-09-14 17:41:49.778607 getswish-0.1.2/getswish/__init__.py
--rw-r--r--   0        0        0     6239 2022-09-14 11:14:03.628096 getswish-0.1.2/getswish/client.py
--rw-r--r--   0        0        0      647 2022-09-14 10:15:18.030856 getswish-0.1.2/getswish/environments.py
--rw-r--r--   0        0        0      249 2022-09-07 09:24:24.684661 getswish-0.1.2/getswish/exceptions.py
--rw-r--r--   0        0        0     2936 2022-09-14 10:32:43.970762 getswish-0.1.2/getswish/models.py
--rw-r--r--   0        0        0     1109 2022-09-14 17:36:30.113593 getswish-0.1.2/getswish/utils.py
--rw-r--r--   0        0        0      538 2022-10-17 07:43:28.022537 getswish-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      632 2022-10-17 08:17:11.135991 getswish-0.1.2/setup.py
--rw-r--r--   0        0        0      345 2022-10-17 08:17:11.136134 getswish-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      482 2023-04-12 11:58:42.537958 getswish-0.2.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0       82 2023-04-12 10:53:14.553712 getswish-0.2.0/.gitignore
+-rw-r--r--   0        0        0      545 2023-04-12 10:52:28.828960 getswish-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-04-12 05:47:29.766259 getswish-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4598 2023-04-12 12:21:45.694971 getswish-0.2.0/README.md
+-rw-r--r--   0        0        0     1700 2023-04-12 05:47:28.634203 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr
+-rw-r--r--   0        0        0     3247 2023-04-12 05:47:28.382191 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key
+-rw-r--r--   0        0        0     7165 2023-04-12 05:47:28.594201 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12
+-rw-r--r--   0        0        0     6006 2023-04-12 05:47:28.550199 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem
+-rw-r--r--   0        0        0     1700 2023-04-12 05:47:28.942218 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr
+-rw-r--r--   0        0        0     3243 2023-04-12 05:47:28.674205 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key
+-rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.462195 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12
+-rw-r--r--   0        0        0     6006 2023-04-12 05:47:28.750209 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem
+-rw-r--r--   0        0        0     1338 2023-04-12 05:47:28.714207 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem
+-rw-r--r--   0        0        0     1700 2023-04-12 05:47:28.306187 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr
+-rw-r--r--   0        0        0     3243 2023-04-12 05:47:28.418193 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key
+-rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.506197 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12
+-rw-r--r--   0        0        0     6006 2023-04-12 05:47:28.790211 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem
+-rw-r--r--   0        0        0     1752 2023-04-12 05:47:28.906216 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr
+-rw-r--r--   0        0        0     3243 2023-04-12 05:47:28.870215 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key
+-rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.830213 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12
+-rw-r--r--   0        0        0     6009 2023-04-12 05:47:28.346189 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem
+-rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.270186 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/mss.p12
+-rw-r--r--   0        0        0   464323 2023-04-12 05:47:28.194182 getswish-0.2.0/mss_test_1.9/MSS_UserGuide_v1.9.pdf
+-rw-r--r--   0        0        0     2565 2023-04-12 05:47:27.938169 getswish-0.2.0/mss_test_1.9/readme.md
+-rw-r--r--   0        0        0      312 2023-04-12 12:01:16.027864 getswish-0.2.0/noxfile.py
+-rw-r--r--   0        0        0     1559 2023-04-12 12:31:41.642105 getswish-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-04-12 12:38:28.701423 getswish-0.2.0/src/getswish/__init__.py
+-rw-r--r--   0        0        0     6451 2023-04-12 10:31:57.423123 getswish-0.2.0/src/getswish/client.py
+-rw-r--r--   0        0        0      668 2023-04-12 07:16:33.425724 getswish-0.2.0/src/getswish/environments.py
+-rw-r--r--   0        0        0      249 2023-04-12 05:47:29.574250 getswish-0.2.0/src/getswish/exceptions.py
+-rw-r--r--   0        0        0     2914 2023-04-12 05:47:29.274235 getswish-0.2.0/src/getswish/models.py
+-rw-r--r--   0        0        0     1109 2023-04-12 05:47:29.686255 getswish-0.2.0/src/getswish/utils.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:47:30.218282 getswish-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5186 2023-04-12 07:18:51.268043 getswish-0.2.0/tests/fixtures.py
+-rw-r--r--   0        0        0     4089 2023-04-12 10:54:24.594831 getswish-0.2.0/tests/test_client.py
+-rw-r--r--   0        0        0      832 2023-04-12 05:47:29.842263 getswish-0.2.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1390 2023-04-12 10:53:53.850345 getswish-0.2.0/tests/test_models.py
+-rw-r--r--   0        0        0     1695 2023-04-12 05:47:29.878265 getswish-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 getswish-0.2.0/PKG-INFO
```

### Comparing `getswish-0.1.2/LICENSE.md` & `getswish-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getswish-0.1.2/getswish/client.py` & `getswish-0.2.0/src/getswish/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import base64
 import hashlib
 import json
 from dataclasses import dataclass
 from datetime import datetime
+from pathlib import Path
 
 import requests
 import rsa
 from requests import Response
 
 from .environments import Certificates, Environment
 from .exceptions import SwishError
 from .models import Payment, Payout, Refund
 from .utils import generate_transaction_id
 
+cert_base = Path(__file__).parent.parent.parent.resolve() / "mss_test_1.9" / "Getswish_Test_Certificates"
+
 
 @dataclass
 class SwishClient:
     environment: Environment
     certificates: Certificates
-    merchant_swish_number: str
+    merchant_swish_number: str = "12345679304"
 
     def _url(self, version: str, path: str) -> str:
         return f"{self.environment.base}{version}{path}"
 
     def _requests(self, method: str, url: str, /, **kwargs) -> Response:
         """Requests wrapper that add client certificates and handles api errors and raise http status errors."""
 
         kwargs.update(
-            cert=(self.certificates.communication.public, self.certificates.communication.private_key),
+            cert=(
+                self.certificates.communication.public,
+                self.certificates.communication.private_key,
+            ),
             verify=self.certificates.verify.public,
         )
         response = getattr(requests, method)(url=url, **kwargs)
         if response.status_code == 422:
             raise SwishError(response.json())
         response.raise_for_status()
         return response
@@ -49,20 +55,20 @@
             key_data = private_file.read()
         private_key = rsa.PrivateKey.load_pkcs1(key_data)
         signature = rsa.sign(payload_hash, private_key, "SHA-512")
         signature_b64 = base64.b64encode(signature)
         return signature_b64.decode("utf-8")
 
     def create_payment(
-        self,
-        amount: int | float,
-        callback_url: str,
-        payer_alias: str = None,
-        /,
-        **kwargs,
+            self,
+            amount: int | float,
+            callback_url: str,
+            payer_alias: str = None,
+            /,
+            **kwargs,
     ) -> Payment:
         """https://developer.swish.nu/api/payment-request/v2#create-payment-request"""
 
         payment = Payment(
             payee_alias=kwargs.get("payee_alias", self.merchant_swish_number),
             payer_alias=payer_alias,
             amount=amount,
@@ -78,38 +84,36 @@
         payment.location = response.headers.get("Location")
         payment.payment_request_token = response.headers.get("PaymentRequestToken")
         return payment
 
     def retrieve_payment(self, transaction_id: str) -> Payment:
         """https://developer.swish.nu/api/payment-request/v2#retrieve-payment-request"""
 
-        return Payment.from_service(
-            self._requests("get", self._url("v1", f"/paymentrequests/{transaction_id}")).json()
-        )
+        return Payment.from_service(self._requests("get", self._url("v1", f"/paymentrequests/{transaction_id}")).json())
 
     def cancel_payment(self, transaction_id: str) -> Payment:
         """https://developer.swish.nu/api/payment-request/v2#cancel-payment-request"""
 
         return Payment.from_service(
             self._requests(
                 "patch",
                 self._url("v1", f"/paymentrequests/{transaction_id}"),
                 json=[{"op": "replace", "path": "/status", "value": "cancelled"}],
                 headers={"Content-Type": "application/json-patch+json"},
             ).json()
         )
 
     def create_refund(
-        self,
-        original_payment_reference: str,
-        callback_url: str,
-        payee_alias: str,
-        amount: int | float,
-        /,
-        **kwargs,
+            self,
+            original_payment_reference: str,
+            callback_url: str,
+            payee_alias: str,
+            amount: int | float,
+            /,
+            **kwargs,
     ) -> Refund:
         """https://developer.swish.nu/api/refunds/v2#create-refund"""
 
         refund = Refund(
             original_payment_reference=original_payment_reference,
             callback_url=callback_url,
             payee_alias=payee_alias,
@@ -121,27 +125,25 @@
         response = self._requests("put", self._url("v2", f"/refunds/{refund.id}"), json=refund.to_service())
         refund.location = response.headers.get("Location")
         return refund
 
     def retrieve_refund(self, transaction_id: str) -> Refund:
         """https://developer.swish.nu/api/refunds/v1#retrieve-refund"""
 
-        return Refund.from_service(
-            self._requests("get", self._url("v1", f"/refunds/{transaction_id}")).json()
-        )
+        return Refund.from_service(self._requests("get", self._url("v1", f"/refunds/{transaction_id}")).json())
 
     def create_payout(
-        self,
-        payer_payment_reference: str,
-        payee_alias: str,
-        payee_ssn: str,
-        amount: int | float,
-        callback_url: str,
-        /,
-        **kwargs,
+            self,
+            payer_payment_reference: str,
+            payee_alias: str,
+            payee_ssn: str,
+            amount: int | float,
+            callback_url: str,
+            /,
+            **kwargs,
     ) -> Payout:
         """https://developer.swish.nu/api/payouts/v1#create-payout"""
 
         payout = Payout(
             payer_payment_reference=payer_payment_reference,
             payee_alias=payee_alias,
             payee_ssn=payee_ssn,
@@ -149,23 +151,21 @@
             payer_alias=kwargs.pop("payer_alias", self.merchant_swish_number),
             instruction_date=datetime.utcnow().isoformat(timespec="seconds") + "Z",
             signing_certificate_serial_number=self.certificates.signing.public_serial,
             **kwargs,
         )
         payout.payout_instruction_uuid = payout.payout_instruction_uuid or generate_transaction_id()
         payload = payout.to_service()
-        url = self._url("v1", f"/payouts")
+        url = self._url("v1", "/payouts")
         payload = {
             "payload": payload,
             "callbackUrl": callback_url,
             "signature": self._sign_payload(payload),
         }
         response = self._requests("post", url, json=payload)
         payout.location = response.headers.get("Location")
         return payout
 
     def retrieve_payout(self, transaction_id: str) -> Payout:
         """https://developer.swish.nu/api/payouts/v1#retrieve-payout"""
 
-        return Payout.from_service(
-            self._requests("get", self._url("v1", f"/payouts/{transaction_id}")).json()
-        )
+        return Payout.from_service(self._requests("get", self._url("v1", f"/payouts/{transaction_id}")).json())
```

### Comparing `getswish-0.1.2/getswish/environments.py` & `getswish-0.2.0/src/getswish/environments.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     public: str = None
     private_key: str = None
     public_serial: str = None
 
 
 @dataclass
 class Certificates:
-    communication: Certificate = field(repr=False)  # cert, private key
-    verify: Certificate = field(repr=False)  # cert
-    signing: Certificate = field(repr=False)  # cert, private key, serial
+    communication: Certificate | None = field(repr=False)  # cert, private key
+    verify: Certificate | None = field(repr=False)  # cert
+    signing: Certificate | None = field(repr=False)  # cert, private key, serial
 
 
 @dataclass
 class Environment:
     name: str
     base: str
```

### Comparing `getswish-0.1.2/getswish/models.py` & `getswish-0.2.0/src/getswish/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 
     def to_service(self) -> dict:
         """Remove empty fields and id which is always sent in URL before sending instance to swish service."""
 
         def _exclude(k, v):
             return v is None or k == "id"
 
-        return {
-            f_name_conv(k, snake2camel): v for k, v in dataclasses.asdict(self).items() if not _exclude(k, v)
-        }
+        return {f_name_conv(k, snake2camel): v for k, v in dataclasses.asdict(self).items() if not _exclude(k, v)}
 
 
 @dataclass
 class Refund(Payment):
     """https://developer.swish.nu/api/refunds/v2#refund-request-object"""
 
     original_payment_reference: str = None
```

### Comparing `getswish-0.1.2/getswish/utils.py` & `getswish-0.2.0/src/getswish/utils.py`

 * *Files identical despite different names*

