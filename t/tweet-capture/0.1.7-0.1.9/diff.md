# Comparing `tmp/tweet-capture-0.1.7.tar.gz` & `tmp/tweet-capture-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweet-capture-0.1.7.tar", last modified: Fri Dec  2 17:58:00 2022, max compression
+gzip compressed data, was "tweet-capture-0.1.9.tar", last modified: Wed Apr 12 20:01:41 2023, max compression
```

## Comparing `tweet-capture-0.1.7.tar` & `tweet-capture-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-12-02 17:58:00.695940 tweet-capture-0.1.7/
--rw-rw-rw-   0        0        0     1085 2021-05-31 19:56:28.000000 tweet-capture-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     2879 2022-12-02 17:58:00.696953 tweet-capture-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2297 2022-11-21 21:01:48.000000 tweet-capture-0.1.7/README.md
--rw-rw-rw-   0        0        0       86 2022-12-02 17:58:00.697948 tweet-capture-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1147 2022-12-02 17:53:47.000000 tweet-capture-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-02 17:58:00.684949 tweet-capture-0.1.7/tweet_capture.egg-info/
--rw-rw-rw-   0        0        0     2879 2022-12-02 17:58:00.000000 tweet-capture-0.1.7/tweet_capture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2022-12-02 17:58:00.000000 tweet-capture-0.1.7/tweet_capture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-02 17:58:00.000000 tweet-capture-0.1.7/tweet_capture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2022-12-02 17:58:00.000000 tweet-capture-0.1.7/tweet_capture.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2022-12-02 17:58:00.000000 tweet-capture-0.1.7/tweet_capture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-12-02 17:58:00.000000 tweet-capture-0.1.7/tweet_capture.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-02 17:58:00.689950 tweet-capture-0.1.7/tweetcapture/
--rw-rw-rw-   0        0        0       60 2021-05-31 18:34:46.000000 tweet-capture-0.1.7/tweetcapture/__init__.py
--rw-rw-rw-   0        0        0     3502 2022-12-01 17:16:07.000000 tweet-capture-0.1.7/tweetcapture/cli.py
--rw-rw-rw-   0        0        0    13630 2022-12-02 17:53:20.000000 tweet-capture-0.1.7/tweetcapture/screenshot.py
-drwxrwxrwx   0        0        0        0 2022-12-02 17:58:00.694947 tweet-capture-0.1.7/tweetcapture/utils/
--rw-rw-rw-   0        0        0        0 2021-05-31 19:53:06.000000 tweet-capture-0.1.7/tweetcapture/utils/__init__.py
--rw-rw-rw-   0        0        0     1831 2022-11-28 00:27:12.000000 tweet-capture-0.1.7/tweetcapture/utils/utils.py
--rw-rw-rw-   0        0        0     1892 2022-12-01 17:04:37.000000 tweet-capture-0.1.7/tweetcapture/utils/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:01:41.669123 tweet-capture-0.1.9/
+-rw-rw-rw-   0        0        0     1085 2021-05-31 19:56:28.000000 tweet-capture-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3238 2023-04-12 20:01:41.669826 tweet-capture-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2656 2023-04-06 14:53:44.000000 tweet-capture-0.1.9/README.md
+-rw-rw-rw-   0        0        0       67 2023-04-06 14:53:44.000000 tweet-capture-0.1.9/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-04-12 20:01:41.670576 tweet-capture-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2023-04-12 19:53:24.000000 tweet-capture-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:01:41.660557 tweet-capture-0.1.9/tweet_capture.egg-info/
+-rw-rw-rw-   0        0        0     3238 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 20:01:41.000000 tweet-capture-0.1.9/tweet_capture.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 20:01:41.664305 tweet-capture-0.1.9/tweetcapture/
+-rw-rw-rw-   0        0        0       60 2021-05-31 18:34:46.000000 tweet-capture-0.1.9/tweetcapture/__init__.py
+-rw-rw-rw-   0        0        0     3502 2023-04-06 14:53:44.000000 tweet-capture-0.1.9/tweetcapture/cli.py
+-rw-rw-rw-   0        0        0    13816 2023-04-06 14:53:44.000000 tweet-capture-0.1.9/tweetcapture/screenshot.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:01:41.668054 tweet-capture-0.1.9/tweetcapture/utils/
+-rw-rw-rw-   0        0        0        0 2021-05-31 19:53:06.000000 tweet-capture-0.1.9/tweetcapture/utils/__init__.py
+-rw-rw-rw-   0        0        0     1831 2023-04-06 13:06:19.000000 tweet-capture-0.1.9/tweetcapture/utils/utils.py
+-rw-rw-rw-   0        0        0     2302 2023-04-06 14:53:44.000000 tweet-capture-0.1.9/tweetcapture/utils/webdriver.py
```

### Comparing `tweet-capture-0.1.7/LICENSE` & `tweet-capture-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tweet-capture-0.1.7/PKG-INFO` & `tweet-capture-0.1.9/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: tweet-capture
-Version: 0.1.7
-Summary: Take a tweet screenshot
-Home-page: https://github.com/Xacnio/tweetcapture
-Author: Alperen Çetin
-Author-email: xacnio@pm.me
-License: MIT
-Keywords: tweet screenshot
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # TweetCapture
 
 Easily take screenshots of tweets/mentions and save them as image.
 
 ## Command-Line Usage
 
 ```
@@ -31,35 +13,44 @@
 ## Code Usage Examples
 
 - [Cli](tweetcapture/cli.py)
 - [Code Examples](tweetcapture/examples/)
 
 ## Testing
 ```
