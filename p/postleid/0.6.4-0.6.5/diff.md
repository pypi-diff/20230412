# Comparing `tmp/postleid-0.6.4.tar.gz` & `tmp/postleid-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postleid-0.6.4.tar", last modified: Tue Apr 11 11:26:37 2023, max compression
+gzip compressed data, was "postleid-0.6.5.tar", last modified: Wed Apr 12 16:51:12 2023, max compression
```

## Comparing `postleid-0.6.4.tar` & `postleid-0.6.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1075 2023-04-05 15:58:25.000000 postleid-0.6.4/LICENSE
--rw-r--r--   0 rainer    (1000) rainer    (1000)     2920 2023-04-11 11:26:37.741488 postleid-0.6.4/PKG-INFO
--rw-r--r--   0 rainer    (1000) rainer    (1000)      288 2023-04-11 10:58:17.000000 postleid-0.6.4/README.md
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1712 2023-04-07 14:20:30.000000 postleid-0.6.4/pyproject.toml
--rw-r--r--   0 rainer    (1000) rainer    (1000)       38 2023-04-11 11:26:37.741488 postleid-0.6.4/setup.cfg
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.737488 postleid-0.6.4/src/
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid/
--rw-r--r--   0 rainer    (1000) rainer    (1000)      580 2023-04-08 12:11:49.000000 postleid-0.6.4/src/postleid/__init__.py
--rwxr-xr-x   0 rainer    (1000) rainer    (1000)     7013 2023-04-09 19:19:40.000000 postleid-0.6.4/src/postleid/__main__.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)     5403 2023-04-09 19:15:27.000000 postleid-0.6.4/src/postleid/commons.py
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid/data/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     3709 2023-04-11 10:34:20.000000 postleid-0.6.4/src/postleid/data/country_names_by_cc.yaml
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1490 2023-04-11 07:13:07.000000 postleid-0.6.4/src/postleid/data/default_user_settings.yaml
--rw-r--r--   0 rainer    (1000) rainer    (1000)    13200 2023-04-11 09:44:57.000000 postleid-0.6.4/src/postleid/data/postal_code_rules_by_cc.yaml
--rw-r--r--   0 rainer    (1000) rainer    (1000)    10384 2023-04-09 19:17:40.000000 postleid-0.6.4/src/postleid/fix_excel_files.py
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid/locale/
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid/locale/de/
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid/locale/de/LC_MESSAGES/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     3749 2023-04-05 15:58:26.000000 postleid-0.6.4/src/postleid/locale/de/LC_MESSAGES/argparse.mo
--rw-r--r--   0 rainer    (1000) rainer    (1000)      738 2023-04-09 19:13:52.000000 postleid-0.6.4/src/postleid/paths.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1194 2023-04-06 08:11:50.000000 postleid-0.6.4/src/postleid/presets.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)    13925 2023-04-05 15:58:26.000000 postleid-0.6.4/src/postleid/rule_checks.py
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid.egg-info/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     2920 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/PKG-INFO
--rw-r--r--   0 rainer    (1000) rainer    (1000)      660 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/SOURCES.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)        1 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/dependency_links.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)       52 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/entry_points.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)       54 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/requires.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)        9 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/top_level.txt
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/tests/
--rw-r--r--   0 rainer    (1000) rainer    (1000)    13336 2023-04-05 15:58:26.000000 postleid-0.6.4/tests/test_commons.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)     3630 2023-04-05 15:58:26.000000 postleid-0.6.4/tests/test_rule_checks.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.817507 postleid-0.6.5/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1075 2023-04-05 15:58:25.000000 postleid-0.6.5/LICENSE
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     2949 2023-04-12 16:51:12.817507 postleid-0.6.5/PKG-INFO
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      317 2023-04-12 16:42:54.000000 postleid-0.6.5/README.md
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1712 2023-04-07 14:20:30.000000 postleid-0.6.5/pyproject.toml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)       38 2023-04-12 16:51:12.817507 postleid-0.6.5/setup.cfg
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.813507 postleid-0.6.5/src/
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.813507 postleid-0.6.5/src/postleid/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      580 2023-04-11 11:31:07.000000 postleid-0.6.5/src/postleid/__init__.py
+-rwxr-xr-x   0 rainer    (1000) rainer    (1000)     7013 2023-04-09 19:19:40.000000 postleid-0.6.5/src/postleid/__main__.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     5403 2023-04-09 19:15:27.000000 postleid-0.6.5/src/postleid/commons.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.817507 postleid-0.6.5/src/postleid/data/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     8989 2023-04-12 16:36:53.000000 postleid-0.6.5/src/postleid/data/country_names_by_cc.yaml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1490 2023-04-11 07:13:07.000000 postleid-0.6.5/src/postleid/data/default_user_settings.yaml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    19220 2023-04-12 16:33:57.000000 postleid-0.6.5/src/postleid/data/postal_code_rules_by_cc.yaml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    12391 2023-04-12 11:18:02.000000 postleid-0.6.5/src/postleid/fix_excel_files.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.813507 postleid-0.6.5/src/postleid/locale/
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.813507 postleid-0.6.5/src/postleid/locale/de/
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.817507 postleid-0.6.5/src/postleid/locale/de/LC_MESSAGES/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     3749 2023-04-05 15:58:26.000000 postleid-0.6.5/src/postleid/locale/de/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      738 2023-04-09 19:13:52.000000 postleid-0.6.5/src/postleid/paths.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1194 2023-04-06 08:11:50.000000 postleid-0.6.5/src/postleid/presets.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    13925 2023-04-05 15:58:26.000000 postleid-0.6.5/src/postleid/rule_checks.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.817507 postleid-0.6.5/src/postleid.egg-info/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     2949 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/PKG-INFO
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      660 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/SOURCES.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)        1 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/dependency_links.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)       52 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/entry_points.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)       54 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/requires.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)        9 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/top_level.txt
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.817507 postleid-0.6.5/tests/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    13336 2023-04-05 15:58:26.000000 postleid-0.6.5/tests/test_commons.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     3630 2023-04-05 15:58:26.000000 postleid-0.6.5/tests/test_rule_checks.py
```

### Comparing `postleid-0.6.4/LICENSE` & `postleid-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/PKG-INFO` & `postleid-0.6.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postleid
-Version: 0.6.4
+Version: 0.6.5
 Summary: Fix postal codes notation in spreadsheet documents
 Author-email: Rainer Schwarzbach <undisclosed@example.com>
 License: MIT License
         
         Copyright (c) 2023 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,11 +50,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Postleid
 
 Skript zum Korrigieren von Postleitzahlen in Excel-Dateien
 
