# Comparing `tmp/bandcamp_name_your_price_dl-0.0.8.tar.gz` & `tmp/bandcamp_name_your_price_dl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandcamp_name_your_price_dl-0.0.8.tar", last modified: Sun May  9 09:40:41 2021, max compression
+gzip compressed data, was "bandcamp_name_your_price_dl-0.0.9.tar", last modified: Sat Jun 19 19:57:10 2021, max compression
```

## Comparing `bandcamp_name_your_price_dl-0.0.8.tar` & `bandcamp_name_your_price_dl-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 layerex   (1000) users      (100)        0 2021-05-09 09:40:41.090247 bandcamp_name_your_price_dl-0.0.8/
--rw-r--r--   0 layerex   (1000) users      (100)    35149 2020-12-19 16:34:13.000000 bandcamp_name_your_price_dl-0.0.8/LICENSE
--rw-r--r--   0 layerex   (1000) users      (100)     4704 2021-05-09 09:40:41.090247 bandcamp_name_your_price_dl-0.0.8/PKG-INFO
--rw-r--r--   0 layerex   (1000) users      (100)     3499 2021-05-09 09:10:57.000000 bandcamp_name_your_price_dl-0.0.8/README.md
-drwxr-xr-x   0 layerex   (1000) users      (100)        0 2021-05-09 09:40:41.090247 bandcamp_name_your_price_dl-0.0.8/bandcamp_name_your_price_dl.egg-info/
--rw-r--r--   0 layerex   (1000) users      (100)     4704 2021-05-09 09:40:40.000000 bandcamp_name_your_price_dl-0.0.8/bandcamp_name_your_price_dl.egg-info/PKG-INFO
--rw-r--r--   0 layerex   (1000) users      (100)      315 2021-05-09 09:40:41.000000 bandcamp_name_your_price_dl-0.0.8/bandcamp_name_your_price_dl.egg-info/SOURCES.txt
--rw-r--r--   0 layerex   (1000) users      (100)        1 2021-05-09 09:40:40.000000 bandcamp_name_your_price_dl-0.0.8/bandcamp_name_your_price_dl.egg-info/dependency_links.txt
--rw-r--r--   0 layerex   (1000) users      (100)       82 2021-05-09 09:40:40.000000 bandcamp_name_your_price_dl-0.0.8/bandcamp_name_your_price_dl.egg-info/entry_points.txt
--rw-r--r--   0 layerex   (1000) users      (100)       28 2021-05-09 09:40:40.000000 bandcamp_name_your_price_dl-0.0.8/bandcamp_name_your_price_dl.egg-info/top_level.txt
--rwxr-xr-x   0 layerex   (1000) users      (100)    15668 2021-05-09 09:37:27.000000 bandcamp_name_your_price_dl-0.0.8/bandcamp_name_your_price_dl.py
--rw-r--r--   0 layerex   (1000) users      (100)       38 2021-05-09 09:40:41.090247 bandcamp_name_your_price_dl-0.0.8/setup.cfg
--rw-r--r--   0 layerex   (1000) users      (100)     1040 2021-05-07 09:58:24.000000 bandcamp_name_your_price_dl-0.0.8/setup.py
+drwxr-xr-x   0 layerex   (1000) users      (100)        0 2021-06-19 19:57:10.523975 bandcamp_name_your_price_dl-0.0.9/
+-rw-r--r--   0 layerex   (1000) users      (100)    35149 2020-12-19 16:34:13.000000 bandcamp_name_your_price_dl-0.0.9/LICENSE
+-rw-r--r--   0 layerex   (1000) users      (100)     4155 2021-06-19 19:57:10.523975 bandcamp_name_your_price_dl-0.0.9/PKG-INFO
+-rw-r--r--   0 layerex   (1000) users      (100)     3499 2021-05-09 09:10:57.000000 bandcamp_name_your_price_dl-0.0.9/README.md
+drwxr-xr-x   0 layerex   (1000) users      (100)        0 2021-06-19 19:57:10.523975 bandcamp_name_your_price_dl-0.0.9/bandcamp_name_your_price_dl.egg-info/
+-rw-r--r--   0 layerex   (1000) users      (100)     4155 2021-06-19 19:57:10.000000 bandcamp_name_your_price_dl-0.0.9/bandcamp_name_your_price_dl.egg-info/PKG-INFO
+-rw-r--r--   0 layerex   (1000) users      (100)      315 2021-06-19 19:57:10.000000 bandcamp_name_your_price_dl-0.0.9/bandcamp_name_your_price_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 layerex   (1000) users      (100)        1 2021-06-19 19:57:10.000000 bandcamp_name_your_price_dl-0.0.9/bandcamp_name_your_price_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 layerex   (1000) users      (100)       82 2021-06-19 19:57:10.000000 bandcamp_name_your_price_dl-0.0.9/bandcamp_name_your_price_dl.egg-info/entry_points.txt
+-rw-r--r--   0 layerex   (1000) users      (100)       28 2021-06-19 19:57:10.000000 bandcamp_name_your_price_dl-0.0.9/bandcamp_name_your_price_dl.egg-info/top_level.txt
+-rwxr-xr-x   0 layerex   (1000) users      (100)    16037 2021-06-19 19:55:02.000000 bandcamp_name_your_price_dl-0.0.9/bandcamp_name_your_price_dl.py
+-rw-r--r--   0 layerex   (1000) users      (100)       38 2021-06-19 19:57:10.523975 bandcamp_name_your_price_dl-0.0.9/setup.cfg
+-rw-r--r--   0 layerex   (1000) users      (100)     1040 2021-05-07 09:58:24.000000 bandcamp_name_your_price_dl-0.0.9/setup.py
```

### Comparing `bandcamp_name_your_price_dl-0.0.8/LICENSE` & `bandcamp_name_your_price_dl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bandcamp_name_your_price_dl-0.0.8/PKG-INFO` & `bandcamp_name_your_price_dl-0.0.9/bandcamp_name_your_price_dl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,90 @@
 Metadata-Version: 2.1
