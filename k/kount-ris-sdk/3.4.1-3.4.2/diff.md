# Comparing `tmp/kount_ris_sdk-3.4.1.tar.gz` & `tmp/kount_ris_sdk-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kount_ris_sdk-3.4.1.tar", last modified: Mon Mar 13 17:00:25 2023, max compression
+gzip compressed data, was "kount_ris_sdk-3.4.2.tar", last modified: Wed Apr 12 17:39:18 2023, max compression
```

## Comparing `kount_ris_sdk-3.4.1.tar` & `kount_ris_sdk-3.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-03-13 17:00:25.108536 kount_ris_sdk-3.4.1/
--rw-rw-rw-   0 root         (0) nogroup  (65534)     4919 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/LICENSE
--rw-rw-rw-   0 root         (0) nogroup  (65534)       76 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) nogroup  (65534)     2016 2023-03-13 17:00:25.108536 kount_ris_sdk-3.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) nogroup  (65534)     1208 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/README.md
--rw-rw-rw-   0 root         (0) nogroup  (65534)      300 2023-03-13 17:00:25.108536 kount_ris_sdk-3.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) nogroup  (65534)     2972 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/setup.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-03-13 17:00:25.104536 kount_ris_sdk-3.4.1/src/
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-03-13 17:00:25.104536 kount_ris_sdk-3.4.1/src/kount/
--rw-rw-rw-   0 root         (0) nogroup  (65534)      543 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/__init__.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     3540 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/client.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     2145 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/config.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     9396 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/inquiry.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)    13832 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/request.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-03-13 17:00:25.104536 kount_ris_sdk-3.4.1/src/kount/resources/
--rw-rw-rw-   0 root         (0) nogroup  (65534)      373 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/resources/__init__.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)      564 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/resources/correct_key_cryp.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)    21008 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/response.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)      178 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/settings.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-03-13 17:00:25.108536 kount_ris_sdk-3.4.1/src/kount/util/
--rw-rw-rw-   0 root         (0) nogroup  (65534)      529 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/util/__init__.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)      371 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/util/a85.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     1532 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/util/address.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     1483 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/util/cartitem.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     4917 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/util/khash.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)    10011 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/util/payment.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)       87 2023-03-13 17:00:19.000000 kount_ris_sdk-3.4.1/src/kount/version.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-03-13 17:00:25.108536 kount_ris_sdk-3.4.1/src/kount_ris_sdk.egg-info/
--rw-r--r--   0 root         (0) nogroup  (65534)     2016 2023-03-13 17:00:25.000000 kount_ris_sdk-3.4.1/src/kount_ris_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) nogroup  (65534)      645 2023-03-13 17:00:25.000000 kount_ris_sdk-3.4.1/src/kount_ris_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) nogroup  (65534)        1 2023-03-13 17:00:25.000000 kount_ris_sdk-3.4.1/src/kount_ris_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) nogroup  (65534)      317 2023-03-13 17:00:25.000000 kount_ris_sdk-3.4.1/src/kount_ris_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) nogroup  (65534)        6 2023-03-13 17:00:25.000000 kount_ris_sdk-3.4.1/src/kount_ris_sdk.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     4919 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/LICENSE
+-rw-rw-rw-   0 root         (0) nogroup  (65534)       76 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) nogroup  (65534)     1408 2023-04-12 17:39:18.173129 kount_ris_sdk-3.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      600 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/README.md
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      300 2023-04-12 17:39:18.177129 kount_ris_sdk-3.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     2972 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/setup.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/src/
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/src/kount/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      543 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/__init__.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     3540 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/client.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     2145 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/config.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     9396 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/inquiry.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)    13833 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/request.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/src/kount/resources/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      373 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/resources/__init__.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      564 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/resources/correct_key_cryp.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)    21008 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/response.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      178 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/settings.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/src/kount/util/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      529 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/__init__.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      371 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/a85.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     1532 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/address.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     1483 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/cartitem.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     4917 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/khash.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)    10011 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/payment.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)       87 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/version.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/
+-rw-r--r--   0 root         (0) nogroup  (65534)     1408 2023-04-12 17:39:18.000000 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) nogroup  (65534)      645 2023-04-12 17:39:18.000000 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) nogroup  (65534)        1 2023-04-12 17:39:18.000000 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) nogroup  (65534)      317 2023-04-12 17:39:18.000000 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) nogroup  (65534)        6 2023-04-12 17:39:18.000000 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/top_level.txt
```

### Comparing `kount_ris_sdk-3.4.1/LICENSE` & `kount_ris_sdk-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/setup.py` & `kount_ris_sdk-3.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/__init__.py` & `kount_ris_sdk-3.4.2/src/kount/__init__.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/client.py` & `kount_ris_sdk-3.4.2/src/kount/client.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/config.py` & `kount_ris_sdk-3.4.2/src/kount/config.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/inquiry.py` & `kount_ris_sdk-3.4.2/src/kount/inquiry.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/request.py` & `kount_ris_sdk-3.4.2/src/kount/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
                     merchant_id = int(self.params["MERC"])
                     payment.payment_token = khasher.hash_gift_card(
                         merchant_id, payment.payment_token)
                 else:
                     payment.payment_token = khasher.hash_payment_token(
                         payment.payment_token)
                 payment.khashed = True
-                self.set_param("PENC", "MASK")
+                self.set_param("PENC", "KHASH")
                 LOG.debug("payment.khashed=%s", payment.khashed)
             except ValueError as nfe:
                 LOG.debug("Error converting Merchant ID to integer"
                           " value. Set a valid Merchant ID. %s",
                           str(nfe))
                 raise nfe
             except Exception as nsae:
```

### Comparing `kount_ris_sdk-3.4.1/src/kount/resources/correct_key_cryp.py` & `kount_ris_sdk-3.4.2/src/kount/resources/correct_key_cryp.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/response.py` & `kount_ris_sdk-3.4.2/src/kount/response.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/util/__init__.py` & `kount_ris_sdk-3.4.2/src/kount/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/util/address.py` & `kount_ris_sdk-3.4.2/src/kount/util/address.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/util/cartitem.py` & `kount_ris_sdk-3.4.2/src/kount/util/cartitem.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/util/khash.py` & `kount_ris_sdk-3.4.2/src/kount/util/khash.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount/util/payment.py` & `kount_ris_sdk-3.4.2/src/kount/util/payment.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.1/src/kount_ris_sdk.egg-info/SOURCES.txt` & `kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