-Bisher werden Postleitzahlenregeln für 83 Länder,
-darunter Belgien, Deutschland, Österreich und die Schweiz,
+Bisher werden Postleitzahlenregeln für 132 Länder,
+darunter die Niederlande, Belgien, Luxemburg, Deutschland,
+Österreich und die Schweiz,
 unterstützt (siehe CHANGELOG.md und countries.txt).
 Die Unterstützung weiterer Länder ist in Arbeit.
```

### Comparing `postleid-0.6.4/pyproject.toml` & `postleid-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/src/postleid/__init__.py` & `postleid-0.6.5/src/postleid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
 
-__version__ = "0.6.4"
+__version__ = "0.6.5"
 
 
 # vim: fileencoding=utf-8 sw=4 ts=4 sts=4 expandtab autoindent syntax=python:
```

### Comparing `postleid-0.6.4/src/postleid/__main__.py` & `postleid-0.6.5/src/postleid/__main__.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/src/postleid/commons.py` & `postleid-0.6.5/src/postleid/commons.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/src/postleid/data/default_user_settings.yaml` & `postleid-0.6.5/src/postleid/data/default_user_settings.yaml`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/src/postleid/data/postal_code_rules_by_cc.yaml` & `postleid-0.6.5/src/postleid/data/postal_code_rules_by_cc.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -308,17 +308,16 @@
   - literal: " "
   - pattern: nn
 de:
   comment: Germany
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Germany"
   compound:
-  - pattern: nn
-    min: 1
-  - pattern: nnn
+  - pattern: nnnnn
+    min: 1000
 dk:
   comment: Denmark
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Denmark"
   variants:
   - pattern: nnnn
   - compound:
@@ -360,40 +359,66 @@
   comment: Finland
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Finland"
   pattern: nnnnn
 fk:
   comment: Falkland Islands
   literal: "FIQQ 1ZZ"
+fm:
+  comment: Micronesia (part of US system)
+  variants:
+  - compound:
+    - pattern: nnnnn
+      min: 96941
+      max: 96944
+    - literal: "-"
+    - pattern: nnnn
+  - pattern: nnnnn
+    min: 96941
+    max: 96944
 fo:
   comment: Faroe Islands
   compound:
     - pattern: cc
     - pattern: nnn
 fr:
   comment: France
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
   compound:
     - pattern: nn
       min: 1
     - pattern: nnn
+gb:
+  comment: United Kingdom
+  urls:
+  - "https://en.wikipedia.org/wiki/Postcodes_in_the_United_Kingdom"
+  compound:
+  - pattern: a
+    except: [C, I, K, M, O, V]
+  - pattern: "[a]"
+    except: [C, I, K, M, O, V]
+  - pattern: n
+  - pattern: "[a/n]"
+    except: [C, I, K, M, O, V]
+  - literal: " "
+  - pattern: naa
 ge:
   comment: Georgia
   pattern: nnnn
 gf:
   comment: French Guiana
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
   compound:
     - literal: "973"
     - pattern: nn
       max: 90
 gg:
-  comment: Guernsey (part of UK  system)
+  comment: Guernsey (part of UK system)
   urls:
   - "https://en.wikipedia.org/wiki/GY_postcode_area"
   compound:
   - literal: "GY"
   - pattern: nn
     min: 1
     max: 10
@@ -591,15 +616,15 @@
   pattern: nnn
 it:
   comment: Italy
   urls:
   - "https://en.wikipedia.org/wiki/Codice_di_avviamento_postale"
   pattern: nnnnn
 je:
-  comment: Jersey (part of UK  system)
+  comment: Jersey (part of UK system)
   urls:
   - "https://en.wikipedia.org/wiki/JE_postcode_area"
   compound:
   - literal: cc
   - pattern: nn
     remove_leading_zeroes: yes
   - literal: " "
@@ -612,58 +637,349 @@
   comment: Japan
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Japan"
   compound:
   - pattern: nnn
     literal: "-"
   - pattern: nnnn
+ke:
+  comment: Kenya
+  pattern: nnnnn
+kg:
+  comment: Kyrgyzstan
+  pattern: nnnnnn
 kh:
   comment: Cambodia
   pattern: nnnnnn
+kr:
+  comment: South Korea
+  pattern: nnnnn
+kw:
+  comment: Kuwait
+  pattern: nnnnn
 ky:
   comment: Cayman Islands
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_the_Cayman_Islands"
   compound:
   - pattern: cc
   - pattern: n
     min: 1
     max: 3
   - literal: "-"
   - pattern: nnnn
+kz:
+  comment: Kazakhstan
+  pattern: nnnnnn
+la:
+  comment: Laos
+  pattern: nnnnn
+lb:
+  comment: Lebanon
+  variants:
+  - compound:
+    - pattern: nnnn
+    - literal: " "
+    - pattern: nnnn
+  - pattern: nnnn
 li:
   comment: Liechtenstein (part of Swiss system)
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Liechtenstein"
   compound:
   - pattern: nnn
     min: 948
     max: 949
   - pattern: n
+lr:
+  comment: Liberia
+  pattern : nnnn
+ls:
+  comment: Lesotho
+  pattern : nnn
+lt:
+  comment: Lithuania
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Lithuania"
+  compound:
+  - pattern: cc
+  - literal: "-"
+  - pattern: nnnnn
+lu:
+  comment: Luxembourg
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Luxembourg"
+  pattern: nnnn
+  min: 1000
+lv:
+  comment: Latvia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Latvia":
+  compound:
+  - pattern: cc
+  - literal: "-"
+  - pattern: nnnn
+ma:
+  comment: Morocco
+  urls:
+  - "https://en.youbianku.com/Morocco"
+  pattern: nnnnn
+mc:
+  comment: Monaco (part of French system)
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France#Monaco"
+  compound:
+  - literal: "980"
+  - pattern: nn
+md:
+  comment: Moldova
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Moldova"
+  compound:
+  - pattern: cc
+  - literal: "-"
+  - pattern: nnnn
+me:
+  comment: Montenegro
+  urls:
+  - "https://en.youbianku.com/Montenegro"
+  pattern: nnnnn
+mg:
+  comment: Madagascar
+  pattern: nnn
+mh:
+  comment: Marshall Islands (part of US system)
+  variants:
+  - compound:
+    - pattern: nnnnn
+      min: 96960
+      max: 96970
+    - literal: "-"
+    - pattern: nnnn
+  - pattern: nnnnn
+    min: 96960
+    max: 96970
+mk:
+  comment: North Macedonia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_North_Macedonia"
+  pattern: nnnn
+mm:
+  comment: Myanmar
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Myanmar"
+  compound:
+  - pattern: nn
+    min: 1
+    max: 15
+  - pattern: nnn
+mn:
+  comment: Mongolia
+  urls:
+  - "https://en.youbianku.com/Mongolia"
+  pattern: nnnnn
+mp:
+  comment: Northern Marianas (part of US system)
+  variants:
+  - compound:
+    - pattern: nnnnn
+      min: 96950
+      max: 96952
+    - literal: "-"
+    - pattern: nnnn
+  - pattern: nnnnn
+    min: 96950
+    max: 96952
+mq:
+  comment: Martinique
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  compound:
+  - literal: "972"
+  - pattern: nn
+    max: 90
+ms:
+  comment: Montserrat
+  urls:
+  - "https://en.wikipedia.org/wiki/Montserrat"
+  compound:
+  - literal: "MSR"
+  - pattern: nnnn
+    min: 1110
+    max: 1350
+mt:
+  comment: Malta
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Malta"
+  variants:
+  - compound:
+    - pattern: aaa
+    - literal: " "
+    - pattern: nnnn
+  - compound:
+    - pattern: aa
+      only: [TP]
+    - literal: " "
+    - pattern: nnnn
+mu:
+  comment: Mauritius
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Mauritius"
+  compound:
+  - pattern: "?"
+    only: ["1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "R"]
+  - pattern: nnnn
+mv:
+  comment: Maldives
+  pattern: nnnnn
+mw:
+  comment: Malawi
+  pattern: nnnnnn
+mx:
+  comment: Mexico
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Mexico"
+  pattern: nnnnn
+my:
+  comment: Malaysia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Malaysia"
+  pattern: nnnnn
+mz:
+  comment:  Mozambique
+  urls:
+  - "https://en.youbianku.com/Mozambique"
+  pattern: nnnn
+na:
+  comment: Namibia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Namibia"
+  pattern: nnnnn
+nc:
+  comment: New Caledonia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  compound:
+  - literal: "988"
+  - pattern: nn
+    max: 90
+ne:
+  comment: Niger
+  urls:
+  - "https://en.youbianku.com/Niger"
+  pattern: nnnn
+nf:
+  comment: Norfolk Island (part of Australian system)
+  urls:
+  - "https://en.youbianku.com/Norfolk_Island"
+  pattern: nnnn
+ng:
+  comment: Nigeria
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Nigeria"
+  pattern: nnnnnn
+ni:
+  comment: Nicaragua
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Nicaragua"
+  compound:
+  - pattern: n
+    min: 1
+  - pattern: nnnn
+nl:
+  comment: Netherlands
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_the_Netherlands"
+  compound:
+  - pattern: nnnn
+    min: 1000
+  - literal: " "
+  - pattern: aa
+    except: [SA, SD, SS]
+"no":
+  comment:  Norway
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Norway"
+  pattern: nnnn
+np:
+  comment:  Nepal
+  urls:
+  - "https://en.youbianku.com/Nepal"
+  pattern: nnnnn
+nz:
+  comment: New Zealand
+  urls:
+  - "https://en.wikipedia.org/wiki/Postcodes_in_New_Zealand"
+  pattern: nnnn
+om:
+  comment:  Oman
+  urls:
+  - "https://en.youbianku.com/Oman"
+  pattern: nnn
 pf:
   comment: French Polynesia
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Oceania#French_overseas_territories"
   compound:
-    - literal: "987"
-    - pattern: nn
-      max: 90
+  - literal: "987"
+  - pattern: nn
+    max: 90
+pl:
+  comment: Poland
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Poland"
+  compound:
+  - pattern: nn
+  - literal: "-"
+  - pattern: nnn
+pt:
+  comment: Portugal
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Portugal"
+  compound:
+  - pattern: nnnn
+    min: 1000
+  - literal: "-"
+  - pattern: nnn
 sv:
   comment: El Salvador
   pattern: nnnn
 sz:
   comment: Eswatini
   compound:
   - pattern: a
     only: [H, M, S, L]
   - pattern: nnn
+us:
+  comment: United States
+  urls:
+  - "https://en.wikipedia.org/wiki/ZIP_Code"
+  variants:
+  - compound:
+    - pattern: nnnnn
+    - literal: "-"
+    - pattern: nnnn
+  - pattern: nnnnn
 vg:
   comment: British Virgin Islands
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_the_British_Virgin_Islands"
   compound:
   - pattern: cc
   - pattern: nnn
     min: 111
     max: 116
   - pattern: n
-
+xk:
+  comment: Kosovo
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Kosovo"
+  pattern: nnnnn
+  min: 10000
+yt:
+  comment: Mayotte
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  compound:
+  - literal: "976"
+  - pattern: nn
+    max: 90
```

