# Comparing `tmp/zoomeye-2.1.2.tar.gz` & `tmp/zoomeye-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomeye-2.1.2.tar", last modified: Fri Aug 26 08:31:50 2022, max compression
+gzip compressed data, was "zoomeye-2.2.0.tar", last modified: Wed Apr 12 08:22:52 2023, max compression
```

## Comparing `zoomeye-2.1.2.tar` & `zoomeye-2.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 08:31:50.934924 zoomeye-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    18046 2022-08-26 08:31:38.000000 zoomeye-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-26 08:31:38.000000 zoomeye-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    30375 2022-08-26 08:31:50.934924 zoomeye-2.1.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)    29442 2022-08-26 08:31:38.000000 zoomeye-2.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-08-26 08:31:38.000000 zoomeye-2.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 08:31:50.934924 zoomeye-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-08-26 08:31:38.000000 zoomeye-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 08:31:50.934924 zoomeye-2.1.2/zoomeye/
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-08-26 08:31:38.000000 zoomeye-2.1.2/zoomeye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7180 2022-08-26 08:31:38.000000 zoomeye-2.1.2/zoomeye/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-08-26 08:31:38.000000 zoomeye-2.1.2/zoomeye/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7324 2022-08-26 08:31:38.000000 zoomeye-2.1.2/zoomeye/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    26788 2022-08-26 08:31:38.000000 zoomeye-2.1.2/zoomeye/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-08-26 08:31:38.000000 zoomeye-2.1.2/zoomeye/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     4425 2022-08-26 08:31:38.000000 zoomeye-2.1.2/zoomeye/plotlib.py
--rw-r--r--   0 runner    (1001) docker     (121)    13921 2022-08-26 08:31:38.000000 zoomeye-2.1.2/zoomeye/sdk.py
--rw-r--r--   0 runner    (1001) docker     (121)    15632 2022-08-26 08:31:38.000000 zoomeye-2.1.2/zoomeye/show.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 08:31:50.934924 zoomeye-2.1.2/zoomeye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    30375 2022-08-26 08:31:50.000000 zoomeye-2.1.2/zoomeye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-08-26 08:31:50.000000 zoomeye-2.1.2/zoomeye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 08:31:50.000000 zoomeye-2.1.2/zoomeye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-26 08:31:50.000000 zoomeye-2.1.2/zoomeye.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-08-26 08:31:50.000000 zoomeye-2.1.2/zoomeye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-26 08:31:50.000000 zoomeye-2.1.2/zoomeye.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:22:52.475527 zoomeye-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-04-12 08:22:38.000000 zoomeye-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 08:22:38.000000 zoomeye-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29764 2023-04-12 08:22:52.475527 zoomeye-2.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28831 2023-04-12 08:22:38.000000 zoomeye-2.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 08:22:38.000000 zoomeye-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 08:22:52.475527 zoomeye-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-12 08:22:38.000000 zoomeye-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:22:52.475527 zoomeye-2.2.0/zoomeye/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-12 08:22:38.000000 zoomeye-2.2.0/zoomeye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-12 08:22:38.000000 zoomeye-2.2.0/zoomeye/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-12 08:22:38.000000 zoomeye-2.2.0/zoomeye/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-12 08:22:38.000000 zoomeye-2.2.0/zoomeye/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26614 2023-04-12 08:22:38.000000 zoomeye-2.2.0/zoomeye/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-12 08:22:38.000000 zoomeye-2.2.0/zoomeye/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-12 08:22:38.000000 zoomeye-2.2.0/zoomeye/plotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-04-12 08:22:38.000000 zoomeye-2.2.0/zoomeye/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-04-12 08:22:38.000000 zoomeye-2.2.0/zoomeye/show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:22:52.475527 zoomeye-2.2.0/zoomeye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29764 2023-04-12 08:22:52.000000 zoomeye-2.2.0/zoomeye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-12 08:22:52.000000 zoomeye-2.2.0/zoomeye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:22:52.000000 zoomeye-2.2.0/zoomeye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 08:22:52.000000 zoomeye-2.2.0/zoomeye.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 08:22:52.000000 zoomeye-2.2.0/zoomeye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 08:22:52.000000 zoomeye-2.2.0/zoomeye.egg-info/top_level.txt
```

### Comparing `zoomeye-2.1.2/LICENSE` & `zoomeye-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoomeye-2.1.2/PKG-INFO` & `zoomeye-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoomeye
-Version: 2.1.2
+Version: 2.2.0
 Summary: Python library and command-line tool for ZoomEye (https://www.zoomeye.org/doc)
 Home-page: https://github.com/knownsec/zoomeye-python
 Author: 404 Team@Knownsec
 Keywords: security tool,zoomeye,command tool
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -75,20 +75,15 @@
 
 
 1.initialize token
 ^^^^^^^^^^^^^^^^^^
 
 Before using the ``ZoomEye-python cli``, the user ``token`` needs to be
 initialized. The credential is used to verify the user’s identity to
-query data from ``ZoomEye``; we provide two authentication methods:
-
-::
-
-   1.username/password
-   2.APIKEY (recommend)
+query data from ``ZoomEye``; only support API-KEY authentication methods.
 
 You can view the help through ``zoomeye init -h``, and use ``APIKEY`` to
 demonstrate below:
 
 ::
 
    $ zoomeye init -apikey "01234567-acbd-00000-1111-22222222222"
@@ -97,18 +92,14 @@
    Quota: 10000
 
 Users can login to ``ZoomEye`` and obtain ``APIKEY`` in personal
 information (https://www.zoomeye.org/profile); ``APIKEY`` will not
 expire, users can reset in personal information according to their
 needs.
 
-in addition, we also provide the initialization method of
-``username/password``. After authentication in this way, the
-``JWT-token`` will be returned, which has certain timeliness and
-requires the user to login again after failure.
 
 2.query quota
 ^^^^^^^^^^^^^
 
 Users can query personal information and data quota through the ``info``
 command, as follows:
 
@@ -641,81 +632,67 @@
 ~~~~~~~~~~~~
 
 .. _initialize-token-1:
 
 1.initialize token
 ^^^^^^^^^^^^^^^^^^
 
-Similarly, the SDK also supports two authentication methods,
-``username/password`` and ``APIKEY``, as follows:
-
-**1.user/pass**
-
-.. code:: python
-
-   from zoomeye.sdk import ZoomEye
-
-   zm = ZoomEye(username="username", password="password")
+Similarly, the SDK also supports API-KEY authentication methods,
+ ``APIKEY``, as follows:
 
-**2.APIKEY**
+**APIKEY**
 
 .. code:: python
 
    from zoomeye.sdk import ZoomEye
 
    zm = ZoomEye(api_key="01234567-acbd-00000-1111-22222222222")
 
 2.SDK API
 ^^^^^^^^^
 
 The following are the interfaces and instructions provided by the SDK:
 
 ::
 
-   1.login()
-     use username/password or APIKEY for authentication
-   2.dork_search(dork, page=0, resource="host", facets=None)
+   1.dork_search(dork, page=0, resource="host", facets=None)
      search the data of the specified page according to dork
-   3.multi_page_search(dork, page=1, resource="host", facets=None)
+   2.multi_page_search(dork, page=1, resource="host", facets=None)
      search multiple pages of data according to dork
-   4.resources_info()
+   3.resources_info()
      get current user information
-   5.show_count()
+   4.show_count()
      get the number of all matching results under the current dork
-   6.dork_filter(keys)
+   5.dork_filter(keys)
      extract the data of the specified field from the search results
-   7.get_facet()
+   6.get_facet()
      get statistical results of all data from search results
-   8.history_ip(ip)
+   7.history_ip(ip)
      query historical data information of an ip
-   9.show_site_ip(data)
+   8.show_site_ip(data)
      traverse the web-search result set, and output the domain name and ip address
-   10.show_ip_port(data)
+   9.show_ip_port(data)
      traverse the host-search result set and output the ip address and port
-   11.generate_dot(self, q, source=0, page=1)
+   10.generate_dot(self, q, source=0, page=1)
      Generate graphviz files and pictures written in the domain center
 
 3.SDK example
 ^^^^^^^^^^^^^
 
 .. code:: python
 
    $ python3
    >>> import zoomeye.sdk as zoomeye
    >>> dir(zoomeye)
    ['ZoomEye', 'ZoomEyeDict', '__builtins__', '__cached__', '__doc__',
    '__file__', '__loader__', '__name__', '__package__', '__spec__',
    'fields_tables_host', 'fields_tables_web', 'getpass', 'requests',
    'show_ip_port', 'show_site_ip', 'zoomeye_api_test']
-   >>> # Use username and password to login
-   >>> zm = zoomeye.ZoomEye()
-   >>> zm.username = 'username@zoomeye.org'
-   >>> zm.password = 'password'
-   >>> print(zm.login())
-   ....JIUzI1NiIsInR5cCI6IkpXVCJ9.....
+   >>> # Use API-KEY search
+   >>> zm = zoomeye.ZoomEye(api_key="01234567-acbd-00000-1111-22222222222")
    >>> data = zm.dork_search('apache country:cn')
    >>> zoomeye.show_site_ip(data)
    213.***.***.46.rev.vo***one.pt ['46.***.***.213']
    me*****on.o****e.net.pg ['203.***.***.114']
    soft********63221110.b***c.net ['126.***.***.110']
    soft********26216022.b***c.net ['126.***.***.22']
    soft********5084068.b***c.net ['126.***.***.68']
```

### Comparing `zoomeye-2.1.2/README.rst` & `zoomeye-2.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -53,20 +53,15 @@
 
 
 1.initialize token
 ^^^^^^^^^^^^^^^^^^
 
 Before using the ``ZoomEye-python cli``, the user ``token`` needs to be
 initialized. The credential is used to verify the user’s identity to
-query data from ``ZoomEye``; we provide two authentication methods:
-
-::
-
-   1.username/password
-   2.APIKEY (recommend)
+query data from ``ZoomEye``; only support API-KEY authentication methods.
 
 You can view the help through ``zoomeye init -h``, and use ``APIKEY`` to
 demonstrate below:
 
 ::
 
    $ zoomeye init -apikey "01234567-acbd-00000-1111-22222222222"
@@ -75,18 +70,14 @@
    Quota: 10000
 
 Users can login to ``ZoomEye`` and obtain ``APIKEY`` in personal
 information (https://www.zoomeye.org/profile); ``APIKEY`` will not
 expire, users can reset in personal information according to their
 needs.
 
-in addition, we also provide the initialization method of
-``username/password``. After authentication in this way, the
-``JWT-token`` will be returned, which has certain timeliness and
-requires the user to login again after failure.
 
 2.query quota
 ^^^^^^^^^^^^^
 
 Users can query personal information and data quota through the ``info``
 command, as follows:
 
@@ -619,81 +610,67 @@
 ~~~~~~~~~~~~
 
 .. _initialize-token-1:
 
 1.initialize token
 ^^^^^^^^^^^^^^^^^^
 
-Similarly, the SDK also supports two authentication methods,
-``username/password`` and ``APIKEY``, as follows:
-
-**1.user/pass**
-
-.. code:: python
-
-   from zoomeye.sdk import ZoomEye
-
-   zm = ZoomEye(username="username", password="password")
+Similarly, the SDK also supports API-KEY authentication methods,
+ ``APIKEY``, as follows:
 
-**2.APIKEY**
+**APIKEY**
 
 .. code:: python
 
    from zoomeye.sdk import ZoomEye
 
    zm = ZoomEye(api_key="01234567-acbd-00000-1111-22222222222")
 
 2.SDK API
 ^^^^^^^^^
 
 The following are the interfaces and instructions provided by the SDK:
 
 ::
 
-   1.login()
-     use username/password or APIKEY for authentication
-   2.dork_search(dork, page=0, resource="host", facets=None)
+   1.dork_search(dork, page=0, resource="host", facets=None)
      search the data of the specified page according to dork
-   3.multi_page_search(dork, page=1, resource="host", facets=None)
+   2.multi_page_search(dork, page=1, resource="host", facets=None)
      search multiple pages of data according to dork
-   4.resources_info()
+   3.resources_info()
      get current user information
-   5.show_count()
+   4.show_count()
      get the number of all matching results under the current dork
-   6.dork_filter(keys)
+   5.dork_filter(keys)
      extract the data of the specified field from the search results
-   7.get_facet()
+   6.get_facet()
      get statistical results of all data from search results
-   8.history_ip(ip)
+   7.history_ip(ip)
      query historical data information of an ip
-   9.show_site_ip(data)
+   8.show_site_ip(data)
      traverse the web-search result set, and output the domain name and ip address
-   10.show_ip_port(data)
+   9.show_ip_port(data)
      traverse the host-search result set and output the ip address and port
-   11.generate_dot(self, q, source=0, page=1)
+   10.generate_dot(self, q, source=0, page=1)
      Generate graphviz files and pictures written in the domain center
 
 3.SDK example
 ^^^^^^^^^^^^^
 
 .. code:: python
 
    $ python3
    >>> import zoomeye.sdk as zoomeye
    >>> dir(zoomeye)
    ['ZoomEye', 'ZoomEyeDict', '__builtins__', '__cached__', '__doc__',
    '__file__', '__loader__', '__name__', '__package__', '__spec__',
    'fields_tables_host', 'fields_tables_web', 'getpass', 'requests',
    'show_ip_port', 'show_site_ip', 'zoomeye_api_test']
-   >>> # Use username and password to login
-   >>> zm = zoomeye.ZoomEye()
-   >>> zm.username = 'username@zoomeye.org'
-   >>> zm.password = 'password'
-   >>> print(zm.login())
-   ....JIUzI1NiIsInR5cCI6IkpXVCJ9.....
+   >>> # Use API-KEY search
+   >>> zm = zoomeye.ZoomEye(api_key="01234567-acbd-00000-1111-22222222222")
    >>> data = zm.dork_search('apache country:cn')
    >>> zoomeye.show_site_ip(data)
    213.***.***.46.rev.vo***one.pt ['46.***.***.213']
    me*****on.o****e.net.pg ['203.***.***.114']
    soft********63221110.b***c.net ['126.***.***.110']
    soft********26216022.b***c.net ['126.***.***.22']
    soft********5084068.b***c.net ['126.***.***.68']
```

### Comparing `zoomeye-2.1.2/setup.py` & `zoomeye-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `zoomeye-2.1.2/zoomeye/cli.py` & `zoomeye-2.2.0/zoomeye/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,16 +149,14 @@
         action="store_true"
     )
     parser_search.set_defaults(func=core.search)
 
     # initial account configuration related commands
     parser_init = subparsers.add_parser("init", help="Initialize the token for ZoomEye-python")
     parser_init.add_argument("-apikey", help="ZoomEye API Key", default=None, metavar='[api key]')
-    parser_init.add_argument("-username", help="ZoomEye account username", default=None, metavar='[username]')
-    parser_init.add_argument("-password", help="ZoomEye account password", default=None, metavar='[password]')
     parser_init.set_defaults(func=core.init)
 
     parser_ip_info = subparsers.add_parser("ip", help="Query IP information")
     parser_ip_info.add_argument("ip", help="search device IP", metavar='ip', type=str)
     parser_ip_info.add_argument(
         "-filter",
         help="output more clearer search results by set filter field,field:[port,service,app,banner,ssl]",
```

### Comparing `zoomeye-2.1.2/zoomeye/config.py` & `zoomeye-2.2.0/zoomeye/config.py`

 * *Files identical despite different names*

### Comparing `zoomeye-2.1.2/zoomeye/core.py` & `zoomeye-2.2.0/zoomeye/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,60 +39,25 @@
     with open(key_file, 'w') as f:
         f.write(key)
     show.printf("successfully initialized", color="green")
     # change the permission of the configuration file to read-only
     os.chmod(key_file, 0o600)
 
 
-def jwt_init(username, password):
-    """
-    initialize through the user name and password, write jwt to the local configuration file,
-    the expiration time is about 12 hours, so it is recommended to initialize through the api key.
-    :param username: str, login zoomeye account
-    :param password: str, login zoomeye account password
-    :return:
-    """
-    file.check_exist(zoomeye_dir)
-    try:
-        zoom = ZoomEye(username=username, password=password)
-        access_token = zoom.login()
-    except Exception:
-        return
-    jwt_file = zoomeye_dir + "/jwt"
-    if access_token:
-        # display the remaining resources of the current account
-        user_data = zoom.resources_info()
-        show.printf("Role: {}".format(user_data["plan"]))
-        show.printf("Quota: {}".format(user_data["resources"].get("search")))
-        with open(jwt_file, 'w') as f:
-            f.write(access_token)
-        show.printf("successfully initialized", color="green")
-        # change the permission of the configuration file to read-only
-        os.chmod(jwt_file, 0o600)
-    else:
-        show.printf("failed initialized!", color="red")
-
-
 def init(args):
     """
     the initialization processing function will select the initialization method according to the user's input.
     :param args:
     :return:
     """
     api_key = args.apikey
-    username = args.username
-    password = args.password
     # use api key init
-    if api_key and username is None and password is None:
+    if api_key:
         key_init(api_key)
         return
-    # use username and password init
-    if api_key is None and username and password:
-        jwt_init(username, password)
-        return
     # invalid parameter
     show.printf("input parameter error", color="red")
     show.printf("please run <zoomeye init -h> for help.", color="red")
 
 
 def search(args):
     dork = args.dork
@@ -130,16 +95,16 @@
 
 def info(args):
     """
     used to print the current identity of the user and the remaining data quota for the month
     :param args:
     :return:
     """
-    api_key, access_token = file.get_auth_key()
-    zm = ZoomEye(api_key=api_key, access_token=access_token)
+    api_key = file.get_auth_key()
+    zm = ZoomEye(api_key=api_key)
     # get user information
     user_data = zm.resources_info()
     if user_data:
         # show in the terminal
         show.printf("Role: {}".format(user_data["plan"]))
         show.printf("Quota: {}".format(user_data["resources"].get("search")))
         show.printf("user_info: {}".format(user_data["user_info"]))
```

### Comparing `zoomeye-2.1.2/zoomeye/data.py` & `zoomeye-2.2.0/zoomeye/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,16 +342,16 @@
         self.facet = facet
         self.force = force
 
         self.dork_data = list()
         self.facet_data = None
         self.total = 0
 
-        self.api_key, self.access_token = file.get_auth_key()
-        self.zoomeye = ZoomEye(api_key=self.api_key, access_token=self.access_token)
+        self.api_key = file.get_auth_key()
+        self.zoomeye = ZoomEye(api_key=self.api_key)
 
     def handle_page(self):
         try:
             num = int(self.num)
             if num % 20 == 0:
                 return int(num / 20)
             return int(num / 20) + 1
@@ -648,16 +648,16 @@
         return host_data
 
     def get_data(self):
         """
         get user level and IP historical data
         """
         normal_user = ['user', 'developer']
-        api_key, access_token = file.get_auth_key()
-        zm = ZoomEye(api_key=api_key, access_token=access_token)
+        api_key = file.get_auth_key()
+        zm = ZoomEye(api_key=api_key)
         role = zm.resources_info()
         # permission restrictions
         if role["plan"] in normal_user:
             show.printf("this function is only open to advanced users and VIP users.", color='red')
             exit(0)
         # the user chooses to force data from the API
         if self.force:
@@ -712,16 +712,16 @@
     def __init__(self, dork):
         self.dork = "ip:{}".format(dork)
 
     def request_data(self):
         """
         get api data
         """
-        api_key, access_token = file.get_auth_key()
-        zm = ZoomEye(api_key=api_key, access_token=access_token)
+        api_key = file.get_auth_key()
+        zm = ZoomEye(api_key=api_key)
         data = zm.dork_search(self.dork)
         return data
 
     def show_information(self):
         """
         show default fields: port,service,app,banner
         """
@@ -751,16 +751,16 @@
     query relation domain or sub domain
     """
 
     def __init__(self, q, source, page):
         self.q = q
         self.source = source
         self.page = page
-        api_key, access_token = file.get_auth_key()
-        self.zm = ZoomEye(api_key=api_key, access_token=access_token)
+        api_key = file.get_auth_key()
+        self.zm = ZoomEye(api_key=api_key)
 
     def show_information(self):
         """show domain search data"""
 
         info_data, total = self.zm.domain_search(self.q, self.source, self.page)
         show.show_domain_info(info_data, total, self.page)
         # return None
```

### Comparing `zoomeye-2.1.2/zoomeye/file.py` & `zoomeye-2.2.0/zoomeye/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,36 +59,27 @@
 
 def get_auth_key():
     """
     read configuration file
     :return:
     """
     api_key = None
-    access_token = None
     try:
         # read the api key from the configuration file,
         # if not, it will throw an exception that the file is not found.
         api_key = get_api_key(zoomeye_dir + "/apikey")
-        return api_key, access_token
+        return api_key
         # catch file not found exception
     except FileNotFoundError:
-        # try to get the json web token in the configuration file
-        try:
-            access_token = get_jwt_token(zoomeye_dir + "/jwt")
-            return api_key, access_token
-        except FileNotFoundError:
-            print("please run 'zoomeye init -apikey <api key>' "
-                  "or 'zoomeye init -username <username> -password <password>before using this command")
-            exit(0)
+        print("please run 'zoomeye init -apikey <api key>' before using this command")
+        exit(0)
         # catch other exceptions
     except Exception:
-        # there is no past api key and json web token in the configuration file
-        # tell users that they need to be initialized before use
-        print("please run 'zoomeye init -apikey <api key>' "
-              "or 'zoomeye init -username <username> -password <password>before using this command")
+        # unknown error
+        print("Unknown Error! Please submit issue.")
         exit(0)
 
 
 def check_exist(file):
     # whether the zoomeye configuration folder exists
     if not os.path.isdir(file):
         try:
```

### Comparing `zoomeye-2.1.2/zoomeye/plotlib.py` & `zoomeye-2.2.0/zoomeye/plotlib.py`

 * *Files identical despite different names*

### Comparing `zoomeye-2.1.2/zoomeye/sdk.py` & `zoomeye-2.2.0/zoomeye/sdk.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,19 +82,16 @@
             return value
         else:
             raise TypeError("the parameter you pass in must be a dictionary, not a {}".format(type(self.dict)))
 
 
 class ZoomEye:
 
-    def __init__(self, username=None, password=None, api_key="", access_token=""):
-        self.username = username
-        self.password = password
+    def __init__(self, api_key=""):
         self.api_key = api_key
-        self.access_token = access_token
 
         self.raw_data = None
         # process data, list
         self.data_list = None
         self.total = None
         self.search_type = None
         self.facet_data = None
@@ -126,47 +123,32 @@
             return data
         # Request data exceeds the total amount of ZoomEye data,
         # return all data instead of throwing an exception
         elif resp.status_code == 403 and 'specified resource' in resp.text:
             return None
         # if response succeed and status code is not 200 return error format json
         # others error return unknown error
-        # mainly users initialized by username and password, access token expires after 12 hours
         else:
             raise ValueError(resp.json().get('message'))
 
     def _check_header(self):
+        """
+        2023-04 remove username & password authenticate
+        only support API-KEY authenticate
+        """
         if self.api_key:
             headers = {
                 'API-KEY': self.api_key,
             }
-        elif self.access_token:
-            headers = {
-                'Authorization': 'JWT %s' % self.access_token
-            }
         else:
             headers = {}
         # add user agent
         headers["User-Agent"] = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.0.0 Safari/537.36"
         return headers
 
-    def login(self):
-        """
-        please see: https://www.zoomeye.org/doc#login
-        :return: json web token
-        """
-        params = '{{"username": "{}", "password": "{}"}}'.format(self.username,
-                                                                 self.password)
-        result = self._request(self.login_api, params, method="POST")
-        if result and "access_token" in result:
-            self.access_token = result.get("access_token")
-            return self.access_token
-        else:
-            return result
-
     def dork_search(self, dork, page=0, resource="host", facets=None):
         """
         Search records with ZoomEye dorks.
         param: dork
                ex: country:cn
                access https://www.zoomeye.org/search/dorks for more details.
         param: page
@@ -396,19 +378,15 @@
     if data:
         for i in data:
             print(i.get('ip'), i.get('portinfo').get('port'))
 
 
 def zoomeye_api_test():
     zoomeye = ZoomEye()
-    zoomeye.api_key = input('ZoomEye API-KEY(If you don\'t use API-KEY , Press Enter): ')
-    zoomeye.username = input('ZoomEye Username: ')
-    zoomeye.password = getpass.getpass(prompt='ZoomEye Password: ')
-    if zoomeye.username != "" and zoomeye.password != "":
-        zoomeye.login()
+    zoomeye.api_key = input('ZoomEye API-KEY:')
     print(zoomeye.resources_info())
 
     data = zoomeye.dork_search('solr')
     show_ip_port(data)
 
     data = zoomeye.dork_search('country:cn')
     show_ip_port(data)
```

### Comparing `zoomeye-2.1.2/zoomeye/show.py` & `zoomeye-2.2.0/zoomeye/show.py`

 * *Files identical despite different names*

### Comparing `zoomeye-2.1.2/zoomeye.egg-info/PKG-INFO` & `zoomeye-2.2.0/zoomeye.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoomeye
-Version: 2.1.2
+Version: 2.2.0
 Summary: Python library and command-line tool for ZoomEye (https://www.zoomeye.org/doc)
 Home-page: https://github.com/knownsec/zoomeye-python
 Author: 404 Team@Knownsec
 Keywords: security tool,zoomeye,command tool
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -75,20 +75,15 @@
 
 
 1.initialize token
 ^^^^^^^^^^^^^^^^^^
 
 Before using the ``ZoomEye-python cli``, the user ``token`` needs to be
 initialized. The credential is used to verify the user’s identity to
-query data from ``ZoomEye``; we provide two authentication methods:
-
-::
-
-   1.username/password
-   2.APIKEY (recommend)
+query data from ``ZoomEye``; only support API-KEY authentication methods.
 
 You can view the help through ``zoomeye init -h``, and use ``APIKEY`` to
 demonstrate below:
 
 ::
 
    $ zoomeye init -apikey "01234567-acbd-00000-1111-22222222222"
@@ -97,18 +92,14 @@
    Quota: 10000
 
 Users can login to ``ZoomEye`` and obtain ``APIKEY`` in personal
 information (https://www.zoomeye.org/profile); ``APIKEY`` will not
 expire, users can reset in personal information according to their
 needs.
 
-in addition, we also provide the initialization method of
-``username/password``. After authentication in this way, the
-``JWT-token`` will be returned, which has certain timeliness and
-requires the user to login again after failure.
 
 2.query quota
 ^^^^^^^^^^^^^
 
 Users can query personal information and data quota through the ``info``
 command, as follows:
 
@@ -641,81 +632,67 @@
 ~~~~~~~~~~~~
 
 .. _initialize-token-1:
 
 1.initialize token
 ^^^^^^^^^^^^^^^^^^
 
-Similarly, the SDK also supports two authentication methods,
-``username/password`` and ``APIKEY``, as follows:
-
-**1.user/pass**
-
-.. code:: python
-
-   from zoomeye.sdk import ZoomEye
-
-   zm = ZoomEye(username="username", password="password")
+Similarly, the SDK also supports API-KEY authentication methods,
+ ``APIKEY``, as follows:
 
-**2.APIKEY**
+**APIKEY**
 
 .. code:: python
 
    from zoomeye.sdk import ZoomEye
 
    zm = ZoomEye(api_key="01234567-acbd-00000-1111-22222222222")
 
 2.SDK API
 ^^^^^^^^^
 
 The following are the interfaces and instructions provided by the SDK:
 
 ::
 
-   1.login()
-     use username/password or APIKEY for authentication
-   2.dork_search(dork, page=0, resource="host", facets=None)
+   1.dork_search(dork, page=0, resource="host", facets=None)
      search the data of the specified page according to dork
-   3.multi_page_search(dork, page=1, resource="host", facets=None)
+   2.multi_page_search(dork, page=1, resource="host", facets=None)
      search multiple pages of data according to dork
-   4.resources_info()
+   3.resources_info()
      get current user information
-   5.show_count()
+   4.show_count()
      get the number of all matching results under the current dork
-   6.dork_filter(keys)
+   5.dork_filter(keys)
      extract the data of the specified field from the search results
-   7.get_facet()
+   6.get_facet()
      get statistical results of all data from search results
-   8.history_ip(ip)
+   7.history_ip(ip)
      query historical data information of an ip
-   9.show_site_ip(data)
+   8.show_site_ip(data)
      traverse the web-search result set, and output the domain name and ip address
-   10.show_ip_port(data)
+   9.show_ip_port(data)
      traverse the host-search result set and output the ip address and port
-   11.generate_dot(self, q, source=0, page=1)
+   10.generate_dot(self, q, source=0, page=1)
      Generate graphviz files and pictures written in the domain center
 
 3.SDK example
 ^^^^^^^^^^^^^
 
 .. code:: python
 
    $ python3
    >>> import zoomeye.sdk as zoomeye
    >>> dir(zoomeye)
    ['ZoomEye', 'ZoomEyeDict', '__builtins__', '__cached__', '__doc__',
    '__file__', '__loader__', '__name__', '__package__', '__spec__',
    'fields_tables_host', 'fields_tables_web', 'getpass', 'requests',
    'show_ip_port', 'show_site_ip', 'zoomeye_api_test']
-   >>> # Use username and password to login
-   >>> zm = zoomeye.ZoomEye()
-   >>> zm.username = 'username@zoomeye.org'
-   >>> zm.password = 'password'
-   >>> print(zm.login())
-   ....JIUzI1NiIsInR5cCI6IkpXVCJ9.....
+   >>> # Use API-KEY search
+   >>> zm = zoomeye.ZoomEye(api_key="01234567-acbd-00000-1111-22222222222")
    >>> data = zm.dork_search('apache country:cn')
    >>> zoomeye.show_site_ip(data)
    213.***.***.46.rev.vo***one.pt ['46.***.***.213']
    me*****on.o****e.net.pg ['203.***.***.114']
    soft********63221110.b***c.net ['126.***.***.110']
    soft********26216022.b***c.net ['126.***.***.22']
    soft********5084068.b***c.net ['126.***.***.68']
```

