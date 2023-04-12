# Comparing `tmp/httpmdhtml-0.0.6.tar.gz` & `tmp/httpmdhtml-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpmdhtml-0.0.6.tar", last modified: Tue Apr  4 17:09:57 2023, max compression
+gzip compressed data, was "httpmdhtml-0.0.7.tar", last modified: Wed Apr 12 16:15:13 2023, max compression
```

## Comparing `httpmdhtml-0.0.6.tar` & `httpmdhtml-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-04 17:09:57.674628 httpmdhtml-0.0.6/
--rwxrwxrwx   0 john      (1000) john      (1000)    35147 2023-02-20 18:24:08.000000 httpmdhtml-0.0.6/LICENSE.txt
--rwxrwxrwx   0 john      (1000) john      (1000)     3263 2023-04-04 17:09:57.676154 httpmdhtml-0.0.6/PKG-INFO
--rwxrwxrwx   0 john      (1000) john      (1000)     2822 2023-03-15 14:36:40.000000 httpmdhtml-0.0.6/README.md
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-04 17:09:57.639737 httpmdhtml-0.0.6/httpmdhtml/
--rwxrwxrwx   0 john      (1000) john      (1000)        0 2023-02-20 16:50:45.000000 httpmdhtml-0.0.6/httpmdhtml/__init__.py
--rwxrwxrwx   0 john      (1000) john      (1000)     2945 2023-04-04 17:06:28.000000 httpmdhtml-0.0.6/httpmdhtml/md_to_html.py
--rwxrwxrwx   0 john      (1000) john      (1000)     4025 2023-03-15 15:03:03.000000 httpmdhtml-0.0.6/httpmdhtml/server.py
-drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-04 17:09:57.669514 httpmdhtml-0.0.6/httpmdhtml.egg-info/
--rwxrwxrwx   0 john      (1000) john      (1000)     3263 2023-04-04 17:09:57.000000 httpmdhtml-0.0.6/httpmdhtml.egg-info/PKG-INFO
--rwxrwxrwx   0 john      (1000) john      (1000)      293 2023-04-04 17:09:57.000000 httpmdhtml-0.0.6/httpmdhtml.egg-info/SOURCES.txt
--rwxrwxrwx   0 john      (1000) john      (1000)        1 2023-04-04 17:09:57.000000 httpmdhtml-0.0.6/httpmdhtml.egg-info/dependency_links.txt
--rwxrwxrwx   0 john      (1000) john      (1000)       39 2023-04-04 17:09:57.000000 httpmdhtml-0.0.6/httpmdhtml.egg-info/requires.txt
--rwxrwxrwx   0 john      (1000) john      (1000)       11 2023-04-04 17:09:57.000000 httpmdhtml-0.0.6/httpmdhtml.egg-info/top_level.txt
--rwxrwxrwx   0 john      (1000) john      (1000)      100 2023-03-13 22:32:33.000000 httpmdhtml-0.0.6/pyproject.toml
--rwxrwxrwx   0 john      (1000) john      (1000)       78 2023-04-04 17:09:57.682026 httpmdhtml-0.0.6/setup.cfg
--rwxrwxrwx   0 john      (1000) john      (1000)      923 2023-04-04 17:07:55.000000 httpmdhtml-0.0.6/setup.py
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-12 16:15:13.398821 httpmdhtml-0.0.7/
+-rwxrwxrwx   0 john      (1000) john      (1000)    35147 2023-04-04 17:12:07.000000 httpmdhtml-0.0.7/LICENSE.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)     3454 2023-04-12 16:15:13.398821 httpmdhtml-0.0.7/PKG-INFO
+-rwxrwxrwx   0 john      (1000) john      (1000)     3017 2023-04-12 16:08:23.000000 httpmdhtml-0.0.7/README.md
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-12 16:15:13.373373 httpmdhtml-0.0.7/httpmdhtml/
+-rwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-04 17:12:07.000000 httpmdhtml-0.0.7/httpmdhtml/__init__.py
+-rwxrwxrwx   0 john      (1000) john      (1000)     3380 2023-04-12 16:04:24.000000 httpmdhtml-0.0.7/httpmdhtml/md_to_html.py
+-rwxrwxrwx   0 john      (1000) john      (1000)     4382 2023-04-12 16:08:29.000000 httpmdhtml-0.0.7/httpmdhtml/server.py
+drwxrwxrwx   0 john      (1000) john      (1000)        0 2023-04-12 16:15:13.396248 httpmdhtml-0.0.7/httpmdhtml.egg-info/
+-rwxrwxrwx   0 john      (1000) john      (1000)     3454 2023-04-12 16:15:13.000000 httpmdhtml-0.0.7/httpmdhtml.egg-info/PKG-INFO
+-rwxrwxrwx   0 john      (1000) john      (1000)      293 2023-04-12 16:15:13.000000 httpmdhtml-0.0.7/httpmdhtml.egg-info/SOURCES.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)        1 2023-04-12 16:15:13.000000 httpmdhtml-0.0.7/httpmdhtml.egg-info/dependency_links.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)       39 2023-04-12 16:15:13.000000 httpmdhtml-0.0.7/httpmdhtml.egg-info/requires.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)       11 2023-04-12 16:15:13.000000 httpmdhtml-0.0.7/httpmdhtml.egg-info/top_level.txt
+-rwxrwxrwx   0 john      (1000) john      (1000)      100 2023-04-04 17:12:07.000000 httpmdhtml-0.0.7/pyproject.toml
+-rwxrwxrwx   0 john      (1000) john      (1000)       78 2023-04-12 16:15:13.401649 httpmdhtml-0.0.7/setup.cfg
+-rwxrwxrwx   0 john      (1000) john      (1000)      923 2023-04-12 15:52:38.000000 httpmdhtml-0.0.7/setup.py
```

### Comparing `httpmdhtml-0.0.6/LICENSE.txt` & `httpmdhtml-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `httpmdhtml-0.0.6/PKG-INFO` & `httpmdhtml-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: httpmdhtml
-Version: 0.0.6
+Version: 0.0.7
 Summary: HTTP server that converts markdown to HTML
 Home-page: https://github.com/treatmesubj/python-md-to-html-server
-Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.6.tar.gz
+Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.7.tar.gz
 Author: John Hupperts
 Author-email: jrock4503@hotmail.com
 License: gpl-3.0
 Project-URL: Source, https://github.com/treatmesubj/python-md-to-html-server
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -24,29 +24,33 @@
 ## Installation
 - from [PyPI](https://pypi.org/project/httpmdhtml/): `pip install httpmdhtml`
 - from [GitHub](https://github.com/treatmesubj/python-md-to-html-server): `pip install "git+https://github.com/treatmesubj/python-md-to-html-server"`
 
 ## Usage
 ### Markdown-to-HTML Server
 ```
