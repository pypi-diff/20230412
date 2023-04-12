# Comparing `tmp/proxlist-0.5.0.tar.gz` & `tmp/proxlist-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxlist-0.5.0.tar", last modified: Sat Mar  5 06:01:48 2022, max compression
+gzip compressed data, was "proxlist-0.5.1.tar", last modified: Wed Apr 12 19:09:33 2023, max compression
```

## Comparing `proxlist-0.5.0.tar` & `proxlist-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 06:01:48.529474 proxlist-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-03-05 06:01:34.000000 proxlist-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-03-05 06:01:48.529474 proxlist-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-03-05 06:01:34.000000 proxlist-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 06:01:48.529474 proxlist-0.5.0/proxlist/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-03-05 06:01:34.000000 proxlist-0.5.0/proxlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4550 2022-03-05 06:01:34.000000 proxlist-0.5.0/proxlist/proxies.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-05 06:01:34.000000 proxlist-0.5.0/proxlist/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 06:01:48.529474 proxlist-0.5.0/proxlist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-03-05 06:01:48.000000 proxlist-0.5.0/proxlist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-03-05 06:01:48.000000 proxlist-0.5.0/proxlist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-05 06:01:48.000000 proxlist-0.5.0/proxlist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-03-05 06:01:48.000000 proxlist-0.5.0/proxlist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-05 06:01:48.000000 proxlist-0.5.0/proxlist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-03-05 06:01:34.000000 proxlist-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-05 06:01:48.529474 proxlist-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-03-05 06:01:34.000000 proxlist-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 06:01:48.529474 proxlist-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-05 06:01:34.000000 proxlist-0.5.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-05 06:01:48.529474 proxlist-0.5.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-05 06:01:34.000000 proxlist-0.5.0/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3586 2022-03-05 06:01:34.000000 proxlist-0.5.0/test/unit/test_proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:33.656476 proxlist-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 19:09:06.000000 proxlist-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-12 19:09:33.656476 proxlist-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-12 19:09:06.000000 proxlist-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:33.656476 proxlist-0.5.1/proxlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 19:09:06.000000 proxlist-0.5.1/proxlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-12 19:09:06.000000 proxlist-0.5.1/proxlist/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:06.000000 proxlist-0.5.1/proxlist/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:33.656476 proxlist-0.5.1/proxlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-12 19:09:33.000000 proxlist-0.5.1/proxlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 19:09:33.000000 proxlist-0.5.1/proxlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:09:33.000000 proxlist-0.5.1/proxlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-12 19:09:33.000000 proxlist-0.5.1/proxlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 19:09:33.000000 proxlist-0.5.1/proxlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-12 19:09:06.000000 proxlist-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 19:09:33.656476 proxlist-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-12 19:09:06.000000 proxlist-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:33.656476 proxlist-0.5.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:33.656476 proxlist-0.5.1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:06.000000 proxlist-0.5.1/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-12 19:09:06.000000 proxlist-0.5.1/test/unit/test_proxies.py
```

### Comparing `proxlist-0.5.0/LICENSE` & `proxlist-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proxlist-0.5.0/PKG-INFO` & `proxlist-0.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: proxlist
-Version: 0.5.0
+Version: 0.5.1
 Summary: Retrieve proxy servers.
 Home-page: http://github.com/Justintime50/proxlist
 Author: Justintime50
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # Proxlist
 