+> pip3 install opencv-python numpy
 > cd tweetcapture/tests/
 > python -m unittest
 ```
 
+## Docker Usage
+```
+docker run --rm -v $(pwd):/app xacnio/tweetcapture -h
+docker run --rm -v $(pwd):/app xacnio/tweetcapture https://twitter.com/jack/status/20
+```
+- *<font size="1">On Windows: Replace `$(pwd)` with `${PWD}`* (**Powershell**)
+- *On Windows: Replace `$(pwd)` with `%cd%`* (**Command Line**)</font>
+
 ## Modes
 
 | #   |                                                   |                                                      |
 | --- | ------------------------------------------------- | ---------------------------------------------------- |
-| 0   | Hide everything outside tweet content and author. | <img src="tweetcapture/assets/test4.png" width="300"> |
-| 1   | Show retweet/like counts.                         | <img src="tweetcapture/assets/test3.png" width="300"> |
-| 2   | Show retweet/like counts and timestamp.           | <img src="tweetcapture/assets/test2.png" width="300"> |
-| 3   | Show everything.                                  | <img src="tweetcapture/assets/test1.png" width="300"> |
-| 4   | Show timestamp.                                   | <img src="tweetcapture/assets/test5.png" width="300"> |
+| 0   | Hide everything outside tweet content and author. | <img src="tweetcapture/assets/mode0.png" width="300"> |
+| 1   | Show retweet/like counts.                         | <img src="tweetcapture/assets/mode1.png" width="300"> |
+| 2   | Show retweet/like counts and timestamp.           | <img src="tweetcapture/assets/mode2.png" width="300"> |
+| 3   | Show everything.                                  | <img src="tweetcapture/assets/mode3.png" width="300"> |
+| 4   | Show timestamp.                                   | <img src="tweetcapture/assets/mode4.png" width="300"> |
 
 ## Night Modes
 
 | #   |            |                                                      |
 | --- | ---------- | ---------------------------------------------------- |
-| 0   | Light mode | <img src="tweetcapture/assets/test4.png" width="300"> |
-| 1   | Dark mode  | <img src="tweetcapture/assets/test3.png" width="300"> |
-| 2   | Black mode | <img src="tweetcapture/assets/test1.png" width="300"> |
+| 0   | Light mode | <img src="tweetcapture/assets/mode4.png" width="300"> |
+| 1   | Dark mode  | <img src="tweetcapture/assets/mode1.png" width="300"> |
+| 2   | Black mode | <img src="tweetcapture/assets/mode3.png" width="300"> |
 
 ## Show Mentions Example
 _If the tweet have a very many mentions, there may be problems because "show more" option not supported. The tool can show only first loaded mentions. You can limit mention count on screenshot by using -sc <count> argument_
 ```
 tweetcapture -sm 3 https://twitter.com/Twitter/status/1445078208190291973
 ```
 <details>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tweet-capture-0.1.7/setup.py` & `tweet-capture-0.1.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,33 +3,31 @@
 # Long description
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 
 # Requirements
 def get_requirements():
-    return [
-        'selenium>=4.0.0',
-        'webdriver-manager>=3.8.5',
-        'packaging',
-        'Pillow>=9.3.0',
-    ]
+    with open('requirements.txt', 'r') as f:
+        requirements = f.read().splitlines()
+        return requirements
 
 
 setuptools.setup(
     name="tweet-capture",
-    version="0.1.7",
+    version="0.1.9",
     author="Alperen Çetin",
     author_email="xacnio@pm.me",
     description="Take a tweet screenshot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xacnio/tweetcapture",
     packages=setuptools.find_packages(),
     install_requires=get_requirements(),
+    data_files=[("", ["requirements.txt"])],
     entry_points={
         "console_scripts": ["tweetcapture=tweetcapture.cli:main"]},
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
```

