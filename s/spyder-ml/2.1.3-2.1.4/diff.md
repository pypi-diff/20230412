# Comparing `tmp/spyder_ml-2.1.3.tar.gz` & `tmp/spyder_ml-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyder_ml-2.1.3.tar", max compression
+gzip compressed data, was "spyder_ml-2.1.4.tar", max compression
```

## Comparing `spyder_ml-2.1.3.tar` & `spyder_ml-2.1.4.tar`

### file list

```diff
@@ -1,20 +1,15 @@
--rw-r--r--   0        0        0     1077 2022-12-31 02:15:12.000000 spyder_ml-2.1.3/LICENSE
--rw-r--r--   0        0        0     3267 2023-03-06 20:41:11.818134 spyder_ml-2.1.3/README.md
--rw-r--r--   0        0        0      798 2023-03-06 20:41:11.806134 spyder_ml-2.1.3/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-06 20:41:48.162277 spyder_ml-2.1.3/spyderml/__init__.py
--rw-r--r--   0        0        0       93 2022-12-31 02:15:12.000000 spyder_ml-2.1.3/spyderml/bin/spyderml
--rw-r--r--   0        0        0        0 2023-01-31 20:48:51.000000 spyder_ml-2.1.3/spyderml/lib/__init__.py
--rw-r--r--   0        0        0      173 2023-01-31 20:49:15.000000 spyder_ml-2.1.3/spyderml/lib/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      189 2022-12-31 02:15:12.000000 spyder_ml-2.1.3/spyderml/lib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1403 2022-12-31 02:15:12.000000 spyder_ml-2.1.3/spyderml/lib/__pycache__/ascarts.cpython-311.pyc
--rw-r--r--   0        0        0     3302 2022-12-31 02:23:56.000000 spyder_ml-2.1.3/spyderml/lib/__pycache__/asciiarts.cpython-310.pyc
--rw-r--r--   0        0        0     1876 2022-12-31 02:15:12.000000 spyder_ml-2.1.3/spyderml/lib/__pycache__/asciiarts.cpython-311.pyc
--rw-r--r--   0        0        0     3038 2022-12-31 02:15:12.000000 spyder_ml-2.1.3/spyderml/lib/asciiarts.py
--rw-r--r--   0        0        0      234 2022-12-31 02:15:12.000000 spyder_ml-2.1.3/spyderml/lib/detectos.py
--rw-r--r--   0        0        0      908 2023-02-26 19:31:39.000000 spyder_ml-2.1.3/spyderml/lib/file.py
--rw-r--r--   0        0        0     1365 2023-02-26 18:47:35.000000 spyder_ml-2.1.3/spyderml/lib/handle_headers_and_proxy.py
--rw-r--r--   0        0        0     5059 2023-03-01 10:32:59.000000 spyder_ml-2.1.3/spyderml/lib/spidercrawler.py
--rw-r--r--   0        0        0     6118 2023-02-26 19:57:39.000000 spyder_ml-2.1.3/spyderml/lib/spyder_reqs.py
--rw-r--r--   0        0        0     4002 2023-02-26 20:13:08.000000 spyder_ml-2.1.3/spyderml/lib/utils.py
--rw-r--r--   0        0        0     8824 2023-03-06 13:32:37.812981 spyder_ml-2.1.3/spyderml/main.py
--rw-r--r--   0        0        0     4335 1970-01-01 00:00:00.000000 spyder_ml-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-11 21:42:32.746636 spyder_ml-2.1.4/LICENSE
+-rw-r--r--   0        0        0     3268 2023-04-11 23:00:16.496628 spyder_ml-2.1.4/README.md
+-rw-r--r--   0        0        0      829 2023-04-11 22:38:33.836626 spyder_ml-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-11 21:42:32.746636 spyder_ml-2.1.4/spyderml/__init__.py
+-rw-r--r--   0        0        0       93 2023-04-11 21:42:32.746636 spyder_ml-2.1.4/spyderml/bin/spyderml
+-rw-r--r--   0        0        0     9970 2023-04-11 22:24:24.916637 spyder_ml-2.1.4/spyderml/main.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:42:32.746636 spyder_ml-2.1.4/spyderml/src/__init__.py
+-rw-r--r--   0        0        0     3038 2023-04-11 21:42:32.746636 spyder_ml-2.1.4/spyderml/src/asciiarts.py
+-rw-r--r--   0        0        0      234 2023-04-11 21:42:32.746636 spyder_ml-2.1.4/spyderml/src/detectos.py
+-rw-r--r--   0        0        0      908 2023-04-11 21:54:02.416639 spyder_ml-2.1.4/spyderml/src/file.py
+-rw-r--r--   0        0        0     1365 2023-04-11 21:54:36.986639 spyder_ml-2.1.4/spyderml/src/handle_headers_and_proxy.py
+-rw-r--r--   0        0        0     5406 2023-04-11 22:37:35.666636 spyder_ml-2.1.4/spyderml/src/spidercrawler.py
+-rw-r--r--   0        0        0     6118 2023-04-11 21:42:32.746636 spyder_ml-2.1.4/spyderml/src/spyder_reqs.py
+-rw-r--r--   0        0        0     4197 2023-04-11 21:58:01.026627 spyder_ml-2.1.4/spyderml/src/utils.py
+-rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 spyder_ml-2.1.4/PKG-INFO
```

### Comparing `spyder_ml-2.1.3/LICENSE` & `spyder_ml-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spyder_ml-2.1.3/README.md` & `spyder_ml-2.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 <h1 align="center">Spyder-HTML</h1>
 
 <p align="center">
 <img src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge"/>
