# Comparing `tmp/python-bol-api-latest-1.2.0.tar.gz` & `tmp/python-bol-api-latest-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bol-api-latest-1.2.0.tar", last modified: Mon Jul 11 07:39:02 2022, max compression
+gzip compressed data, was "python-bol-api-latest-1.3.0.tar", last modified: Wed Apr 12 14:04:43 2023, max compression
```

## Comparing `python-bol-api-latest-1.2.0.tar` & `python-bol-api-latest-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 07:39:02.836741 python-bol-api-latest-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     8153 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-07-11 07:39:02.836741 python-bol-api-latest-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 07:39:02.832741 python-bol-api-latest-1.2.0/bol/
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/bol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 07:39:02.832741 python-bol-api-latest-1.2.0/bol/openapi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/bol/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/bol/openapi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 07:39:02.832741 python-bol-api-latest-1.2.0/bol/retailer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/bol/retailer/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17607 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/bol/retailer/api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10172 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/bol/retailer/models.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 07:39:02.836741 python-bol-api-latest-1.2.0/python_bol_api_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-07-11 07:39:02.000000 python-bol-api-latest-1.2.0/python_bol_api_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-07-11 07:39:02.000000 python-bol-api-latest-1.2.0/python_bol_api_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 07:39:02.000000 python-bol-api-latest-1.2.0/python_bol_api_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 07:39:02.000000 python-bol-api-latest-1.2.0/python_bol_api_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-11 07:39:02.000000 python-bol-api-latest-1.2.0/python_bol_api_latest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-11 07:39:02.000000 python-bol-api-latest-1.2.0/python_bol_api_latest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-07-11 07:39:02.836741 python-bol-api-latest-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-07-11 07:38:48.000000 python-bol-api-latest-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:04:43.521305 python-bol-api-latest-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-12 14:04:43.521305 python-bol-api-latest-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:04:43.521305 python-bol-api-latest-1.3.0/bol/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/bol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:04:43.521305 python-bol-api-latest-1.3.0/bol/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/bol/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/bol/openapi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:04:43.521305 python-bol-api-latest-1.3.0/bol/retailer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/bol/retailer/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17860 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/bol/retailer/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10220 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/bol/retailer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:04:43.521305 python-bol-api-latest-1.3.0/python_bol_api_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-12 14:04:43.000000 python-bol-api-latest-1.3.0/python_bol_api_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-12 14:04:43.000000 python-bol-api-latest-1.3.0/python_bol_api_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:04:43.000000 python-bol-api-latest-1.3.0/python_bol_api_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:04:43.000000 python-bol-api-latest-1.3.0/python_bol_api_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:04:43.000000 python-bol-api-latest-1.3.0/python_bol_api_latest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 14:04:43.000000 python-bol-api-latest-1.3.0/python_bol_api_latest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-12 14:04:43.521305 python-bol-api-latest-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:04:43.521305 python-bol-api-latest-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-12 14:04:31.000000 python-bol-api-latest-1.3.0/tests/test_openapi.py
```

### Comparing `python-bol-api-latest-1.2.0/LICENSE` & `python-bol-api-latest-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bol-api-latest-1.2.0/PKG-INFO` & `python-bol-api-latest-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bol-api-latest
-Version: 1.2.0
+Version: 1.3.0
 Summary: Wrapper for the bol.com API
 Home-page: https://dreambits.in
 Author: Raymond Penners, Dreambits Technologies Pvt. Ltd.
 Author-email: office@dreambits.in
 Keywords: bol bol.com api wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -58,15 +58,15 @@
 
     >>> data['products'][0]['ean']
     u'0093155141650'
 
 Retailer API
 ============
 
-Supports the BOL Api v7, documented here: https://api.bol.com/retailer/public/Retailer-API/selling-on-bolcom-processflow.html
+Supports the BOL Api v8, documented here: https://api.bol.com/retailer/public/Retailer-API/selling-on-bolcom-processflow.html
 
 Instantiate the API::
 
     >>> from bol.retailer.api import RetailerAPI
     >>> api = RetailerAPI()
 
 Authenticate::
```

### Comparing `python-bol-api-latest-1.2.0/README.rst` & `python-bol-api-latest-1.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     >>> data['products'][0]['ean']
     u'0093155141650'
 
 Retailer API
 ============
 
-Supports the BOL Api v7, documented here: https://api.bol.com/retailer/public/Retailer-API/selling-on-bolcom-processflow.html
+Supports the BOL Api v8, documented here: https://api.bol.com/retailer/public/Retailer-API/selling-on-bolcom-processflow.html
 
 Instantiate the API::
 
     >>> from bol.retailer.api import RetailerAPI
     >>> api = RetailerAPI()
 
 Authenticate::
```

### Comparing `python-bol-api-latest-1.2.0/bol/openapi/api.py` & `python-bol-api-latest-1.3.0/bol/openapi/api.py`

 * *Files identical despite different names*

### Comparing `python-bol-api-latest-1.2.0/bol/retailer/api.py` & `python-bol-api-latest-1.3.0/bol/retailer/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,27 @@
         return self.api.request(method, uri, params=params, **kwargs)
 
 
 class OrderMethods(MethodGroup):
     def __init__(self, api):
         super(OrderMethods, self).__init__(api, "orders")
 
-    def list(self, fulfilment_method=None, page=None, status=None):
+    def list(self, fulfilment_method=None, page=None, status=None, change_interval_minute=None, latest_change_date=None):
         params = {}
         if fulfilment_method:
             params["fulfilment-method"] = fulfilment_method
         if page is not None:
             params["page"] = page
         if status:
             params["status"] = status
