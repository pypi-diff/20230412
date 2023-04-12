# Comparing `tmp/tw_invoice-2022.6.27.tar.gz` & `tmp/tw_invoice-2023.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tw_invoice-2022.6.27.tar", last modified: Sun Jun 26 18:55:51 2022, max compression
+gzip compressed data, was "tw_invoice-2023.4.9.tar", last modified: Wed Apr 12 08:18:49 2023, max compression
```

## Comparing `tw_invoice-2022.6.27.tar` & `tw_invoice-2023.4.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      106 2022-06-26 18:55:47.348460 tw_invoice-2022.6.27/.flake8
--rw-r--r--   0        0        0      772 2022-06-26 18:55:47.348460 tw_invoice-2022.6.27/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      968 2022-06-26 18:55:47.348460 tw_invoice-2022.6.27/.github/workflows/publish-testpypi.yml
--rw-r--r--   0        0        0      919 2022-06-26 18:55:47.348460 tw_invoice-2022.6.27/.github/workflows/test.yml
--rw-r--r--   0        0        0     3299 2022-06-26 18:55:47.348460 tw_invoice-2022.6.27/.gitignore
--rw-r--r--   0        0        0      693 2022-06-26 18:55:47.348460 tw_invoice-2022.6.27/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1077 2022-06-26 18:55:47.348460 tw_invoice-2022.6.27/LICENSE
--rw-r--r--   0        0        0     1460 2022-06-26 18:55:47.348460 tw_invoice-2022.6.27/README.md
--rw-r--r--   0        0        0     1478 2022-06-26 18:55:47.352460 tw_invoice-2022.6.27/README_zh.md
--rw-r--r--   0        0        0     1462 2022-06-26 18:55:47.352460 tw_invoice-2022.6.27/pyproject.toml
--rw-r--r--   0        0        0  1287642 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/references/Application API v1.7.pdf
--rw-r--r--   0        0        0      116 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/references/README.md
--rw-r--r--   0        0        0        0 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/tests/__init__.py
--rw-r--r--   0        0        0    16442 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/tests/test_app_api_client.py
--rw-r--r--   0        0        0      434 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/tests/test_exception.py
--rw-r--r--   0        0        0     2679 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/tests/test_utils.py
--rw-r--r--   0        0        0      176 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/tw_invoice/__init__.py
--rw-r--r--   0        0        0    10744 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/tw_invoice/app_client.py
--rw-r--r--   0        0        0     1447 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/tw_invoice/carrier.py
--rw-r--r--   0        0        0      307 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/tw_invoice/exception.py
--rw-r--r--   0        0        0     3945 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/tw_invoice/schema.py
--rw-r--r--   0        0        0     2298 2022-06-26 18:55:47.356460 tw_invoice-2022.6.27/tw_invoice/utils.py
--rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 tw_invoice-2022.6.27/PKG-INFO
+-rw-r--r--   0        0        0      106 2023-04-12 08:18:44.087931 tw_invoice-2023.4.9/.flake8
+-rw-r--r--   0        0        0      772 2023-04-12 08:18:44.091931 tw_invoice-2023.4.9/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0     1082 2023-04-12 08:18:44.091931 tw_invoice-2023.4.9/.github/workflows/publish-testpypi.yml
+-rw-r--r--   0        0        0      963 2023-04-12 08:18:44.091931 tw_invoice-2023.4.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3299 2023-04-12 08:18:44.091931 tw_invoice-2023.4.9/.gitignore
+-rw-r--r--   0        0        0      693 2023-04-12 08:18:44.091931 tw_invoice-2023.4.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1077 2023-04-12 08:18:44.091931 tw_invoice-2023.4.9/LICENSE
+-rw-r--r--   0        0        0     1472 2023-04-12 08:18:44.091931 tw_invoice-2023.4.9/README.md
+-rw-r--r--   0        0        0     1502 2023-04-12 08:18:44.091931 tw_invoice-2023.4.9/README_zh.md
+-rw-r--r--   0        0        0     1462 2023-04-12 08:18:44.091931 tw_invoice-2023.4.9/pyproject.toml
+-rw-r--r--   0        0        0  1287642 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/references/Application API v1.7.pdf
+-rw-r--r--   0        0        0      116 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/references/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/tests/__init__.py
+-rw-r--r--   0        0        0    16442 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/tests/test_app_api_client.py
+-rw-r--r--   0        0        0      434 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/tests/test_exception.py
+-rw-r--r--   0        0        0     2679 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/tests/test_utils.py
+-rw-r--r--   0        0        0      175 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/tw_invoice/__init__.py
+-rw-r--r--   0        0        0    11832 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/tw_invoice/app_client.py
+-rw-r--r--   0        0        0     1447 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/tw_invoice/carrier.py
+-rw-r--r--   0        0        0      307 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/tw_invoice/exception.py
+-rw-r--r--   0        0        0     3961 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/tw_invoice/schema.py
+-rw-r--r--   0        0        0     2298 2023-04-12 08:18:44.095931 tw_invoice-2023.4.9/tw_invoice/utils.py
+-rw-r--r--   0        0        0     2995 1970-01-01 00:00:00.000000 tw_invoice-2023.4.9/PKG-INFO
```

### Comparing `tw_invoice-2022.6.27/.github/workflows/publish-pypi.yml` & `tw_invoice-2023.4.9/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `tw_invoice-2022.6.27/.github/workflows/test.yml` & `tw_invoice-2023.4.9/.github/workflows/test.yml`

 * *Files 24% similar despite different names*