-<img src="http://img.shields.io/static/v1?label=VERSION&message=2.1.3&color=blue&style=for-the-badge"/>
+<img src="http://img.shields.io/static/v1?label=VERSION&message=2.1.4&color=blue&style=for-the-badge"/>
 <img src="https://img.shields.io/github/license/accessmaker/Spyder-ml?style=for-the-badge"/>
 </p>
 
-
 A tool made to facilitate the analysis of html code.
 
 <h2>INSTALL(git clone):</h2>
 
-git clone https://github.com/accessmaker/Spyder-ml
+git clone <https://github.com/accessmaker/Spyder-ml>
 
 python setup.py install
 
-
 <h2>INSTALL(PIP):</h2>
 
-
 pip install spyder-ml
 
-
 <h2>USAGE:</h2>
 
 spyderml       [-h] [-t TARGET] [--tr TR] [--update]
                [--tags TAGS | --comments | --attribs ATTRIBS | --getjs | --techs | --geturls | --html | --jsr]
                [-o OUTPUT] [-C COOKIE] [-A AGENT] [-hf HEADERSFILE] [-S]
                [-w WORKERS] [--domain DOMAIN] [--cache] [--proxy PROXY]
                [-D DATA [DATA ...]]
 
 A tool made to facilitate the analysis of html code.
 
 options:<br>
   -h, --help            show this help message and exit<br>
   -t TARGET, --target TARGET<br>
                         Parameter that defines the target URL<
-                        http://example.com/index.html <br>
+                        <http://example.com/index.html> <br>
   --tr TR               Type of request(POST or GET(Default)).
   --update              Flag responsible for updating the database.<br>
   --tags TAGS           Flag that defines which tags the program will bring<br>
   --comments            Flag that brings the comments<br>
   --attribs ATTRIBS     Flag that defines which attributes the application
                         will look for.<br>
   --getjs               Flag that brings all JS files from the page.<br>
@@ -68,8 +64,8 @@
   --proxy PROXY         Defines the proxy that will be used (Which can be
                         passed tor or burpsuite to use these two default
                         proxies).<br>
   -D DATA [DATA ...], --data DATA [DATA ...]
                         Data to send with the request in format key1:value1
                         key2:value2 key3:value3...<br>
 