### Comparing `tweet-capture-0.1.7/tweetcapture/cli.py` & `tweet-capture-0.1.9/tweetcapture/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     parser.add_argument('-t', type=float, help="Waiting time while the page loading (1.0-10.0)", default=5.0)
     parser.add_argument("-n", "--night-mode", type=int, help="Twitter night mode theme (0-2)", default=0)
     parser.add_argument('--lang', type=str,help="Browser language code (tr,en,es,..)", default="")
     parser.add_argument('--chromedriver', type=str, help="Custom chromedriver path", default="")
     parser.add_argument('-o', '--output', type=str, help="Output file name", default="")
     parser.add_argument('-sp', '--show-parent-tweets', dest='show_parent_tweets', action='store_true', help="Show parent tweets")
     parser.add_argument('-sm', '--show-mentions', type=int, help="Show mentions count (default: 0)", default=0)
-    parser.add_argument('-r', '--radius', type=int, help="Image radius", default=30)
+    parser.add_argument('-r', '--radius', type=int, help="Image radius", default=15)
 
     parser.add_argument('-hp', '--hide-photos', dest='hide_tweet_photos', action='store_true', help="Hide tweet photos")
     parser.add_argument('-hv', '--hide-videos', dest='hide_tweet_videos', action='store_true', help="Hide tweet videos")
     parser.add_argument('-hg', '--hide-gifs', dest='hide_tweet_gifs', action='store_true', help="Hide tweet gifs")
     parser.add_argument('-hq', '--hide-quotes', dest='hide_tweet_quotes', action='store_true', help="Hide tweet quotes")
     parser.add_argument('-hlp', '--hide-link-previews', dest='hide_tweet_link_previews', action='store_true', help="Hide tweet link previews")
     parser.add_argument('-ha', '--hide-all', dest='hide_all_tweet_medias', action='store_true', help="Hide all tweet medias")
```

### Comparing `tweet-capture-0.1.7/tweetcapture/screenshot.py` & `tweet-capture-0.1.9/tweetcapture/screenshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,25 @@
     wait_time = 5
     chrome_opts = []
     lang = None
     test = False
     show_parent_tweets = False
     show_mentions_count = 0
     overwrite = False
-    radius = 30
+    radius = 15
 
     hide_link_previews = False
     hide_photos = False
     hide_videos = False
     hide_gifs = False
     hide_quotes = False
 
-    def __init__(self, mode=3, night_mode=0, test=False, show_parent_tweets=False, show_mentions_count=0, overwrite=False, radius=30):
+    __web = 1
+
+    def __init__(self, mode=3, night_mode=0, test=False, show_parent_tweets=False, show_mentions_count=0, overwrite=False, radius=15):
         self.set_night_mode(night_mode)
         self.set_mode(mode)
         self.test = test
         self.show_parent_tweets = show_parent_tweets
         self.show_mentions_count = show_mentions_count
         self.overwrite = overwrite
         self.radius = radius
@@ -49,25 +51,29 @@
         url = is_valid_tweet_url(url)
         if self.lang:
             url += "?lang=" + self.lang
 
             
         radius = self.radius if radius is None else radius
         driver = await get_driver(self.chrome_opts, self.driver_path, self.gui)
+        if driver is None:
+            raise Exception("webdriver cannot be initialized")
         try:
             driver.get(url)
             driver.add_cookie(
                 {"name": "night_mode", "value": str(self.night_mode if night_mode is None else night_mode)})
             driver.get(url)
             await sleep(self.wait_time)
            
             self.__hide_global_items(driver)
             driver.execute_script("!!document.activeElement ? document.activeElement.blur() : 0")
 
-            if self.test is True: driver.save_screenshot("web.png")
+            if self.test is True: 
+                driver.save_screenshot(f"web{self.__web}.png")
+                self.__web += 1
             await sleep(2.0)
             elements, main = self.__get_tweets(driver, self.show_parent_tweets if show_parent_tweets is None else show_parent_tweets, self.show_mentions_count if show_mentions_count is None else show_mentions_count)
             if len(elements) == 0:
                 raise Exception("Tweets not found")
             else:
                 for i, element in enumerate(elements):
                     if i == main:
@@ -116,15 +122,15 @@
                     new_im.paste(im, (0,y))
                     y += im.size[1]
                     im.close()
                     remove(im.filename)
                 
                 if radius > 0:
                     new_im = add_corners(new_im, self.radius)
-                new_im.save(path)
+                new_im.save(path, quality=100)
                 new_im.close()
   
             driver.quit()
         except Exception as err:
             driver.quit()
             raise err
         return path
```

### Comparing `tweet-capture-0.1.7/tweetcapture/utils/utils.py` & `tweet-capture-0.1.9/tweetcapture/utils/utils.py`

 * *Files identical despite different names*