-python -m httpmdhtml.server -b 127.0.0.1 -d . --css_file ../mystyle.css
+python -m httpmdhtml.server -b 127.0.0.1 -d . --css_file ../mystyle.css -l 5000
 ---
-usage: server.py [-h] [--cgi] [--bind ADDRESS] [--directory DIRECTORY] [--css_file CSS_FILE] [port]
+usage: server.py [-h] [--cgi] [--bind ADDRESS] [--directory DIRECTORY] [--css_file CSS_FILE]
+                 [--live_md_rr LIVE_MD_RR]
+                 [port]
 
 positional arguments:
   port                  Specify alternate port [default: 8000]
 
 optional arguments:
   -h, --help            show this help message and exit
   --cgi                 Run as CGI Server
   --bind ADDRESS, -b ADDRESS
                         Specify alternate bind address [default: all interfaces]
   --directory DIRECTORY, -d DIRECTORY
                         Specify alternative directory [default:current directory]
   --css_file CSS_FILE   css-file-path; its content will be written to the <style> element
+  --live_md_rr LIVE_MD_RR, -l LIVE_MD_RR
+                        Continuous refresh rate of MD page, in ms. Respects cache
 ```
 
 ### Markdown-to-HTML Out-File
 ```
 python -m httpmdhtml.md_to_html -i in_file.md -o out_file.html --encode_local_images
 ---
 usage: md_to_html.py [-h] [--in_file_path IN_FILE_PATH] [--out_file_path OUT_FILE_PATH] [--encode_local_images]
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_l72aizk__/tmp3e5jle04_TarContainer/0/2", line 67, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_l72aizk__/tmp3e5jle04_TarContainer/0/2", line 67, column 0: CDATA terminal not found*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: httpmdhtml Version: 0.0.6 Summary: HTTP server that
+Metadata-Version: 2.1 Name: httpmdhtml Version: 0.0.7 Summary: HTTP server that
 converts markdown to HTML Home-page: https://github.com/treatmesubj/python-md-
 to-html-server Download-URL: https://github.com/treatmesubj/python-md-to-html-
