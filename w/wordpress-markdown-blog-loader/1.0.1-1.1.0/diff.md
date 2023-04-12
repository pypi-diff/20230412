# Comparing `tmp/wordpress-markdown-blog-loader-1.0.1.tar.gz` & `tmp/wordpress-markdown-blog-loader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordpress-markdown-blog-loader-1.0.1.tar", last modified: Sun Feb 26 19:02:45 2023, max compression
+gzip compressed data, was "wordpress-markdown-blog-loader-1.1.0.tar", last modified: Wed Apr 12 12:24:00 2023, max compression
```

## Comparing `wordpress-markdown-blog-loader-1.0.1.tar` & `wordpress-markdown-blog-loader-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:02:45.179718 wordpress-markdown-blog-loader-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-02-26 19:02:45.179718 wordpress-markdown-blog-loader-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-02-26 19:02:09.000000 wordpress-markdown-blog-loader-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-26 19:02:45.179718 wordpress-markdown-blog-loader-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-26 19:02:09.000000 wordpress-markdown-blog-loader-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:02:45.171718 wordpress-markdown-blog-loader-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:02:45.175718 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 19:02:09.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-26 19:02:09.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-02-26 19:02:09.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-02-26 19:02:09.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-02-26 19:02:09.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-02-26 19:02:09.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/name_to_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-02-26 19:02:09.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-02-26 19:02:09.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:02:45.175718 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-02-26 19:02:45.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-26 19:02:45.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 19:02:45.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-26 19:02:45.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 19:02:22.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-26 19:02:45.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-26 19:02:45.000000 wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:24:00.846010 wordpress-markdown-blog-loader-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18268 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/check_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/name_to_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/remove_newlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:23:39.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 12:24:00.000000 wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:24:00.850010 wordpress-markdown-blog-loader-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-12 12:23:24.000000 wordpress-markdown-blog-loader-1.1.0/tests/test_blog.py
```

### Comparing `wordpress-markdown-blog-loader-1.0.1/PKG-INFO` & `wordpress-markdown-blog-loader-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-markdown-blog-loader
-Version: 1.0.1
+Version: 1.1.0
 Summary: load markdown blogs into wordpress
 Home-page: https://github.com/binxio/wordpress-markdown-blog-loader
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: APL2
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -23,14 +23,16 @@
 This utility loads markdown blogs into Wordpress as a post. It allows you to work on your blog
 in your favorite editor and keeps all your blogs in git.
 
 ## features
 - converts markdown into plain html, with syntax hightlighting support
 - uploads and synchronizes any locally referenced images
 - generates an opengraph image including the title, subtitle and author in Binx.io or xebia.com style
+- sets the Yoast focus keywords
+- sets the canonical url, if specified
 
 ## caveats
 - changing the slug may orphan images
 - removing images from the markdown, will leave dangling images in Wordpress
 
 ## required Wordpress Plugins
 
@@ -41,23 +43,24 @@
 
 ## configuration
 to configure the access credentials, you need to add your WordPress application password to the file `~/.wordpress.ini`  
 and add a section for your Wordpress installation:
 
 ```
 [DEFAULT]
-host = example.com
+host = xebia.com
 
-[example.com]
-api_host = example.wpengine.com
+[xebia.com]
 username = <your wordpress username>
 password = <your application passwoird>
 ```
 Note that the application password is different from the password you use to login to your WordPress installation.
 
+If the site is served through a CDN, you can also set the `api_host` which will be used as the hostname to invoke the WP REST API. 
+
 ## Using the image
 To use the docker image, you have to login using a GitHub container registry access token:
 
 1. Browse to https://github.com/settings/tokens
 2. Create new token with 'read:packages' permission
 3. Copy the token
 4. login to  ghcr.io with Docker.