### Comparing `postleid-0.6.4/src/postleid/fix_excel_files.py` & `postleid-0.6.5/src/postleid/fix_excel_files.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
 
-from typing import Any, Dict, List, Union
+import re
+
+from typing import Any, Dict, List, Set, Union
 
 import numpy
 import pandas
 
 # local imports
 from postleid import commons
 from postleid import paths
@@ -34,14 +36,16 @@
 
 class DataFixer:
 
     """Fix cells in a workbook"""
 
     cc_column = "country_code"
 
+    prx_parenthesized = re.compile(r"\((.+?)\)")
+
     results_by_error = {
         rule_checks.InvalidFormatError: commons.S_WRONG_FORMAT,
         rule_checks.MissingRulesError: commons.S_MISSING_RULES,
         rule_checks.OutOfRangeError: commons.S_OUT_OF_RANGE,
         rule_checks.UnsupportedDataTypeError: commons.S_WRONG_DATA_TYPE,
     }
 
@@ -79,47 +83,91 @@
             #
             if column_name == self.cc_column:
                 self.cc_column = f"{column_name}_x"
             #
         #
         # Build a cc column
         self.__cc_lookup: Dict[str, str] = {}
-        for (
-            iso_cc,
-            country_names,
-        ) in commons.load_country_names_from_file().items():
-            for name in country_names:
-                self.__cc_lookup[name.lower()] = iso_cc
-            #
-        #
-
         if self.country_column:
