# Comparing `tmp/gordo_core-0.3.0-py3-none-any.whl.zip` & `tmp/gordo_core-0.3.0rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 60874 bytes, number of entries: 26
+Zip file size: 60901 bytes, number of entries: 26
 -rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx       74 b- defN 80-Jan-01 00:00 gordo_core/__init__.py
--rw-r--r--  2.0 unx       81 b- defN 80-Jan-01 00:00 gordo_core/_version.py
+-rw-r--r--  2.0 unx       84 b- defN 80-Jan-01 00:00 gordo_core/_version.py
 -rw-r--r--  2.0 unx     2233 b- defN 80-Jan-01 00:00 gordo_core/back_compatibles.py
 -rw-r--r--  2.0 unx     7723 b- defN 80-Jan-01 00:00 gordo_core/base.py
 -rw-r--r--  2.0 unx      102 b- defN 80-Jan-01 00:00 gordo_core/data_providers/__init__.py
 -rw-r--r--  2.0 unx     5269 b- defN 80-Jan-01 00:00 gordo_core/data_providers/base.py
 -rw-r--r--  2.0 unx     1942 b- defN 80-Jan-01 00:00 gordo_core/data_providers/partition.py
 -rw-r--r--  2.0 unx     8455 b- defN 80-Jan-01 00:00 gordo_core/data_providers/providers.py
 -rw-r--r--  2.0 unx      482 b- defN 80-Jan-01 00:00 gordo_core/data_providers/utils.py
@@ -17,12 +17,12 @@
 -rw-r--r--  2.0 unx     9178 b- defN 80-Jan-01 00:00 gordo_core/filters/rows.py
 -rw-r--r--  2.0 unx     3800 b- defN 80-Jan-01 00:00 gordo_core/import_utils.py
 -rw-r--r--  2.0 unx     2454 b- defN 80-Jan-01 00:00 gordo_core/metadata.py
 -rw-r--r--  2.0 unx     9017 b- defN 80-Jan-01 00:00 gordo_core/sensor_tag.py
 -rw-r--r--  2.0 unx    30462 b- defN 80-Jan-01 00:00 gordo_core/time_series.py
 -rw-r--r--  2.0 unx    13507 b- defN 80-Jan-01 00:00 gordo_core/utils.py
 -rw-r--r--  2.0 unx     3834 b- defN 80-Jan-01 00:00 gordo_core/validators.py
--rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 gordo_core-0.3.0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 gordo_core-0.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2153 b- defN 16-Jan-01 00:00 gordo_core-0.3.0.dist-info/METADATA
-?rw-r--r--  2.0 unx     2148 b- defN 16-Jan-01 00:00 gordo_core-0.3.0.dist-info/RECORD
-26 files, 186898 bytes uncompressed, 57420 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 gordo_core-0.3.0rc0.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 gordo_core-0.3.0rc0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2147 b- defN 16-Jan-01 00:00 gordo_core-0.3.0rc0.dist-info/METADATA
+?rw-r--r--  2.0 unx     2160 b- defN 16-Jan-01 00:00 gordo_core-0.3.0rc0.dist-info/RECORD
+26 files, 186907 bytes uncompressed, 57423 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -60,20 +60,20 @@
 
 Filename: gordo_core/utils.py
 Comment: 
 
 Filename: gordo_core/validators.py
 Comment: 
 
-Filename: gordo_core-0.3.0.dist-info/LICENSE
+Filename: gordo_core-0.3.0rc0.dist-info/LICENSE
 Comment: 
 
-Filename: gordo_core-0.3.0.dist-info/WHEEL
+Filename: gordo_core-0.3.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: gordo_core-0.3.0.dist-info/METADATA
+Filename: gordo_core-0.3.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: gordo_core-0.3.0.dist-info/RECORD
+Filename: gordo_core-0.3.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gordo_core/_version.py

```diff
@@ -1,3 +1,3 @@
 # coding: utf-8
 # file generated by scripts/prepare_version.sh
-version = "0.3.0"
+version = "0.3.0rc0"
```