+        if change_interval_minute:
+            params["change-interval-minute"] = change_interval_minute
+        if latest_change_date:
+            params["latest-change-date"] = latest_change_date
+
         resp = self.request("GET", params=params)
         return Orders.parse(self.api, resp.text)
 
     def get(self, order_id):
         resp = self.request("GET", path=order_id)
         return Order.parse(self.api, resp.text)
 
@@ -221,15 +226,15 @@
                 "shippingLabelOfferId" : label_id
             }
             response = self.request("POST", json=payload)
             return ProcessStatus.parse(self.api, response.text)
 
     def getShippingLabel(self, shipping_label_id):
         headers = {
-            "accept": "application/vnd.retailer.v7+pdf"
+            "accept": "application/vnd.retailer.v8+pdf"
         }
         response = self.request('GET', path=str(shipping_label_id), headers=headers)
         return response
 
 class OffersMethods(MethodGroup):
 
     def __init__(self, api):
@@ -278,15 +283,15 @@
             'format': 'CSV'
         }
         response = self.request('POST', path='export', json=payload)
         return ProcessStatus.parse(self.api, response.text)
 
     def getOffersFile(self, export_id):
         headers = {
-            "accept": "application/vnd.retailer.v7+csv"
+            "accept": "application/vnd.retailer.v8+csv"
         }
         response = self.request('GET', path='export/{}'.format(export_id),
                                 headers=headers)
         return response
 
     def deleteOffers(self, offer_id):
         response = self.request('DELETE', path='{}'.format(offer_id))
@@ -343,37 +348,37 @@
     def getProductLabels(self, labelFormat, products):
         params = {
             "labelFormat" : labelFormat,
             "products" : products
         }
 
         headers = {
-            "accept": "application/vnd.retailer.v7+pdf"
+            "accept": "application/vnd.retailer.v8+pdf"
         }
         response = self.request("POST", path="product-labels", headers=headers, json=params)
         return response
 
     def getById(self, replenishment_id):
         response = self.request("GET", path=str(replenishment_id))
         return Replenishment.parse(self.api, response.text)
 
     def update(self, replenishment_id, **param):
         response = self.request("PUT", path=str(replenishment_id), json=param)
         return ProcessStatus.parse(self.api, response.text)
 
     def getLoadCarrierLabels(self, replenishment_id, label_type="WAREHOUSE"):
         headers = {
-            "accept": "application/vnd.retailer.v7+pdf"
+            "accept": "application/vnd.retailer.v8+pdf"
         }
         response = self.request("GET", path='{}/load-carrier-labels'.format(replenishment_id), headers=headers, json=label_type)
         return response
 
     def getPickList(self, replenishment_id):
         headers = {
-            "accept": "application/vnd.retailer.v7+pdf"
+            "accept": "application/vnd.retailer.v8+pdf"
         }
         response = self.request("GET", path='{}/pick-list'.format(replenishment_id), headers=headers)
         return response
 
 class InventoryMethods(MethodGroup):
     def __init__(self, api):
         super(InventoryMethods, self).__init__(api, "inventory")
@@ -485,15 +490,15 @@
         self.set_access_token(data["access_token"])
         return data
 
     def set_access_token(self, access_token):
         self.session.headers.update(
             {
                 "Authorization": "Bearer " + access_token,
-                "Accept": "application/vnd.retailer.v7+json",
+                "Accept": "application/vnd.retailer.v8+json",
             }
         )
 
     def request(self, method, uri, params={}, **kwargs):
         request_kwargs = dict(**kwargs)
         request_kwargs.update(
             {
@@ -505,15 +510,15 @@
         )
         if "json" in request_kwargs:
             if "headers" not in request_kwargs:
                 request_kwargs["headers"] = {}
             # If these headers are not added, the api returns a 400
             # Reference:
             #   https://api.bol.com/retailer/public/conventions/index.html
-            content_header = "application/vnd.retailer.v7+json"
+            content_header = "application/vnd.retailer.v8+json"
 
             request_kwargs["headers"].update({
                 "content-type": content_header
             })
 
         resp = self.session.request(**request_kwargs)
         resp.raise_for_status()
```

### Comparing `python-bol-api-latest-1.2.0/bol/retailer/models.py` & `python-bol-api-latest-1.3.0/bol/retailer/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
     class Meta:
         fulfilment = ModelField(Fulfilment)
         offer = ModelField(Offer)
         product = ModelField(Product)
         additionalServices = ModelField(additionalServices)
         offerPrice = DecimalField()
         transactionFee = DecimalField()
+        latestChangedDateTime = DateTimeField()
 
 
 class OrderItems(ModelList):
     class Meta:
         item_type = OrderItem
```

### Comparing `python-bol-api-latest-1.2.0/python_bol_api_latest.egg-info/PKG-INFO` & `python-bol-api-latest-1.3.0/python_bol_api_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bol-api-latest
-Version: 1.2.0
+Version: 1.3.0
 Summary: Wrapper for the bol.com API
 Home-page: https://dreambits.in
 Author: Raymond Penners, Dreambits Technologies Pvt. Ltd.
 Author-email: office@dreambits.in
 Keywords: bol bol.com api wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -58,15 +58,15 @@
 
     >>> data['products'][0]['ean']
     u'0093155141650'
 
 Retailer API
 ============
 
-Supports the BOL Api v7, documented here: https://api.bol.com/retailer/public/Retailer-API/selling-on-bolcom-processflow.html
+Supports the BOL Api v8, documented here: https://api.bol.com/retailer/public/Retailer-API/selling-on-bolcom-processflow.html
 
 Instantiate the API::
 
     >>> from bol.retailer.api import RetailerAPI
     >>> api = RetailerAPI()
 
 Authenticate::
```

### Comparing `python-bol-api-latest-1.2.0/setup.py` & `python-bol-api-latest-1.3.0/setup.py`

 * *Files identical despite different names*