+            # Build the cc lookup mapping
+            self.__build_cc_lookup()
+            # Build the cc_column directly:
+            # Map ISO-3166-1 ALPHA-2 codes to country names
+            # using the self.lookup_country_code() function because
+            # a simple dict is not sufficient (that would produce
+            # NaN values for unmatched country names), and we need
+            # even more flexibility than a collections.defaultdict()
+            # could provide.
             commons.LogWrapper.debug(
                 f"Reading country data from {self.country_column}"
             )
-            country_source = self.dataframe[self.country_column]
+            self.dataframe[self.cc_column] = self.dataframe[
+                self.country_column
+            ].map(self.lookup_country_code)
         else:
-            country_source = pandas.Series(self.dataframe.index)
+            # Build the cc column as a pandas.Series from "" * len(...)
+            self.dataframe[self.cc_column] = pandas.Series(
+                [""] * len(self.dataframe.index)
+            )
         #
-        # Map ISO-3166-1 ALPHA-2 codes to country names
-        # using the self.lookup_country_code() function because
-        # a simple dict is not sufficient (that would produce
-        # NaN values for unmatched country names), and we need
-        # even more flexibility than a collections.defaultdict()
-        # could provide.
-        self.dataframe[self.cc_column] = country_source.map(
-            self.lookup_country_code
-        )
         for line in str(self.dataframe).splitlines():
             commons.LogWrapper.debug(line)
         #
         self.__validator = rule_checks.ValidatorsCache(
             default_cc=self.user_settings.default_country_code
         )
 
