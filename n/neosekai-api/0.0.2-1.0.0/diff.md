# Comparing `tmp/neosekai_api-0.0.2-py3-none-any.whl.zip` & `tmp/neosekai_api-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 5650 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      189 b- defN 23-Apr-08 11:37 neosekai_api/__init__.py
--rw-rw-rw-  2.0 fat     1565 b- defN 23-Apr-08 11:38 neosekai_api/chapter.py
+Zip file size: 6337 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      219 b- defN 23-Apr-12 07:51 neosekai_api/__init__.py
+-rw-rw-rw-  2.0 fat     2474 b- defN 23-Apr-12 07:49 neosekai_api/chapter.py
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Apr-12 07:50 neosekai_api/constants.py
 -rw-rw-rw-  2.0 fat      294 b- defN 23-Apr-05 08:07 neosekai_api/helper.py
--rw-rw-rw-  2.0 fat     4087 b- defN 23-Apr-08 11:38 neosekai_api/novel.py
+-rw-rw-rw-  2.0 fat     4731 b- defN 23-Apr-12 07:47 neosekai_api/novel.py
 -rw-rw-rw-  2.0 fat      789 b- defN 23-Apr-08 09:56 neosekai_api/test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-08 11:45 neosekai_api-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1152 b- defN 23-Apr-08 11:45 neosekai_api-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-08 11:45 neosekai_api-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-08 11:45 neosekai_api-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      803 b- defN 23-Apr-08 11:45 neosekai_api-0.0.2.dist-info/RECORD
-10 files, 10075 bytes uncompressed, 4280 bytes compressed:  57.5%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-12 07:58 neosekai_api-1.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1152 b- defN 23-Apr-12 07:58 neosekai_api-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 07:58 neosekai_api-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-12 07:58 neosekai_api-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      883 b- defN 23-Apr-12 07:58 neosekai_api-1.0.0.dist-info/RECORD
+11 files, 11757 bytes uncompressed, 4841 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: neosekai_api/__init__.py
 Comment: 
 
 Filename: neosekai_api/chapter.py
 Comment: 
 
+Filename: neosekai_api/constants.py
+Comment: 
+
 Filename: neosekai_api/helper.py
 Comment: 
 
 Filename: neosekai_api/novel.py
 Comment: 
 
 Filename: neosekai_api/test.py
 Comment: 
 
-Filename: neosekai_api-0.0.2.dist-info/LICENSE
+Filename: neosekai_api-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: neosekai_api-0.0.2.dist-info/METADATA
+Filename: neosekai_api-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: neosekai_api-0.0.2.dist-info/WHEEL
+Filename: neosekai_api-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: neosekai_api-0.0.2.dist-info/top_level.txt
+Filename: neosekai_api-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: neosekai_api-0.0.2.dist-info/RECORD
+Filename: neosekai_api-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neosekai_api/__init__.py

```diff
@@ -1,7 +1,7 @@
 from .chapter import NovelChapter
 from .novel import Novel
-
+from .constants import VERSION
 __author__ = "John Erinjery"
-__version__ = "0.0.2"
+__version__ = VERSION
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2023 John Erinjery"
```

## neosekai_api/chapter.py

```diff
@@ -1,38 +1,73 @@
-from neosekai_api import Novel
+from neosekai_api.novel import Novel
 import requests
 from bs4 import BeautifulSoup
 
 
 class NovelChapter:
+    '''
+    NovelChapter object
 
-    def __init__(self, _url) -> None:
+    :params _url : The Mangadex Chapter URL
+    '''
+
+    def __init__(self, _url: str) -> None:
         self.url = self.__urlformatter(_url)
         self.__response_object = requests.get(self.url, timeout=10)
         self.details = self.chapter_details()
         self.volume = self.details['volume']
         self.name = self.details['chapter_name']
         self.release_date = self.details['release_date']
 
     def __urlformatter(self, _url):
+        """
+        formats url to standard form to be used in the program
+        """
         __url = ''
         if 'https://' not in _url:
             _url == 'https://' + _url
         else:
             return _url
 
     def chapter_details(self):
+        """
+        returns chapter details : 
+
+        - chapter volume
+        - chapter name
+        - url
+        - chapter release date
+
+        In the given order in JSON format
+
+        """
         novel_url = self.url[:self.url.index('/', 43)]
         novel = Novel(novel_url)
         index_page = novel.get_index_page()
         for i in index_page:
             if index_page[i]['url'] == self.url:
                 return index_page[i]
 
     def get_chapter_content(self):
+        """
+        returns main chapter content in JSON format
+
+        JSON format:
+        ```json
+            {
+                "1" : {
+                    "type" : '...', "content" : '...'
+                }
+            }
+        ```
+        - each key will be a paragraph
+        - ```type```  can have a value of ```text``` for textual content
+        - ```type``` can have a value of ```img``` if the content is an image. link to the image will be provided in ```content```
+
+        """
         soup = BeautifulSoup(self.__response_object.text, 'lxml')
         div = soup.find('div', attrs={'class': 'text-left'})
         paras = div.find_all('p')
         content = {}
         n = 1
         for i in paras:
             if i.span != None:
```