-server/archive/refs/tags/v0.0.6.tar.gz Author: John Hupperts Author-email:
+server/archive/refs/tags/v0.0.7.tar.gz Author: John Hupperts Author-email:
 jrock4503@hotmail.com License: gpl-3.0 Project-URL: Source, https://github.com/
 treatmesubj/python-md-to-html-server Description-Content-Type: text/markdown
 License-File: LICENSE.txt # Python Markdown-to-HTML Server It's the standard
 Python [http.server module](https://docs.python.org/3/library/http.server.html)
 but via [markdown-it-py](https://github.com/executablebooks/markdown-it-py),
 requested Markdown files are rendered and served as HTML The `http.server`
 module's `SimpleHTTPRequestHandler` class is inherited by a new class with its
```

### Comparing `httpmdhtml-0.0.6/README.md` & `httpmdhtml-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,33 @@
 ## Installation
 - from [PyPI](https://pypi.org/project/httpmdhtml/): `pip install httpmdhtml`
 - from [GitHub](https://github.com/treatmesubj/python-md-to-html-server): `pip install "git+https://github.com/treatmesubj/python-md-to-html-server"`
 
 ## Usage
 ### Markdown-to-HTML Server
 ```
-python -m httpmdhtml.server -b 127.0.0.1 -d . --css_file ../mystyle.css
+python -m httpmdhtml.server -b 127.0.0.1 -d . --css_file ../mystyle.css -l 5000
 ---
-usage: server.py [-h] [--cgi] [--bind ADDRESS] [--directory DIRECTORY] [--css_file CSS_FILE] [port]
+usage: server.py [-h] [--cgi] [--bind ADDRESS] [--directory DIRECTORY] [--css_file CSS_FILE]
+                 [--live_md_rr LIVE_MD_RR]
+                 [port]
 
 positional arguments:
   port                  Specify alternate port [default: 8000]
 
 optional arguments:
   -h, --help            show this help message and exit
   --cgi                 Run as CGI Server
   --bind ADDRESS, -b ADDRESS
                         Specify alternate bind address [default: all interfaces]
   --directory DIRECTORY, -d DIRECTORY
                         Specify alternative directory [default:current directory]
   --css_file CSS_FILE   css-file-path; its content will be written to the <style> element
+  --live_md_rr LIVE_MD_RR, -l LIVE_MD_RR
+                        Continuous refresh rate of MD page, in ms. Respects cache
 ```
 
 ### Markdown-to-HTML Out-File
 ```
 python -m httpmdhtml.md_to_html -i in_file.md -o out_file.html --encode_local_images
 ---
 usage: md_to_html.py [-h] [--in_file_path IN_FILE_PATH] [--out_file_path OUT_FILE_PATH] [--encode_local_images]
```

### Comparing `httpmdhtml-0.0.6/httpmdhtml/md_to_html.py` & `httpmdhtml-0.0.7/httpmdhtml/md_to_html.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,33 +8,40 @@
 import argparse
 import re
 from markdown_it import MarkdownIt
 from bs4 import BeautifulSoup, element
 
 
 def markdown_to_html(MarkdownIt_obj, in_file_path, out_file_path="tmp.html",
-        encode_local_images=False, css_file=None):
+        encode_local_images=False, css_file=None, live_md_rr=None):
 
     text = open(in_file_path, "r").read()
     tokens = MarkdownIt_obj.parse(text)
     html_text = MarkdownIt_obj.render(text)
     # pretty CSS
     soup = BeautifulSoup(html_text, 'html5lib') # adds <html>, <head>,  <body>
     soup.select_one('head').append(soup.new_tag("meta"))
     soup.select_one('meta').attrs['charset'] = "UTF-8"
+    # if lots of images, caching is preferable more often than not
+    # soup.select_one('meta').attrs['http-equiv'] = "Cache-control"
+    # soup.select_one('meta').attrs['content'] = "no-cache"
     soup.select_one('head').append(soup.new_tag("style"))
     if css_file:
         with open(css_file, 'r') as f:
             css=f.read()
     else:
         css="""body { background-color: #272822; color: white; font-family: Courier; }
         a[href] { color: #66d9ef; }
         code { color: #ae81ff; background-color: #272b33; border-radius: 6px; }
         table, th, td { border: 1px solid; border-collapse: collapse; padding-left: 4px; padding-right: 4px; }"""
     soup.select_one("style").string = css
+    if live_md_rr:
+        script = f"setTimeout(function(){{ document.location.reload(); }}, {live_md_rr});"
+        soup.select_one('head').append(soup.new_tag("script"))
+        soup.select_one("script").string = script
     if encode_local_images:
         img_elems = soup.select("img")
         url_pattern = "^https?:\\/\\/(?:www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b(?:[-a-zA-Z0-9()@:%_\\+.~#?&\\/=]*)$"
         for img in img_elems:
             if not re.match(url_pattern, img.attrs['src']):
                 img_path = os.path.join(os.path.dirname(in_file_path), img.attrs['src'])
                 with open(img_path, "rb") as image_obj:
```

### Comparing `httpmdhtml-0.0.6/httpmdhtml/server.py` & `httpmdhtml-0.0.7/httpmdhtml/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,31 +27,33 @@
 
 from bs4 import BeautifulSoup, element
 
 from httpmdhtml import md_to_html
 
 
 class md_to_html_SimpleHTTPRequestHandler(SimpleHTTPRequestHandler):
-    def __init__(self, *args, MarkdownIt_obj=None, css_file=None, **kwargs):
+    def __init__(self, *args, MarkdownIt_obj=None, css_file=None, live_md_rr=False, **kwargs):
         self.MarkdownIt_obj = MarkdownIt_obj
         self.css_file = css_file
+        self.live_md_rr = live_md_rr
         super().__init__(*args, **kwargs)
 
 
     def do_GET(self, rm_temp_html=False):
         """Serve a GET request."""
         self.url_dc_path = urllib.parse.unquote(urllib.parse.urlsplit(self.path).path)  # url decode, strip query params for file check
-        if self.url_dc_path.endswith(".md") and os.path.exists(os.path.join(self.directory, f".{self.url_dc_path}")):  # check for markdown file request
+        if self.MarkdownIt_obj and self.url_dc_path.endswith(".md") and os.path.exists(os.path.join(self.directory, f".{self.url_dc_path}")):  # check for markdown file request
             in_file_path=os.path.join(self.directory, f".{self.url_dc_path}")
             out_file_path=os.path.join(self.directory, f".{os.path.splitext(self.url_dc_path)[0]}.html")
             md_to_html.markdown_to_html(
                     self.MarkdownIt_obj,
                     in_file_path=in_file_path,
                     out_file_path=out_file_path,
-                    css_file=self.css_file)
+                    css_file=self.css_file,
+                    live_md_rr=self.live_md_rr)
             self.path = f"{os.path.splitext(self.path)[0]}.html"
             rm_temp_html = True
         f = self.send_head()
         if f:
             try:
                 self.copyfile(f, self.wfile)
             finally:
@@ -69,29 +71,32 @@
                         help='Specify alternate bind address '
                              '[default: all interfaces]')
     parser.add_argument('--directory', '-d', default=os.getcwd(),
                         help='Specify alternative directory '
                         '[default:current directory]')
     parser.add_argument('--css_file', default=None,
                          help='css-file-path; its content will be written to the <style> element')
+    parser.add_argument('--live_md_rr', '-l', action='store', type=int, default=None,
+                         help='Continuous refresh rate of MD page, in ms. Respects cache')
     parser.add_argument('port', action='store',
                         default=8000, type=int,
                         nargs='?',
                         help='Specify alternate port [default: 8000]')
     args = parser.parse_args()
     if args.cgi:
         handler_class = CGIHTTPRequestHandler
     else:
         MarkdownIt_obj = MarkdownIt("commonmark").enable("table").enable("strikethrough")
         if args.css_file and not os.path.isfile(args.css_file):
-            raise FileNotFoundError(f"looks like the given `css_file` argument's value - {args.css_file} - is not actually a file")
+            raise FileNotFoundError(f"looks like the given `css_file` argument's value - {args.css_file} - cannot be found")
         handler_class = partial(md_to_html_SimpleHTTPRequestHandler,
                                 directory=args.directory,
                                 MarkdownIt_obj=MarkdownIt_obj,
-                                css_file=args.css_file)
+                                css_file=args.css_file,
+                                live_md_rr=args.live_md_rr)
 
     # ensure dual-stack is not disabled; ref #38907
     class DualStackServer(ThreadingHTTPServer):
         def server_bind(self):
             # suppress exception when protocol is IPv4
             with contextlib.suppress(Exception):
                 self.socket.setsockopt(
```

### Comparing `httpmdhtml-0.0.6/httpmdhtml.egg-info/PKG-INFO` & `httpmdhtml-0.0.7/httpmdhtml.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: httpmdhtml
-Version: 0.0.6
+Version: 0.0.7
 Summary: HTTP server that converts markdown to HTML
 Home-page: https://github.com/treatmesubj/python-md-to-html-server
-Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.6.tar.gz
+Download-URL: https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.7.tar.gz
 Author: John Hupperts
 Author-email: jrock4503@hotmail.com
 License: gpl-3.0
 Project-URL: Source, https://github.com/treatmesubj/python-md-to-html-server
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -24,29 +24,33 @@
 ## Installation
 - from [PyPI](https://pypi.org/project/httpmdhtml/): `pip install httpmdhtml`
 - from [GitHub](https://github.com/treatmesubj/python-md-to-html-server): `pip install "git+https://github.com/treatmesubj/python-md-to-html-server"`
 
 ## Usage
 ### Markdown-to-HTML Server
 ```
-python -m httpmdhtml.server -b 127.0.0.1 -d . --css_file ../mystyle.css
+python -m httpmdhtml.server -b 127.0.0.1 -d . --css_file ../mystyle.css -l 5000
 ---
-usage: server.py [-h] [--cgi] [--bind ADDRESS] [--directory DIRECTORY] [--css_file CSS_FILE] [port]
+usage: server.py [-h] [--cgi] [--bind ADDRESS] [--directory DIRECTORY] [--css_file CSS_FILE]
+                 [--live_md_rr LIVE_MD_RR]
+                 [port]
 
 positional arguments:
   port                  Specify alternate port [default: 8000]
 
 optional arguments:
   -h, --help            show this help message and exit
   --cgi                 Run as CGI Server
   --bind ADDRESS, -b ADDRESS
                         Specify alternate bind address [default: all interfaces]
   --directory DIRECTORY, -d DIRECTORY
                         Specify alternative directory [default:current directory]
   --css_file CSS_FILE   css-file-path; its content will be written to the <style> element
+  --live_md_rr LIVE_MD_RR, -l LIVE_MD_RR
+                        Continuous refresh rate of MD page, in ms. Respects cache
 ```
 
 ### Markdown-to-HTML Out-File
 ```
 python -m httpmdhtml.md_to_html -i in_file.md -o out_file.html --encode_local_images
 ---
 usage: md_to_html.py [-h] [--in_file_path IN_FILE_PATH] [--out_file_path OUT_FILE_PATH] [--encode_local_images]
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_l72aizk__/tmp3e5jle04_TarContainer/0/9", line 67, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_l72aizk__/tmp3e5jle04_TarContainer/0/9", line 67, column 0: CDATA terminal not found*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: httpmdhtml Version: 0.0.6 Summary: HTTP server that
+Metadata-Version: 2.1 Name: httpmdhtml Version: 0.0.7 Summary: HTTP server that
 converts markdown to HTML Home-page: https://github.com/treatmesubj/python-md-
 to-html-server Download-URL: https://github.com/treatmesubj/python-md-to-html-
-server/archive/refs/tags/v0.0.6.tar.gz Author: John Hupperts Author-email:
+server/archive/refs/tags/v0.0.7.tar.gz Author: John Hupperts Author-email:
 jrock4503@hotmail.com License: gpl-3.0 Project-URL: Source, https://github.com/
 treatmesubj/python-md-to-html-server Description-Content-Type: text/markdown
 License-File: LICENSE.txt # Python Markdown-to-HTML Server It's the standard
 Python [http.server module](https://docs.python.org/3/library/http.server.html)
 but via [markdown-it-py](https://github.com/executablebooks/markdown-it-py),
 requested Markdown files are rendered and served as HTML The `http.server`
 module's `SimpleHTTPRequestHandler` class is inherited by a new class with its
```

### Comparing `httpmdhtml-0.0.6/setup.py` & `httpmdhtml-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="httpmdhtml",
-    version="0.0.6",
+    version="0.0.7",
     license="gpl-3.0",
     author="John Hupperts",
     author_email="jrock4503@hotmail.com",
     description="HTTP server that converts markdown to HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/treatmesubj/python-md-to-html-server",
-    download_url="https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.6.tar.gz",
+    download_url="https://github.com/treatmesubj/python-md-to-html-server/archive/refs/tags/v0.0.7.tar.gz",
     packages=["httpmdhtml"],
     package_dir={"python-md-to-html-server": "httpmdhtml"},
     project_urls={
         "Source": "https://github.com/treatmesubj/python-md-to-html-server",
     },
     install_requires=[
         "markdown-it-py",
```

