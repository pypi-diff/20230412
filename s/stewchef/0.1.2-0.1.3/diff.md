# Comparing `tmp/stewchef-0.1.2.tar.gz` & `tmp/stewchef-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stewchef-0.1.2.tar", max compression
+gzip compressed data, was "stewchef-0.1.3.tar", max compression
```

## Comparing `stewchef-0.1.2.tar` & `stewchef-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5654 2023-04-11 15:37:45.191398 stewchef-0.1.2/README.md
--rw-r--r--   0        0        0      489 2023-04-12 10:20:18.124101 stewchef-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.2/stewchef/__init__.py
--rw-r--r--   0        0        0    13128 2023-04-12 10:17:17.299510 stewchef-0.1.2/stewchef/main.py
--rw-r--r--   0        0        0     6390 1970-01-01 00:00:00.000000 stewchef-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5808 2023-04-12 10:26:35.957338 stewchef-0.1.3/README.md
+-rw-r--r--   0        0        0      489 2023-04-12 10:21:10.875274 stewchef-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.3/stewchef/__init__.py
+-rw-r--r--   0        0        0    13128 2023-04-12 10:17:17.299510 stewchef-0.1.3/stewchef/main.py
+-rw-r--r--   0        0        0     6544 1970-01-01 00:00:00.000000 stewchef-0.1.3/PKG-INFO
```

### Comparing `stewchef-0.1.2/README.md` & `stewchef-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # **StewChef: Cook up some RegiSoup**
 
-StewChef is a MediaWiki API wrapper for RegiSoup. It was developed since I came to the realization that I cannot edit the contents of a Wiki's `.xml` dump manually as each `<text>` block is also given a size in bytes and a `sha1` hash. The next easiest approach was to edit pages while they are already on the Wiki and that is possible through MediaWiki's API.  
+`StewChef` is a MediaWiki API wrapper for [`RegiSoup`](https://pypi.org/project/regisoup/). It was developed since I came to the realization that I cannot edit the contents of a Wiki's `.xml` dump manually as each `<text>` block is also given a size in bytes and a `sha1` hash. The next easiest approach was to edit pages while they are already on the Wiki and that is possible through MediaWiki's API.  
 
 ## **Usage:**
-First, to use StewChef, we must create a `config.toml` file where the API endpoint URL and bot credentials are specified. In your projects working directory create a `.toml` file anyway you like or with the command line as such:
+First, to use `StewChef`, we must create a `config.toml` file where the API endpoint URL and bot credentials are specified. In your projects working directory create a `.toml` file anyway you like or with the command line as such:
 ```
 nano config.toml
 ```
 and enter the following contents:
 ```
 [server]
 url = "[SERVER_IP]/api.php"
@@ -24,17 +24,17 @@
 
 #### **`stewchef single`**
 This command is meant more as the debug helper tool as it only gets the contents of one page. It is meant to make direct debugging of RegiSoup easier by retrieving pages from the Wiki. Usage is simple but you need to already know what you're looking for meaning the title. There is currently no way to search by title and then select. I might add that as a feature later on if I'll require it. Anyhow, it is generally meant that you run `stewchef feast` first which will print out the titles of the pages on the Wiki.
 Basic usage is meant as follows:
 ```
 stewchef single [page_title]
 ```
-This will just output the page contents to stdout. To explicitly save as a file you must supply the command with the ``--save` flag and a save path as such:
+This will just output the page contents to stdout. To explicitly save as a file you must supply the command with the ``--save` flag. By default the file save path is the page's title with the spaces removed but you can specify your own save path as such:
 ```
-stewchef single --save [page_title] [save_path]
+stewchef single --save [page_title] config.toml [save_path]
 ```
 Additionally the page can be saved as HTML by adding the flag `--as-html` and be made more verbose by adding `--verbose`. You can always get a reminder for this information by running:
 ```
 stewchef single --help
 ```
 
 #### **`stewchef feast`**
```

### Comparing `stewchef-0.1.2/stewchef/main.py` & `stewchef-0.1.3/stewchef/main.py`

 * *Files identical despite different names*

### Comparing `stewchef-0.1.2/PKG-INFO` & `stewchef-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stewchef
-Version: 0.1.2
+Version: 0.1.3
 Summary: A MediaWiki API wrapper for RegiSoup
 Author: pengu5055
 Author-email: urbancmarko1@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -16,18 +16,18 @@
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # **StewChef: Cook up some RegiSoup**
 
-StewChef is a MediaWiki API wrapper for RegiSoup. It was developed since I came to the realization that I cannot edit the contents of a Wiki's `.xml` dump manually as each `<text>` block is also given a size in bytes and a `sha1` hash. The next easiest approach was to edit pages while they are already on the Wiki and that is possible through MediaWiki's API.  
+`StewChef` is a MediaWiki API wrapper for [`RegiSoup`](https://pypi.org/project/regisoup/). It was developed since I came to the realization that I cannot edit the contents of a Wiki's `.xml` dump manually as each `<text>` block is also given a size in bytes and a `sha1` hash. The next easiest approach was to edit pages while they are already on the Wiki and that is possible through MediaWiki's API.  
 
 ## **Usage:**
-First, to use StewChef, we must create a `config.toml` file where the API endpoint URL and bot credentials are specified. In your projects working directory create a `.toml` file anyway you like or with the command line as such:
+First, to use `StewChef`, we must create a `config.toml` file where the API endpoint URL and bot credentials are specified. In your projects working directory create a `.toml` file anyway you like or with the command line as such:
 ```
 nano config.toml
 ```
 and enter the following contents:
 ```
 [server]
 url = "[SERVER_IP]/api.php"
@@ -44,17 +44,17 @@
 
 #### **`stewchef single`**
 This command is meant more as the debug helper tool as it only gets the contents of one page. It is meant to make direct debugging of RegiSoup easier by retrieving pages from the Wiki. Usage is simple but you need to already know what you're looking for meaning the title. There is currently no way to search by title and then select. I might add that as a feature later on if I'll require it. Anyhow, it is generally meant that you run `stewchef feast` first which will print out the titles of the pages on the Wiki.
 Basic usage is meant as follows:
 ```
 stewchef single [page_title]
 ```
-This will just output the page contents to stdout. To explicitly save as a file you must supply the command with the ``--save` flag and a save path as such:
+This will just output the page contents to stdout. To explicitly save as a file you must supply the command with the ``--save` flag. By default the file save path is the page's title with the spaces removed but you can specify your own save path as such:
 ```
-stewchef single --save [page_title] [save_path]
+stewchef single --save [page_title] config.toml [save_path]
 ```
 Additionally the page can be saved as HTML by adding the flag `--as-html` and be made more verbose by adding `--verbose`. You can always get a reminder for this information by running:
 ```
 stewchef single --help
 ```
 
 #### **`stewchef feast`**
```