```

### Comparing `wordpress-markdown-blog-loader-1.0.1/README.md` & `wordpress-markdown-blog-loader-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 This utility loads markdown blogs into Wordpress as a post. It allows you to work on your blog
 in your favorite editor and keeps all your blogs in git.
 
 ## features
 - converts markdown into plain html, with syntax hightlighting support
 - uploads and synchronizes any locally referenced images
 - generates an opengraph image including the title, subtitle and author in Binx.io or xebia.com style
+- sets the Yoast focus keywords
+- sets the canonical url, if specified
 
 ## caveats
 - changing the slug may orphan images
 - removing images from the markdown, will leave dangling images in Wordpress
 
 ## required Wordpress Plugins
 
@@ -20,23 +22,24 @@
 
 ## configuration
 to configure the access credentials, you need to add your WordPress application password to the file `~/.wordpress.ini`  
 and add a section for your Wordpress installation:
 
 ```
 [DEFAULT]
-host = example.com
+host = xebia.com
 
-[example.com]
-api_host = example.wpengine.com
+[xebia.com]
 username = <your wordpress username>
 password = <your application passwoird>
 ```
 Note that the application password is different from the password you use to login to your WordPress installation.
 
+If the site is served through a CDN, you can also set the `api_host` which will be used as the hostname to invoke the WP REST API. 
+
 ## Using the image
 To use the docker image, you have to login using a GitHub container registry access token:
 
 1. Browse to https://github.com/settings/tokens
 2. Create new token with 'read:packages' permission
 3. Copy the token
 4. login to  ghcr.io with Docker.
```

### Comparing `wordpress-markdown-blog-loader-1.0.1/setup.py` & `wordpress-markdown-blog-loader-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,25 @@
     "Pillow",
     "binx-og-image-generator>=1.2.5",
     "markdownify",
     "bs4",
     "html5lib",
     "lxml",
     "python-slugify",
-    "unidecode"
+    "unidecode",
+    "stopwords",
 ]
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="wordpress-markdown-blog-loader",
-    version="1.0.1",
+    version="1.1.0",
     url="https://github.com/binxio/wordpress-markdown-blog-loader",
     license="APL2",
     author="Mark van Holsteijn",
     author_email="markvanholsteijn@binx.io",
     description="load markdown blogs into wordpress",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/__main__.py` & `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import click
-from wordpress_markdown_blog_loader import upload, download, new
+from wordpress_markdown_blog_loader import upload, download, new, check_links
 
 
 @click.group()
 def main():
     """
     Wordpress CLI
     """
