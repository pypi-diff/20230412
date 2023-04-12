# Comparing `tmp/datahtml-0.3.0rc0.tar.gz` & `tmp/datahtml-0.4.0rc0.tar.gz`

## Comparing `datahtml-0.3.0rc0.tar` & `datahtml-0.4.0rc0.tar`

### file list

```diff
@@ -1,41 +1,52 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/.pylintrc
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/readthedocs.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/_utils.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/base.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/crawler.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/defaults.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/errors.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/google.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/news.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/parsers.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/rss.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/sitemap.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/types.py
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/web.py
--rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/datahtml/youtube.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/docs/Makefile
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/docs/conf.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/docs/make.bat
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/__init__.py
--rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/google_search.html
--rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/lanacion_article.html
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/robots.txt
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/root_carrefour_sitemap.xml
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/test_google.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/test_root.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/test_youtube.py
--rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/youtube_channel.html
--rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/youtube_channel_rss.xml
--rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/youtube_search.html
--rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/youtube_video.html
--rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/tests/youtube_video.json
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/LICENSE
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/README.md
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/pyproject.toml
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 datahtml-0.3.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/.pylintrc
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/readthedocs.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/_utils.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/base.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/crawler.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/defaults.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/errors.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/google.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/news.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/parsers.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/rss.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/sitemap.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/types.py
+-rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/web.py
+-rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/youtube.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/apis/__init__.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/apis/youtube.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/Makefile
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/api_reference.rst
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/conf.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/make.bat
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/api/crawler.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/api/sitemap.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/api/types.rst
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/api/web.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/google_search.html
+-rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/lanacion_article.html
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/robots.txt
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/root_carrefour_sitemap.xml
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/test_apis_youtube.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/test_google.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/test_root.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/test_youtube.py
+-rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_channel.html
+-rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_channel_rss.xml
+-rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_search.html
+-rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_search_response.json
+-rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_video.html
+-rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_video.json
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_video_multiple_ids.json
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_video_response.json
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/LICENSE
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/README.md
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/PKG-INFO
```

### Comparing `datahtml-0.3.0rc0/.pylintrc` & `datahtml-0.4.0rc0/.pylintrc`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/datahtml/base.py` & `datahtml-0.4.0rc0/datahtml/base.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/datahtml/crawler.py` & `datahtml-0.4.0rc0/datahtml/crawler.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/datahtml/defaults.py` & `datahtml-0.4.0rc0/datahtml/defaults.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/datahtml/errors.py` & `datahtml-0.4.0rc0/datahtml/errors.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/datahtml/google.py` & `datahtml-0.4.0rc0/datahtml/google.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/datahtml/news.py` & `datahtml-0.4.0rc0/datahtml/news.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/datahtml/parsers.py` & `datahtml-0.4.0rc0/datahtml/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     is_a_file = bool(a_file)
 
     parsed = urlparse(href)
     if not parsed.netloc:
         protocol = "http"
         if url.secure:
             protocol = "https"
-        href = f"{protocol}://{url.netloc}/{parsed.path}"
+        href = f"{protocol}://{url.netloc}{parsed.path}"
     if url.domain_base in href:
         internal = True
 
     return types.Link(
         title=text.strip(), href=href.strip(), internal=internal, is_file=is_a_file
     )
 
@@ -177,15 +177,14 @@
                 links.add(link)
         except KeyError:
             pass
     return list(links)
 
 
 def extract_images(soup: BS) -> List[types.Image]:
-
     images = [
         types.Image(alt=x.get("alt", ""), src=x.get("src", ""))
         for x in soup.findAll("img")
     ]
     return images
```

### Comparing `datahtml-0.3.0rc0/datahtml/rss.py` & `datahtml-0.4.0rc0/datahtml/rss.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/datahtml/sitemap.py` & `datahtml-0.4.0rc0/datahtml/sitemap.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/datahtml/types.py` & `datahtml-0.4.0rc0/datahtml/types.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/datahtml/web.py` & `datahtml-0.4.0rc0/datahtml/web.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,119 @@
 from typing import Any, Dict, List, Optional
 
 from datahtml import errors, news, parsers, rss, sitemap, types
 from datahtml._utils import difference_from_now
 from datahtml.base import CrawlerSpec
 
 