+    def __build_cc_lookup(self) -> None:
+        """Build the country code lookup mapping from the
+        country codes configuration file
+        """
+        for (
+            iso_cc,
+            country_names,
+        ) in commons.load_country_names_from_file().items():
+            keys: Set[str] = set()
+            for configured_name in country_names:
+                lower_name = configured_name.lower()
+                has_parentheses = self.prx_parenthesized.search(lower_name)
+                if has_parentheses:
+                    # Add both variants:
+                    # with the paranthesized part deleted,
+                    # and with the parenthesized part stripped from the
+                    # parentheses.
+                    keys.add(
+                        self.prx_parenthesized.sub("", lower_name).strip()
+                    )
+                    keys.add(self.prx_parenthesized.sub(r"\1", lower_name))
+                else:
+                    keys.add(lower_name)
+                #
+            #
+            for single_key in keys:
+                try:
+                    existing_cc_entry = self.__cc_lookup[single_key]
+                except KeyError:
+                    self.__cc_lookup[single_key] = iso_cc
+                else:
+                    if existing_cc_entry != iso_cc:
+                        commons.LogWrapper.warning(
+                            f"Not adding {single_key} → {iso_cc} lookup",
+                            f"because {single_key} → {existing_cc_entry}"
+                            " has already been defined.",
+                        )
+                    #
+                #
+            #
+        #
+        commons.LogWrapper.debug(
+            f"Country codes lookup ({len(self.__cc_lookup)} items):"
+        )
+        for single_key, iso_cc in sorted(self.__cc_lookup.items()):
+            commons.LogWrapper.debug(f" - {single_key!r} → {iso_cc!r}")
+        #
+
     def lookup_country_code(self, country: Union[float, int, str]) -> str:
         """Lookup the country code for the given country"""
         country_code = ""
         if isinstance(country, (float, int)):
             return country_code
         #
         preprocessed_name = country.strip().lower()
