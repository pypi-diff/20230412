# Comparing `tmp/ReverseBox-0.4.7.tar.gz` & `tmp/ReverseBox-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseBox-0.4.7.tar", last modified: Mon Jan  9 23:12:28 2023, max compression
+gzip compressed data, was "ReverseBox-0.4.8.tar", last modified: Wed Apr 12 21:01:42 2023, max compression
```

## Comparing `ReverseBox-0.4.7.tar` & `ReverseBox-0.4.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.698268 ReverseBox-0.4.7/
--rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:47.000000 ReverseBox-0.4.7/LICENSE
--rw-rw-rw-   0        0        0     5007 2023-01-09 23:12:28.698268 ReverseBox-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     3745 2023-01-09 23:09:08.000000 ReverseBox-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.647256 ReverseBox-0.4.7/ReverseBox.egg-info/
--rw-rw-rw-   0        0        0     5007 2023-01-09 23:12:28.000000 ReverseBox-0.4.7/ReverseBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1667 2023-01-09 23:12:28.000000 ReverseBox-0.4.7/ReverseBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-09 23:12:28.000000 ReverseBox-0.4.7/ReverseBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-09 23:12:28.000000 ReverseBox-0.4.7/ReverseBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-01-09 23:12:28.000000 ReverseBox-0.4.7/ReverseBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.648257 ReverseBox-0.4.7/reversebox/
--rw-rw-rw-   0        0        0        0 2022-06-25 12:19:26.000000 ReverseBox-0.4.7/reversebox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.652258 ReverseBox-0.4.7/reversebox/checksum/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.7/reversebox/checksum/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-08 20:51:07.000000 ReverseBox-0.4.7/reversebox/checksum/checksum_adler32.py
--rw-rw-rw-   0        0        0      403 2023-01-09 21:19:57.000000 ReverseBox-0.4.7/reversebox/checksum/checksum_fletcher16.py
--rw-rw-rw-   0        0        0      510 2023-01-09 22:41:53.000000 ReverseBox-0.4.7/reversebox/checksum/checksum_fletcher32.py
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.655287 ReverseBox-0.4.7/reversebox/common/
--rw-rw-rw-   0        0        0        0 2022-06-25 16:29:13.000000 ReverseBox-0.4.7/reversebox/common/__init__.py
--rw-rw-rw-   0        0        0      276 2022-12-27 22:06:13.000000 ReverseBox-0.4.7/reversebox/common/common.py
--rw-rw-rw-   0        0        0      730 2022-09-07 19:55:27.000000 ReverseBox-0.4.7/reversebox/common/logger.py
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.660259 ReverseBox-0.4.7/reversebox/compression/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.7/reversebox/compression/__init__.py
--rw-rw-rw-   0        0        0      484 2022-10-16 11:14:45.000000 ReverseBox-0.4.7/reversebox/compression/compression_jcalg1.py
--rw-rw-rw-   0        0        0      335 2022-12-27 14:56:59.000000 ReverseBox-0.4.7/reversebox/compression/compression_lzo.py
--rw-rw-rw-   0        0        0      330 2022-10-15 10:41:38.000000 ReverseBox-0.4.7/reversebox/compression/compression_zlib.py
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.669261 ReverseBox-0.4.7/reversebox/crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:26:29.000000 ReverseBox-0.4.7/reversebox/crc/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:19.000000 ReverseBox-0.4.7/reversebox/crc/crc16_arc.py
--rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:31.000000 ReverseBox-0.4.7/reversebox/crc/crc16_ccitt.py
--rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:06.000000 ReverseBox-0.4.7/reversebox/crc/crc16_dnp.py
--rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:19.000000 ReverseBox-0.4.7/reversebox/crc/crc16_kermit.py
--rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:37.000000 ReverseBox-0.4.7/reversebox/crc/crc16_modbus.py
--rw-rw-rw-   0        0        0      735 2022-07-21 21:35:31.000000 ReverseBox-0.4.7/reversebox/crc/crc16_sick.py
--rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:19.000000 ReverseBox-0.4.7/reversebox/crc/crc32_iso_hdlc.py
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.673262 ReverseBox-0.4.7/reversebox/encryption/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.7/reversebox/encryption/__init__.py
--rw-rw-rw-   0        0        0      579 2022-07-17 23:25:19.000000 ReverseBox-0.4.7/reversebox/encryption/encryption_xor_basic.py
--rw-rw-rw-   0        0        0      574 2022-07-17 23:25:19.000000 ReverseBox-0.4.7/reversebox/encryption/encryption_xor_retro64_eco.py
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.677263 ReverseBox-0.4.7/reversebox/hash/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.7/reversebox/hash/__init__.py
--rw-rw-rw-   0        0        0      280 2022-09-11 18:48:36.000000 ReverseBox-0.4.7/reversebox/hash/hash_md5.py
--rw-rw-rw-   0        0        0      283 2023-01-08 14:05:01.000000 ReverseBox-0.4.7/reversebox/hash/hash_sha1.py
--rw-rw-rw-   0        0        0      289 2023-01-08 14:07:31.000000 ReverseBox-0.4.7/reversebox/hash/hash_sha2.py
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.680264 ReverseBox-0.4.7/reversebox/image/
--rw-rw-rw-   0        0        0        0 2022-12-27 21:18:24.000000 ReverseBox-0.4.7/reversebox/image/__init__.py
--rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:19.000000 ReverseBox-0.4.7/reversebox/image/image_finder_gui.py
--rw-rw-rw-   0        0        0      715 2022-12-31 14:42:11.000000 ReverseBox-0.4.7/reversebox/image/image_finder_main.py
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.685265 ReverseBox-0.4.7/reversebox/io_files/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.7/reversebox/io_files/__init__.py
--rw-rw-rw-   0        0        0      306 2023-01-02 21:01:57.000000 ReverseBox-0.4.7/reversebox/io_files/bytes_handler.py
--rw-rw-rw-   0        0        0      951 2022-09-03 13:15:52.000000 ReverseBox-0.4.7/reversebox/io_files/check_file.py
--rw-rw-rw-   0        0        0     6322 2022-12-05 21:47:33.000000 ReverseBox-0.4.7/reversebox/io_files/file_handler.py
--rw-rw-rw-   0        0        0       42 2023-01-09 23:12:28.698268 ReverseBox-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1816 2023-01-09 23:11:07.000000 ReverseBox-0.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.687265 ReverseBox-0.4.7/tests/
--rw-rw-rw-   0        0        0        0 2022-07-19 22:27:10.000000 ReverseBox-0.4.7/tests/__init__.py
--rw-rw-rw-   0        0        0      517 2023-01-08 12:35:15.000000 ReverseBox-0.4.7/tests/common.py
-drwxrwxrwx   0        0        0        0 2023-01-09 23:12:28.696267 ReverseBox-0.4.7/tests/tests_crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:28:33.000000 ReverseBox-0.4.7/tests/tests_crc/__init__.py
--rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:08.000000 ReverseBox-0.4.7/tests/tests_crc/test_crc16_arc.py
--rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:08.000000 ReverseBox-0.4.7/tests/tests_crc/test_crc16_ccitt.py
--rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:08.000000 ReverseBox-0.4.7/tests/tests_crc/test_crc16_dnp.py
--rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:08.000000 ReverseBox-0.4.7/tests/tests_crc/test_crc16_kermit.py
--rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:08.000000 ReverseBox-0.4.7/tests/tests_crc/test_crc16_modbus.py
--rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:08.000000 ReverseBox-0.4.7/tests/tests_crc/test_crc16_sick.py
--rw-rw-rw-   0        0        0     2657 2023-01-09 18:34:08.000000 ReverseBox-0.4.7/tests/tests_crc/test_crc32_iso_hdlc.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.107985 ReverseBox-0.4.8/
+-rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:47.000000 ReverseBox-0.4.8/LICENSE
+-rw-rw-rw-   0        0        0     5165 2023-04-12 21:01:42.106987 ReverseBox-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3903 2023-04-12 20:48:35.000000 ReverseBox-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.053973 ReverseBox-0.4.8/ReverseBox.egg-info/
+-rw-rw-rw-   0        0        0     5165 2023-04-12 21:01:41.000000 ReverseBox-0.4.8/ReverseBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1667 2023-04-12 21:01:41.000000 ReverseBox-0.4.8/ReverseBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 21:01:41.000000 ReverseBox-0.4.8/ReverseBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-12 21:01:41.000000 ReverseBox-0.4.8/ReverseBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-12 21:01:41.000000 ReverseBox-0.4.8/ReverseBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.054974 ReverseBox-0.4.8/reversebox/
+-rw-rw-rw-   0        0        0        0 2022-06-25 12:19:26.000000 ReverseBox-0.4.8/reversebox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.058974 ReverseBox-0.4.8/reversebox/checksum/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.8/reversebox/checksum/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-01-08 20:51:07.000000 ReverseBox-0.4.8/reversebox/checksum/checksum_adler32.py
+-rw-rw-rw-   0        0        0      403 2023-01-09 21:19:57.000000 ReverseBox-0.4.8/reversebox/checksum/checksum_fletcher16.py
+-rw-rw-rw-   0        0        0      510 2023-01-09 22:41:53.000000 ReverseBox-0.4.8/reversebox/checksum/checksum_fletcher32.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.061976 ReverseBox-0.4.8/reversebox/common/
+-rw-rw-rw-   0        0        0        0 2022-06-25 16:29:13.000000 ReverseBox-0.4.8/reversebox/common/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-04-12 20:41:34.000000 ReverseBox-0.4.8/reversebox/common/common.py
+-rw-rw-rw-   0        0        0      730 2022-09-07 19:55:27.000000 ReverseBox-0.4.8/reversebox/common/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.066976 ReverseBox-0.4.8/reversebox/compression/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.8/reversebox/compression/__init__.py
+-rw-rw-rw-   0        0        0      484 2022-10-16 11:14:45.000000 ReverseBox-0.4.8/reversebox/compression/compression_jcalg1.py
+-rw-rw-rw-   0        0        0      335 2022-12-27 14:56:59.000000 ReverseBox-0.4.8/reversebox/compression/compression_lzo.py
+-rw-rw-rw-   0        0        0      330 2022-10-15 10:41:38.000000 ReverseBox-0.4.8/reversebox/compression/compression_zlib.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.075978 ReverseBox-0.4.8/reversebox/crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:26:29.000000 ReverseBox-0.4.8/reversebox/crc/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:19.000000 ReverseBox-0.4.8/reversebox/crc/crc16_arc.py
+-rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:31.000000 ReverseBox-0.4.8/reversebox/crc/crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:06.000000 ReverseBox-0.4.8/reversebox/crc/crc16_dnp.py
+-rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:19.000000 ReverseBox-0.4.8/reversebox/crc/crc16_kermit.py
+-rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:37.000000 ReverseBox-0.4.8/reversebox/crc/crc16_modbus.py
+-rw-rw-rw-   0        0        0      735 2022-07-21 21:35:31.000000 ReverseBox-0.4.8/reversebox/crc/crc16_sick.py
+-rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:19.000000 ReverseBox-0.4.8/reversebox/crc/crc32_iso_hdlc.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.079980 ReverseBox-0.4.8/reversebox/encryption/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.8/reversebox/encryption/__init__.py
+-rw-rw-rw-   0        0        0      579 2022-07-17 23:25:19.000000 ReverseBox-0.4.8/reversebox/encryption/encryption_xor_basic.py
+-rw-rw-rw-   0        0        0      574 2022-07-17 23:25:19.000000 ReverseBox-0.4.8/reversebox/encryption/encryption_xor_retro64_eco.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.083980 ReverseBox-0.4.8/reversebox/hash/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.8/reversebox/hash/__init__.py
+-rw-rw-rw-   0        0        0      280 2022-09-11 18:48:36.000000 ReverseBox-0.4.8/reversebox/hash/hash_md5.py
+-rw-rw-rw-   0        0        0      283 2023-01-08 14:05:01.000000 ReverseBox-0.4.8/reversebox/hash/hash_sha1.py
+-rw-rw-rw-   0        0        0      289 2023-01-08 14:07:31.000000 ReverseBox-0.4.8/reversebox/hash/hash_sha2.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.087981 ReverseBox-0.4.8/reversebox/image/
+-rw-rw-rw-   0        0        0        0 2022-12-27 21:18:24.000000 ReverseBox-0.4.8/reversebox/image/__init__.py
+-rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:19.000000 ReverseBox-0.4.8/reversebox/image/image_finder_gui.py
+-rw-rw-rw-   0        0        0      715 2022-12-31 14:42:11.000000 ReverseBox-0.4.8/reversebox/image/image_finder_main.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.092982 ReverseBox-0.4.8/reversebox/io_files/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.8/reversebox/io_files/__init__.py
+-rw-rw-rw-   0        0        0      306 2023-01-02 21:01:57.000000 ReverseBox-0.4.8/reversebox/io_files/bytes_handler.py
+-rw-rw-rw-   0        0        0      951 2022-09-03 13:15:52.000000 ReverseBox-0.4.8/reversebox/io_files/check_file.py
+-rw-rw-rw-   0        0        0     6621 2023-04-12 20:36:37.000000 ReverseBox-0.4.8/reversebox/io_files/file_handler.py
+-rw-rw-rw-   0        0        0       42 2023-04-12 21:01:42.107985 ReverseBox-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1816 2023-04-12 21:01:41.000000 ReverseBox-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.095982 ReverseBox-0.4.8/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-19 22:27:10.000000 ReverseBox-0.4.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-04-12 20:56:38.000000 ReverseBox-0.4.8/tests/common.py
+drwxrwxrwx   0        0        0        0 2023-04-12 21:01:42.105986 ReverseBox-0.4.8/tests/tests_crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:28:33.000000 ReverseBox-0.4.8/tests/tests_crc/__init__.py
+-rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:08.000000 ReverseBox-0.4.8/tests/tests_crc/test_crc16_arc.py
+-rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:08.000000 ReverseBox-0.4.8/tests/tests_crc/test_crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:08.000000 ReverseBox-0.4.8/tests/tests_crc/test_crc16_dnp.py
+-rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:08.000000 ReverseBox-0.4.8/tests/tests_crc/test_crc16_kermit.py
+-rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:08.000000 ReverseBox-0.4.8/tests/tests_crc/test_crc16_modbus.py
+-rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:08.000000 ReverseBox-0.4.8/tests/tests_crc/test_crc16_sick.py
+-rw-rw-rw-   0        0        0     2657 2023-01-09 18:34:08.000000 ReverseBox-0.4.8/tests/tests_crc/test_crc32_iso_hdlc.py
```

### Comparing `ReverseBox-0.4.7/LICENSE` & `ReverseBox-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/PKG-INFO` & `ReverseBox-0.4.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.4.7
+Version: 0.4.8
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -98,20 +98,23 @@
   - (game-specific) Hercules (TODO) ❌
   - (game-specific) E-racer (TODO) ❌
 
 * Image
   - Image Finder  (in progress) ❌
   - PS2 Swizzling/Twiddling (TODO) ❌
   - PSP Swizzling/Twiddling (TODO) ❌