-class Web:
-    def __init__(self, url, *, html_txt, is_root=False):
+class WebDocument:
+    """
+    It's the main object for the library. It represents a HTML Document.
+    This page could be a root link or a subpage.
+    """
+    def __init__(self, url: str, *, html_txt: str, is_root=False):
+        """
+        :param url: url where the document belongs.
+        :type url: str
+        :param html_txt: html text of the document.
+        :type html_txt: str
+        :param is_root: if is the root site or a subpage.
+        :type is_root: bool
+        """
         self.url: types.URL = parsers.parse_url(url)
         self._html = html_txt
         self.soup = parsers.text2soup(html_txt)
         self.is_root = is_root
 
     @classmethod
     def parse(
         cls,
         url: str,
         *,
         crawler: CrawlerSpec,
         is_root=False,
-    ) -> "Web":
+    ) -> "WebDocument":
+        """
+        It crawl and parse a url passed.
+
+        .. deprecated:: 0.3.0
+           Use :func:`datahtml.web.download`
+
+        """
         rsp = crawler.get(url)
         obj = cls(url=url, html_txt=rsp.text, is_root=is_root)
         return obj
 
     def links(self) -> List[types.Link]:
-        links = parsers.extract_links(self.soup, fullurl=self.url.fullurl)
+        links = parsers.extract_links(self.soup, fullurl=self.url.fullurl.strip("/"))
         return links
 
     def images(self) -> List[types.Image]:
         return parsers.extract_images(self.soup)
 
     def ld_json(self) -> Dict[str, Any]:
         return parsers.extract_ld_json(self.soup)
 
     def meta_og(
         self, keys=["og:url", "og:image", "og:description", "og:type"]
     ) -> Dict[str, str]:
         return parsers.extract_meta_og(self.soup, meta=keys)
 
     def article(self) -> news.ArticleData:
-        ad = news.ArticleData.from_html(url=self.url, html=self._html)
+        ad = news.ArticleData.from_html(url=self.url.fullurl, html=self._html)
         return ad
 
+    def __repr__(self):
+        return f"<WebDocument '{self.url.fullurl}'>"
+
+    def __str__(self):
+        return f"<WebDocument '{self.url.fullurl}'>"
+
 
 def download(
     url: str,
     *,
     crawler: CrawlerSpec,
     is_root=True,
-) -> Web:
+) -> WebDocument:
+    """
+    It crawls the url passed.
+
+    :param url: url to crawl
+    :type url: str
+    :param crawler: A class:`CrawlerSpec` implementation.
+    :type crawler: CrawlerSpec
+    :param is_root: if it's a root site or not.
+    :type is_root: bool
+    :return: A web object.
+    :rtype: WebDocument
+    """
     rsp = crawler.get(url)
-    w = Web(url=url, html_txt=rsp.text, is_root=is_root)
+    w = WebDocument(url=url, html_txt=rsp.text, is_root=is_root)
     return w
 
 
 def build_sitemap(
-    url, *, crawler: CrawlerSpec, filter_dt=1
+    url: str, *, crawler: CrawlerSpec, filter_dt: int = 1
 ) -> List[sitemap.SitemapLink]:
-    rsp_txt = crawler.get(f"{url.strip()}/robots.txt")
+    """
+    It try to get the sitemap of the site based on the robots.txt protocol.
+    After finding sitemaps links, it starts crawling each link.
+
+    :param url: Base url of the site
+    :type url: str
+    :param crawler: A crawler based on the :class:`CrawlerSpec`
+    :type crawler: CrawlerSpec
+    :param filter_dt: some sites could have a lot of sitemaps and links,
+        like media site, `filter_dt` helps to filter old content.
+
+    :return: A list of links extracted from the sitemaps.
+    :rtype: List[sitemap.SitemapLink]
+    """
+    rsp_txt = crawler.get(f"{url.strip('/')}/robots.txt")
     sitesmaps = sitemap.get_sitemaps_from_robots(rsp_txt.text)
 
     total_sites = []
     for site in sitesmaps:
         w = download(site, crawler=crawler)
         urls = w.soup.findAll("url")
         if urls:
@@ -74,51 +125,58 @@
             # for l in locs:
             xmlsites = w.soup.findAll("sitemap")
             for site2 in xmlsites:
                 try:
                     diff = difference_from_now(site2.lastmod.text)
                     if diff.days <= filter_dt:
                         _w = download(site2.loc.text, crawler=crawler)