```diff
@@ -9,32 +9,33 @@
       - "tw_invoice/**"
       - "tests/**"
   pull_request:
     branches: ["main"]
 
 jobs:
   test:
+    name: 🧪 Test
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     steps:
-      - name: Checkout repository
+      - name: 🛒 Checkout
         uses: actions/checkout@v3
 
-      - name: Set up Python ${{ matrix.python-version }}
+      - name: 🐍 Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
 
-      - name: Install dependencies
+      - name: 📦 Install dependencies
         run: |
           python -m pip install --upgrade pip flit
           flit install --deps develop --symlink
 
-      - name: Test with pytest
+      - name: 🧪 Test with pytest
         run: |
           pytest --cov=tw_invoice --cov-report=xml
 
-      - name: Upload coverage report
+      - name: ⬆️ Upload coverage report
         uses: codecov/codecov-action@v2
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tw_invoice-2022.6.27/.gitignore` & `tw_invoice-2023.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tw_invoice-2022.6.27/.pre-commit-config.yaml` & `tw_invoice-2023.4.9/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.3.0"
+    rev: "v4.4.0"
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/flake8
-    rev: "4.0.1"
+    rev: "6.0.0"
     hooks:
       - id: flake8
   - repo: https://github.com/pycqa/isort
-    rev: "5.10.1"
+    rev: "5.12.0"
     hooks:
       - id: isort
         name: isort (python)
       - id: isort
         name: isort (cython)
         types: [cython]
       - id: isort
         name: isort (pyi)
         types: [pyi]
   - repo: https://github.com/psf/black
-    rev: "22.3.0"
+    rev: "23.1.0"
     hooks:
       - id: black
         language_version: python3
```

