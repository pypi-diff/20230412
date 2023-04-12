# Comparing `tmp/django_gbasedbtdb-1.10.1.tar.gz` & `tmp/django_gbasedbtdb-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_gbasedbtdb-1.10.1.tar", last modified: Wed Apr 12 04:57:47 2023, max compression
+gzip compressed data, was "django_gbasedbtdb-1.7.0.tar", last modified: Wed Apr 12 04:45:43 2023, max compression
```

## Comparing `django_gbasedbtdb-1.10.1.tar` & `django_gbasedbtdb-1.7.0.tar`

### file list

```diff
@@ -1,37 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:57:47.119084 django_gbasedbtdb-1.10.1/
--rw-rw-r--   0 root         (0) root         (0)    11357 2023-04-07 16:59:43.000000 django_gbasedbtdb-1.10.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1401 2023-04-12 04:57:47.119084 django_gbasedbtdb-1.10.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      530 2023-04-12 04:57:28.000000 django_gbasedbtdb-1.10.1/README.md
--rw-rw-r--   0 root         (0) root         (0)     7193 2023-04-07 17:05:51.000000 django_gbasedbtdb-1.10.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:57:47.111084 django_gbasedbtdb-1.10.1/django_gbasedbtdb/
--rw-rw-r--   0 root         (0) root         (0)       23 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    21273 2023-04-11 09:37:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/base.py
--rw-rw-r--   0 root         (0) root         (0)     2914 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/client.py
--rw-rw-r--   0 root         (0) root         (0)     1684 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/compiler.py
--rw-rw-r--   0 root         (0) root         (0)     1251 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/creation.py
--rw-rw-r--   0 root         (0) root         (0)     2023 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/datatypes.py
--rw-rw-r--   0 root         (0) root         (0)      781 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/features.py
--rw-rw-r--   0 root         (0) root         (0)     1279 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/fields.py
--rw-rw-r--   0 root         (0) root         (0)     5897 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/introspection.py
--rw-rw-r--   0 root         (0) root         (0)     5528 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/operations.py
--rw-rw-r--   0 root         (0) root         (0)     1847 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/schema.py
--rw-rw-r--   0 root         (0) root         (0)     1337 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/tableignore.py
--rw-rw-r--   0 root         (0) root         (0)      176 2023-04-07 17:10:06.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:57:47.115084 django_gbasedbtdb-1.10.1/django_gbasedbtdb.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     1401 2023-04-12 04:57:47.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      814 2023-04-12 04:57:47.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-12 04:57:47.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       71 2023-04-12 04:57:47.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       23 2023-04-12 04:57:47.000000 django_gbasedbtdb-1.10.1/django_gbasedbtdb.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      120 2023-04-12 04:57:47.119084 django_gbasedbtdb-1.10.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1401 2023-04-12 04:47:37.000000 django_gbasedbtdb-1.10.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:57:47.115084 django_gbasedbtdb-1.10.1/test/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-07 16:59:43.000000 django_gbasedbtdb-1.10.1/test/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      660 2023-04-07 16:59:43.000000 django_gbasedbtdb-1.10.1/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:57:47.119084 django_gbasedbtdb-1.10.1/test/datatypes/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-07 16:59:43.000000 django_gbasedbtdb-1.10.1/test/datatypes/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      462 2023-04-07 16:59:43.000000 django_gbasedbtdb-1.10.1/test/datatypes/models.py
--rw-rw-r--   0 root         (0) root         (0)     3899 2023-04-07 16:59:43.000000 django_gbasedbtdb-1.10.1/test/datatypes/test_datatypes.py
--rw-rw-r--   0 root         (0) root         (0)     9006 2023-04-07 16:59:43.000000 django_gbasedbtdb-1.10.1/test/test_base.py
--rw-rw-r--   0 root         (0) root         (0)      281 2023-04-07 16:59:43.000000 django_gbasedbtdb-1.10.1/test/test_integration.py
--rw-rw-r--   0 root         (0) root         (0)      156 2023-04-07 16:59:43.000000 django_gbasedbtdb-1.10.1/test/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:45:43.055185 django_gbasedbtdb-1.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-04-12 04:45:43.055185 django_gbasedbtdb-1.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      492 2023-04-12 04:42:44.000000 django_gbasedbtdb-1.7.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     7123 2023-04-07 19:20:34.000000 django_gbasedbtdb-1.7.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:45:43.055185 django_gbasedbtdb-1.7.0/django_gbasedbtdb/
+-rw-r--r--   0 root         (0) root         (0)       22 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18706 2023-04-07 19:22:08.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/base.py
+-rw-r--r--   0 root         (0) root         (0)     2914 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/client.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/creation.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      781 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/features.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/fields.py
+-rw-r--r--   0 root         (0) root         (0)     5599 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/introspection.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/operations.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/schema.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/tableignore.py
+-rw-r--r--   0 root         (0) root         (0)      176 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:45:43.055185 django_gbasedbtdb-1.7.0/django_gbasedbtdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-04-12 04:45:42.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      649 2023-04-12 04:45:43.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 04:45:42.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-12 04:45:43.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 04:45:43.000000 django_gbasedbtdb-1.7.0/django_gbasedbtdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-12 04:45:43.055185 django_gbasedbtdb-1.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1294 2023-04-12 04:44:51.000000 django_gbasedbtdb-1.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 04:45:43.055185 django_gbasedbtdb-1.7.0/test/
+-rw-r--r--   0 root         (0) root         (0)     5423 2020-08-28 04:24:31.000000 django_gbasedbtdb-1.7.0/test/test_base.py
```

### Comparing `django_gbasedbtdb-1.10.1/PKG-INFO` & `django_gbasedbtdb-1.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 Metadata-Version: 2.1
 Name: django_gbasedbtdb
