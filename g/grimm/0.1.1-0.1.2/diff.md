# Comparing `tmp/grimm-0.1.1.tar.gz` & `tmp/grimm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimm-0.1.1.tar", max compression
+gzip compressed data, was "grimm-0.1.2.tar", max compression
```

## Comparing `grimm-0.1.1.tar` & `grimm-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2022-11-09 00:29:41.774821 grimm-0.1.1/README.md
--rw-r--r--   0        0        0       39 2022-11-09 02:19:48.669381 grimm-0.1.1/grimm/__init__.py
--rw-r--r--   0        0        0    14966 2023-04-12 00:59:46.951413 grimm-0.1.1/grimm/cleaner_core.py
--rw-r--r--   0        0        0        0 2022-11-01 21:35:12.246873 grimm-0.1.1/grimm/support/__init__.py
--rw-r--r--   0        0        0     2878 2022-11-01 21:35:12.247048 grimm-0.1.1/grimm/support/magicwords.py
--rw-r--r--   0        0        0     1263 2022-11-01 21:35:12.247153 grimm-0.1.1/grimm/support/tags.py
--rw-r--r--   0        0        0      318 2023-04-12 01:00:52.395667 grimm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 grimm-0.1.1/setup.py
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 grimm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-11-09 00:29:41.774821 grimm-0.1.2/README.md
+-rw-r--r--   0        0        0       39 2022-11-09 02:19:48.669381 grimm-0.1.2/grimm/__init__.py
+-rw-r--r--   0        0        0    14966 2023-04-12 01:14:20.002504 grimm-0.1.2/grimm/cleaner_core.py
+-rw-r--r--   0        0        0        0 2022-11-01 21:35:12.246873 grimm-0.1.2/grimm/support/__init__.py
+-rw-r--r--   0        0        0     2878 2022-11-01 21:35:12.247048 grimm-0.1.2/grimm/support/magicwords.py
+-rw-r--r--   0        0        0     1263 2022-11-01 21:35:12.247153 grimm-0.1.2/grimm/support/tags.py
+-rw-r--r--   0        0        0      318 2023-04-12 01:08:33.458583 grimm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 grimm-0.1.2/setup.py
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 grimm-0.1.2/PKG-INFO
```

### Comparing `grimm-0.1.1/grimm/cleaner_core.py` & `grimm-0.1.2/grimm/cleaner_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,19 +270,19 @@
 
 # Constants needed for external link processing
 # Everything except bracket, space, or control characters
 # \p{Zs} is unicode 'separator, space' category. It covers the space 0x20
 # as well as U+3000 is IDEOGRAPHIC SPACE for bug 19052
 external_link_url_class = r'[^][<>"\x00-\x20\x7F\s]'
 external_link_regex = re.compile(
-    r'\[(((?i)' + '|'.join(wiki_url_protocols) + ')' + external_link_url_class + r'+)\s*([^\]\x00-\x08\x0a-\x1F]*?)\]',
+    r'(?i)\[((' + '|'.join(wiki_url_protocols) + ')' + external_link_url_class + r'+)\s*([^\]\x00-\x08\x0a-\x1F]*?)\]',
     re.S | re.U)
 external_image_regex = re.compile(
-    r"""^(http://|https://)([^][<>"\x00-\x20\x7F\s]+)
-    /([A-Za-z0-9_.,~%\-+&;#*?!=()@\x80-\xFF]+)\.((?i)gif|png|jpg|jpeg)$""",
+    r"""(?i)^(http://|https://)([^][<>"\x00-\x20\x7F\s]+)
+    /([A-Za-z0-9_.,~%\-+&;#*?!=()@\x80-\xFF]+)\.(gif|png|jpg|jpeg)$""",
     re.X | re.S | re.U)
 
 
 def parse_external_links(text):
     result = ''
     links = []
     images = []
```

### Comparing `grimm-0.1.1/grimm/support/magicwords.py` & `grimm-0.1.2/grimm/support/magicwords.py`

 * *Files identical despite different names*

### Comparing `grimm-0.1.1/grimm/support/tags.py` & `grimm-0.1.2/grimm/support/tags.py`

 * *Files identical despite different names*