### Comparing `tw_invoice-2022.6.27/LICENSE` & `tw_invoice-2023.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tw_invoice-2022.6.27/README.md` & `tw_invoice-2023.4.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 🇹🇼 Taiwan Invoice
 
 [![PyPI](https://img.shields.io/pypi/v/tw_invoice?color=brightgreen&logo=pypi&logoColor=white)](https://pypi.org/project/tw_invoice)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tw_invoice?color=brightgreen&logo=python&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tw_invoice?color=brightgreen)
 ![PyPI - License](https://img.shields.io/pypi/l/tw_invoice?color=brightgreen)
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/tomy0000000/tw-invoice/Test?logo=Github)](https://github.com/tomy0000000/tw-invoice/actions/workflows/test.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/tomy0000000/tw-invoice/test.yml?branch=main&logo=Github)](https://github.com/tomy0000000/tw-invoice/actions/workflows/test.yml)
 [![Coverage](https://img.shields.io/codecov/c/github/tomy0000000/tw-invoice?color=brightgreen&logo=codecov&logoColor=white&token=ESgHfrrk6z)](https://codecov.io/gh/tomy0000000/tw-invoice)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/tomy0000000/tw-invoice/main.svg)](https://results.pre-commit.ci/latest/github/tomy0000000/tw-invoice/main)
 
 [中文版 README](https://github.com/tomy0000000/tw-invoice/blob/main/README_zh.md)
 
 SDK for Ministry of Finance, R.O.C. [E-invoice platform](https://www.einvoice.nat.gov.tw)
 
@@ -17,8 +17,8 @@
 
 See [Wiki](https://github.com/tomy0000000/tw-invoice/wiki)
 
 ## LICENSE and disclaimer
 
 The source code is released under MIT license, versions with suffix b represent beta version, use at your own risk.
 
-The author is not affiliated in any kind to the platform, or MoF in any kind.
+The author is not affiliated to MoF, or the platform in any kind.
```

### Comparing `tw_invoice-2022.6.27/README_zh.md` & `tw_invoice-2023.4.9/README_zh.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 🇹🇼 Taiwan Invoice
 
 [![PyPI](https://img.shields.io/pypi/v/tw_invoice?color=brightgreen&logo=pypi&logoColor=white)](https://pypi.org/project/tw_invoice)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tw_invoice?color=brightgreen&logo=python&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tw_invoice?color=brightgreen)
 ![PyPI - License](https://img.shields.io/pypi/l/tw_invoice?color=brightgreen)
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/tomy0000000/tw-invoice/Test?logo=Github)](https://github.com/tomy0000000/tw-invoice/actions/workflows/test.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/tomy0000000/tw-invoice/test.yml?branch=main&logo=Github)](https://github.com/tomy0000000/tw-invoice/actions/workflows/test.yml)
 [![Coverage](https://img.shields.io/codecov/c/github/tomy0000000/tw-invoice?color=brightgreen&logo=codecov&logoColor=white&token=ESgHfrrk6z)](https://codecov.io/gh/tomy0000000/tw-invoice)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/tomy0000000/tw-invoice/main.svg)](https://results.pre-commit.ci/latest/github/tomy0000000/tw-invoice/main)
 
 [English README](https://github.com/tomy0000000/tw-invoice/blob/main/README.md)
 
 財政部[電子發票整合服務平台](https://www.einvoice.nat.gov.tw) SDK
```

### Comparing `tw_invoice-2022.6.27/pyproject.toml` & `tw_invoice-2023.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tw_invoice-2022.6.27/references/Application API v1.7.pdf` & `tw_invoice-2023.4.9/references/Application API v1.7.pdf`

 * *Files identical despite different names*

### Comparing `tw_invoice-2022.6.27/tests/test_app_api_client.py` & `tw_invoice-2023.4.9/tests/test_app_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         invoice_random=TEST_INVOICE_RANDOM,
         invoice_encrypt=TEST_INVOICE_ENCRYPT,
         seller_id=TEST_SELLER_ID,
     )
     mocked_session_post.assert_called_once_with(
         build_api_url("invapp"),
         data={
-            "version": 0.5,
+            "version": 0.6,
             "type": "QRCode",
             "invNum": TEST_INVOICE_NUMBER,
             "action": "qryInvDetail",
             "generation": "V2",
             "invTerm": None,
             "invDate": TEST_DATE_STR,
             "encrypt": TEST_INVOICE_ENCRYPT,
@@ -268,15 +268,15 @@
         invoice_date=TEST_DATE,
         invoice_random=TEST_INVOICE_RANDOM,
         invoice_term=TEST_INVOICE_TERM,
     )
     mocked_session_post.assert_called_once_with(
         build_api_url("invapp"),
         data={
-            "version": 0.5,
+            "version": 0.6,
             "type": "Barcode",
             "invNum": TEST_INVOICE_NUMBER,
             "action": "qryInvDetail",
             "generation": "V2",
             "invTerm": TEST_INVOICE_TERM,
             "invDate": TEST_DATE_STR,
             "encrypt": None,
```

### Comparing `tw_invoice-2022.6.27/tests/test_utils.py` & `tw_invoice-2023.4.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tw_invoice-2022.6.27/tw_invoice/app_client.py` & `tw_invoice-2023.4.9/tw_invoice/app_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from datetime import date
 from time import time
 from typing import Union
 from uuid import uuid4
 
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
+
+from requests import Session
+from requests.adapters import HTTPAdapter, Retry
+
 from .schema import (
     AggregateCarrierResponse,
     CarrierInvoiceDonateResponse,
     CarrierInvoicesDetailResponse,
     CarrierInvoicesHeaderResponse,
     InvoiceDetailResponse,
     InvoiceHeaderResponse,
     LotteryNumberResponse,
     LoveCodeResponse,
 )
-
-try:
-    from typing import Literal
-except ImportError:
-    from typing_extensions import Literal
-
-from requests import Session
-
 from .utils import (
     build_api_url,
     check_api_error,
     sign,
     validate_invoice_number,
     validate_invoice_random,
     validate_invoice_term,
@@ -34,14 +34,15 @@
 class AppAPIClient(object):
     def __init__(
         self,
         app_id: str,
         api_key: str,
         uuid: Union[str, None] = None,
         ts_tolerance: int = 20,
+        max_retries: int = 20,
         skip_validation: bool = False,
     ):
         self.app_id = app_id
         self.api_key = api_key
         self.uuid = str(uuid) if uuid else str(uuid4())
         if ts_tolerance < 10 or ts_tolerance > 180:
             raise ValueError("ts_tolerance must be between 10 and 180")
@@ -50,14 +51,26 @@
             raise ValueError("skip_validation must be a boolean")
         self.skip_validation = skip_validation
         self.serial = 1
         self.session = Session()
         self.session.headers.update(
             {"Content-Type": "application/x-www-form-urlencoded"}
         )
+        self.session.mount(
+            "https://",
+            HTTPAdapter(
+                max_retries=Retry(
+                    total=max_retries,
+                    backoff_factor=0.1,
+                    allowed_methods=["POST"],
+                    status_forcelist=[500, 502, 503, 504],
+                    raise_on_status=False,
+                )
+            ),
+        )
 
     def get_lottery_numbers(
         self, invoice_term: str
     ) -> Union[LotteryNumberResponse, dict]:
         """查詢中獎發票號碼清單 v0.2"""
         URL = build_api_url("invapp")
         VERSION = 0.2
@@ -109,17 +122,35 @@
         invoice_number: str,
         invoice_date: date,
         invoice_random: str,
         invoice_term: Union[str, None] = None,
         invoice_encrypt: Union[str, None] = None,
         seller_id: Union[str, None] = None,
     ):
-        """查詢發票明細 v0.5"""
+        """
+        查詢發票明細 v0.6
+        `invoice_random`: 錯誤將僅回傳發票表頭，正確將回傳完整明細
+
+        `barcode_type`: "Barcode"
+        `invoice_number`: 發票號碼
+        `invoice_date`: 發票日期
+        `invoice_random`: 發票隨機碼 (4位)
+        `invoice_term`: 發票期別， 3 位民國年+ 2 位雙數月份，如：11006
+
+        or
+
+        `barcode_type`: "QRCode"
+        `invoice_number`: 發票號碼
+        `invoice_date`: 發票日期
+        `invoice_random`: 發票隨機碼 (4位)
+        `invoice_encrypt`: 發票檢驗碼 (左側QRCode中，24位)
+        `seller_id`: 商家統編
+        """
         URL = build_api_url("invapp")
-        VERSION = 0.5
+        VERSION = 0.6
         if barcode_type == "QRCode":
             if not invoice_encrypt:
                 raise ValueError(
                     "invoice_encrypt is required when barcode_type is QRCode"
                 )
             if not isinstance(invoice_encrypt, str) or len(invoice_encrypt) != 24:
                 raise ValueError("invoice_encrypt must be a string of 24 characters")
```

### Comparing `tw_invoice-2022.6.27/tw_invoice/carrier.py` & `tw_invoice-2023.4.9/tw_invoice/carrier.py`

 * *Files identical despite different names*

### Comparing `tw_invoice-2022.6.27/tw_invoice/schema.py` & `tw_invoice-2023.4.9/tw_invoice/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     invStatus: str
     invPeriod: str
     sellerBan: str
     sellerAddress: str
     invoiceTime: str
     buyerBan: str
     currency: str
+    amount: str
     details: Union[List[InvoiceDetail], None] = None
 
 
 # LoveCodeResponse
 
 
 class LoveCode(BaseModel):
```

### Comparing `tw_invoice-2022.6.27/tw_invoice/utils.py` & `tw_invoice-2023.4.9/tw_invoice/utils.py`

 * *Files identical despite different names*

### Comparing `tw_invoice-2022.6.27/PKG-INFO` & `tw_invoice-2023.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tw_invoice
-Version: 2022.6.27
+Version: 2023.4.9
 Summary: 🇹🇼🧾 Python SDK for accessing Taiwan E-Inovice API
 Keywords: taiwan,tw,invoice,tax,taxation,tax-invoice,invoice-api
 Author-email: Tomy Hsieh <pypi@tomy.me>
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -35,15 +35,15 @@
 # 🇹🇼 Taiwan Invoice
 
 [![PyPI](https://img.shields.io/pypi/v/tw_invoice?color=brightgreen&logo=pypi&logoColor=white)](https://pypi.org/project/tw_invoice)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tw_invoice?color=brightgreen&logo=python&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tw_invoice?color=brightgreen)
 ![PyPI - License](https://img.shields.io/pypi/l/tw_invoice?color=brightgreen)
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/tomy0000000/tw-invoice/Test?logo=Github)](https://github.com/tomy0000000/tw-invoice/actions/workflows/test.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/tomy0000000/tw-invoice/test.yml?branch=main&logo=Github)](https://github.com/tomy0000000/tw-invoice/actions/workflows/test.yml)
 [![Coverage](https://img.shields.io/codecov/c/github/tomy0000000/tw-invoice?color=brightgreen&logo=codecov&logoColor=white&token=ESgHfrrk6z)](https://codecov.io/gh/tomy0000000/tw-invoice)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/tomy0000000/tw-invoice/main.svg)](https://results.pre-commit.ci/latest/github/tomy0000000/tw-invoice/main)
 
 [中文版 README](https://github.com/tomy0000000/tw-invoice/blob/main/README_zh.md)
 
 SDK for Ministry of Finance, R.O.C. [E-invoice platform](https://www.einvoice.nat.gov.tw)
 
@@ -51,9 +51,9 @@
 
 See [Wiki](https://github.com/tomy0000000/tw-invoice/wiki)
 
 ## LICENSE and disclaimer
 
 The source code is released under MIT license, versions with suffix b represent beta version, use at your own risk.
 
-The author is not affiliated in any kind to the platform, or MoF in any kind.
+The author is not affiliated to MoF, or the platform in any kind.
```

