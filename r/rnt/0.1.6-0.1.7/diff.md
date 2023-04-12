# Comparing `tmp/rnt-0.1.6.tar.gz` & `tmp/rnt-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnt-0.1.6.tar", last modified: Fri Mar 31 21:11:04 2023, max compression
+gzip compressed data, was "rnt-0.1.7.tar", last modified: Wed Apr 12 04:44:38 2023, max compression
```

## Comparing `rnt-0.1.6.tar` & `rnt-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jacobrohde   (501) staff       (20)        0 2023-03-31 21:11:04.555495 rnt-0.1.6/
--rw-------   0 jacobrohde   (501) staff       (20)     1073 2022-05-25 17:23:10.000000 rnt-0.1.6/LICENSE
--rw-r--r--   0 jacobrohde   (501) staff       (20)    10119 2023-03-31 21:11:04.555354 rnt-0.1.6/PKG-INFO
--rw-------   0 jacobrohde   (501) staff       (20)     9676 2023-03-31 21:08:56.000000 rnt-0.1.6/README.md
--rw-------   0 jacobrohde   (501) staff       (20)       84 2022-05-25 17:08:34.000000 rnt-0.1.6/pyproject.toml
--rw-r--r--   0 jacobrohde   (501) staff       (20)       38 2023-03-31 21:11:04.555526 rnt-0.1.6/setup.cfg
--rw-------   0 jacobrohde   (501) staff       (20)      778 2023-03-18 18:15:00.000000 rnt-0.1.6/setup.py
-drwxr-xr-x   0 jacobrohde   (501) staff       (20)        0 2023-03-31 21:11:04.553636 rnt-0.1.6/src/
-drwxr-xr-x   0 jacobrohde   (501) staff       (20)        0 2023-03-31 21:11:04.554393 rnt-0.1.6/src/rnt/
--rw-------   0 jacobrohde   (501) staff       (20)      203 2023-03-23 04:27:43.000000 rnt-0.1.6/src/rnt/__init__.py
--rw-------   0 jacobrohde   (501) staff       (20)    36889 2023-03-31 21:09:58.000000 rnt-0.1.6/src/rnt/rnt.py
-drwxr-xr-x   0 jacobrohde   (501) staff       (20)        0 2023-03-31 21:11:04.555209 rnt-0.1.6/src/rnt/url_functions/
--rw-------   0 jacobrohde   (501) staff       (20)      195 2023-03-24 02:09:17.000000 rnt-0.1.6/src/rnt/url_functions/__init__.py
--rw-r--r--   0 jacobrohde   (501) staff       (20)     4094 2023-03-31 20:57:51.000000 rnt-0.1.6/src/rnt/url_functions/url_functions.py
-drwxr-xr-x   0 jacobrohde   (501) staff       (20)        0 2023-03-31 21:11:04.554971 rnt-0.1.6/src/rnt.egg-info/
--rw-r--r--   0 jacobrohde   (501) staff       (20)    10119 2023-03-31 21:11:04.000000 rnt-0.1.6/src/rnt.egg-info/PKG-INFO
--rw-r--r--   0 jacobrohde   (501) staff       (20)      303 2023-03-31 21:11:04.000000 rnt-0.1.6/src/rnt.egg-info/SOURCES.txt
--rw-r--r--   0 jacobrohde   (501) staff       (20)        1 2023-03-31 21:11:04.000000 rnt-0.1.6/src/rnt.egg-info/dependency_links.txt
--rw-r--r--   0 jacobrohde   (501) staff       (20)       27 2023-03-31 21:11:04.000000 rnt-0.1.6/src/rnt.egg-info/requires.txt
--rw-r--r--   0 jacobrohde   (501) staff       (20)        4 2023-03-31 21:11:04.000000 rnt-0.1.6/src/rnt.egg-info/top_level.txt
+drwxr-xr-x   0 jacobrohde   (501) staff       (20)        0 2023-04-12 04:44:38.455235 rnt-0.1.7/
+-rw-------   0 jacobrohde   (501) staff       (20)     1073 2022-05-25 17:23:10.000000 rnt-0.1.7/LICENSE
+-rw-r--r--   0 jacobrohde   (501) staff       (20)    10390 2023-04-12 04:44:38.455088 rnt-0.1.7/PKG-INFO
+-rw-------   0 jacobrohde   (501) staff       (20)     9947 2023-04-12 04:35:16.000000 rnt-0.1.7/README.md
+-rw-------   0 jacobrohde   (501) staff       (20)       84 2022-05-25 17:08:34.000000 rnt-0.1.7/pyproject.toml
+-rw-r--r--   0 jacobrohde   (501) staff       (20)       38 2023-04-12 04:44:38.455278 rnt-0.1.7/setup.cfg
+-rw-------   0 jacobrohde   (501) staff       (20)      778 2023-04-12 04:30:28.000000 rnt-0.1.7/setup.py
+drwxr-xr-x   0 jacobrohde   (501) staff       (20)        0 2023-04-12 04:44:38.453162 rnt-0.1.7/src/
+drwxr-xr-x   0 jacobrohde   (501) staff       (20)        0 2023-04-12 04:44:38.453983 rnt-0.1.7/src/rnt/
+-rw-------   0 jacobrohde   (501) staff       (20)      203 2023-04-12 04:36:32.000000 rnt-0.1.7/src/rnt/__init__.py
+-rw-------   0 jacobrohde   (501) staff       (20)    38330 2023-04-12 04:43:48.000000 rnt-0.1.7/src/rnt/rnt.py
+drwxr-xr-x   0 jacobrohde   (501) staff       (20)        0 2023-04-12 04:44:38.454914 rnt-0.1.7/src/rnt/url_functions/
+-rw-------   0 jacobrohde   (501) staff       (20)      195 2023-03-24 02:09:17.000000 rnt-0.1.7/src/rnt/url_functions/__init__.py
+-rw-r--r--   0 jacobrohde   (501) staff       (20)     4094 2023-03-31 20:57:51.000000 rnt-0.1.7/src/rnt/url_functions/url_functions.py
+drwxr-xr-x   0 jacobrohde   (501) staff       (20)        0 2023-04-12 04:44:38.454643 rnt-0.1.7/src/rnt.egg-info/
+-rw-r--r--   0 jacobrohde   (501) staff       (20)    10390 2023-04-12 04:44:38.000000 rnt-0.1.7/src/rnt.egg-info/PKG-INFO
+-rw-r--r--   0 jacobrohde   (501) staff       (20)      303 2023-04-12 04:44:38.000000 rnt-0.1.7/src/rnt.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobrohde   (501) staff       (20)        1 2023-04-12 04:44:38.000000 rnt-0.1.7/src/rnt.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobrohde   (501) staff       (20)       27 2023-04-12 04:44:38.000000 rnt-0.1.7/src/rnt.egg-info/requires.txt
+-rw-r--r--   0 jacobrohde   (501) staff       (20)        4 2023-04-12 04:44:38.000000 rnt-0.1.7/src/rnt.egg-info/top_level.txt
```

### Comparing `rnt-0.1.6/LICENSE` & `rnt-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rnt-0.1.6/PKG-INFO` & `rnt-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnt
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple tool for generating and analyzing Reddit networks.
 Home-page: https://github.com/jarohde/rnt
 Author: Jacob Rohde
 Author-email: jarohde1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 
 -   The "url_functions" sub-package provides additional features for extracting URL information from Reddit data.
 
 ## General
 
 **Current version:**
 