@@ -21,11 +21,12 @@
     """
 
 
 posts.add_command(upload.command)
 posts.add_command(download.command)
 posts.add_command(new.command)
 posts.add_command(new.update_banner_command)
+posts.add_command(check_links.command)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/api.py` & `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/api.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/blog.py` & `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/blog.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 import pytz
 from PIL import Image
 from binx_og_image_generator import generate as generate_og_image
 from binx_og_image_generator.generator import Blog as ImageGeneratorBlog
 from markdown import markdown
 from wordpress_markdown_blog_loader.api import Post, Medium
 from wordpress_markdown_blog_loader.api import Wordpress, WordpressEndpoint
+from wordpress_markdown_blog_loader.remove_newlines import (
+    remove_newlines_from_paragraphs,
+)
 
 
 class Blog(object):
     def __init__(self):
         self.dir: Path = None
         self.path: Path = None
         self.blog: frontmatter.Post = frontmatter.Post(content="")
-        self.uploaded_images: dict[str, Image] = {}
+        self.uploaded_images: dict[str, Media] = {}
         self.markdown_image_pattern = re.compile(
             r'\!\[(?P<alt_text>[^]]*)\]\((?P<url>.*?)(?P<caption>\s*"[^"]*?")?\)'
         )
 
     @staticmethod
     def load(path: str) -> "Blog":
         result = Blog()
@@ -250,15 +253,18 @@
                 caption = ""
                 if match.group("caption"):
                     caption = match.group("caption")
                 return f"![{match.group('alt_text')}]({image.url}{caption})"
             return match.group(0)
 
         content = self.markdown_image_pattern.sub(replace_references, self.content)
-        return markdown(content, extensions=["fenced_code", "attr_list", "tables"])
+        html = markdown(
+            content, extensions=["fenced_code", "attr_list", "tables", "footnotes"]
+        )
+        return remove_newlines_from_paragraphs(html)
 
     @property
     def local_image_references(self) -> set[str]:
         return set(
             map(
                 lambda u: u.path,
                 filter(
@@ -397,14 +403,17 @@
         blog.author = wordpress.get_user_by_id(post.author).name
         blog.guid = post.guid
         blog.categories = [categories[c] for c in post.categories]
         blog.date = post.date
         blog.slug = post.slug
         blog.status = post.status
         blog.brand = wordpress.endpoint.host
+        blog.canonical = post.get("yoast_head_json", {}).get(
+            "canonical", blog.canonical
+        )
 
         if post.permalink_template and not blog.permalink_template:
             # keeping the permalink template registered in the blog metadata.
             # Wordpress does not return the template that was set.
             blog.permalink_template = post.permalink_template
 
         if post.og_description:
```

### Comparing `wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/download.py` & `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/download.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/name_to_email.py` & `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/name_to_email.py`

 * *Files identical despite different names*

### Comparing `wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/new.py` & `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/new.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from urllib.request import urlopen
 from urllib.parse import urlparse
 from pathlib import Path
 from slugify import slugify
 from PIL import Image
 from wordpress_markdown_blog_loader.blog import Blog
 from wordpress_markdown_blog_loader.name_to_email import name_to_email
+import stopwords
+
 from datetime import datetime, timedelta
 import logging
 from io import BytesIO
 from pathlib import Path
 
 
 class ImageType(click.ParamType):
@@ -33,23 +35,24 @@
             self.fail("%s, cannot read image url" % value, param, ctx)
 
 
 @click.command(name="new")
 @click.option("--title", required=True, help="of the blog")
 @click.option("--subtitle", required=True, help="of the blog")
 @click.option("--author", required=True, help="of the blog")
+@click.option("--email", required=False, help="of the author")
 @click.option("--image", required=False, type=ImageType(), help="for the banner")
 @click.option(
     "--brand",
     type=click.Choice(["xebia.com", "binx.io"]),
     required=True,
     default="xebia.com",
     help="of the banner",
 )
-def command(title, subtitle, author, image, brand):
+def command(title, subtitle, author, image, brand, email):
     """
     a new frontmatter blog
 
     the index.md will be written in a subdirectory with the name of the slug for the blog.
     The slug is created from the title. The image will be resized and cropped to 1200x630.
     """
     slug = slugify(title)
@@ -60,19 +63,20 @@
 
     Path(slug).mkdir()
     blog = Blog()
     blog.dir = directory
     blog.path = directory.joinpath("index.md")
     blog.title = title
     blog.subtitle = subtitle
+    blog.focus_keywords = " ".join(stopwords.clean(title.lower().split(), "en"))
     blog.status = "draft"
     blog.slug = slug
     blog.author = author
     blog.brand = brand
-    blog.email = name_to_email(author)
+    blog.email = email if email else name_to_email(author)
     blog.date = (datetime.now().astimezone() + timedelta(days=7)).replace(
         hour=0, minute=0, second=0, microsecond=0
     )
     if image:
         image_path = save_og_image(image, directory.joinpath("images/banner"))
         blog.image = image_path.relative_to(directory).as_posix()
     blog.save()
```

### Comparing `wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader/upload.py` & `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 from difflib import diff_bytes, unified_diff
 
 import click
 
 from wordpress_markdown_blog_loader.api import Wordpress, Post
 from wordpress_markdown_blog_loader.blog import Blog
+from wordpress_markdown_blog_loader.check_links import check_links
 import sys
 
 
 def upsert_post(wp: Wordpress, blog: Blog) -> int:
 
     if blog.guid:
         if not wp.is_host_for(blog.guid):
@@ -53,14 +54,17 @@
             )
 
     if blog.image:
         banner = wp.upload_media(f"{blog.slug}-banner", blog.image_path)
         if post.featured_media != banner.medium_id:
             wp.update_post(blog.guid, {"featured_media": banner.medium_id})
 
+    broken = check_links(post.content)
+    for link in broken:
+        logging.warning("broken link in post: %s", broken)
     logging.info("post available at %s", post.link)
 
     return 0
 
 
 @click.command(name="upload")
 @click.option(
```

### Comparing `wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO` & `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-markdown-blog-loader
-Version: 1.0.1
+Version: 1.1.0
 Summary: load markdown blogs into wordpress
 Home-page: https://github.com/binxio/wordpress-markdown-blog-loader
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: APL2
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -23,14 +23,16 @@
 This utility loads markdown blogs into Wordpress as a post. It allows you to work on your blog
 in your favorite editor and keeps all your blogs in git.
 
 ## features
 - converts markdown into plain html, with syntax hightlighting support
 - uploads and synchronizes any locally referenced images
 - generates an opengraph image including the title, subtitle and author in Binx.io or xebia.com style
+- sets the Yoast focus keywords
+- sets the canonical url, if specified
 
 ## caveats
 - changing the slug may orphan images
 - removing images from the markdown, will leave dangling images in Wordpress
 
 ## required Wordpress Plugins
 
@@ -41,23 +43,24 @@
 
 ## configuration
 to configure the access credentials, you need to add your WordPress application password to the file `~/.wordpress.ini`  
 and add a section for your Wordpress installation:
 
 ```
 [DEFAULT]
-host = example.com
+host = xebia.com
 
-[example.com]
-api_host = example.wpengine.com
+[xebia.com]
 username = <your wordpress username>
 password = <your application passwoird>
 ```
 Note that the application password is different from the password you use to login to your WordPress installation.
 
+If the site is served through a CDN, you can also set the `api_host` which will be used as the hostname to invoke the WP REST API. 
+
 ## Using the image
 To use the docker image, you have to login using a GitHub container registry access token:
 
 1. Browse to https://github.com/settings/tokens
 2. Create new token with 'read:packages' permission
 3. Copy the token
 4. login to  ghcr.io with Docker.
```

### Comparing `wordpress-markdown-blog-loader-1.0.1/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt` & `wordpress-markdown-blog-loader-1.1.0/src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 README.md
 setup.py
 src/wordpress_markdown_blog_loader/__init__.py
 src/wordpress_markdown_blog_loader/__main__.py
 src/wordpress_markdown_blog_loader/api.py
 src/wordpress_markdown_blog_loader/blog.py
+src/wordpress_markdown_blog_loader/check_links.py
 src/wordpress_markdown_blog_loader/download.py
 src/wordpress_markdown_blog_loader/name_to_email.py
 src/wordpress_markdown_blog_loader/new.py
+src/wordpress_markdown_blog_loader/remove_newlines.py
 src/wordpress_markdown_blog_loader/upload.py
 src/wordpress_markdown_blog_loader.egg-info/PKG-INFO
 src/wordpress_markdown_blog_loader.egg-info/SOURCES.txt
 src/wordpress_markdown_blog_loader.egg-info/dependency_links.txt
 src/wordpress_markdown_blog_loader.egg-info/entry_points.txt
 src/wordpress_markdown_blog_loader.egg-info/not-zip-safe
 src/wordpress_markdown_blog_loader.egg-info/requires.txt
-src/wordpress_markdown_blog_loader.egg-info/top_level.txt
+src/wordpress_markdown_blog_loader.egg-info/top_level.txt
+tests/test_blog.py
```