-                        # _w = Web.parse(site2.loc.text, crawler=crawler)
                         if _w.soup:
                             _urls = _w.soup.findAll("url")
                             sites = sitemap.parse_sitemap_links(_urls)
                             total_sites.extend(sites)
                 except AttributeError:
                     pass
     return total_sites
 
 
-def find_rss_links(url, *, crawler: CrawlerSpec, web: Web = None) -> List[rss.RSSLink]:
-    """Main method, it will scrap from the url provided looking for links related
-    to rss feed. If it found rss links then, it will try to get the feed.
+def find_rss_links(
+    url: str, *, crawler: CrawlerSpec, web: WebDocument = None
+) -> List[rss.RSSLink]:
+    """
+    It will scrap the url, looking for links related to rss feeds.
+    If it found rss links, then it will try to get the feed from those urls.
+
+    :param url: base url to crawl, it should be the root url.
+    :type url: str
+    :param crawler: class:`CrawlerSpec` implementation to be used
+    :type crawler: CrawlerSpec
+    :param web: Optional, if a class:`WebDocument`  object is passed, then it wouldn't
+        crawl the site.
+    :return: A list of RSS link already parsed.
+    :rtype: List[rss.RSSLink]
     """
     _rss: List[rss.RSSLink] = []
     _urls = set()
     _parsed = set()
-    # breakpoint()
-    # print(url)
-    # w = Web.parse(url=url, crawler=crawler)
+
     w = web or download(url=url, crawler=crawler)
 
     rss_links = rss.find_rss_realated_links(w.links())
     for x in rss_links:
         if x not in _parsed:
-            # print(x)
-            # req = fetch.from_url(x)
             try:
                 possible = crawler.get(x)
                 _parsed.add(x)
 
                 if possible.is_xml:
                     if x not in _urls:
                         _urls.add(x)
                         _rss.append(rss.RSSLink(url=x, xmlcontent=possible.text))
                 else:
-                    w2 = Web(x, html_txt=possible.text)
+                    w2 = WebDocument(x, html_txt=possible.text)
                     rss_links2 = rss.find_rss_realated_links(w2.links())
                     for y in rss_links2:
                         if y not in _parsed:
                             # print(y)
                             possible2 = crawler.get(y)
                             _parsed.add(y)
                             try:
```

### Comparing `datahtml-0.3.0rc0/datahtml/youtube.py` & `datahtml-0.4.0rc0/datahtml/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/docs/Makefile` & `datahtml-0.4.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/docs/conf.py` & `datahtml-0.4.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/docs/index.rst` & `datahtml-0.4.0rc0/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 Under the hood datahtml uses libraries like BeautifoulSoup, Newspaper2k, feedparser between others
 
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
+   api_reference
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `datahtml-0.3.0rc0/docs/make.bat` & `datahtml-0.4.0rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/tests/google_search.html` & `datahtml-0.4.0rc0/tests/google_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/tests/lanacion_article.html` & `datahtml-0.4.0rc0/tests/lanacion_article.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/tests/root_carrefour_sitemap.xml` & `datahtml-0.4.0rc0/tests/root_carrefour_sitemap.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/tests/test_youtube.py` & `datahtml-0.4.0rc0/tests/test_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/tests/youtube_channel.html` & `datahtml-0.4.0rc0/tests/youtube_channel.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/tests/youtube_channel_rss.xml` & `datahtml-0.4.0rc0/tests/youtube_channel_rss.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/tests/youtube_search.html` & `datahtml-0.4.0rc0/tests/youtube_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/tests/youtube_video.html` & `datahtml-0.4.0rc0/tests/youtube_video.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/tests/youtube_video.json` & `datahtml-0.4.0rc0/tests/youtube_video.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/.gitignore` & `datahtml-0.4.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/LICENSE` & `datahtml-0.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `datahtml-0.3.0rc0/README.md` & `datahtml-0.4.0rc0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # datahtml
 
 [![PyPI - Version](https://img.shields.io/pypi/v/datahtml.svg)](https://pypi.org/project/datahtml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datahtml.svg)](https://pypi.org/project/datahtml)
+[![readthedocs](https://readthedocs.org/projects/datahtml/badge/?version=latest)](https://datahtml.readthedocs.io/en/latest/)
+
+-------
 
 **datahtml** is a library for crawling and extraction of data from html and xml content. 
 
 Datahtml lets you:
 
 * Extract ld+json data from html
 * Extract frequently used meta tags from html (those that are used for SEO and social media, between others)
@@ -20,11 +23,19 @@
 
 ## Quickstart
 
 ```console
 pip install datahtml
 ```
 
+```python
+
+from datahtml import web, crawler
+
+c = crawler.LocalCrawler()
+w = web.download("https://www.infobae.com", crawler=c)
+w.links()
+```
 
 ## License
 
-`datahtml` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`datahtml` is distributed under the terms of the [MPL-2.0](https://www.mozilla.org/en-US/MPL/2.0/) license.
```

### Comparing `datahtml-0.3.0rc0/pyproject.toml` & `datahtml-0.4.0rc0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "datahtml"
 description = 'A lib to work with html and web data'
 readme = "README.md"
 requires-python = ">=3.7"
-license = "MIT"
+license = "MPL-2.0"
 keywords = []
 authors = [
   { name = "Xavier Petit", email = "nuxion@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
@@ -28,14 +28,16 @@
 	"lxml~=4.6.3",
 	"ujson~=4.2.0",
 	"extruct~=0.13.0",
 	"feedparser~=6.0.8",
 	# "reppy~=0.4.14",
 	"newspaper3k~=0.2.8",
 	"httpx~=0.23.0",
+        "pydantic~=1.10.7"
+        
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/algorinfo/datahtml#readme"
 Issues = "https://github.com/algorinfo/datahtml/issues"
 Source = "https://github.com/algorinfo/datahtml"
@@ -43,14 +45,16 @@
 [tool.hatch.version]
 path = "datahtml/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
+  "pytest-asyncio",
+  "mypy~=1.0.1",
   "pip-tools",
   "isort",
   "pylint>2.6.0", # https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html#id4
   "black~=22.10.0",
   "black-macchiato", # for partial update of buffers in emacs
   "Sphinx~=5.3.0",
   "sphinx-autobuild",
```

### Comparing `datahtml-0.3.0rc0/PKG-INFO` & `datahtml-0.4.0rc0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: datahtml
-Version: 0.3.0rc0
+Version: 0.4.0rc0
 Summary: A lib to work with html and web data
 Project-URL: Documentation, https://github.com/algorinfo/datahtml#readme
 Project-URL: Issues, https://github.com/algorinfo/datahtml/issues
 Project-URL: Source, https://github.com/algorinfo/datahtml
 Author-email: Xavier Petit <nuxion@gmail.com>
+License-Expression: MPL-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,21 +20,25 @@
 Requires-Python: >=3.7
 Requires-Dist: beautifulsoup4~=4.10.0
 Requires-Dist: extruct~=0.13.0
 Requires-Dist: feedparser~=6.0.8
 Requires-Dist: httpx~=0.23.0
 Requires-Dist: lxml~=4.6.3
 Requires-Dist: newspaper3k~=0.2.8
+Requires-Dist: pydantic~=1.10.7
 Requires-Dist: ujson~=4.2.0
 Description-Content-Type: text/markdown
 
 # datahtml
 
 [![PyPI - Version](https://img.shields.io/pypi/v/datahtml.svg)](https://pypi.org/project/datahtml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datahtml.svg)](https://pypi.org/project/datahtml)
+[![readthedocs](https://readthedocs.org/projects/datahtml/badge/?version=latest)](https://datahtml.readthedocs.io/en/latest/)
+
+-------
 
 **datahtml** is a library for crawling and extraction of data from html and xml content. 
 
 Datahtml lets you:
 
 * Extract ld+json data from html
 * Extract frequently used meta tags from html (those that are used for SEO and social media, between others)
@@ -48,11 +53,19 @@
 
 ## Quickstart
 
 ```console
 pip install datahtml
 ```
 
+```python
+
+from datahtml import web, crawler
+
+c = crawler.LocalCrawler()
+w = web.download("https://www.infobae.com", crawler=c)
+w.links()
+```
 
 ## License
 
-`datahtml` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`datahtml` is distributed under the terms of the [MPL-2.0](https://www.mozilla.org/en-US/MPL/2.0/) license.
```