-0.1.6 (released 03/31/2023)
+0.1.7 (released 04/12/2023)
 
 *Note: The minor changes in this release reflect Pushshift's modified endpoints after the recent server migration. There are still some Pushshift bugs and timeouts that may affect how the* `GetRedditData()` *feature in this package works. I will be sure to address future bugs ASAP. Version 0.1.6 also added a sub-package for extracting URL information from Reddit data*.
 
 **Import RNT library:**
 
     import rnt
 
@@ -90,14 +90,16 @@
 
 `GetRedditData.df`: Object attribute; extracts the Reddit data set as a pandas DataFrame object.
 
 `GetRedditData.write_data()`: Object method that writes the pandas DataFrame object to file. The method can take `file_type` and `file_name` as optional arguments. `file_type` indicates what file format to use when writing the data set and accepts a string argument of either 'json' or 'csv'; default set to 'json'. `file_name` takes a string to indicate what the file name should be saved as; default set to the search term provided.
 
 `GetRedditData.extract_urls()`: Object method to extract and append a list of URLs and URL domains in the Reddit data set.
 
+`GetRedditData.anonymize_authors()`: Object method to change Reddit usernames ('author' column) to anonymized random character strings. The name of the column containing the original Reddit usernames will be changed to 'author_original'. This method takes no arguments.
+
 ### GetRedditNetwork()
 
     rnt.GetRedditNetwork(reddit_dataset, 
                          edge_type, 
                          text_attribute) 
 
 **Overview:** A class object for generating edge and node lists, and a NetworkX graph object from a Reddit data set.