-Version: 1.10.1
-Summary: A database driver for Django to connect to an GBase 8s database via ODBC
+Version: 1.7.0
+Summary: A database driver for Django to connect to an GBase 8s db via ODBC
 Home-page: https://gbasedbt.com
 Author: liaosnet
 Author-email: liaosnet@gbasedbt.com
 License: APLv2
 Keywords: django gbasedbt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
 
 ## A database driver for Django to connect to an GBase 8s database via pyodbc.  
 
 **Some limitations**:
 
 - Does not support default values  
 - GBase 8s automatically creates indexes on foreign keys, but Django attempts to do that
   manually; the current implementation here just attempts to catch the error on index
   creation. It may unintentionally catch other index creation errors where the index
   already exists.
 
 ### Release History  
 
-Version 1.10.1  
+Version 1.7.0  
 
 - Fork from django_informixdb  
-- Fix 'unsupported column type -114'
```

### Comparing `django_gbasedbtdb-1.10.1/README.rst` & `django_gbasedbtdb-1.7.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,210 +1,179 @@
-Django GBasedbtDB
-==================
-
-A database driver for Django to connect to an GBase 8s database via pyodbc.
-
-**Some limitations**:
-
-- Does not support default values
-- GBase 8s automatically creates indexes on foreign keys, but Django attempts to do that
-  manually; the current implementation here just attempts to catch the error on index
-  creation. It may unintentionally catch other index creation errors where the index
-  already exists.
-
-
-Configure local environment
----------------------------
-
-The following environment variables should exist:
-
-GBASEDBTDIR
-    The path to the GBase 8s client install directory
-
-GBASEDBTSERVER
-    The name of the GBase 8s service to which we need to connect
-
-GBASEDBTSQLHOSTS
-    The path to the ``sqlhosts`` file that the GBase 8s driver should use
-
-LD_LIBRARY_PATH
-    The path(s) to the various GBase 8s library files: Usually
-    ``$GBASEDBTDIR/lib:$GBASEDBTDIR/lib/cli:$GBASEDBTDIR/lib/esql``
-
-DB_LOCALE
-    In case of ``Database locale information mismatch.`` error during connection,
-    you should specify your database locale, e.g. ``DB_LOCALE=en_US.8859-15``
-
-You will also need to add an entry within your ``sqlhosts`` file for each remote/local GBase 8s 
-server connection in the following format::
-
-    <GBASEDBT_SERVER_NAME>    onsoctcp     <GBASEDBT_HOST_NAME>    <GBASEDBT_SERVICE_NAME>
-
-For example::
-
-    dev    onsoctcp    localhost    9088
-
-You may alternatively use a symbolic name in that line in place of the port number, typically ``sqlexec`` and
-then configure the port number in the ``/etc/services`` file::
-
-    sqlexec    9088/tcp
-
-
-Configure settings.py
----------------------
-
-Django’s settings.py uses the following to connect to an GBase 8s database:
-
-.. code-block:: python
-
-    'default': {
-        'ENGINE': 'django_gbasedbtdb',
-        'NAME': 'myproject',
-        'SERVER': 'dbtserver',
-        'USER' : 'testuser',
-        'PASSWORD': 'passw0rd',
-        'OPTIONS': {
-            'DRIVER': '/path/to/iclit09b.so'. # Or iclit09b.dylib on macOS
-            'CPTIMEOUT': 120,
-            'CONN_TIMEOUT': 120,
-            'ISOLATION_LEVEL': 'READ_UNCOMMITTED',
-            'LOCK_MODE_WAIT': 0,
-            'VALIDATE_CONNECTION': True,
-        },
-        'CONNECTION_RETRY': {
-            'MAX_ATTEMPTS': 10,
-        },
-        'TEST': {
-            'NAME': 'myproject',
-            'CREATE_DB': False
-        }
-    }
-
-CPTIMEOUT
-    This will set connection pooling timeout.
-    Possible values::
-
-        0 - Turn off connection pooling
-        nn - timeout set nn seconds
-
-CONN_TIMEOUT
-    This will set timeout for operations on connections (connection, ??closing??, we're not sure).
-    Possible values::
-
-        0 - Default timeout to the database (which could mean no timeout)
-        nn - timeout set nn seconds
-
-ISOLATION_LEVEL
-    This will set database isolation level at connection level
-    Possible values::
-
-        READ_COMMITED
-        READ_UNCOMMITTED
-        SERIALIZABLE
-
-LOCK_MODE_WAIT
-    This will set database LOCK MODE WAIT at connection level
-    Application can use this property to override the default server
-    process for accessing a locked row or table.
-    The default value is 0 (do not wait for the lock).
-    Possible values::
-
-        -1 - WAIT until the lock is released.
-        0 - DO NOT WAIT, end the operation, and return with error.
-        nn - WAIT for nn seconds for the lock to be released.
-
-VALIDATE_CONNECTION
-    Whether existing connections should be validated at the start of the request. Defaults to
-    `False`.
-
-VALIDATION_INTERVAL
-    How often in seconds to revalidate connections if `VALIDATE_CONNECTION` is enabled. Defaults to
-    `300` (5 minutes).
-
-VALIDATION_QUERY
-    Query used to validate whether a connection is usable. Defaults to
-    `"SELECT 1 FROM dual"`.
-
-CONNECTION_RETRY
-    When opening a new connection to the database, automatically retry up to ``MAX_ATTEMPTS`` times
-    in the case of errors. Only error codes in ``ERRORS`` will trigger a retry. The wait time
-    between retries is calculated using an exponential backoff with jitter formula::
-
-        random_between(WAIT_MIN, min(WAIT_MAX, WAIT_MULTIPLIER * WAIT_EXP_BASE ** (attempt - 1)))
-
-    Defaults (wait times are in milliseconds)::
-
-        MAX_ATTEMPTS: 1  # this implies no retries
-        WAIT_MIN: 0
-        WAIT_MAX: 1000
-        WAIT_MULTIPLIER: 25
-        WAIT_EXP_BASE: 2
-        ERRORS: ['-908', '-930', '-27001']
-
-    Each of these settings can be overridden in the ``CONNECTION_RETRY`` section of the database
-    configuration in ``settings.py``. For example::
-
-        DATABASES = {
-           'default': {
-               'ENGINE': 'django_gbasedbtdb',
-               'CONNECTION_RETRY': {
-                   'MAX_ATTEMPTS': 10,
-                   'WAIT_MIN': 0,
-                   'WAIT_MAX': 500,
-               },
-               # ...
-            },
-         }
-
-    The error codes that are retried by default correspond to the following errors:
-
-    * ``-908 Attempt to connect to database server (servername) failed``
-    * ``-930 Cannot connect to database server servername``
-    * ``-27001 Read error occurred during connection attempt``
-
-    These errors are often seen when the database server is too busy, too many clients are
-    attempting to connect at the same time or a network firewall has chopped the connection.
-
-
-.. note:
-    The ``DRIVER`` option is optional, default locations will be used per platform if it is not provided.
-
-.. note:
-    The ``TEST`` option sets test parametes.  Use ``NAME`` to override the name of the test database
-    and set ``CREATE_DB`` to ``False`` to prevent Django from attempting to create a new test
-    database.
-
-
-Testing against an GBase 8s Database
-------------------------------------
-
-Due to a bug in the GBase 8s ODBC driver, it is not currently possible to run Django tests normally. Specifically, it is not possible for Django to create a test database. As such, you will need to do it manually. By default Django will attempt to create a database with a name equal to the default database name with a ``test_`` prefix. e.g. if you database name is ``my_database``, the test database name would be ``test_my_database``.  This can be overridden with the ``NAME`` option under ``TEST``.
-
-To prevent Django from attempting to create a test database, set the ``CREATE_DB`` option
-under ``TEST`` to ``False``: see 'Configure settings.py' above.
-
-You can follow the steps above, in the section on using GBase 8s locally with Docker to create a test database. Then when running the test you can tell Django to re-use an existing database, rather than trying to create a new one with the ``-k`` parameter:
-
-.. code-block:: bash
-
-    ./manage.py test -k
-
-
-For django_gbasedbtdb Developers
---------------------------------
-
-To run the django_gbasedbtdb test suite, you need to set the GBASEDBTDIR environment variable, and the tests
-expect an GBase 8s database at host "gbase01". Change that host in `test/conftest.py` if you need to.
-Then run the test suite with:
-
-    tox
-
-This will run the tests under Django 2 and 3.
-
-
-Release History
----------------
-
-Version 1.10.1
-
-- Fork from django_informixdb
-
+        A database driver for Django to connect to an GBase 8s database via pyodbc.
+        
+        **Some limitations**:
+        
+        - Does not support default values
+        - GBase 8s automatically creates indexes on foreign keys, but Django attempts to do that
+          manually; the current implementation here just attempts to catch the error on index
+          creation. It may unintentionally catch other index creation errors where the index
+          already exists.
+        
+        
+        Configure local environment
+        ---------------------------
+        
+        The following environment variables should exist:
+        
+        GBASEDBTDIR
+            The path to the GBasedbt client install directory
+        
+        GBASEDBTSERVER
+            The name of the GBasedbt service to which we need to connect
+        
+        GBASEDBTSQLHOSTS
+            The path to the ``sqlhosts`` file that the GBasedbt driver should use
+        
+        LD_LIBRARY_PATH
+            The path(s) to the various GBasedbt library files: Usually
+            ``$GBASEDBTDIR/lib:$GBASEDBTDIR/lib/cli:$GBASEDBTDIR/lib/esql``
+        
+        DB_LOCALE
+            In case of ``Database locale information mismatch.`` error during connection,
+            you should specify your database locale, e.g. ``DB_LOCALE=en_US.8859-15``
+        
+        You will also need to add an entry within your ``sqlhosts`` file for each remote/local GBasedbt
+        server connection in the following format::
+        
+            <GBASEDBT_SERVER_NAME>    onsoctcp     <GBASEDBT_HOST_NAME>    <GBASEDBT_SERVICE_NAME>
+        
+        For example::
+        
+            dev    onsoctcp    localhost    9088
+        
+        You may alternatively use a symbolic name in that line in place of the port number, typically ``sqlexec`` and
+        then configure the port number in the ``/etc/services`` file::
+        
+            sqlexec    9088/tcp
+        
+        
+        Configure settings.py
+        ---------------------
+        
+        Django’s settings.py uses the following to connect to an GBasedbt database:
+        
+        .. code-block:: python
+        
+            'default': {
+                'ENGINE': 'django_gbasedbtdb',
+                'NAME': 'myproject',
+                'SERVER': 'ifxserver',
+                'USER' : 'testuser',
+                'PASSWORD': 'passw0rd',
+                'OPTIONS': {
+                    'DRIVER': '/path/to/iclit09b.so'. # Or iclit09b.dylib on macOS
+                    'CPTIMEOUT': 120,
+                    'CONN_TIMEOUT': 120,
+                    'ISOLATION_LEVEL': 'READ_UNCOMMITTED',
+                    'LOCK_MODE_WAIT': 0,
+                },
+                'CONNECTION_RETRY': {
+                    'MAX_ATTEMPTS': 10,
+                },
+                'TEST': {
+                    'NAME': 'myproject',
+                    'CREATE_DB': False
+                }
+            }
+        
+        CPTIMEOUT
+            This will set connection pooling timeout.
+            Possible values::
+        
+                0 - Turn off connection pooling
+                nn - timeout set nn seconds
+        
+        CONN_TIMEOUT
+            This will set timeout for operations on connections (connection, ??closing??, we're not sure).
+            Possible values::
+        
+                0 - Default timeout to the database (which could mean no timeout)
+                nn - timeout set nn seconds
+        
+        ISOLATION_LEVEL
+            This will set database isolation level at connection level
+            Possible values::
+        
+                READ_COMMITED
+                READ_UNCOMMITTED
+                SERIALIZABLE
+        
+        LOCK_MODE_WAIT
+            This will set database LOCK MODE WAIT at connection level
+            Application can use this property to override the default server
+            process for accessing a locked row or table.
+            The default value is 0 (do not wait for the lock).
+            Possible values::
+        
+                -1 - WAIT until the lock is released.
+                0 - DO NOT WAIT, end the operation, and return with error.
+                nn - WAIT for nn seconds for the lock to be released.
+        
+        CONNECTION_RETRY
+            When opening a new connection to the database, automatically retry up to ``MAX_ATTEMPTS`` times
+            in the case of errors. Only error codes in ``ERRORS`` will trigger a retry. The wait time
+            between retries is calculated using an exponential backoff with jitter formula::
+        
+                random_between(WAIT_MIN, min(WAIT_MAX, WAIT_MULTIPLIER * WAIT_EXP_BASE ** (attempt - 1)))
+        
+            Defaults (wait times are in milliseconds)::
+        
+                MAX_ATTEMPTS: 1  # this implies no retries
+                WAIT_MIN: 0
+                WAIT_MAX: 1000
+                WAIT_MULTIPLIER: 25
+                WAIT_EXP_BASE: 2
+                ERRORS: ['-908', '-930', '-27001']
+        
+            Each of these settings can be overridden in the ``CONNECTION_RETRY`` section of the database
+            configuration in ``settings.py``. For example::
+        
+                DATABASES = {
+                   'default': {
+                       'ENGINE': 'django_gbasedbtdb',
+                       'CONNECTION_RETRY': {
+                           'MAX_ATTEMPTS': 10,
+                           'WAIT_MIN': 0,
+                           'WAIT_MAX': 500,
+                       },
+                       # ...
+                    },
+                 }
+        
+            The error codes that are retried by default correspond to the following errors:
+        
+            * ``-908 Attempt to connect to database server (servername) failed``
+            * ``-930 Cannot connect to database server servername``
+            * ``-27001 Read error occurred during connection attempt``
+        
+            These errors are often seen when the database server is too busy, too many clients are
+            attempting to connect at the same time or a network firewall has chopped the connection.
+        
+        
+        .. note:
+            The ``DRIVER`` option is optional, default locations will be used per platform if it is not provided.
+        
+        .. note:
+            The ``TEST`` option sets test parametes.  Use ``NAME`` to override the name of the test database
+            and set ``CREATE_DB`` to ``False`` to prevent Django from attempting to create a new test
+            database.
+        
+        
+        For django_gbasedbtdb Developers
+        --------------------------------
+        
+        To run the django_gbasedbtdb test suite, you need to set the GBASEDBTDIR environment variable, and the tests
+        expect an GBasedbt database at host "dev". Change that host in `test/testproject/settings.py` if you need to.
+        Then run the test suite with:
+        
+            tox
+        
+        This will run the tests under Django 1 and 2.
+        
+        
+        Release History
+        ---------------
+        
+        Version 1.7.0
+        
+        - Fork from django_informixdb
+
```

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/base.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 import os
 import sys
 import platform
 import time
 import random
 import re
 
-from django.db import connections
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.base.validation import BaseDatabaseValidation
 from django.core.exceptions import ImproperlyConfigured
-from django.core import signals
+
+from django.utils.six import binary_type, text_type
 from django.utils.encoding import smart_str
 
 from .client import DatabaseClient
 from .creation import DatabaseCreation
 from .introspection import DatabaseIntrospection
 from .operations import DatabaseOperations
 from .features import DatabaseFeatures
@@ -34,15 +34,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def decoder(value, encodings=('utf-8',)):
     """This decoder tries multiple encodings before giving up"""
 
-    if not isinstance(value, bytes):
+    if not isinstance(value, binary_type):
         raise ValueError(f"Not a binary type: {value} {type(value)}")
 
     for enc in encodings:
         try:
             return value.decode(enc)
         except UnicodeDecodeError:
             pass
@@ -51,15 +51,15 @@
 
 
 class DatabaseWrapper(BaseDatabaseWrapper):
     vendor = 'gbasedbtdb'
     Database = pyodbc
 
     DRIVER_MAP = {
-        'DARWIN': '/Applications/GBS/gbasedbt/lib/cli/iclit09b.dylib',
+        'DARWIN': '/Applications/gbasedbt/lib/cli/iclit09b.dylib',
         'LINUX': '/opt/gbase/lib/cli/iclit09b.so',
         'WINDOWS32bit': 'GBase ODBC DRIVER',
         'WINDOWS64bit': 'GBase ODBC DRIVER (64-bit)',
     }
 
     ISOLATION_LEVEL = {
         'READ_COMMITED': pyodbc.SQL_TXN_READ_COMMITTED,
@@ -69,15 +69,15 @@
     }
 
     data_types = {
         'AutoField': 'serial',
         'BigAutoField': 'bigserial',
         'BinaryField': 'blob',
         'BooleanField': 'boolean',
-        'CharField': 'lvarchar(%(max_length)s)',
+        'CharField': 'varchar(%(max_length)s)',
         'CommaSeparatedIntegerField': 'lvarchar(%(max_length)s)',
         'DateField': 'date',
         'DateTimeField': 'datetime year to fraction(5)',
         'DecimalField': 'decimal',
         'DurationField': 'interval',
         'FileField': 'lvarchar(%(max_length)s)',
         'FilePathField': 'lvarchar(%(max_length)s)',
@@ -145,18 +145,14 @@
     validation_class = BaseDatabaseValidation
 
     def __init__(self, *args, **kwargs):
         super(DatabaseWrapper, self).__init__(*args, **kwargs)
 
         options = self.settings_dict.get('OPTIONS', {})
 
-        self._validation_enabled = options.get("VALIDATE_CONNECTION", False)
-        self._validation_interval = options.get("VALIDATION_INTERVAL", 300)
-        self._next_validation = time.time() + self._validation_interval
-        self._validation_query = options.get("VALIDATION_QUERY", "SELECT 1 FROM dual")
         self.encodings = options.get('encodings', ('utf-8', 'cp1252', 'iso-8859-1'))
         # make lookup operators to be collation-sensitive if needed
         self.collation = options.get('collation', None)
         if self.collation:
             self.operators = dict(self.__class__.operators)
             ops = {}
             for op in self.operators:
@@ -168,34 +164,14 @@
         self.features = self.features_class(self)
         self.ops = self.ops_class(self)
         self.client = self.client_class(self)
         self.creation = self.creation_class(self)
         self.introspection = self.introspection_class(self)
         self.validation = self.validation_class(self)
 
-    def validate_connection(self):
-        """
-        This method is invoked at the start of a request to verify an existing
-        connection is still functional. This is achieved by doing a simple query
-        against the database.
-        """
-        if not self._validation_enabled or time.time() < self._next_validation:
-            return
-
-        self._next_validation = time.time() + self._validation_interval
-
-        # We call close_if_unusable_or_obsolete to ensure obsolete connections
-        # are closed before we consider validating them. This will result in
-        # close_if_unusable_or_obsolete being called twice since it is also
-        # called automatically by django. This is ok since the second call is
-        # essentially a no-op.
-        self.close_if_unusable_or_obsolete()
-        if self.connection is not None and not self.is_usable():
-            self.close()
-
     def get_driver_path(self):
         system = platform.system().upper()
         if system == 'WINDOWS':
             system = system + platform.architecture()[0]
         try:
             return self.DRIVER_MAP[system]
         except KeyError:
@@ -213,17 +189,17 @@
         # Ensure the driver is set in the options
         options = conn_params.get('OPTIONS', {})
         if 'DRIVER' not in options or options['DRIVER'] is None:
             options['DRIVER'] = self.get_driver_path()
         if platform.system().upper() != 'WINDOWS':
             sqlhosts = os.environ.get('GBASEDBTSQLHOSTS')
             if not sqlhosts or not os.path.exists(sqlhosts):
-                raise ImproperlyConfigured('Cannot find GBase 8s sqlhosts at {}'.format(sqlhosts))
+                raise ImproperlyConfigured('Cannot find GBasedbt sqlhosts at {}'.format(sqlhosts))
             if not os.path.exists(options['DRIVER']):
-                raise ImproperlyConfigured('cannot find GBase 8s driver at {}'.format(options['DRIVER']))
+                raise ImproperlyConfigured('cannot find GBasedbt driver at {}'.format(options['DRIVER']))
         conn_params['OPTIONS'] = options
 
         conn_params['AUTOCOMMIT'] = False if 'AUTOCOMMIT' not in conn_params else conn_params['AUTOCOMMIT']
 
         return conn_params
 
     def get_new_connection(self, conn_params):
@@ -243,15 +219,15 @@
             parts.append('Uid={}'.format(conn_params['USER']))
         if 'PASSWORD' in conn_params:
             parts.append('Pwd={}'.format(conn_params['PASSWORD']))
         if 'CPTIMEOUT' in conn_params['OPTIONS']:
             parts.append('CPTimeout={}'.format(conn_params['OPTIONS']['CPTIMEOUT']))
 
         connection_string = ';'.join(parts)
-        logging.debug('Connecting to GBase 8s')
+        logging.debug('Connecting to GBasedbt')
         self.connection = self._get_connection_with_retries(connection_string, conn_params)
         self.connection.setencoding(encoding='UTF-8')
 
         # This will set database isolation level at connection level
         if 'ISOLATION_LEVEL' in conn_params['OPTIONS']:
             self.connection.set_attr(pyodbc.SQL_ATTR_TXN_ISOLATION,
                                      self.ISOLATION_LEVEL[conn_params['OPTIONS']['ISOLATION_LEVEL']])
@@ -263,16 +239,14 @@
         # This limit will not effect schema defined lengths, which will just
         # truncate values greater than the limit.
         self.connection.maxwrite = 32000
 
         self.connection.add_output_converter(-101, lambda r: r.decode('utf-8'))  # Constraints
         self.connection.add_output_converter(-391, lambda r: r.decode('utf-16-be'))  # Integrity Error
 
-        self.connection.add_output_converter(-114, self.handle_sql_infx_bigint_as_bigint)
-
         self.connection.add_output_converter(pyodbc.SQL_CHAR, self._output_converter)
         self.connection.add_output_converter(pyodbc.SQL_WCHAR, self._output_converter)
         self.connection.add_output_converter(pyodbc.SQL_VARCHAR, self._output_converter)
         self.connection.add_output_converter(pyodbc.SQL_WVARCHAR, self._output_converter)
         self.connection.add_output_converter(pyodbc.SQL_LONGVARCHAR, self._output_converter)
         self.connection.add_output_converter(pyodbc.SQL_WLONGVARCHAR, self._output_converter)
 
@@ -315,33 +289,30 @@
                 else:
                     raise
             else:
                 return conn
 
     def _unescape(self, raw):
         """
-        For some reason the GBase 8s ODBC driver seems to double escape new line characters.
+        For some reason the GBasedbt ODBC driver seems to double escape new line characters.
 
         This little handler converts them back.
 
         @todo: See if this applies to other escape characters
         """
         return raw.replace(b'\\n', b'\n')
 
     def _output_converter(self, raw):
         return decoder(self._unescape(raw), self.encodings)
 
-    def handle_sql_infx_bigint_as_bigint(self, value):
-        return int.from_bytes(value, byteorder='little', signed=False) 
-
     def init_connection_state(self):
         pass
 
     def create_cursor(self, name=None):
-        logging.debug('Creating GBase 8s cursor')
+        logging.debug('Creating GBasedbt cursor')
         return CursorWrapper(self.connection.cursor(), self)
 
     def _set_autocommit(self, autocommit):
         with self.wrap_database_errors:
             self.connection.autocommit = autocommit
 
     def check_constraints(self, table_names=None):
@@ -356,40 +327,21 @@
         """
         Start a transaction explicitly in autocommit mode.
         """
         start_sql = self.ops.start_transaction_sql()
         self.cursor().execute(start_sql)
 
     def is_usable(self):
-        # We create a cursor and then explicitly close it as there is a bug
-        # that is encountered when relying on garbage collection to close the
-        # cursor: https://github.com/mkleehammer/pyodbc/issues/585
         try:
-            cursor = self.connection.cursor()
-        except pyodbc.Error as exc:
-            logger.info(f"error creating cursor: {exc}")
+            # Use a cursor directly, bypassing Django's utilities.
+            self.connection.cursor().execute("SELECT 1")
+        except pyodbc.Error:
             return False
-
-        try:
-            cursor.execute(self._validation_query)
+        else:
             return True
-        except pyodbc.Error as exc:
-            logger.info(f"error executing query: {exc}")
-            return False
-        finally:
-            # We close the cursor explicitly to work around the pyodbc bug
-            # described at the top of this function. If closing the cursor
-            # fails we set the return value to `False`. Otherwise it
-            # remains what was returned in the `try` or `except` block, which
-            # depends on whether `cursor.execute` succeeded or not.
-            try:
-                cursor.close()
-            except pyodbc.Error as exc:
-                logger.info(f"error closing cursor: {exc}")
-                return False
 
     def read_dirty(self):
         self.cursor().execute('set isolation to dirty read;')
 
     def read_committed(self):
         self.cursor().execute('set isolation to committed read;')
 
@@ -445,15 +397,15 @@
 
     def close(self):
         if self.active:
             self.active = False
             self.cursor.close()
 
     def format_sql(self, sql, params):
-        if isinstance(sql, str):
+        if isinstance(sql, text_type):
             # FreeTDS (and other ODBC drivers?) doesn't support Unicode
             # yet, so we need to encode the SQL clause itself in utf-8
             sql = smart_str(sql, self.driver_charset)
 
         # pyodbc uses '?' instead of '%s' as parameter placeholder.
         if params is not None:
             pass
@@ -461,23 +413,23 @@
 
         return sql
 
     def format_params(self, params):
         fp = []
         if params is not None:
             for p in params:
-                if isinstance(p, str):
+                if isinstance(p, text_type):
                     if self.driver_charset:
                         # FreeTDS (and other ODBC drivers?) doesn't support Unicode
                         # yet, so we need to encode parameters in utf-8
                         fp.append(smart_str(p, self.driver_charset))
                     else:
                         fp.append(p)
 
-                elif isinstance(p, bytes):
+                elif isinstance(p, binary_type):
                     fp.append(p)
 
                 elif isinstance(p, type(True)):
                     if p:
                         fp.append(1)
                     else:
                         fp.append(0)
@@ -511,15 +463,15 @@
         (pyodbc Rows are not sliceable).
         """
         if self.driver_charset:
             for i in range(len(row)):
                 f = row[i]
                 # FreeTDS (and other ODBC drivers?) doesn't support Unicode
                 # yet, so we need to decode utf-8 data coming from the DB
-                if isinstance(f, bytes):
+                if isinstance(f, binary_type):
                     row[i] = f.decode(self.driver_charset)
         return tuple(row)
 
     def fetchone(self):
         row = self.cursor.fetchone()
         if row is not None:
             row = self.format_row(row)
@@ -537,16 +489,7 @@
     def __getattr__(self, attr):
         if attr in self.__dict__:
             return self.__dict__[attr]
         return getattr(self.cursor, attr)
 
     def __iter__(self):
         return iter(self.cursor)
-
-
-def _validate_connection(**kwargs):
-    for conn in connections.all():
-        if isinstance(conn, DatabaseWrapper):
-            conn.validate_connection()
-
-
-signals.request_started.connect(_validate_connection)
```

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/client.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/client.py`

 * *Files identical despite different names*

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/compiler.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/compiler.py`

 * *Files identical despite different names*

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/creation.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/creation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class DatabaseCreation(BaseDatabaseCreation):
 
     def sql_table_creation_suffix(self):
         test_settings = self.connection.settings_dict['TEST']
         assert test_settings['COLLATION'] is None, (
-            "GBase 8s does not support collation setting at database creation time."
+            "GBasedbt does not support collation setting at database creation time."
         )
         if test_settings['CHARSET']:
             return "WITH ENCODING '%s'" % test_settings['CHARSET']
         return 'WITH BUFFERED LOG'
 
     def create_test_db(self, verbosity=1, autoclobber=False, serialize=True, keepdb=False):
         """
```

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/datatypes.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/datatypes.py`

 * *Files identical despite different names*

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/features.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/features.py`

 * *Files identical despite different names*

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/fields.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/fields.py`

 * *Files identical despite different names*

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/introspection.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/introspection.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,40 +13,33 @@
         # We want to ignore all the internal 'sys' tables in the exclude list
         return [
             TableInfo(x[0], x[1].lower()) for x in cursor.fetchall()
             if x[0] not in EXCLUDED_TABLES
         ]
 
     def get_table_description(self, cursor, table_name):
-        """Returns a description of the table, with the DB-API cursor.description interface.
-
-        The FieldInfo metadata must be provided in the format described in Django's
-        django/db/backends/base/introspection.py:
-
-        name, type_code, display_size, internal_size, precision, scale, null_ok, default, collation
-
-        At present, this driver doesn't support table-specific collation settings, but Django
-        requires a collation value in the FieldInfo, so None is used.
-        """
+        "Returns a description of the table, with the DB-API cursor.description interface."
         query_format = """
             SELECT c.*
             FROM syscolumns c
             JOIN systables t
             ON c.tabid=t.tabid
             WHERE t.tabname='{}'
         """
 
         cursor.execute(query_format.format(table_name))
-        columns = [[c[0], c[3] % 256, None, c[4], c[4], None, 0 if c[3] > 256 else 1, None, None]
+        columns = [[c[0], c[3] % 256, None, c[4], c[4], None, 0 if c[3] > 256 else 1, None]
                    for c in cursor.fetchall()]
         items = []
         for column in columns:
             if column[1] in (GBasedbtTypes.SQL_TYPE_NUMERIC.num, GBasedbtTypes.SQL_TYPE_DECIMAL.num):
                 column[4] = int(column[3] / 256)
                 column[5] = column[3] - column[4] * 256
+            # FieldInfo:
+            #   name, type_code, display_size, internal_size, precision, scale, null_ok, default
             items.append(FieldInfo(*column))
 
         return items
 
     def get_key_columns(self, cursor, table_name):
         key_columns_query = """
             SELECT col1.colname AS column_name,
```

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/operations.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,19 +117,16 @@
         # since gbasedbt only support fraction(5),
         # we need remove the last digit for micro-seconds
         return value.strftime('%Y-%m-%d %H:%M:%S.f')[:-1] if value else value
 
     def adapt_timefield_value(self, value):
         return value
 
-    def sql_flush(self, style, tables, sequences=(), reset_sequences=True, allow_cascade=False):
-        # The reset_sequences keyword arg is provided by Django 3.1 and later,
-        # but like the sequences arg, it is ignored by this driver.
-
-        # NB: The generated SQL below is specific to GBase 8s 
+    def sql_flush(self, style, tables, sequences, allow_cascade=False):
+        # NB: The generated SQL below is specific to GBasedbt
         sql = ['%s %s %s;' % (
             style.SQL_KEYWORD('DELETE'),
             style.SQL_KEYWORD('FROM'),
             style.SQL_FIELD(self.quote_name(table))
         ) for table in tables]
         return sql
```

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/schema.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     sql_alter_column_type = "MODIFY %(column)s %(type)s"
     sql_alter_column_default = "MODIFY %(column)s DEFAULT "
     sql_alter_column_no_default = "MODIFY %(column)s DROP DEFAULT"
     sql_delete_column = "ALTER TABLE %(table)s DROP %(column)s"
 
     def execute(self, sql, params=[]):
         """
-        GBase 8s adds an index to foreign keys automatically
+        GBasedbt adds an index to foreign keys automatically
 
         This silences the error when Django tries to do the same thing independently
         """
         try:
             super(DatabaseSchemaEditor, self).execute(sql, params)
         except (ProgrammingError, DatabaseError) as e:
             if "CREATE INDEX" not in str(sql) and 'Index already exists' not in str(e):
```

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb/tableignore.py` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb/tableignore.py`

 * *Files identical despite different names*

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb.egg-info/PKG-INFO` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 Metadata-Version: 2.1
 Name: django-gbasedbtdb
-Version: 1.10.1
-Summary: A database driver for Django to connect to an GBase 8s database via ODBC
+Version: 1.7.0
+Summary: A database driver for Django to connect to an GBase 8s db via ODBC
 Home-page: https://gbasedbt.com
 Author: liaosnet
 Author-email: liaosnet@gbasedbt.com
 License: APLv2
 Keywords: django gbasedbt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
 
 ## A database driver for Django to connect to an GBase 8s database via pyodbc.  
 
 **Some limitations**:
 
 - Does not support default values  
 - GBase 8s automatically creates indexes on foreign keys, but Django attempts to do that
   manually; the current implementation here just attempts to catch the error on index
   creation. It may unintentionally catch other index creation errors where the index
   already exists.
 
 ### Release History  
 
-Version 1.10.1  
+Version 1.7.0  
 
 - Fork from django_informixdb  
-- Fix 'unsupported column type -114'
```

### Comparing `django_gbasedbtdb-1.10.1/django_gbasedbtdb.egg-info/SOURCES.txt` & `django_gbasedbtdb-1.7.0/django_gbasedbtdb.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 README.rst
 setup.cfg
 setup.py
 django_gbasedbtdb/__init__.py
 django_gbasedbtdb/base.py
 django_gbasedbtdb/client.py
@@ -17,15 +16,8 @@
 django_gbasedbtdb/tableignore.py
 django_gbasedbtdb/utils.py
 django_gbasedbtdb.egg-info/PKG-INFO
 django_gbasedbtdb.egg-info/SOURCES.txt
 django_gbasedbtdb.egg-info/dependency_links.txt
 django_gbasedbtdb.egg-info/requires.txt
 django_gbasedbtdb.egg-info/top_level.txt
-test/__init__.py
-test/conftest.py
-test/test_base.py
-test/test_integration.py
-test/urls.py
-test/datatypes/__init__.py
-test/datatypes/models.py
-test/datatypes/test_datatypes.py
+test/test_base.py
```

### Comparing `django_gbasedbtdb-1.10.1/setup.py` & `django_gbasedbtdb-1.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,32 @@
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='django_gbasedbtdb',
     version=__version__,
-    description='A database driver for Django to connect to an GBase 8s database via ODBC',
+    description='A database driver for Django to connect to an GBase 8s db via ODBC',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://gbasedbt.com',
     author='liaosnet',
     author_email='liaosnet@gbasedbt.com',
     license='APLv2',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
     ],
     keywords='django gbasedbt',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
-    install_requires=['django>=2.2.0,<4', 'pyodbc~=4.0.21'],
+    install_requires=['django>=1.9.6', 'pyodbc>=4.0.21'],
     extras_require={
         'dev': ['check-manifest'],
         'test': ['coverage'],
     },
 )
```