+  - [SourceSDK Swizzling](https://forum.xentax.com/viewtopic.php?p=139510#p139510) (TODO) ❌
 
 * IO
   - File Reader ✔️
   - File Writer ✔️
   - Bytes Handler ✔️
   - File extension checking ✔️
+  - Padding calculation ✔️
+  - File size checking ✔️
 
 # Checksum calculation - example
 
 // CRC32 calculation
 ```
 from reversebox.crc import crc32_iso_hdlc
 from reversebox.common import common
```

### Comparing `ReverseBox-0.4.7/README.md` & `ReverseBox-0.4.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -69,20 +69,23 @@
   - (game-specific) Hercules (TODO) ❌
   - (game-specific) E-racer (TODO) ❌
 
 * Image
   - Image Finder  (in progress) ❌
   - PS2 Swizzling/Twiddling (TODO) ❌
   - PSP Swizzling/Twiddling (TODO) ❌
+  - [SourceSDK Swizzling](https://forum.xentax.com/viewtopic.php?p=139510#p139510) (TODO) ❌
 
 * IO
   - File Reader ✔️
   - File Writer ✔️
   - Bytes Handler ✔️
   - File extension checking ✔️
+  - Padding calculation ✔️
+  - File size checking ✔️
 
 # Checksum calculation - example
 
 // CRC32 calculation
 ```
 from reversebox.crc import crc32_iso_hdlc
 from reversebox.common import common
```

### Comparing `ReverseBox-0.4.7/ReverseBox.egg-info/PKG-INFO` & `ReverseBox-0.4.8/ReverseBox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.4.7
+Version: 0.4.8
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -98,20 +98,23 @@
   - (game-specific) Hercules (TODO) ❌
   - (game-specific) E-racer (TODO) ❌
 
 * Image
   - Image Finder  (in progress) ❌
   - PS2 Swizzling/Twiddling (TODO) ❌
   - PSP Swizzling/Twiddling (TODO) ❌
+  - [SourceSDK Swizzling](https://forum.xentax.com/viewtopic.php?p=139510#p139510) (TODO) ❌
 
 * IO
   - File Reader ✔️
   - File Writer ✔️
   - Bytes Handler ✔️
   - File extension checking ✔️
+  - Padding calculation ✔️
+  - File size checking ✔️
 
 # Checksum calculation - example
 
 // CRC32 calculation
 ```
 from reversebox.crc import crc32_iso_hdlc
 from reversebox.common import common
```

### Comparing `ReverseBox-0.4.7/ReverseBox.egg-info/SOURCES.txt` & `ReverseBox-0.4.8/ReverseBox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/common/logger.py` & `ReverseBox-0.4.8/reversebox/common/logger.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/crc/crc16_arc.py` & `ReverseBox-0.4.8/reversebox/crc/crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/crc/crc16_ccitt.py` & `ReverseBox-0.4.8/reversebox/crc/crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/crc/crc16_dnp.py` & `ReverseBox-0.4.8/reversebox/crc/crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/crc/crc16_kermit.py` & `ReverseBox-0.4.8/reversebox/crc/crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/crc/crc16_modbus.py` & `ReverseBox-0.4.8/reversebox/crc/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/crc/crc16_sick.py` & `ReverseBox-0.4.8/reversebox/crc/crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/crc/crc32_iso_hdlc.py` & `ReverseBox-0.4.8/reversebox/crc/crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/encryption/encryption_xor_basic.py` & `ReverseBox-0.4.8/reversebox/encryption/encryption_xor_basic.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/encryption/encryption_xor_retro64_eco.py` & `ReverseBox-0.4.8/reversebox/encryption/encryption_xor_retro64_eco.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/image/image_finder_gui.py` & `ReverseBox-0.4.8/reversebox/image/image_finder_gui.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/image/image_finder_main.py` & `ReverseBox-0.4.8/reversebox/image/image_finder_main.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/io_files/check_file.py` & `ReverseBox-0.4.8/reversebox/io_files/check_file.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/reversebox/io_files/file_handler.py` & `ReverseBox-0.4.8/reversebox/io_files/file_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,24 +69,31 @@
         if "w" not in self.open_mode:
             error_message = 'Wrong file open mode! You need to specify one of the "write" open modes!'
             logger.error(error_message)
             raise Exception(error_message)
         return True
 
     def seek(self, seek_value, seek_type: int = 0):
-        # 0 = SEEK_SET
-        # 1 = SEEK_CUR
-        # 2 = SEEK_END
+        # 0 = SEEK_SET (from file start)
+        # 1 = SEEK_CUR (from current offset)
+        # 2 = SEEK_END (from file end)
         self._check_file()
         self.file.seek(seek_value, seek_type)
 
     def get_position(self) -> int:
         self._check_file()
         return self.file.tell()
 
+    def get_file_size(self) -> int:
+        current_position = self.get_position()
+        self.seek(0, 2)
+        end_of_file__position = self.get_position()
+        self.seek(current_position, 0)
+        return end_of_file__position
+
     def read_str(self, str_length: int, encoding: str = "utf8") -> str:
         self._check_file()
         self._check_read_mode()
         data = self.file.read(str_length)
         return data.decode(encoding)
 
     def read_bytes(self, number_of_bytes: int) -> bytes:
```

### Comparing `ReverseBox-0.4.7/setup.py` & `ReverseBox-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 License: GPL-3.0 License
 """
 
 import os
 
 import setuptools
 
-VERSION_NUM = "0.4.7"
+VERSION_NUM = "0.4.8"
 
 
 def get_long_description() -> str:
     with open(
         os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf8"
     ) as readme:
         readme_text = readme.read()
```

### Comparing `ReverseBox-0.4.7/tests/common.py` & `ReverseBox-0.4.8/tests/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,7 +27,14 @@
     expected_result: bytes
 
 
 @dataclass
 class HashTestEntry:
     test_data: bytes
     expected_result: bytes
+
+
+@dataclass
+class PaddingTestEntry:
+    test_offset: int
+    test_div: int
+    expected_padding: int
```

### Comparing `ReverseBox-0.4.7/tests/tests_crc/test_crc16_arc.py` & `ReverseBox-0.4.8/tests/tests_crc/test_crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/tests/tests_crc/test_crc16_ccitt.py` & `ReverseBox-0.4.8/tests/tests_crc/test_crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/tests/tests_crc/test_crc16_dnp.py` & `ReverseBox-0.4.8/tests/tests_crc/test_crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/tests/tests_crc/test_crc16_kermit.py` & `ReverseBox-0.4.8/tests/tests_crc/test_crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/tests/tests_crc/test_crc16_modbus.py` & `ReverseBox-0.4.8/tests/tests_crc/test_crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/tests/tests_crc/test_crc16_sick.py` & `ReverseBox-0.4.8/tests/tests_crc/test_crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.7/tests/tests_crc/test_crc32_iso_hdlc.py` & `ReverseBox-0.4.8/tests/tests_crc/test_crc32_iso_hdlc.py`

 * *Files identical despite different names*