```

### Comparing `rnt-0.1.6/README.md` & `rnt-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 -   The "url_functions" sub-package provides additional features for extracting URL information from Reddit data.
 
 ## General
 
 **Current version:**
 
-0.1.6 (released 03/31/2023)
+0.1.7 (released 04/12/2023)
 
 *Note: The minor changes in this release reflect Pushshift's modified endpoints after the recent server migration. There are still some Pushshift bugs and timeouts that may affect how the* `GetRedditData()` *feature in this package works. I will be sure to address future bugs ASAP. Version 0.1.6 also added a sub-package for extracting URL information from Reddit data*.
 
 **Import RNT library:**
 
     import rnt
 
@@ -76,14 +76,16 @@
 
 `GetRedditData.df`: Object attribute; extracts the Reddit data set as a pandas DataFrame object.
 
 `GetRedditData.write_data()`: Object method that writes the pandas DataFrame object to file. The method can take `file_type` and `file_name` as optional arguments. `file_type` indicates what file format to use when writing the data set and accepts a string argument of either 'json' or 'csv'; default set to 'json'. `file_name` takes a string to indicate what the file name should be saved as; default set to the search term provided.
 
 `GetRedditData.extract_urls()`: Object method to extract and append a list of URLs and URL domains in the Reddit data set.
 
+`GetRedditData.anonymize_authors()`: Object method to change Reddit usernames ('author' column) to anonymized random character strings. The name of the column containing the original Reddit usernames will be changed to 'author_original'. This method takes no arguments.
+
 ### GetRedditNetwork()
 
     rnt.GetRedditNetwork(reddit_dataset, 
                          edge_type, 
                          text_attribute) 
 
 **Overview:** A class object for generating edge and node lists, and a NetworkX graph object from a Reddit data set.