-Retrieve proxy servers.
+Retrieve free, open-source proxy servers.
 
 [![Build Status](https://github.com/Justintime50/proxlist/workflows/build/badge.svg)](https://github.com/Justintime50/proxlist/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Justintime50/proxlist/badge.svg?branch=main)](https://coveralls.io/github/Justintime50/proxlist?branch=main)
 [![PyPi](https://img.shields.io/pypi/v/proxlist)](https://pypi.org/project/proxlist)
 [![Licence](https://img.shields.io/github/license/Justintime50/proxlist)](LICENSE)
 
 <img src="https://raw.githubusercontent.com/justintime50/assets/main/src/proxlist/showcase.png" alt="Showcase">
 
 </div>
 
-Finding and storing a list of proxies can be taxing - especially ones that are free and actually work. `proxlist` will validate and return a rotating random proxy to you so you don't need to keep a list of proxies or ensure the list is still valid.
+Finding and storing a list of proxies can be taxing - especially ones that are free and actually work. `proxlist` will validate and return a rotating random proxy so you don't need to keep a list of proxies or ensure the list is still valid.
 
 Proxies are returned in the form of strings (eg: `ip:port`).
 
-These proxies come from all over the world and may not be performant for a production application. For a production application, you should really use a paid proxy service or a self-hosted solution. This package is intended for testing purposes and there are no guarantees about where the data sent through these proxies goes or how it's handled. The list of proxies rotates rapidly and is free and open source - your mileage may vary.
+These proxies come from all over the world and may not be performant for a production application. Instead, you should use a paid proxy service or a self-hosted solution. This package is intended for testing purposes and there are no guarantees about where the data sent through these proxies goes or how it's handled. The list and quality of proxies rotates rapidly - your mileage may vary.
 
 ## Install
 
 ```bash
 # Install tool
 pip3 install proxlist
 
@@ -78,9 +77,7 @@
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
 make help
 ```
-
-
```

### Comparing `proxlist-0.5.0/README.md` & `proxlist-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <div align="center">
 
 # Proxlist
 
-Retrieve proxy servers.
+Retrieve free, open-source proxy servers.
 
 [![Build Status](https://github.com/Justintime50/proxlist/workflows/build/badge.svg)](https://github.com/Justintime50/proxlist/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Justintime50/proxlist/badge.svg?branch=main)](https://coveralls.io/github/Justintime50/proxlist?branch=main)
 [![PyPi](https://img.shields.io/pypi/v/proxlist)](https://pypi.org/project/proxlist)
 [![Licence](https://img.shields.io/github/license/Justintime50/proxlist)](LICENSE)
 
 <img src="https://raw.githubusercontent.com/justintime50/assets/main/src/proxlist/showcase.png" alt="Showcase">
 
 </div>
 
-Finding and storing a list of proxies can be taxing - especially ones that are free and actually work. `proxlist` will validate and return a rotating random proxy to you so you don't need to keep a list of proxies or ensure the list is still valid.
+Finding and storing a list of proxies can be taxing - especially ones that are free and actually work. `proxlist` will validate and return a rotating random proxy so you don't need to keep a list of proxies or ensure the list is still valid.
 
 Proxies are returned in the form of strings (eg: `ip:port`).
 
-These proxies come from all over the world and may not be performant for a production application. For a production application, you should really use a paid proxy service or a self-hosted solution. This package is intended for testing purposes and there are no guarantees about where the data sent through these proxies goes or how it's handled. The list of proxies rotates rapidly and is free and open source - your mileage may vary.
+These proxies come from all over the world and may not be performant for a production application. Instead, you should use a paid proxy service or a self-hosted solution. This package is intended for testing purposes and there are no guarantees about where the data sent through these proxies goes or how it's handled. The list and quality of proxies rotates rapidly - your mileage may vary.
 
 ## Install
 
 ```bash
 # Install tool
 pip3 install proxlist
```

### Comparing `proxlist-0.5.0/proxlist/proxies.py` & `proxlist-0.5.1/proxlist/proxies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,25 @@
-from concurrent.futures import ALL_COMPLETED, ThreadPoolExecutor, wait
-from typing import List, Optional
+from concurrent.futures import (
+    ALL_COMPLETED,
+    ThreadPoolExecutor,
+    wait,
+)
+from typing import (
+    List,
+    Optional,
+)
 
 import requests
 import woodchips
 from bs4 import BeautifulSoup  # type: ignore
 
+
 LOGGER_NAME = 'proxlist'
 NUM_THREADS = 20
+LOG_LEVEL = 'NOTSET'  # Intentionally hide all loggers. During development, set to `DEBUG`
 
 
 def random_proxy(country: Optional[str] = None, google_verified: bool = False) -> Optional[str]:
     """Returns a 'random' proxy (ip:port) from the currently configured list.
 
     This is accomplished by testing each proxy concurrently until we find one that works.
     """
@@ -49,18 +58,18 @@
     return proxy_list
 
 
 def get_proxies(country: Optional[str] = None, google_verified: bool = False) -> List[str]:
     """Gets a list of proxies from https://www.sslproxies.org by scraping the proxy table."""
     proxy_list = []
 
-    try:
-        website = requests.get('https://www.sslproxies.org')
-    except Exception:
-        raise
+    website = requests.get(
+        url='https://www.sslproxies.org',
+        timeout=3,
+    )
 
     soup = BeautifulSoup(website.text, 'html.parser')
     table = soup.find('table').find('tbody')
 
     for table_entry in table.find_all('tr'):
         entry_elements = [td.text.strip() for td in table_entry.find_all('td')]
         ip_address = entry_elements[0]
@@ -115,15 +124,15 @@
         logger.debug(f'Couldn\'t connect to proxy: {proxy}')
 
     return valid_proxy
 
 
 def _setup_logger():
     """Setup a `woodchips` logger instance."""
-    logging_level = 'ERROR'  # Intentionally hide all loggers. During development, set to `DEBUG`
+    logging_level = LOG_LEVEL
 
     logger = woodchips.Logger(
         name=LOGGER_NAME,
         level=logging_level,
     )
     logger.log_to_console()
```

### Comparing `proxlist-0.5.0/proxlist.egg-info/PKG-INFO` & `proxlist-0.5.1/proxlist.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: proxlist
-Version: 0.5.0
+Version: 0.5.1
 Summary: Retrieve proxy servers.
 Home-page: http://github.com/Justintime50/proxlist
 Author: Justintime50
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # Proxlist
 
-Retrieve proxy servers.
+Retrieve free, open-source proxy servers.
 
 [![Build Status](https://github.com/Justintime50/proxlist/workflows/build/badge.svg)](https://github.com/Justintime50/proxlist/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Justintime50/proxlist/badge.svg?branch=main)](https://coveralls.io/github/Justintime50/proxlist?branch=main)
 [![PyPi](https://img.shields.io/pypi/v/proxlist)](https://pypi.org/project/proxlist)
 [![Licence](https://img.shields.io/github/license/Justintime50/proxlist)](LICENSE)
 
 <img src="https://raw.githubusercontent.com/justintime50/assets/main/src/proxlist/showcase.png" alt="Showcase">
 
 </div>
 
-Finding and storing a list of proxies can be taxing - especially ones that are free and actually work. `proxlist` will validate and return a rotating random proxy to you so you don't need to keep a list of proxies or ensure the list is still valid.
+Finding and storing a list of proxies can be taxing - especially ones that are free and actually work. `proxlist` will validate and return a rotating random proxy so you don't need to keep a list of proxies or ensure the list is still valid.
 
 Proxies are returned in the form of strings (eg: `ip:port`).
 
-These proxies come from all over the world and may not be performant for a production application. For a production application, you should really use a paid proxy service or a self-hosted solution. This package is intended for testing purposes and there are no guarantees about where the data sent through these proxies goes or how it's handled. The list of proxies rotates rapidly and is free and open source - your mileage may vary.
+These proxies come from all over the world and may not be performant for a production application. Instead, you should use a paid proxy service or a self-hosted solution. This package is intended for testing purposes and there are no guarantees about where the data sent through these proxies goes or how it's handled. The list and quality of proxies rotates rapidly - your mileage may vary.
 
 ## Install
 
 ```bash
 # Install tool
 pip3 install proxlist
 
@@ -78,9 +77,7 @@
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
 make help
 ```
-
-
```

### Comparing `proxlist-0.5.0/setup.py` & `proxlist-0.5.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 import setuptools
 
+
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 REQUIREMENTS = [
     'beautifulsoup4 == 4.*',
     'requests == 2.*',
     'woodchips == 0.2.*',
 ]
 
 DEV_REQUIREMENTS = [
-    'black',
-    'coveralls == 3.*',
-    'flake8',
-    'isort',
-    'mypy',
+    'bandit == 1.7.*',
+    'black == 23.*',
+    'build == 0.10.*',
+    'flake8 == 5.*',
+    'isort == 5.*',
+    'mypy == 1.2.*',
     'pytest == 7.*',
-    'pytest-cov == 3.*',
+    'pytest-cov == 4.*',
+    'twine == 4.*',
     'types-requests',
 ]
 
 setuptools.setup(
     name='proxlist',
-    version='0.5.0',
+    version='0.5.1',
     description='Retrieve proxy servers.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/Justintime50/proxlist',
     author='Justintime50',
     license='MIT',
-    packages=setuptools.find_packages(),
-    package_data={'proxlist': ['py.typed']},
+    packages=setuptools.find_packages(
+        exclude=[
+            'examples',
+            'test',
+        ]
+    ),
+    package_data={
+        'proxlist': [
+            'py.typed',
+        ]
+    },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=REQUIREMENTS,
     extras_require={
```

### Comparing `proxlist-0.5.0/test/unit/test_proxies.py` & `proxlist-0.5.1/test/unit/test_proxies.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,19 @@
         assert type(random_proxy) == str
         assert ':' in random_proxy
         assert 12 < len(random_proxy) < 25
 
 
 def test_random_proxy_filter_country():
     """Tests that we can retrieve a random proxy when filtering by country."""
-    countries_to_try = ['US', 'CA', 'MX']
+    countries_to_try = [
+        'US',
+        'CA',
+        'MX',
+    ]  # Purposefully sorted by distance from most-likely origin so tests run faster
 
     for country in countries_to_try:
         try:
             random_proxy = proxlist.random_proxy(country=country)
         except Exception:
             # If we fail to find a valid proxy from one country, try another country
             continue
```