## neosekai_api/novel.py

```diff
@@ -1,22 +1,27 @@
 import requests
 from bs4 import BeautifulSoup
 from neosekai_api.helper import heavy_translate
 import json
 
 
 class Novel:
+    """
+    Novel Object
+    """
 
     def __init__(self, url):
         self.url = url
         self.response_object = requests.get(self.url, timeout=10)
         self.novel_tags = self.__initialiser()
 
     def __initialiser(self):
-
+        '''
+        returns novel tags as ```dict```
+        '''
         soup = BeautifulSoup(self.response_object.content, 'lxml')
 
         # finding title
         title = soup.find('title').text.split(' - NeoSekai')[0]
 
         # finding rating
         rating = soup.find('span', attrs={'id': 'averagerate'}).parent.text + \
@@ -62,24 +67,46 @@
                                 continue
 
                             novel_tags[key] = value
 
         return novel_tags
 
     def get_synopsis(self, fancy=True):
+        """
+        returns the synopsis text
+
+        fancy : if False, replaces all fancy punctuation marks with regular ones.
+        """
         soup = BeautifulSoup(self.response_object.content, 'lxml')
         synopsis = soup.find('div', attrs={
             'class': ['summary__content', 'show-more']}).text
 
         if fancy:
             return synopsis
         else:
             return heavy_translate(synopsis)
 
     def get_index_page(self):
+        """
+        returns the chapter list in JSON format
+
+        JSON : 
+        ```json
+            {
+                "1" : {
+                    "volume" : '...',
+                    "chapter_name" : '...',
+                    "url" : '...',
+                    "release_date" : '...'
+                },
+
+                "2" : {'...'}
+            }
+        ```
+        """
         url = 'https://www.neosekaitranslations.com/wp-admin/admin-ajax.php'
         soup = BeautifulSoup(self.response_object.content, 'lxml')
         data_id = soup.find(
             'div', attrs={'id': 'manga-chapters-holder'})['data-id']
         data = {'action': 'manga_get_chapters', 'manga': data_id}
         soup_2 = BeautifulSoup(requests.post(url, data).content, 'lxml')
         content_dict = {}
```

## Comparing `neosekai_api-0.0.2.dist-info/LICENSE` & `neosekai_api-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `neosekai_api-0.0.2.dist-info/METADATA` & `neosekai_api-1.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosekai-api
-Version: 0.0.2
+Version: 1.0.0
 Summary: An Unofficial API for NeoSekaiTranslations.com
 Home-page: https://github.com/john-erinjery/neosekai-api/
 Author: John Erinjery
 Author-email: jancyvinod415@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Customer Service
```

## Comparing `neosekai_api-0.0.2.dist-info/RECORD` & `neosekai_api-1.0.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-neosekai_api/__init__.py,sha256=-HWrX14AWeJNk3C9rYph6gErl6GE-QvkzpEWYuufm1E,189
-neosekai_api/chapter.py,sha256=DQYTZj7a_Bj0aGhFtYcYQ3EiFPoHOGCCUEYedNl14c4,1565
+neosekai_api/__init__.py,sha256=2mTOZgz2NPHku8xLpaSWbESVenEZutISVPG1Zkdkncc,219
+neosekai_api/chapter.py,sha256=hFNqw9TjtQlkjcnfCGAogmkMxgPkSNyzqeQF9DJAxN8,2474
+neosekai_api/constants.py,sha256=AWYQ4gHEit0Zv0vQW6fH_1MMyc0IO3zrT3ngo0xPptg,19
 neosekai_api/helper.py,sha256=pMbC0I3l7-3QIjVzA_omfqqF-N01G0j6-xmSx0OHa_4,294
-neosekai_api/novel.py,sha256=MtwZgRLzkGd8GgLs-dEcIR_XdgYtYfoXucafXWsnomg,4087
+neosekai_api/novel.py,sha256=5rO6FwzTOM_u_PKoku0RHw98cWy8ZRxIunlivjPIE1Q,4731
 neosekai_api/test.py,sha256=Eu_I25oZopbrvdx3Jo7tza2PLDNmSd8R0FzjLY1VyQk,789
-neosekai_api-0.0.2.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-neosekai_api-0.0.2.dist-info/METADATA,sha256=ATT-UXlwBnNUVGyZXoSHdChwtSYBsbvGVJWjQIqN8tE,1152
-neosekai_api-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neosekai_api-0.0.2.dist-info/top_level.txt,sha256=yhhnZQTXvjhjj5sIHCH99u0SXUqWkMfdfXrXuR585Us,13
-neosekai_api-0.0.2.dist-info/RECORD,,
+neosekai_api-1.0.0.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+neosekai_api-1.0.0.dist-info/METADATA,sha256=fyNMd08ChoABVK40hbIIujswjB89hKyQV03uWJcUT8Q,1152
+neosekai_api-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neosekai_api-1.0.0.dist-info/top_level.txt,sha256=yhhnZQTXvjhjj5sIHCH99u0SXUqWkMfdfXrXuR585Us,13
+neosekai_api-1.0.0.dist-info/RECORD,,
```