```

### Comparing `rnt-0.1.6/setup.py` & `rnt-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rnt",
-    version="0.1.6",
+    version="0.1.7",
     author="Jacob Rohde",
     author_email="jarohde1@gmail.com",
     description="A simple tool for generating and analyzing Reddit networks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jarohde/rnt",
     classifiers=[
```

### Comparing `rnt-0.1.6/src/rnt/rnt.py` & `rnt-0.1.7/src/rnt/rnt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Package name: 'rnt' (Reddit Network Toolkit)
-Version number: 0.1.6 (released 03/31/2023)
+Version number: 0.1.7 (released 04/12/2023)
 Author: Jacob A. Rohde
 Author_email: jarohde1@gmail.com
 Description: A simple tool for generating and analyzing Reddit networks
 Github url: https://github.com/jarohde/rnt
 License: MIT
 """
 
@@ -46,14 +46,21 @@
 
     Methods:
 
     - GetRedditData.write_data(): Object method that writes the pandas DataFrame object to file. The method can take
       file_type and file_name as optional arguments. file_type indicates what file format to use when writing the data
       set and accepts a string argument of either 'json' or 'csv'; default set to 'json'. file_name takes a string to
       indicate what the file name should be saved as; default set to the search term provided.
+
+    - GetRedditData.extract_urls(): Object method to extract and append a list of URLs and URL domains to the data set.
+      This method takes no additional arguments.
+
+    - GetRedditData.anonymize_authors(): Object method to change Reddit usernames ('author' column) to anonymized random
+      character strings. The name of the column containing the original Reddit usernames will be changed to
+      'author_original'. This method takes no arguments.
     """
 
     def __init__(self, search_term, **kwargs):
 
         self.search_term = search_term
         self.search_term_is_subreddit = kwargs.get('search_term_is_subreddit', False)
         self.start_date = kwargs.get('start_date', None)
@@ -250,14 +257,40 @@
             domain_list.append(rnt_url.domain_extractor(text))
             number_of_urls.append(len(post_urls))
 
         self.df['url_list'] = url_list
         self.df['domain_list'] = domain_list
         self.df['number_of_urls'] = number_of_urls
 
+    def anonymize_authors(self):
+        """
+        Method to change Reddit usernames ('author' column) to anonymized random character strings. The name of the
+        column containing the original Reddit usernames will be changed to 'author_original'.
+        """
+        import random
+        import string
+
+        authors = self.df.author.unique()
+        author_mapping = {}
+
+        for author in authors:
+            if author == '[deleted]' or author == 'AutoModerator':
+                author_mapping[author] = author
+
+            else:
+                mapping_value = ''.join([random.choice(string.ascii_letters) for _ in range(8)])
+
+                while mapping_value in author_mapping.values():
+                    mapping_value = ''.join([random.choice(string.ascii_letters) for _ in range(8)])
+
+                author_mapping[author] = mapping_value
+
+        self.df['author_original'] = self.df.author
+        self.df['author'] = self.df.author.map(author_mapping)
+
 
 class GetRedditNetwork:
     """
     A class object for generating edge and node lists, and a NetworkX graph object from a Reddit data set.
 
     Arguments:
```

### Comparing `rnt-0.1.6/src/rnt/url_functions/url_functions.py` & `rnt-0.1.7/src/rnt/url_functions/url_functions.py`

 * *Files identical despite different names*

### Comparing `rnt-0.1.6/src/rnt.egg-info/PKG-INFO` & `rnt-0.1.7/src/rnt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnt
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple tool for generating and analyzing Reddit networks.
 Home-page: https://github.com/jarohde/rnt
 Author: Jacob Rohde
 Author-email: jarohde1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,15 @@
 
 -   The "url_functions" sub-package provides additional features for extracting URL information from Reddit data.
 
 ## General
 
 **Current version:**
 
-0.1.6 (released 03/31/2023)
+0.1.7 (released 04/12/2023)
 
 *Note: The minor changes in this release reflect Pushshift's modified endpoints after the recent server migration. There are still some Pushshift bugs and timeouts that may affect how the* `GetRedditData()` *feature in this package works. I will be sure to address future bugs ASAP. Version 0.1.6 also added a sub-package for extracting URL information from Reddit data*.
 
 **Import RNT library:**
 
     import rnt
 
@@ -90,14 +90,16 @@
 
 `GetRedditData.df`: Object attribute; extracts the Reddit data set as a pandas DataFrame object.
 
 `GetRedditData.write_data()`: Object method that writes the pandas DataFrame object to file. The method can take `file_type` and `file_name` as optional arguments. `file_type` indicates what file format to use when writing the data set and accepts a string argument of either 'json' or 'csv'; default set to 'json'. `file_name` takes a string to indicate what the file name should be saved as; default set to the search term provided.
 
 `GetRedditData.extract_urls()`: Object method to extract and append a list of URLs and URL domains in the Reddit data set.
 
+`GetRedditData.anonymize_authors()`: Object method to change Reddit usernames ('author' column) to anonymized random character strings. The name of the column containing the original Reddit usernames will be changed to 'author_original'. This method takes no arguments.
+
 ### GetRedditNetwork()
 
     rnt.GetRedditNetwork(reddit_dataset, 
                          edge_type, 
                          text_attribute) 
 
 **Overview:** A class object for generating edge and node lists, and a NetworkX graph object from a Reddit data set.
```