-Name: bandcamp_name_your_price_dl
-Version: 0.0.8
+Name: bandcamp-name-your-price-dl
+Version: 0.0.9
 Summary: Automate process of downloading name your price albums from bandcamp.
 Home-page: https://github.com/Layerex/bandcamp_name_your_price_dl
 Author: Layerex
 Author-email: layerex@dismail.de
 License: UNKNOWN
-Description: # bandcamp_name_your_price_dl
-        
-        Automate process of downloading name your price albums from [bandcamp](bandcamp.com) with Selenium.
-        
-        ## Installation
-        
-        ```sh
-        pip install bandcamp_name_your_price_dl
-        ```
-        
-        Also you need to install a selenium browser driver. Refer to [selenium installation guide](https://selenium-python.readthedocs.io/installation.html#drivers).
-        
-        ## Usage
-        
-        ```text
-        usage: bandcamp_name_your_price_dl [-h] [--download-dir DOWNLOAD_DIR] [--encoding {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}]
-                                           [--skip-nyp-check] [--wait-time SECONDS] [--preparing-wait-time SECONDS]
-                                           [--driver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}]
-                                           [--show-browser-window] [--print-url] [--dont-skip-if-file-exists] [--ignore-cache] [--email EMAIL]
-                                           [--country-abbrev COUNTRY_ABBREV] [--postal-code POSTAL_CODE]
-                                           ALBUM_URL [DOWNLOAD_DIR]
-        
-        Automate process of downloading name your price albums from bandcamp.
-        
-        positional arguments:
-          ALBUM_URL             url of desired bandcamp album
-          DOWNLOAD_DIR          directory to download album to
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --download-dir DOWNLOAD_DIR, -d DOWNLOAD_DIR
-                                directory to download album to
-          --encoding {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, -e {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, --format {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, -f {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}
-                                desired encoding
-          --skip-nyp-check, --skip-name-your-price-check
-                                don't check if album is name your price before trying to download
-          --wait-time SECONDS   period to wait for pages loading (in seconds) (default is 10)
-          --preparing-wait-time SECONDS
-                                period to wait for bandcamp preparing download (in seconds) (default is 60)
-          --driver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}, --webdriver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}
-                                desired webdriver (default is chromium)
-          --show-browser-window
-                                show browser window (is hidden by default)
-          --print-url, -p       print url to stdout instead of downloading
-          --dont-skip-if-file-exists
-                                don't skip downloading if desired file already exists in current directory or was already downloaded
-          --ignore-cache        don't load cache and don't write anything to it
-          --email EMAIL         your email address (is used if bandcamp asks for email)
-          --country-abbrev COUNTRY_ABBREV, --country COUNTRY_ABBREV
-                                country abbreviation used if bandcamp asks for email
-          --postal-code POSTAL_CODE, --postcode POSTAL_CODE, --zip-code POSTAL_CODE
-                                postal code used if bandcamp asks for email
-        ```
-        
-        ## Usage example
-        
-        ### Download discography of an artist
-        
-        To list albums of an artist you may use [bandcamp_list_albums](https://github.com/Layerex/bandcamp_list_albums).
-        
-        [bandcamp-dl](https://github.com/iheanyi/bandcamp-dl) may be used to download not name your price albums.
-        
-        ```bash
-        for album in $(bandcamp_list_albums "$BANDCAMP_PAGE_URL" --print-urls)
-        do
-            bandcamp_name_your_price_dl "$album" || bandcamp-dl "$album"
-        done
-        ```
-        
-        You may also want to specify email, country and postcode in case bandcamp asks for those and download directory.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# bandcamp_name_your_price_dl
+
+Automate process of downloading name your price albums from [bandcamp](bandcamp.com) with Selenium.
+
+## Installation
+
+```sh
+pip install bandcamp_name_your_price_dl
+```
+
+Also you need to install a selenium browser driver. Refer to [selenium installation guide](https://selenium-python.readthedocs.io/installation.html#drivers).
+
+## Usage
+
+```text
+usage: bandcamp_name_your_price_dl [-h] [--download-dir DOWNLOAD_DIR] [--encoding {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}]
+                                   [--skip-nyp-check] [--wait-time SECONDS] [--preparing-wait-time SECONDS]
+                                   [--driver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}]
+                                   [--show-browser-window] [--print-url] [--dont-skip-if-file-exists] [--ignore-cache] [--email EMAIL]
+                                   [--country-abbrev COUNTRY_ABBREV] [--postal-code POSTAL_CODE]
+                                   ALBUM_URL [DOWNLOAD_DIR]
+
+Automate process of downloading name your price albums from bandcamp.
+
+positional arguments:
+  ALBUM_URL             url of desired bandcamp album
+  DOWNLOAD_DIR          directory to download album to
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --download-dir DOWNLOAD_DIR, -d DOWNLOAD_DIR
+                        directory to download album to
+  --encoding {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, -e {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, --format {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, -f {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}
+                        desired encoding
+  --skip-nyp-check, --skip-name-your-price-check
+                        don't check if album is name your price before trying to download
+  --wait-time SECONDS   period to wait for pages loading (in seconds) (default is 10)
+  --preparing-wait-time SECONDS
+                        period to wait for bandcamp preparing download (in seconds) (default is 60)
+  --driver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}, --webdriver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}
+                        desired webdriver (default is chromium)
+  --show-browser-window
+                        show browser window (is hidden by default)
+  --print-url, -p       print url to stdout instead of downloading
+  --dont-skip-if-file-exists
+                        don't skip downloading if desired file already exists in current directory or was already downloaded
+  --ignore-cache        don't load cache and don't write anything to it
+  --email EMAIL         your email address (is used if bandcamp asks for email)
+  --country-abbrev COUNTRY_ABBREV, --country COUNTRY_ABBREV
+                        country abbreviation used if bandcamp asks for email
+  --postal-code POSTAL_CODE, --postcode POSTAL_CODE, --zip-code POSTAL_CODE
+                        postal code used if bandcamp asks for email
+```
+
+## Usage example
+
+### Download discography of an artist
+
+To list albums of an artist you may use [bandcamp_list_albums](https://github.com/Layerex/bandcamp_list_albums).
+
+[bandcamp-dl](https://github.com/iheanyi/bandcamp-dl) may be used to download not name your price albums.
+
+```bash
+for album in $(bandcamp_list_albums "$BANDCAMP_PAGE_URL" --print-urls)
+do
+    bandcamp_name_your_price_dl "$album" || bandcamp-dl "$album"
+done
+```
+
+You may also want to specify email, country and postcode in case bandcamp asks for those and download directory.
+
+
```

### Comparing `bandcamp_name_your_price_dl-0.0.8/README.md` & `bandcamp_name_your_price_dl-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bandcamp_name_your_price_dl-0.0.8/bandcamp_name_your_price_dl.egg-info/PKG-INFO` & `bandcamp_name_your_price_dl-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,90 @@
 Metadata-Version: 2.1
-Name: bandcamp-name-your-price-dl
-Version: 0.0.8
+Name: bandcamp_name_your_price_dl
+Version: 0.0.9
 Summary: Automate process of downloading name your price albums from bandcamp.
 Home-page: https://github.com/Layerex/bandcamp_name_your_price_dl
 Author: Layerex
 Author-email: layerex@dismail.de
 License: UNKNOWN
-Description: # bandcamp_name_your_price_dl
-        
-        Automate process of downloading name your price albums from [bandcamp](bandcamp.com) with Selenium.
-        
-        ## Installation
-        
-        ```sh
-        pip install bandcamp_name_your_price_dl
-        ```
-        
-        Also you need to install a selenium browser driver. Refer to [selenium installation guide](https://selenium-python.readthedocs.io/installation.html#drivers).
-        
-        ## Usage
-        
-        ```text
-        usage: bandcamp_name_your_price_dl [-h] [--download-dir DOWNLOAD_DIR] [--encoding {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}]
-                                           [--skip-nyp-check] [--wait-time SECONDS] [--preparing-wait-time SECONDS]
-                                           [--driver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}]
-                                           [--show-browser-window] [--print-url] [--dont-skip-if-file-exists] [--ignore-cache] [--email EMAIL]
-                                           [--country-abbrev COUNTRY_ABBREV] [--postal-code POSTAL_CODE]
-                                           ALBUM_URL [DOWNLOAD_DIR]
-        
-        Automate process of downloading name your price albums from bandcamp.
-        
-        positional arguments:
-          ALBUM_URL             url of desired bandcamp album
-          DOWNLOAD_DIR          directory to download album to
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --download-dir DOWNLOAD_DIR, -d DOWNLOAD_DIR
-                                directory to download album to
-          --encoding {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, -e {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, --format {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, -f {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}
-                                desired encoding
-          --skip-nyp-check, --skip-name-your-price-check
-                                don't check if album is name your price before trying to download
-          --wait-time SECONDS   period to wait for pages loading (in seconds) (default is 10)
-          --preparing-wait-time SECONDS
-                                period to wait for bandcamp preparing download (in seconds) (default is 60)
-          --driver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}, --webdriver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}
-                                desired webdriver (default is chromium)
-          --show-browser-window
-                                show browser window (is hidden by default)
-          --print-url, -p       print url to stdout instead of downloading
-          --dont-skip-if-file-exists
-                                don't skip downloading if desired file already exists in current directory or was already downloaded
-          --ignore-cache        don't load cache and don't write anything to it
-          --email EMAIL         your email address (is used if bandcamp asks for email)
-          --country-abbrev COUNTRY_ABBREV, --country COUNTRY_ABBREV
-                                country abbreviation used if bandcamp asks for email
-          --postal-code POSTAL_CODE, --postcode POSTAL_CODE, --zip-code POSTAL_CODE
-                                postal code used if bandcamp asks for email
-        ```
-        
-        ## Usage example
-        
-        ### Download discography of an artist
-        
-        To list albums of an artist you may use [bandcamp_list_albums](https://github.com/Layerex/bandcamp_list_albums).
-        
-        [bandcamp-dl](https://github.com/iheanyi/bandcamp-dl) may be used to download not name your price albums.
-        
-        ```bash
-        for album in $(bandcamp_list_albums "$BANDCAMP_PAGE_URL" --print-urls)
-        do
-            bandcamp_name_your_price_dl "$album" || bandcamp-dl "$album"
-        done
-        ```
-        
-        You may also want to specify email, country and postcode in case bandcamp asks for those and download directory.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# bandcamp_name_your_price_dl
+
+Automate process of downloading name your price albums from [bandcamp](bandcamp.com) with Selenium.
+
+## Installation
+
+```sh
+pip install bandcamp_name_your_price_dl
+```
+
+Also you need to install a selenium browser driver. Refer to [selenium installation guide](https://selenium-python.readthedocs.io/installation.html#drivers).
+
+## Usage
+
+```text
+usage: bandcamp_name_your_price_dl [-h] [--download-dir DOWNLOAD_DIR] [--encoding {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}]
+                                   [--skip-nyp-check] [--wait-time SECONDS] [--preparing-wait-time SECONDS]
+                                   [--driver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}]
+                                   [--show-browser-window] [--print-url] [--dont-skip-if-file-exists] [--ignore-cache] [--email EMAIL]
+                                   [--country-abbrev COUNTRY_ABBREV] [--postal-code POSTAL_CODE]
+                                   ALBUM_URL [DOWNLOAD_DIR]
+
+Automate process of downloading name your price albums from bandcamp.
+
+positional arguments:
+  ALBUM_URL             url of desired bandcamp album
+  DOWNLOAD_DIR          directory to download album to
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --download-dir DOWNLOAD_DIR, -d DOWNLOAD_DIR
+                        directory to download album to
+  --encoding {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, -e {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, --format {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}, -f {mp3,mp3v0,flac,aac,ogg,alac,wav,aiff}
+                        desired encoding
+  --skip-nyp-check, --skip-name-your-price-check
+                        don't check if album is name your price before trying to download
+  --wait-time SECONDS   period to wait for pages loading (in seconds) (default is 10)
+  --preparing-wait-time SECONDS
+                        period to wait for bandcamp preparing download (in seconds) (default is 60)
+  --driver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}, --webdriver {chromium,chrome,edge,firefox,gecko,opera,phantomjs,safari,webkit}
+                        desired webdriver (default is chromium)
+  --show-browser-window
+                        show browser window (is hidden by default)
+  --print-url, -p       print url to stdout instead of downloading
+  --dont-skip-if-file-exists
+                        don't skip downloading if desired file already exists in current directory or was already downloaded
+  --ignore-cache        don't load cache and don't write anything to it
+  --email EMAIL         your email address (is used if bandcamp asks for email)
+  --country-abbrev COUNTRY_ABBREV, --country COUNTRY_ABBREV
+                        country abbreviation used if bandcamp asks for email
+  --postal-code POSTAL_CODE, --postcode POSTAL_CODE, --zip-code POSTAL_CODE
+                        postal code used if bandcamp asks for email
+```
+
+## Usage example
+
+### Download discography of an artist
+
+To list albums of an artist you may use [bandcamp_list_albums](https://github.com/Layerex/bandcamp_list_albums).
+
+[bandcamp-dl](https://github.com/iheanyi/bandcamp-dl) may be used to download not name your price albums.
+
+```bash
+for album in $(bandcamp_list_albums "$BANDCAMP_PAGE_URL" --print-urls)
+do
+    bandcamp_name_your_price_dl "$album" || bandcamp-dl "$album"
+done
+```
+
+You may also want to specify email, country and postcode in case bandcamp asks for those and download directory.
+
+
```

### Comparing `bandcamp_name_your_price_dl-0.0.8/bandcamp_name_your_price_dl.py` & `bandcamp_name_your_price_dl-0.0.9/bandcamp_name_your_price_dl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __desc__ = "Automate process of downloading name your price albums from bandcamp."
 
 import argparse
 import json
 import os
 import re
 import shutil
 import sys
+from enum import IntEnum
 from pathlib import Path
 from urllib.parse import urljoin, urlparse
 
 import requests
 from selenium import webdriver
 from selenium.common.exceptions import *
 from selenium.webdriver.common.by import By
@@ -29,14 +30,21 @@
     "opera",
     "phantomjs",
     "safari",
     "webkit",
 )
 
 
+class ExitCodes(IntEnum):
+    SUCCESS = 0
+    UNDOWNLOADABLE = 1
+    EMAIL_UNSPECIFIED = 2
+    CACHE_CORRUPTED = 3
+
+
 def main():
     parser = argparse.ArgumentParser(
         prog="bandcamp_name_your_price_dl",
         description=__desc__,
     )
     parser.add_argument(
         "album_url",
@@ -166,15 +174,15 @@
         Path(cache_file).touch()
         try:
             with open(cache_file) as f:
                 loaded_cache = json.load(f)
         except json.JSONDecodeError as e:
             print(e.msg)
             if not ask_to_overwrite_cache():
-                exit(3)
+                exit(ExitCodes.CACHE_CORRUPTED)
     else:
         loaded_cache = []
 
     def write_cache():
         if not args.ignore_cache:
             cache_entry["album_url"] = album_url
             if cache_entry not in loaded_cache:
@@ -185,24 +193,24 @@
     # Search for entry with desired url in cache, if not found then create new one
 
     for entry in loaded_cache:
         if remove_url_query_parameters(entry["album_url"]) == album_url:
             try:
                 if "downloadable" in entry.keys() and not entry["downloadable"]:
                     eprint("Album marked as undownloadable in cache. Aborting.")
-                    exit(1)
+                    exit(ExitCodes.UNDOWNLOADABLE)
                 download_url = entry["download_url"]
                 local_file_name = entry["local_file_name"]
                 cache_entry = entry
                 loaded_cache.remove(entry)
                 break
             except KeyError as e:
                 print(e.msg)
                 if not ask_to_overwrite_cache():
-                    exit(3)
+                    exit(ExitCodes.CACHE_CORRUPTED)
     else:
         loaded_cache.append({"album_url": album_url})
         cache_entry = loaded_cache[-1]
 
     if not args.download_dir:
         download_dir = os.path.curdir
     else:
@@ -230,15 +238,15 @@
             file_name_to_print = local_file_name
         else:
             file_name_to_print = download_directory_file_name
         eprint(
             f"File exists in {file_name_to_print}. Skipping scrapping and downloading.",
             "Rerun program with --dont-skip-if-file-exists to redownload.",
         )
-        finish_and_exit(0)
+        finish_and_exit(ExitCodes.SUCCESS)
 
     if (
         download_url is None
         or requests.get(download_url, stream=True).status_code != 200
     ):
         if args.encoding is not None:
             if args.encoding == "mp3":
@@ -264,15 +272,15 @@
         elif args.driver == "edge":
             driver = webdriver.Edge()
         elif args.driver in ("firefox", "gecko"):
             profile = FirefoxProfile()
             profile.set_preference("permissions.default.image", 2)
             if not args.show_browser_window:
                 os.environ["MOZ_HEADLESS"] = "1"
-            driver = webdriver.Firefox(profile)
+            driver = webdriver.Firefox(profile, service_log_path=os.devnull)
         elif args.driver == "opera":
             driver = webdriver.Opera()
         elif args.driver == "phantomjs":
             driver = webdriver.PhantomJS()
         elif args.driver == "safari":
             driver = webdriver.Safari()
         elif args.driver == "webkit":
@@ -304,33 +312,33 @@
                         "//span[@class='buyItemExtra buyItemNyp secondaryText']"
                     ).text
                     != "name your price"
                 ):
                     eprint("Album is not name your price. Aborting.")
                     cache_entry["downloadable"] = False
                     write_cache()
-                    finish_and_exit(1)
+                    finish_and_exit(ExitCodes.UNDOWNLOADABLE)
             except NoSuchElementException:
                 eprint(
                     "Element indicating if is album name your price not found. Aborting."
                 )
                 cache_entry["downloadable"] = False
                 write_cache()
-                finish_and_exit(1)
+                finish_and_exit(ExitCodes.UNDOWNLOADABLE)
 
             try:
                 buy_link = driver.find_element_by_xpath(
                     "//button[@class='download-link buy-link']"
                 )
                 buy_link.click()
             except NoSuchElementException:
                 eprint('"Buy Digital Album" link not found. Aborting')
                 cache_entry["downloadable"] = False
                 write_cache()
-                finish_and_exit(1)
+                finish_and_exit(ExitCodes.UNDOWNLOADABLE)
 
             price_input_filled = driver.find_element_by_xpath(
                 "//input[@class='display-price numeric']"
             )
             price_input_filled.clear()
             price_input_filled.send_keys("0")
 
@@ -352,15 +360,15 @@
 
                 asked_for_email = True
                 if email_address is None or postal_code is None:
                     eprint(
                         "Bandcamp asked for email, but no email address or postal code specified."
                         " Aborting."
                     )
-                    finish_and_exit(2)
+                    finish_and_exit(ExitCodes.EMAIL_UNSPECIFIED)
                 if country_abbrev is not None:
                     country_dropdown_list = Select(
                         driver.find_element_by_xpath("//*[@id='fan_email_country']")
                     )
                     country_dropdown_list.select_by_value(country_abbrev.upper())
                 postal_code_input = driver.find_element_by_xpath(
                     "//*[@id='fan_email_postalcode']"
@@ -432,15 +440,15 @@
     # Add album url, download url and local file name to json file in cache in order to avoid
     # scrapping the page or downloading the album twice
     if not args.ignore_cache:
         cache_entry["download_url"] = download_url
         cache_entry["local_file_name"] = local_file_name
         write_cache()
 
-    finish_and_exit(0)
+    finish_and_exit(ExitCodes.SUCCESS)
 
 
 def remove_url_query_parameters(url):
     return urljoin(url, urlparse(url).path)
 
 
 def eprint(*args, **kwargs):
```

### Comparing `bandcamp_name_your_price_dl-0.0.8/setup.py` & `bandcamp_name_your_price_dl-0.0.9/setup.py`

 * *Files identical despite different names*