```

### Comparing `postleid-0.6.4/src/postleid/locale/de/LC_MESSAGES/argparse.mo` & `postleid-0.6.5/src/postleid/locale/de/LC_MESSAGES/argparse.mo`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/src/postleid/paths.py` & `postleid-0.6.5/src/postleid/paths.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/src/postleid/presets.py` & `postleid-0.6.5/src/postleid/presets.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/src/postleid/rule_checks.py` & `postleid-0.6.5/src/postleid/rule_checks.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/src/postleid.egg-info/PKG-INFO` & `postleid-0.6.5/src/postleid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postleid
-Version: 0.6.4
+Version: 0.6.5
 Summary: Fix postal codes notation in spreadsheet documents
 Author-email: Rainer Schwarzbach <undisclosed@example.com>
 License: MIT License
         
         Copyright (c) 2023 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,11 +50,12 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Postleid
 
 Skript zum Korrigieren von Postleitzahlen in Excel-Dateien
 
-Bisher werden Postleitzahlenregeln für 83 Länder,
-darunter Belgien, Deutschland, Österreich und die Schweiz,
+Bisher werden Postleitzahlenregeln für 132 Länder,
+darunter die Niederlande, Belgien, Luxemburg, Deutschland,
+Österreich und die Schweiz,
 unterstützt (siehe CHANGELOG.md und countries.txt).
 Die Unterstützung weiterer Länder ist in Arbeit.
```

### Comparing `postleid-0.6.4/src/postleid.egg-info/SOURCES.txt` & `postleid-0.6.5/src/postleid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/tests/test_commons.py` & `postleid-0.6.5/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.4/tests/test_rule_checks.py` & `postleid-0.6.5/tests/test_rule_checks.py`

 * *Files identical despite different names*