## Comparing `gordo_core-0.3.0.dist-info/LICENSE` & `gordo_core-0.3.0rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gordo_core-0.3.0.dist-info/METADATA` & `gordo_core-0.3.0rc0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordo-core
-Version: 0.3.0
+Version: 0.3.0rc0
 Summary: Gordo core library
 Home-page: https://github.com/equinor/gordo-core
 License: AGPLv3
 Keywords: gordo-core
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 Requires-Python: >=3.9,<4.0
@@ -34,15 +34,15 @@
 
 # Gordo core library.
 
 The main component can be found [here](https://github.com/equinor/gordo).
 
 ## Installation
 
-At least python 3.9 need to be installed in the system first.
+Python 3.9 need to be installed in the system first.
 
 ```
 pip3 install gordo-core
 ```
 
 ## Developers Instructions
```

## Comparing `gordo_core-0.3.0.dist-info/RECORD` & `gordo_core-0.3.0rc0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
 gordo_core/__init__.py,sha256=mTrf257jMCRzJp5xkvHK-J0QizBoYgDfQPl-yBDB3hk,74
-gordo_core/_version.py,sha256=4mogbHsyfdVD2TOaQN8Bb3xIBaK85CzMjKy78QpFRDU,81
+gordo_core/_version.py,sha256=57KQg8o_h7GMcucxaINMce-dqmv7lUVI0xH2Gv81km4,84
 gordo_core/back_compatibles.py,sha256=ilX1rgalv-4fgR2svsQeOjiSI4keglZukoqJ694_njY,2233
 gordo_core/base.py,sha256=r0ukWnbA-0avKkabWOqxWVKiwZ_J3N5cHcIOXWvgGzc,7723
 gordo_core/data_providers/__init__.py,sha256=Sbp5nXdc-NSvq4l5p0CvjlNCx5C9Tkm4ybVCy1iy_NA,102
 gordo_core/data_providers/base.py,sha256=2ZG8qFil61ggja9d5QFMUbzMWMHdZkQG5u1x4vCr8ro,5269
 gordo_core/data_providers/partition.py,sha256=q9xw2OsMOacUb-FkjkavmDuVWX4lJmT1KJ1hDE11j3E,1942
 gordo_core/data_providers/providers.py,sha256=mKNX6DQ9wXFpHkpGSU0Q4FLGJ5OmLRXlP_eaSuAmzoc,8455
 gordo_core/data_providers/utils.py,sha256=eUW64pN1ipNUAU87ELvI9QeozeOyS7pL6flYUt8PTpU,482
@@ -16,11 +16,11 @@
 gordo_core/filters/rows.py,sha256=NAcgyhAXnWNU3ANpZ79h3qxveGmp52sqMN7SuUTmcjY,9178
 gordo_core/import_utils.py,sha256=o_5acStlAziT8n4sUSAXXWd4-x2CIVNyEjSYZucuc-8,3800
 gordo_core/metadata.py,sha256=4nzDdZJ2vtlR1T_G8-Od9oShNrQIqs2xN3w7jQIjW60,2454
 gordo_core/sensor_tag.py,sha256=2_-ZAgmILVwR5iv963CDvQ-tPKCwjElAEd2pthraUbU,9017
 gordo_core/time_series.py,sha256=ZK7XR-p_H-g8EHnEtGigIHI8KmxYubOEOZVJUlsQwvY,30462
 gordo_core/utils.py,sha256=mtotB2xC0kzZ8d9hi75NUpYIW6u4Ba3CjFJIlBVVOis,13507
 gordo_core/validators.py,sha256=sNgWZx72KgPBb86yT9IpupTkP1MerTmVVFEGf6js0jw,3834
-gordo_core-0.3.0.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-gordo_core-0.3.0.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
-gordo_core-0.3.0.dist-info/METADATA,sha256=VCBj8f55kJCotxHhNoFQ6ekJHUvuIZTrZZnGQ2JQWwA,2153
-gordo_core-0.3.0.dist-info/RECORD,,
+gordo_core-0.3.0rc0.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+gordo_core-0.3.0rc0.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
+gordo_core-0.3.0rc0.dist-info/METADATA,sha256=YYwSeEMRnheOqoUtb1luDq5xZbAv4q9f0Rc-yESkEp0,2147
+gordo_core-0.3.0rc0.dist-info/RECORD,,
```