-'Functionality': It searches the html document for specific things
+'Functionality': It searches the html document for specific things
```

### Comparing `spyder_ml-2.1.3/pyproject.toml` & `spyder_ml-2.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spyder-ml"
-version = "2.1.3"
+version = "2.1.4"
 description = "A tool made to facilitate the analysis of html code."
 authors = ["Lucas dSilva <accessmaker.mlbb@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 classifiers = ["Development Status :: 5 - Production/Stable"]
 packages = [{include = "spyderml"}]
 repository = "https://github.com/accessmaker/Spyder-ml"
@@ -15,14 +15,15 @@
 colorama = "^0.4.6"
 webtech = "^1.3.2"
 beautifulsoup4 = "^4.11.1"
 requests = "^2.28.2"
 urllib3 = "^1.26.14"
 pysocks = "^1.7.1"
 argcomplete = "^2.0.5"
+types-requests = "^2.28.11.17"
 
 [tool.poetry.scripts]
 spyderml = "spyderml.main:main"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.0"
 autopep8 = "^2.0.1"
```

### Comparing `spyder_ml-2.1.3/spyderml/lib/asciiarts.py` & `spyder_ml-2.1.4/spyderml/src/asciiarts.py`

 * *Files identical despite different names*

### Comparing `spyder_ml-2.1.3/spyderml/lib/file.py` & `spyder_ml-2.1.4/spyderml/src/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from spyderml.lib.detectos import detect
+from spyderml.src.detectos import detect
 
 
 def open_file(filepath):
     try:
         if '~/' in filepath:
             filepath = filepath.replace('~/', detect())
         with open(filepath, 'r') as file:
```

### Comparing `spyder_ml-2.1.3/spyderml/lib/handle_headers_and_proxy.py` & `spyder_ml-2.1.4/spyderml/src/handle_headers_and_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from spyderml.lib.file import open_headers_file
+from spyderml.src.file import open_headers_file
 
 
 def handle_headers(useragent, cookies, headersfile):
     if useragent is not None or cookies is not None:
         if useragent and cookies:
             headers = {
                 "User-Agent": useragent,
```

### Comparing `spyder_ml-2.1.3/spyderml/lib/spidercrawler.py` & `spyder_ml-2.1.4/spyderml/src/spidercrawler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import sys
 import threading
 import queue
-
 import requests
 
 from bs4 import XMLParsedAsHTMLWarning, BeautifulSoup as Bs
 from colorama import Fore, Style
-from spyderml.lib.file import save_output
+from spyderml.src.file import save_output
 
 
 def request(url):
     try:
         response = requests.get(url, timeout=5, allow_redirects=True)
-
         html = response.text
         return html
     except requests.exceptions.MissingSchema:
         pass
     except requests.exceptions.ReadTimeout:
         pass
+    except requests.exceptions.InvalidSchema:
+        pass
     except requests.exceptions.ConnectTimeout:
         pass
     except requests.exceptions.SSLError:
         pass
     except requests.exceptions.ConnectionError:
         pass
 
@@ -32,44 +32,55 @@
     urls = set([a['href'] for a in soup.find_all('a', href=True)])
     print(f"{Fore.BLUE}[*]{Style.RESET_ALL} URLs encontradas: {len(urls)}")
     for url in urls:
         try:
             response = requests.get(url=url, timeout=10, allow_redirects=True)
             if 200 <= response.status_code < 300:
                 print(
-                    f"\t{Fore.BLUE}[+]{Style.RESET_ALL} {url} <{Fore.GREEN}{response.status_code}{Style.RESET_ALL}>" +
-                    f"\tSize: <{len(response.content)}>")
+                    f"\t{Fore.BLUE}[+]{Style.RESET_ALL} {url} "
+                    + f"<{Fore.GREEN}{response.status_code}{Style.RESET_ALL}>"
+                    + f"\tSize: <{len(response.content)}>")
             elif 300 <= response.status_code < 400:
                 print(
-                    f"\t{Fore.YELLOW}[!]{Style.RESET_ALL} {url} <{Fore.YELLOW}{response.status_code}{Style.RESET_ALL}>"
+                    f"\t{Fore.YELLOW}[!]{Style.RESET_ALL} {url} "
+                    + f"<{Fore.YELLOW}{response.status_code}{Style.RESET_ALL}>"
                     + f"\tSize: <{len(response.content)}>")
             elif 400 <= response.status_code < 500:
                 print(
-                    f"\t{Fore.RED}[-]{Style.RESET_ALL} {url} <{Fore.RED}{response.status_code}{Style.RESET_ALL}>"
+                    f"\t{Fore.RED}[-]{Style.RESET_ALL} {url} "
+                    + f"<{Fore.RED}{response.status_code}{Style.RESET_ALL}>"
                     + f"\tSize: <{len(response.content)}>")
             elif 500 <= response.status_code <= 504:
                 print(
-                    f"\t{Fore.YELLOW}[!]{Style.RESET_ALL} {url} <{Fore.CYAN}{response.status_code}{Style.RESET_ALL}>"
+                    f"\t{Fore.YELLOW}[!]{Style.RESET_ALL} {url} "
+                    + f"<{Fore.CYAN}{response.status_code}{Style.RESET_ALL}>"
                     + f"\tSize: <{len(response.content)}>")
             else:
                 print(
-                    f"\t{Fore.YELLOW}[?]{Style.RESET_ALL} {url}<{response.status_code}>"
+                    f"\t{Fore.YELLOW}[?]{Style.RESET_ALL} {url}"
+                    + f"<{response.status_code}>"
                     + f"\tSize: <{len(response.content)}>")
 
         except requests.exceptions.MissingSchema:
             pass
         except requests.exceptions.SSLError:
-            print(f"\t{Fore.RED}[-]{Style.RESET_ALL} {url} <{Fore.RED}SSL Error{Style.RESET_ALL}>")
+            print(
+                f"\t{Fore.RED}[-]{Style.RESET_ALL} {url} "
+                + f"<{Fore.RED}SSL Error{Style.RESET_ALL}>")
         except requests.exceptions.ConnectTimeout:
-            print(f"\t{Fore.RED}[-]{Style.RESET_ALL} {url} <{Fore.RED}Timeout{Style.RESET_ALL}>")
+            print(
+                f"\t{Fore.RED}[-]{Style.RESET_ALL} {url} "
+                + f"<{Fore.RED}Timeout{Style.RESET_ALL}>")
         except Exception as e:
             if "javascript:void(0)" in str(response.content):
                 continue
             else:
-                print(f"\n\t{Fore.RED}ERROR:{Style.RESET_ALL} {url} <{Fore.RED}{e}{Style.RESET_ALL}>\n")
+                print(
+                    f"\n\t{Fore.RED}ERROR:{Style.RESET_ALL} {url} "
+                    + f"<{Fore.RED}{e}{Style.RESET_ALL}>\n")
 
         else:
             if file is not None:
                 save_output(filename=file, text=url)
 
 
 def get_links(html, domain):
@@ -109,19 +120,20 @@
     def send_request(self):
         while True:
             try:
                 url = self.to_crawl.get_nowait()
             except queue.Empty:
                 break
             try:
-                html= request(url=url)
+                html = request(url=url)
                 links = get_links(html=html, domain=self.domain)
                 if links:
                     for link in links:
-                        if link not in self.crawled and link not in self.to_crawl.queue:
+                        if link not in self.crawled and \
+                                link not in self.to_crawl.queue:
                             self.to_crawl.put(link)
 
                 if self.filepath is not None:
                     save_output(filename=self.filepath, text=url)
                 print(f"[{Fore.BLUE}+{Style.RESET_ALL}] {url}")
             except KeyboardInterrupt:
                 print("\nClossing....\n")
```

### Comparing `spyder_ml-2.1.3/spyderml/lib/spyder_reqs.py` & `spyder_ml-2.1.4/spyderml/src/spyder_reqs.py`

 * *Files identical despite different names*

### Comparing `spyder_ml-2.1.3/spyderml/lib/utils.py` & `spyder_ml-2.1.4/spyderml/src/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-import logging
 import json
 from urllib.parse import urljoin
 
-import requests
-import urllib3
 import webtech
 from bs4 import BeautifulSoup as Bs
 from bs4 import Comment
 from colorama import Fore, Style
 
-from spyderml.lib.file import save_output
+from spyderml.src.file import save_output
 
 
-def treat_objects(objects: str):
+def treat_objects(objects):
     if "," in objects:
         objects = objects.split(',')
         return objects
     return objects
 
 
 def update_database():
@@ -34,15 +31,17 @@
         techs = report['tech']
         if filepath is not None:
             save_output(filename=filepath, text=f"\nSite: {url} technologies:")
         print("Site: {} technologies:".format(url))
 
         for tech in techs:
             if filepath is not None:
-                save_output(filename=filepath, text=f"Name: {tech['name']}\tVersion: {tech['version']}")
+                save_output(
+                    filename=filepath, text=f"Name: {tech['name']}\tVersion: "
+                    + f"{tech['version']}")
             print(f'''{tech['version']}
             ''')
         print('\n')
     except webtech.utils.ConnectionException:
         print("Connection error")
 
 
@@ -102,22 +101,31 @@
     print(json.dumps(json_content, indent=4))
 
 
 def print_headers(headers_dict_list, filenane=None):
     if filenane is not None:
         for index, headers_dict in enumerate(headers_dict_list):
             if index == 0:
-                save_output(filename=filenane, text="------------Request Headers-----------")
+                save_output(filename=filenane,
+                            text="------------Request Headers-----------")
             elif index == 1:
-                save_output(filename=filenane, text="------------Response Headers-----------")
+                save_output(filename=filenane,
+                            text="------------Response Headers-----------")
             for key in headers_dict:
-                save_output(filename=filenane, text=f"{key}: {headers_dict[key]}")
+                save_output(filename=filenane,
+                            text=f"{key}: {headers_dict[key]}")
             save_output(filename=filenane, text="-"*39+"\n")
     for index, headers_dict in enumerate(headers_dict_list):
         if index == 0:
-            print(f"------------{Fore.CYAN}Request Headers{Style.RESET_ALL}-----------")
+            print(
+                f"------------{Fore.CYAN}Request Headers{Style.RESET_ALL}"
+                + "-----------")
         elif index == 1:
-            print(f"------------{Fore.CYAN}Response Headers{Style.RESET_ALL}-----------")
+            print(
+                f"------------{Fore.CYAN}Response Headers{Style.RESET_ALL}"
+                + "-----------")
         for key in headers_dict.keys():
-            print(f"{Fore.LIGHTMAGENTA_EX}{key}{Style.RESET_ALL}: {headers_dict[key]}")
+            print(
+                f"{Fore.LIGHTMAGENTA_EX}{key}{Style.RESET_ALL}: "
+                + f"{headers_dict[key]}")
 
         print("-"*39+"\n")
```

### Comparing `spyder_ml-2.1.3/spyderml/main.py` & `spyder_ml-2.1.4/spyderml/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import argparse
 import sys
 import argcomplete
 
-from spyderml.lib import spyder_reqs
-from spyderml.lib.asciiarts import banner
-from spyderml.lib.handle_headers_and_proxy import handle_headers, handle_proxy, handle_data
-from spyderml.lib.spidercrawler import get_all_urls, WebCrawling
-from spyderml.lib.utils import treat_objects, soup_tags, soup_comments, soup_attrs, get_js, \
-    detect_technologies, update_database, print_html, json_response, print_headers
-from spyderml.lib.file import open_file
+from spyderml.src import spyder_reqs
+from spyderml.src.asciiarts import banner
+from spyderml.src.handle_headers_and_proxy import handle_headers,\
+    handle_proxy, handle_data
+from spyderml.src.spidercrawler import get_all_urls, WebCrawling
+from spyderml.src.utils import treat_objects, soup_tags,\
+    soup_comments, soup_attrs, get_js, \
+    detect_technologies, update_database, print_html,\
+    json_response, print_headers
 
+'''
 sys.stdin.reconfigure(encoding='utf-8')
 sys.stdout.reconfigure(encoding='utf-8')
-
+'''
 
 # Classe que trata os argumentos passados pela função main()
+
+
 class TreatArguments:
     def __init__(self, args):
         self.args = args
 
     # Método que trata e define a ação que será tratada pela aplicação
     def run(self):
         print(banner())
@@ -32,120 +37,155 @@
         data = handle_data(self.args['data'])
         try:
             if self.args['update']:
                 update_database()
 
             else:
                 if headers is not None:
-                    spyder_request = spyder_reqs.Cacherequest(life=60, cache=self.args['cache'],
+                    spyder_request = spyder_reqs.Cacherequest(life=60,
+                                                              cache=self.args[
+                                                                  'cache'],
                                                               proxy=proxy,
                                                               headers=headers)
                     if self.args['tr'].lower() == 'post':
                         spyder_request.post(url=self.args['target'], data=data)
                     elif self.args['tr'].lower() == 'get':
                         spyder_request.get(url=self.args['target'])
                     html_document = spyder_request.text
                 else:
-                    spyder_request = spyder_reqs.Cacherequest(life=60, cache=self.args['cache'],
+                    spyder_request = spyder_reqs.Cacherequest(life=60,
+                                                              cache=self.args[
+                                                                  'cache'],
                                                               proxy=proxy)
                     if self.args['tr'].lower() == 'post':
                         spyder_request.post(url=self.args['target'], data=data)
                     elif self.args['tr'].lower() == 'get':
                         spyder_request.get(url=self.args['target'])
                     html_document = spyder_request.text
 
                 if self.args['tags']:
                     tags = treat_objects(objects=self.args['tags'])
-                    soup_tags(document=html_document, object=tags, file=self.args['output'])
+                    soup_tags(document=html_document, object=tags,
+                              file=self.args['output'])
                 elif self.args['comments']:
-                    soup_comments(document=html_document, file=self.args['output'])
+                    soup_comments(document=html_document,
+                                  file=self.args['output'])
                 elif self.args['getjs']:
-                    get_js(url=self.args['target'], document=html_document, file=self.args['output'])
+                    get_js(
+                        url=self.args['target'], document=html_document,
+                        file=self.args['output'])
                 elif self.args['techs']:
-                    detect_technologies(url=self.args['target'], filepath=self.args['output'])
+                    detect_technologies(
+                        url=self.args['target'], filepath=self.args['output'])
                 elif self.args['geturls']:
                     if self.args['spider']:
-                        wc = WebCrawling(permission=self.args['spider'], workers=self.args['workers'],
-                                         filepath=self.args['output'], domain=self.args['domain'])
+                        wc = WebCrawling(permission=self.args['spider'],
+                                         workers=self.args['workers'],
+                                         filepath=self.args['output'],
+                                         domain=self.args['domain'])
                         wc.pre_queue_to_crawling(url=self.args['target'])
                     else:
-                        get_all_urls(document=html_document, file=self.args['output'])
+                        get_all_urls(document=html_document,
+                                     file=self.args['output'])
                 elif self.args['html']:
-                    print_html(document=html_document, file=self.args['output'])
+                    print_html(document=html_document,
+                               file=self.args['output'])
                 elif self.args['jsr']:
-                    json_response(document=html_document, file=self.args['output'])
+                    json_response(document=html_document,
+                                  file=self.args['output'])
 
                 elif self.args['attribs']:
                     attr = treat_objects(objects=self.args['attribs'])
-                    soup_attrs(document=html_document, object=attr, file=self.args['output'])
+                    soup_attrs(document=html_document, object=attr,
+                               file=self.args['output'])
                 else:
-                    spyder_request.response_and_request_headers(url=self.args['target'])
-                    print_headers(spyder_request.headers_text, filenane=self.args['output'])
+                    spyder_request.response_and_request_headers(
+                        url=self.args['target'])
+                    print_headers(spyder_request.headers_text,
+                                  filenane=self.args['output'])
         except KeyboardInterrupt:
             print("\nClossing...\n")
             sys.exit(0)
 
 
 # Passando os argumentos de linha de comando com o argparse
 def main():
-    parser = argparse.ArgumentParser(description="A tool made to facilitate the analysis of html code.")
+    parser = argparse.ArgumentParser(
+        description="A tool made to facilitate the analysis of html code.")
 
     group_target = parser.add_mutually_exclusive_group()
 
     group_action = parser.add_mutually_exclusive_group()
 
-    group_target.add_argument('-t', '--target', type=str, help="Parameter that defines the target URL "
-                                                               "http://example.com/index.html")
+    group_target.add_argument('-t', '--target', type=str, help="Parameter that"
+                              + " defines the target URL "
+                              + "http://example.com/index.html")
     parser.add_argument('--tr', type=str, default="GET",
                         help='Type of request.')
-    group_target.add_argument('--update', help='Flag responsible for updating the database.',
+    group_target.add_argument('--update', help='Flag responsible for '
+                              + 'updating the database.',
                               default=False, action='store_true')
-    group_action.add_argument('--tags', type=str, help="Flag that defines which tags the program will bring")
-
-    group_action.add_argument('--comments', help="Flag that brings the comments", default=False, action='store_true', )
+    group_action.add_argument(
+        '--tags', type=str, help="Flag that defines which tags the"
+        + " program will bring")
+
+    group_action.add_argument(
+        '--comments', help="Flag that brings the comments",
+        default=False, action='store_true', )
 
     group_action.add_argument('--attribs', type=str,
-                              help="Flag that defines which attributes the application will look for.")
+                              help="Flag that defines which "
+                              + "attributes the application will look for.")
 
-    group_action.add_argument('--getjs', help='Flag that brings all JS files from the page.',
+    group_action.add_argument('--getjs', help='Flag that brings all JS files '
+                              + 'from the page.',
                               default=False, action='store_true')
-    group_action.add_argument('--techs', help='Flag trying to discover the technologies of the page.',
+    group_action.add_argument('--techs', help='Flag trying to discover '
+                              + 'the technologies of the page.',
                               default=False, action='store_true')
-    group_action.add_argument('--geturls', help='This flag takes all the target\'s urls and tries to access them.',
+    group_action.add_argument('--geturls', help='This flag takes all '
+                              + 'the target\'s urls and tries to access them.',
                               default=False, action='store_true')
 
-    group_action.add_argument('--html', help='This Flag results in all the page\'s html code.',
+    group_action.add_argument('--html', help='This Flag results in '
+                              + 'all the page\'s html code.',
                               default=False, action='store_true')
     group_action.add_argument('--jsr', action='store_true', default=False,
                               help="Makes a request that returns a JSON.")
     parser.add_argument('-o', '--output', type=str,
-                        help="Flag that defines in which file the command output will be "
+                        help="Flag that defines in which file "
+                        + "the command output will be "
                              "saved.")
-    parser.add_argument('-C', '--cookie', type=str, help="Cookie to send with the request",
+    parser.add_argument('-C', '--cookie', type=str, help="Cookie to send "
+                        + "with the request",
                         default=None)
-    parser.add_argument('-A', '--agent', type=str, help="User-Agent to send with the request",
+    parser.add_argument('-A', '--agent', type=str, help="User-Agent to send "
+                        + "with the request",
                         default=None)
     parser.add_argument('-hf', '--headersfile', type=str, default=None,
                         help="Parameter that passes an HTTP request"
                              + " header file to be scanned.")
 
     parser.add_argument('-S', '--spider', action='store_true',
                         help='flag to run spider', default=False)
 
     parser.add_argument('-w', '--workers', type=int, default=4,
                         help="Defines the number of workers.")
     parser.add_argument('--domain', type=str, default=None,
                         help="Defines the domain of the web crawler.")
     parser.add_argument('--cache', action='store_true', default=False,
-                        help="Defines whether to create cache or not (default: false).")
+                        help="Defines whether to create cache or "
+                        + "not (default: false).")
     parser.add_argument('--proxy', type=str, default=None,
-                        help="Defines the proxy that will be used (Which can be passed tor or burpsuite to use these"
+                        help="Defines the proxy that will be used "
+                        + "(Which can be passed tor or burpsuite to use these"
                              + " two default proxies).")
     parser.add_argument('-D', '--data', nargs='+',
-                        help="Data to send with the request in format key1:value1 key2:value2 key3:value3...")
+                        help="Data to send with the request in format "
+                        + "key1:value1 key2:value2 key3:value3...")
 
     argcomplete.autocomplete(parser)
 
     args = vars(parser.parse_args())
 
     if not any(args.values()):
         parser.error('No arguments provided.')
@@ -153,21 +193,25 @@
     if not args['target'] and not args['update']:
         parser.error('No url the file with defined urls.')
         sys.exit(0)
     if args['spider'] and not args['geturls']:
         parser.error('--spider can only be used with --geturls')
         sys.exit(0)
     if args['agent'] and args['cookie'] and args['headersfile']:
-        parser.error("The arguments --cookie, --agent --headers file cannot be used together.")
+        parser.error(
+            "The arguments --cookie, --agent --headers "
+            + "file cannot be used together.")
         sys.exit(0)
     if args['agent'] and args['headersfile']:
-        parser.error("The arguments --agent, --headers file cannot be used together.")
+        parser.error(
+            "The arguments --agent, --headers file cannot be used together.")
         sys.exit(0)
     if args['cookie'] and args['headersfile']:
-        parser.error("The arguments --cookie, --headers file cannot be used together.")
+        parser.error(
+            "The arguments --cookie, --headers file cannot be used together.")
         sys.exit(0)
     sp = TreatArguments(args)
     sp.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `spyder_ml-2.1.3/PKG-INFO` & `spyder_ml-2.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyder-ml
-Version: 2.1.3
+Version: 2.1.4
 Summary: A tool made to facilitate the analysis of html code.
 Home-page: https://github.com/accessmaker/Spyder-ml
 License: MIT
 Author: Lucas dSilva
 Author-email: accessmaker.mlbb@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,58 +16,55 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argcomplete (>=2.0.5,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: types-requests (>=2.28.11.17,<3.0.0.0)
 Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
 Requires-Dist: webtech (>=1.3.2,<2.0.0)
 Project-URL: Repository, https://github.com/accessmaker/Spyder-ml
 Description-Content-Type: text/markdown
 
 <h1 align="center">Spyder-HTML</h1>
 
 <p align="center">
 <img src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge"/>
-<img src="http://img.shields.io/static/v1?label=VERSION&message=2.1.3&color=blue&style=for-the-badge"/>
+<img src="http://img.shields.io/static/v1?label=VERSION&message=2.1.4&color=blue&style=for-the-badge"/>
 <img src="https://img.shields.io/github/license/accessmaker/Spyder-ml?style=for-the-badge"/>
 </p>
 
-
 A tool made to facilitate the analysis of html code.
 
 <h2>INSTALL(git clone):</h2>
 
-git clone https://github.com/accessmaker/Spyder-ml
+git clone <https://github.com/accessmaker/Spyder-ml>
 
 python setup.py install
 
-
 <h2>INSTALL(PIP):</h2>
 
-
 pip install spyder-ml
 
-
 <h2>USAGE:</h2>
 
 spyderml       [-h] [-t TARGET] [--tr TR] [--update]
                [--tags TAGS | --comments | --attribs ATTRIBS | --getjs | --techs | --geturls | --html | --jsr]
                [-o OUTPUT] [-C COOKIE] [-A AGENT] [-hf HEADERSFILE] [-S]
                [-w WORKERS] [--domain DOMAIN] [--cache] [--proxy PROXY]
                [-D DATA [DATA ...]]
 
 A tool made to facilitate the analysis of html code.
 
 options:<br>
   -h, --help            show this help message and exit<br>
   -t TARGET, --target TARGET<br>
                         Parameter that defines the target URL<
-                        http://example.com/index.html <br>
+                        <http://example.com/index.html> <br>
   --tr TR               Type of request(POST or GET(Default)).
   --update              Flag responsible for updating the database.<br>
   --tags TAGS           Flag that defines which tags the program will bring<br>
   --comments            Flag that brings the comments<br>
   --attribs ATTRIBS     Flag that defines which attributes the application
                         will look for.<br>
   --getjs               Flag that brings all JS files from the page.<br>
@@ -96,7 +93,8 @@
                         passed tor or burpsuite to use these two default
                         proxies).<br>
   -D DATA [DATA ...], --data DATA [DATA ...]
                         Data to send with the request in format key1:value1
                         key2:value2 key3:value3...<br>
 
 'Functionality': It searches the html document for specific things
+
```

