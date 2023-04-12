# Comparing `tmp/pychee-0.2.0-py3-none-any.whl.zip` & `tmp/pychee-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 19288 bytes, number of entries: 8
+Zip file size: 19284 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      175 b- defN 23-Feb-19 10:21 pychee/__init__.py
--rw-r--r--  2.0 unx    15019 b- defN 23-Feb-20 14:54 pychee/pychee.py
--rw-r--r--  2.0 unx      766 b- defN 23-Feb-20 14:47 pychee/test.py
--rw-r--r--  2.0 unx    34523 b- defN 23-Feb-20 15:03 pychee-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2687 b- defN 23-Feb-20 15:03 pychee-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-20 15:03 pychee-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Feb-20 15:03 pychee-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      599 b- defN 23-Feb-20 15:03 pychee-0.2.0.dist-info/RECORD
-8 files, 53868 bytes uncompressed, 18254 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx    15035 b- defN 23-Apr-12 21:27 pychee/pychee.py
+-rw-r--r--  2.0 unx      766 b- defN 23-Apr-12 21:26 pychee/test.py
+-rw-r--r--  2.0 unx    34523 b- defN 23-Apr-12 21:28 pychee-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2687 b- defN 23-Apr-12 21:28 pychee-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 21:28 pychee-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-12 21:28 pychee-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      599 b- defN 23-Apr-12 21:28 pychee-0.2.1.dist-info/RECORD
+8 files, 53884 bytes uncompressed, 18250 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pychee/pychee.py
 Comment: 
 
 Filename: pychee/test.py
 Comment: 
 
-Filename: pychee-0.2.0.dist-info/LICENSE
+Filename: pychee-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: pychee-0.2.0.dist-info/METADATA
+Filename: pychee-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: pychee-0.2.0.dist-info/WHEEL
+Filename: pychee-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: pychee-0.2.0.dist-info/top_level.txt
+Filename: pychee-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pychee-0.2.0.dist-info/RECORD
+Filename: pychee-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pychee/pychee.py

```diff
@@ -6,15 +6,15 @@
 For additonal information, visit: https://github.com/LycheeOrg/Lychee.
 """
 from posixpath import join
 from typing import List
 from requests import Session
 from urllib.parse import unquote
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 class LycheeForbidden(Exception):
     """Raised when the Lychee request is unauthorized."""
 
 class LycheeNotFound(Exception):
     """Raised when the requested ressource was not found."""
 
@@ -79,15 +79,16 @@
         CSRF generally prevents an attacker from forging a request
         sent from another website, e.g. in a JS script, by forcing
         requests to contain a specific value which has been set
         as a cookie in a previous GET request.
 
         Thus, a previous GET request is needed so this method works.
         """
-        if (csrf_token := self.cookies.get(self._CSRF_COOKIE)) is not None:
+        csrf_token = self.cookies.get(self._CSRF_COOKIE)
+        if csrf_token is not None:
             if csrf_token != self.headers.get(self._CSRF_HEADER):
                 self.headers[self._CSRF_HEADER] = unquote(csrf_token).replace('=', '')
 
 class LycheeClient:
     """
     Lychee API Client.
```

## pychee/test.py

```diff
@@ -3,15 +3,15 @@
 client.login('Chosto', 'TWM4W3APC9J2Oczn2RSeb6tmoPJYyUMQVNAtqDvh')
 
 # Create a new album
 album_name = 'test_name'
 album_id = client.add_album(album_name)['id']
 
 # Add a photo in the created album
-path_to_your_photo = '/home/img/screenshots/2023-02-20_15-39-46.png'
+path_to_your_photo = '/home/images/screenshots/2023-02-19_19-48.png'
 with open(path_to_your_photo, 'rb') as f:
     photo_id = client.add_photo(f, 'photo.jpg', album_id)['id']
 
 # Set uploaded photo public
 client.set_photo_public(photo_id)
 
 # Set licence of uploaded photo
```

## Comparing `pychee-0.2.0.dist-info/LICENSE` & `pychee-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pychee-0.2.0.dist-info/METADATA` & `pychee-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychee
-Version: 0.2.0
+Version: 0.2.1
 Summary: Client for Lychee, written in Python.
 Home-page: https://github.com/Chostakovitch/pychee
 Author: Quentin Duchemin
 Author-email: quentinduchemin@tuta.io
 License: AGPL-3.0
 Keywords: lychee
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

## Comparing `pychee-0.2.0.dist-info/RECORD` & `pychee-0.2.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 pychee/__init__.py,sha256=ghjLFvHybz-ABmLZBlXRWTinydNnmsqMiZ5j9fbwZZk,175
-pychee/pychee.py,sha256=9klOvEriCLpm4Tfd3wOVENqb21h_8a5rNL2snbtSSw0,15019
-pychee/test.py,sha256=tnM7thu2odVWliIeW5yUewbgsY3v3AlEozuOH4ZBGho,766
-pychee-0.2.0.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-pychee-0.2.0.dist-info/METADATA,sha256=Z6uOMIacySdaLPq6jFkNFWAyp2fmnltBDtb86Jwcl7Y,2687
-pychee-0.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pychee-0.2.0.dist-info/top_level.txt,sha256=JGcwDtuVtkyJz6Lj49wqpY74jPPdKZHbLBMjpVqFXyk,7
-pychee-0.2.0.dist-info/RECORD,,
+pychee/pychee.py,sha256=72h9Cdx_mIjGYElLKlVOtPboTicjEFCMgk9tQzePXVA,15035
+pychee/test.py,sha256=zpQKAWbCq_9lAaJCVhyOXLR8sAGmnw6xe5t5oeGQwBg,766
+pychee-0.2.1.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+pychee-0.2.1.dist-info/METADATA,sha256=RrnK7PMmd_PwgJMGiS3zrfXnbKNuG-4nS3bhNKp4eno,2687
+pychee-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pychee-0.2.1.dist-info/top_level.txt,sha256=JGcwDtuVtkyJz6Lj49wqpY74jPPdKZHbLBMjpVqFXyk,7
+pychee-0.2.1.dist-info/RECORD,,
```

