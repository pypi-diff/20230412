# Comparing `tmp/bitsmiths-mettle-2.2.8.tar.gz` & `tmp/bitsmiths-mettle-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitsmiths-mettle-2.2.8.tar", last modified: Wed Apr  5 08:21:36 2023, max compression
+gzip compressed data, was "bitsmiths-mettle-2.2.9.tar", last modified: Wed Apr 12 15:24:59 2023, max compression
```

## Comparing `bitsmiths-mettle-2.2.8.tar` & `bitsmiths-mettle-2.2.9.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.697228 bitsmiths-mettle-2.2.8/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)       89 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/.gitignore
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     1142 2023-04-05 08:21:36.000000 bitsmiths-mettle-2.2.8/LICENCE
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5821 2023-04-05 08:21:36.697228 bitsmiths-mettle-2.2.8/PKG-INFO
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     4443 2023-04-05 08:20:44.000000 bitsmiths-mettle-2.2.8/README.md
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.693228 bitsmiths-mettle-2.2.8/bitsmiths_mettle.egg-info/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5821 2023-04-05 08:21:36.000000 bitsmiths-mettle-2.2.8/bitsmiths_mettle.egg-info/PKG-INFO
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     8758 2023-04-05 08:21:36.000000 bitsmiths-mettle-2.2.8/bitsmiths_mettle.egg-info/SOURCES.txt
--rw-rw-r--   0 bitter    (1000) bitter    (1000)        1 2023-04-05 08:21:36.000000 bitsmiths-mettle-2.2.8/bitsmiths_mettle.egg-info/dependency_links.txt
--rw-rw-r--   0 bitter    (1000) bitter    (1000)       81 2023-04-05 08:21:36.000000 bitsmiths-mettle-2.2.8/bitsmiths_mettle.egg-info/entry_points.txt
--rw-rw-r--   0 bitter    (1000) bitter    (1000)        1 2023-04-05 08:21:36.000000 bitsmiths-mettle-2.2.8/bitsmiths_mettle.egg-info/not-zip-safe
--rw-rw-r--   0 bitter    (1000) bitter    (1000)      251 2023-04-05 08:21:36.000000 bitsmiths-mettle-2.2.8/bitsmiths_mettle.egg-info/requires.txt
--rw-rw-r--   0 bitter    (1000) bitter    (1000)        7 2023-04-05 08:21:36.000000 bitsmiths-mettle-2.2.8/bitsmiths_mettle.egg-info/top_level.txt
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.661229 bitsmiths-mettle-2.2.8/mettle/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2670 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2173 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/__main__.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.669228 bitsmiths-mettle-2.2.8/mettle/braze/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     4174 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2899 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/bool_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2901 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/char_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     4891 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/client.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2901 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/date_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2916 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/datetime_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2911 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/double_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2906 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/float_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2901 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/guid_list.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.669228 bitsmiths-mettle-2.2.8/mettle/braze/http/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2557 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/http/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2488 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/http/http_header.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     6985 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/http/transport_client.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2557 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/http/transport_client_settings.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5237 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/http/transport_server.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2262 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/http/transport_server_settings.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2403 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/iclient_marshaler.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2906 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/int16_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2906 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/int32_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2906 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/int64_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2902 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/int8_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     4278 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/iserver_interface.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2676 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/iserver_marshaler.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5681 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/itransport.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2255 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/itransport_settings.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2901 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/json_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2915 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/memblock_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    12727 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/rdc.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3568 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/rpc_header.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    15319 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/server.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5407 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/server_multimarsh.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2911 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/string_list.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.673228 bitsmiths-mettle-2.2.8/mettle/braze/tcp/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2717 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/tcp/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     7284 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/tcp/socket_tcp.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     4470 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/tcp/socket_tcp_client.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     8135 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/tcp/socket_tcp_server.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3258 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/tcp/tcp_header.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     6429 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/tcp/transport_client.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2785 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/tcp/transport_client_settings.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     6968 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/tcp/transport_server.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3207 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/tcp/transport_server_settings.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2902 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/time_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2911 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/uint16_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2911 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/uint32_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2911 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/uint64_list.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2906 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/braze/uint8_list.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.673228 bitsmiths-mettle-2.2.8/mettle/db/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2584 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2673 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/db_lock.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.673228 bitsmiths-mettle-2.2.8/mettle/db/encode_io_databases/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)        0 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/encode_io_databases/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     9440 2023-03-13 15:37:02.000000 bitsmiths-mettle-2.2.8/mettle/db/encode_io_databases/aconnect.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5306 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/encode_io_databases/aconnect_postgres.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2548 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/encode_io_databases/statement.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     7563 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/iaconnect.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     9179 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/iconnect.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3146 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/iprimary_key.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.673228 bitsmiths-mettle-2.2.8/mettle/db/psycopg2/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2106 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/psycopg2/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    14405 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/psycopg2/connect.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2554 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/psycopg2/statement.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.677228 bitsmiths-mettle-2.2.8/mettle/db/psycopg3/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2106 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/psycopg3/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    14393 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/psycopg3/aconnect.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2566 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/psycopg3/astatement.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    14036 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/psycopg3/connect.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2554 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/psycopg3/statement.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.677228 bitsmiths-mettle-2.2.8/mettle/db/sqlalc/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2106 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/sqlalc/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     8751 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/sqlalc/connect.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     6211 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/sqlalc/connect_postgres.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2674 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/sqlalc/statement.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.677228 bitsmiths-mettle-2.2.8/mettle/db/sqlite/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2106 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/sqlite/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     9605 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/sqlite/connect.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2553 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/sqlite/statement.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2510 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/sqlvar.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     8474 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/db/statement.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.677228 bitsmiths-mettle-2.2.8/mettle/genes/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     6976 2023-04-05 08:18:23.000000 bitsmiths-mettle-2.2.8/mettle/genes/__init__.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.681228 bitsmiths-mettle-2.2.8/mettle/genes/braze/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2789 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/braze/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    59745 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/braze/gen_cpp.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    35353 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/braze/gen_js.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    84595 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/braze/gen_py3.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    42127 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/braze/gen_ts.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    20269 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/braze/generator.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    22566 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/braze_project.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5703 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/common.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2473 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/data_types.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     8763 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/database_project.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.689228 bitsmiths-mettle-2.2.8/mettle/genes/db/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3518 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     8573 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/database.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3529 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/db_mssql.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2500 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/db_oracle.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2704 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/db_postgres.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3121 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/db_sqlite.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2366 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/db_std.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    75649 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/gen_cpp.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    22692 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/gen_js.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    95136 2023-03-13 15:37:02.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/gen_py3.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    22930 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/gen_py3sqlalchemy.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    12625 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/gen_sql.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     9099 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/gen_sql_mssql.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     8054 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/gen_sql_postgres.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     7282 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/gen_sql_sqlite.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    28023 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/gen_ts.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    29794 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/generator.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    14502 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/db/table.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.689228 bitsmiths-mettle-2.2.8/mettle/genes/mk/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2853 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/mk/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     7925 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/mk/gen_angular.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    24517 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/mk/gen_cpp.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5590 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/mk/gen_mettleproj.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    10151 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/mk/gen_mksln.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5317 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/mk/gen_pythondist.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    14366 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/mk/generator.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     4967 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/mk_project.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3632 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/project.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    26653 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/service.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    11219 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/genes/zip_buddy.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.693228 bitsmiths-mettle-2.2.8/mettle/io/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2366 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     7590 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/big_endian_reader.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     7347 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/big_endian_writer.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3962 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/dict_stream.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     7401 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/ireader.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3007 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/iserializable.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3733 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/istream.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     7501 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/iwriter.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3961 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/list_stream.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     4070 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/memory_stream.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     8813 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/py_dict_reader.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     6885 2023-03-13 15:37:02.000000 bitsmiths-mettle-2.2.8/mettle/io/py_dict_writer.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5966 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/py_json_dict_reader.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3907 2023-03-13 15:37:02.000000 bitsmiths-mettle-2.2.8/mettle/io/py_json_dict_writer.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5754 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/py_json_list_reader.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     4047 2023-03-13 15:37:02.000000 bitsmiths-mettle-2.2.8/mettle/io/py_json_list_writer.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5373 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/py_list_reader.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5202 2023-03-13 15:37:02.000000 bitsmiths-mettle-2.2.8/mettle/io/py_list_writer.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    13542 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/io/util.py
-drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-05 08:21:36.693228 bitsmiths-mettle-2.2.8/mettle/lib/
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2474 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/lib/__init__.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)    12778 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/lib/dav.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     9936 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/lib/dav_cache.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     3023 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/lib/ref.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5002 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/lib/timezone.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     5372 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/lib/xmettle.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2646 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/mettle/lib/xterminate.py
--rw-rw-r--   0 bitter    (1000) bitter    (1000)      151 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/pip-requirements.txt
--rw-rw-r--   0 bitter    (1000) bitter    (1000)      106 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/pyproject.toml
--rw-rw-r--   0 bitter    (1000) bitter    (1000)     2001 2023-04-05 08:21:36.697228 bitsmiths-mettle-2.2.8/setup.cfg
--rw-rw-r--   0 bitter    (1000) bitter    (1000)      211 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.8/setup.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.367325 bitsmiths-mettle-2.2.9/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)       89 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/.gitignore
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     1142 2023-04-12 15:24:59.000000 bitsmiths-mettle-2.2.9/LICENCE
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     6030 2023-04-12 15:24:59.367325 bitsmiths-mettle-2.2.9/PKG-INFO
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     4652 2023-04-12 15:24:31.000000 bitsmiths-mettle-2.2.9/README.md
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.363325 bitsmiths-mettle-2.2.9/bitsmiths_mettle.egg-info/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     6030 2023-04-12 15:24:59.000000 bitsmiths-mettle-2.2.9/bitsmiths_mettle.egg-info/PKG-INFO
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     8758 2023-04-12 15:24:59.000000 bitsmiths-mettle-2.2.9/bitsmiths_mettle.egg-info/SOURCES.txt
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)        1 2023-04-12 15:24:59.000000 bitsmiths-mettle-2.2.9/bitsmiths_mettle.egg-info/dependency_links.txt
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)       81 2023-04-12 15:24:59.000000 bitsmiths-mettle-2.2.9/bitsmiths_mettle.egg-info/entry_points.txt
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)        1 2023-04-12 15:24:59.000000 bitsmiths-mettle-2.2.9/bitsmiths_mettle.egg-info/not-zip-safe
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)      251 2023-04-12 15:24:59.000000 bitsmiths-mettle-2.2.9/bitsmiths_mettle.egg-info/requires.txt
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)        7 2023-04-12 15:24:59.000000 bitsmiths-mettle-2.2.9/bitsmiths_mettle.egg-info/top_level.txt
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.335325 bitsmiths-mettle-2.2.9/mettle/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2670 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2173 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/__main__.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.339325 bitsmiths-mettle-2.2.9/mettle/braze/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     4174 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2899 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/bool_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2901 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/char_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     4891 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/client.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2901 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/date_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2916 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/datetime_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2911 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/double_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2906 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/float_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2901 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/guid_list.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.339325 bitsmiths-mettle-2.2.9/mettle/braze/http/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2557 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/http/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2488 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/http/http_header.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     6985 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/http/transport_client.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2557 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/http/transport_client_settings.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5237 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/http/transport_server.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2262 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/http/transport_server_settings.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2403 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/iclient_marshaler.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2906 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/int16_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2906 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/int32_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2906 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/int64_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2902 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/int8_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     4278 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/iserver_interface.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2676 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/iserver_marshaler.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5681 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/itransport.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2255 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/itransport_settings.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2901 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/json_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2915 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/memblock_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    12727 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/rdc.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3568 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/rpc_header.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    15319 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/server.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5407 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/server_multimarsh.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2911 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/string_list.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.343325 bitsmiths-mettle-2.2.9/mettle/braze/tcp/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2717 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/tcp/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     7284 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/tcp/socket_tcp.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     4470 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/tcp/socket_tcp_client.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     8135 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/tcp/socket_tcp_server.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3258 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/tcp/tcp_header.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     6429 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/tcp/transport_client.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2785 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/tcp/transport_client_settings.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     6968 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/tcp/transport_server.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3207 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/tcp/transport_server_settings.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2902 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/time_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2911 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/uint16_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2911 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/uint32_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2911 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/uint64_list.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2906 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/braze/uint8_list.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.343325 bitsmiths-mettle-2.2.9/mettle/db/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2584 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2673 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/db_lock.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.343325 bitsmiths-mettle-2.2.9/mettle/db/encode_io_databases/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)        0 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/encode_io_databases/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     9440 2023-04-12 15:20:08.000000 bitsmiths-mettle-2.2.9/mettle/db/encode_io_databases/aconnect.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5306 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/encode_io_databases/aconnect_postgres.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2548 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/encode_io_databases/statement.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     7563 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/iaconnect.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     9179 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/iconnect.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3146 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/iprimary_key.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.343325 bitsmiths-mettle-2.2.9/mettle/db/psycopg2/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2106 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/psycopg2/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    14405 2023-04-12 15:20:21.000000 bitsmiths-mettle-2.2.9/mettle/db/psycopg2/connect.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2554 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/psycopg2/statement.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.343325 bitsmiths-mettle-2.2.9/mettle/db/psycopg3/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2106 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/psycopg3/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    14393 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/psycopg3/aconnect.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2566 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/psycopg3/astatement.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    14036 2023-04-12 15:20:21.000000 bitsmiths-mettle-2.2.9/mettle/db/psycopg3/connect.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2554 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/psycopg3/statement.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.343325 bitsmiths-mettle-2.2.9/mettle/db/sqlalc/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2106 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/sqlalc/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     8751 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/sqlalc/connect.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     6211 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/sqlalc/connect_postgres.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2674 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/sqlalc/statement.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.347325 bitsmiths-mettle-2.2.9/mettle/db/sqlite/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2106 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/sqlite/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     9605 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/sqlite/connect.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2553 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/sqlite/statement.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2510 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/sqlvar.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     8474 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/db/statement.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.347325 bitsmiths-mettle-2.2.9/mettle/genes/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     6976 2023-04-12 15:20:08.000000 bitsmiths-mettle-2.2.9/mettle/genes/__init__.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.351325 bitsmiths-mettle-2.2.9/mettle/genes/braze/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2789 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/braze/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    59745 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/braze/gen_cpp.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    35353 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/braze/gen_js.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    84595 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/braze/gen_py3.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    42127 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/braze/gen_ts.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    20269 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/braze/generator.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    22566 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/braze_project.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5703 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/common.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2473 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/data_types.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     8763 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/database_project.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.355325 bitsmiths-mettle-2.2.9/mettle/genes/db/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3518 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     8573 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/database.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3529 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/db_mssql.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2500 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/db_oracle.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2704 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/db_postgres.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3121 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/db_sqlite.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2366 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/db_std.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    75649 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/gen_cpp.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    22692 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/gen_js.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    95136 2023-04-12 15:20:08.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/gen_py3.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    22930 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/gen_py3sqlalchemy.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    12625 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/gen_sql.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     9099 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/gen_sql_mssql.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     8054 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/gen_sql_postgres.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     7282 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/gen_sql_sqlite.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    28023 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/gen_ts.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    29794 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/generator.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    14502 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/db/table.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.355325 bitsmiths-mettle-2.2.9/mettle/genes/mk/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2853 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/mk/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     7925 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/mk/gen_angular.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    24517 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/mk/gen_cpp.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5590 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/mk/gen_mettleproj.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    10151 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/mk/gen_mksln.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5317 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/mk/gen_pythondist.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    14366 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/mk/generator.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     4967 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/mk_project.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3632 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/project.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    26653 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/service.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    11219 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/genes/zip_buddy.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.359325 bitsmiths-mettle-2.2.9/mettle/io/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2366 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     7590 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/big_endian_reader.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     7347 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/big_endian_writer.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3962 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/dict_stream.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     7401 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/ireader.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3007 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/iserializable.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3733 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/istream.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     7501 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/iwriter.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3961 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/list_stream.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     4070 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/memory_stream.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     8813 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/py_dict_reader.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     6885 2023-03-13 15:37:02.000000 bitsmiths-mettle-2.2.9/mettle/io/py_dict_writer.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5966 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/py_json_dict_reader.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3907 2023-03-13 15:37:02.000000 bitsmiths-mettle-2.2.9/mettle/io/py_json_dict_writer.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5754 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/py_json_list_reader.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     4047 2023-03-13 15:37:02.000000 bitsmiths-mettle-2.2.9/mettle/io/py_json_list_writer.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5373 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/py_list_reader.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5202 2023-03-13 15:37:02.000000 bitsmiths-mettle-2.2.9/mettle/io/py_list_writer.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    13542 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/io/util.py
+drwxrwxr-x   0 bitter    (1000) bitter    (1000)        0 2023-04-12 15:24:59.363325 bitsmiths-mettle-2.2.9/mettle/lib/
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2474 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/lib/__init__.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)    12778 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/lib/dav.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     9936 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/lib/dav_cache.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     3023 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/lib/ref.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5002 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/lib/timezone.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     5372 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/lib/xmettle.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2646 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/mettle/lib/xterminate.py
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)      151 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/pip-requirements.txt
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)      106 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/pyproject.toml
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)     2001 2023-04-12 15:24:59.367325 bitsmiths-mettle-2.2.9/setup.cfg
+-rw-rw-r--   0 bitter    (1000) bitter    (1000)      211 2023-01-10 13:18:37.000000 bitsmiths-mettle-2.2.9/setup.py
```

### Comparing `bitsmiths-mettle-2.2.8/LICENCE` & `bitsmiths-mettle-2.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/PKG-INFO` & `bitsmiths-mettle-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitsmiths-mettle
-Version: 2.2.8
+Version: 2.2.9
 Summary: A three tier systems code generator that targets serveral databases and languages
 Home-page: https://bitbucket.org/bitsmiths_za/mettle.git
 Author: Nicolas Milicevic, Steven van Niekerk, Darrly Daniels
 Author-email: nicolas@bitsmiths.co.za, steven@bitsmiths.co.za, darryl@bitsmiths.co.za
 License: MIT
 Project-URL: Source, https://bitbucket.org/bitsmiths_za/mettle.git
 Keywords: generators,libraries
@@ -51,14 +51,21 @@
 $ pip install bitsmiths-mettle
 
 ---> 100%
 ```
 
 ## Change History ##
 
+### 2.2.9 ###
+
+| Type   | Description |
+| ------ | ----------- |
+| Fix | Fixed an exception priority issue with the `mettle-psycopg` driver where reset connections were being caught by the lock exception. |
+
+
 ### 2.2.8 ###
 
 | Type   | Description |
 | ------ | ----------- |
 | New | The `mettle-sql-build` entry point in the python package now accepts wild card inputs.  |
 
 ### 2.2.7 ###
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bitsmiths-mettle Version: 2.2.8 Summary: A three
+Metadata-Version: 2.1 Name: bitsmiths-mettle Version: 2.2.9 Summary: A three
 tier systems code generator that targets serveral databases and languages Home-
 page: https://bitbucket.org/bitsmiths_za/mettle.git Author: Nicolas Milicevic,
 Steven van Niekerk, Darrly Daniels Author-email: nicolas@bitsmiths.co.za,
 steven@bitsmiths.co.za, darryl@bitsmiths.co.za License: MIT Project-URL:
 Source, https://bitbucket.org/bitsmiths_za/mettle.git Keywords:
 generators,libraries Platform: unix Platform: linux Platform: osx Platform:
 cygwin Platform: win32 Classifier: Development Status :: 5 - Production/Stable
@@ -16,29 +16,32 @@
 Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
 postgresql_psycopg2 Provides-Extra: postgresql_psycopg3 Provides-Extra:
 postgresql_async Provides-Extra: sqlite_async Provides-Extra: sqlalchemy
 License-File: LICENCE # Mettle # Bitsmiths-Mettle is the supporting code
 generators and python libraries for the Mettle project. See our repo and main
 *README* for more details! ## Requirements ## Python 3.10+ ## Installation ##
 ```console $ pip install bitsmiths-mettle ---> 100% ``` ## Change History ##
-### 2.2.8 ### | Type | Description | | ------ | ----------- | | New | The
-`mettle-sql-build` entry point in the python package now accepts wild card
-inputs. | ### 2.2.7 ### | Type | Description | | ------ | ----------- | | Fix |
-Python database table generetor respects not null columns that are integers and
-floats properly for pydantic and dataclass generation. | ### 2.2.6 ### | Type |
-Description | | ------ | ----------- | | Fix | The python encoded.databases
-[postgresql] driver was not handling null floats. Bug squashed. | ### 2.2.5 ###
-| Type | Description | | ------ | ----------- | | Fix | Changed PostgreSQL
-package dependency from `postgres` to `postgresql`. | | Fix | The python braze
-serializers now use `isinstance` instead of `type` when checking value types. |
-### 2.2.4 ### | Type | Description | | ------ | ----------- | | Fix | Improved
-package dependencies, thank-you Bradley Kirton. | | New | Added a new optional
-`global-settings.file-header` setting to projects. Allows customization or
-removal or the generated header in all generated files. | ### 2.2.3 ### | Type
-| Description | | ------ | ----------- | | New | Implemented auto (reset) to
+### 2.2.9 ### | Type | Description | | ------ | ----------- | | Fix | Fixed an
+exception priority issue with the `mettle-psycopg` driver where reset
+connections were being caught by the lock exception. | ### 2.2.8 ### | Type |
+Description | | ------ | ----------- | | New | The `mettle-sql-build` entry
+point in the python package now accepts wild card inputs. | ### 2.2.7 ### |
+Type | Description | | ------ | ----------- | | Fix | Python database table
+generetor respects not null columns that are integers and floats properly for
+pydantic and dataclass generation. | ### 2.2.6 ### | Type | Description | | ---
+--- | ----------- | | Fix | The python encoded.databases[postgresql] driver was
+not handling null floats. Bug squashed. | ### 2.2.5 ### | Type | Description |
+| ------ | ----------- | | Fix | Changed PostgreSQL package dependency from
+`postgres` to `postgresql`. | | Fix | The python braze serializers now use
+`isinstance` instead of `type` when checking value types. | ### 2.2.4 ### |
+Type | Description | | ------ | ----------- | | Fix | Improved package
+dependencies, thank-you Bradley Kirton. | | New | Added a new optional `global-
+settings.file-header` setting to projects. Allows customization or removal or
+the generated header in all generated files. | ### 2.2.3 ### | Type |
+Description | | ------ | ----------- | | New | Implemented auto (reset) to
 database connections on failure for all python database drivers. (This excludes
 `asynpg` because it uses a pool that does it for us). | | Bug | Fixed a python
 async code generation issue, where some `methods` and `with` statements were
 not using await or async. | ### 2.2.2 ### | Type | Description | | ------ | ---
 -------- | | Fix | Fixed an import issue with the Braze TCP overload in python.
 | ### 2.2.1 ### | Type | Description | | ------ | ----------- | | Fix | Applied
 `couplet` identifier improvement to braze couplets on python. | ### 2.2.0 ### |
```

### Comparing `bitsmiths-mettle-2.2.8/README.md` & `bitsmiths-mettle-2.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 $ pip install bitsmiths-mettle
 
 ---> 100%
 ```
 
 ## Change History ##
 
+### 2.2.9 ###
+
+| Type   | Description |
+| ------ | ----------- |
+| Fix | Fixed an exception priority issue with the `mettle-psycopg` driver where reset connections were being caught by the lock exception. |
+
+
 ### 2.2.8 ###
 
 | Type   | Description |
 | ------ | ----------- |
 | New | The `mettle-sql-build` entry point in the python package now accepts wild card inputs.  |
 
 ### 2.2.7 ###
```

#### html2text {}

```diff
@@ -1,32 +1,35 @@
 # Mettle # Bitsmiths-Mettle is the supporting code generators and python
 libraries for the Mettle project. See our repo and main *README* for more
 details! ## Requirements ## Python 3.10+ ## Installation ## ```console $ pip
-install bitsmiths-mettle ---> 100% ``` ## Change History ## ### 2.2.8 ### |
-Type | Description | | ------ | ----------- | | New | The `mettle-sql-build`
-entry point in the python package now accepts wild card inputs. | ### 2.2.7 ###
-| Type | Description | | ------ | ----------- | | Fix | Python database table
-generetor respects not null columns that are integers and floats properly for
-pydantic and dataclass generation. | ### 2.2.6 ### | Type | Description | | ---
---- | ----------- | | Fix | The python encoded.databases[postgresql] driver was
-not handling null floats. Bug squashed. | ### 2.2.5 ### | Type | Description |
-| ------ | ----------- | | Fix | Changed PostgreSQL package dependency from
-`postgres` to `postgresql`. | | Fix | The python braze serializers now use
-`isinstance` instead of `type` when checking value types. | ### 2.2.4 ### |
-Type | Description | | ------ | ----------- | | Fix | Improved package
-dependencies, thank-you Bradley Kirton. | | New | Added a new optional `global-
-settings.file-header` setting to projects. Allows customization or removal or
-the generated header in all generated files. | ### 2.2.3 ### | Type |
-Description | | ------ | ----------- | | New | Implemented auto (reset) to
-database connections on failure for all python database drivers. (This excludes
-`asynpg` because it uses a pool that does it for us). | | Bug | Fixed a python
-async code generation issue, where some `methods` and `with` statements were
-not using await or async. | ### 2.2.2 ### | Type | Description | | ------ | ---
--------- | | Fix | Fixed an import issue with the Braze TCP overload in python.
-| ### 2.2.1 ### | Type | Description | | ------ | ----------- | | Fix | Applied
+install bitsmiths-mettle ---> 100% ``` ## Change History ## ### 2.2.9 ### |
+Type | Description | | ------ | ----------- | | Fix | Fixed an exception
+priority issue with the `mettle-psycopg` driver where reset connections were
+being caught by the lock exception. | ### 2.2.8 ### | Type | Description | | --
+---- | ----------- | | New | The `mettle-sql-build` entry point in the python
+package now accepts wild card inputs. | ### 2.2.7 ### | Type | Description | |
+------ | ----------- | | Fix | Python database table generetor respects not
+null columns that are integers and floats properly for pydantic and dataclass
+generation. | ### 2.2.6 ### | Type | Description | | ------ | ----------- | |
+Fix | The python encoded.databases[postgresql] driver was not handling null
+floats. Bug squashed. | ### 2.2.5 ### | Type | Description | | ------ | -------
+---- | | Fix | Changed PostgreSQL package dependency from `postgres` to
+`postgresql`. | | Fix | The python braze serializers now use `isinstance`
+instead of `type` when checking value types. | ### 2.2.4 ### | Type |
+Description | | ------ | ----------- | | Fix | Improved package dependencies,
+thank-you Bradley Kirton. | | New | Added a new optional `global-settings.file-
+header` setting to projects. Allows customization or removal or the generated
+header in all generated files. | ### 2.2.3 ### | Type | Description | | -----
+- | ----------- | | New | Implemented auto (reset) to database connections on
+failure for all python database drivers. (This excludes `asynpg` because it
+uses a pool that does it for us). | | Bug | Fixed a python async code
+generation issue, where some `methods` and `with` statements were not using
+await or async. | ### 2.2.2 ### | Type | Description | | ------ | ----------- |
+| Fix | Fixed an import issue with the Braze TCP overload in python. | ###
+2.2.1 ### | Type | Description | | ------ | ----------- | | Fix | Applied
 `couplet` identifier improvement to braze couplets on python. | ### 2.2.0 ### |
 Type | Description | | ------ | ----------- | | New | Added a `database_name()`
 method to all db connections. | | New | Select one statements that fail, will
 now raise the new `DBNotFound` error code. | | New | Added `psycopg3` database
 extension for `python3`. | | New | Added `psycopg3 async` database extension
 for `python3`. | | New | Python generation for `__slots__` added, requires
 python 3.10 and up. | | New | Added a `must_exist` optional parameter to the
```

### Comparing `bitsmiths-mettle-2.2.8/bitsmiths_mettle.egg-info/PKG-INFO` & `bitsmiths-mettle-2.2.9/bitsmiths_mettle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitsmiths-mettle
-Version: 2.2.8
+Version: 2.2.9
 Summary: A three tier systems code generator that targets serveral databases and languages
 Home-page: https://bitbucket.org/bitsmiths_za/mettle.git
 Author: Nicolas Milicevic, Steven van Niekerk, Darrly Daniels
 Author-email: nicolas@bitsmiths.co.za, steven@bitsmiths.co.za, darryl@bitsmiths.co.za
 License: MIT
 Project-URL: Source, https://bitbucket.org/bitsmiths_za/mettle.git
 Keywords: generators,libraries
@@ -51,14 +51,21 @@
 $ pip install bitsmiths-mettle
 
 ---> 100%
 ```
 
 ## Change History ##
 
+### 2.2.9 ###
+
+| Type   | Description |
+| ------ | ----------- |
+| Fix | Fixed an exception priority issue with the `mettle-psycopg` driver where reset connections were being caught by the lock exception. |
+
+
 ### 2.2.8 ###
 
 | Type   | Description |
 | ------ | ----------- |
 | New | The `mettle-sql-build` entry point in the python package now accepts wild card inputs.  |
 
 ### 2.2.7 ###
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bitsmiths-mettle Version: 2.2.8 Summary: A three
+Metadata-Version: 2.1 Name: bitsmiths-mettle Version: 2.2.9 Summary: A three
 tier systems code generator that targets serveral databases and languages Home-
 page: https://bitbucket.org/bitsmiths_za/mettle.git Author: Nicolas Milicevic,
 Steven van Niekerk, Darrly Daniels Author-email: nicolas@bitsmiths.co.za,
 steven@bitsmiths.co.za, darryl@bitsmiths.co.za License: MIT Project-URL:
 Source, https://bitbucket.org/bitsmiths_za/mettle.git Keywords:
 generators,libraries Platform: unix Platform: linux Platform: osx Platform:
 cygwin Platform: win32 Classifier: Development Status :: 5 - Production/Stable
@@ -16,29 +16,32 @@
 Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
 postgresql_psycopg2 Provides-Extra: postgresql_psycopg3 Provides-Extra:
 postgresql_async Provides-Extra: sqlite_async Provides-Extra: sqlalchemy
 License-File: LICENCE # Mettle # Bitsmiths-Mettle is the supporting code
 generators and python libraries for the Mettle project. See our repo and main
 *README* for more details! ## Requirements ## Python 3.10+ ## Installation ##
 ```console $ pip install bitsmiths-mettle ---> 100% ``` ## Change History ##
-### 2.2.8 ### | Type | Description | | ------ | ----------- | | New | The
-`mettle-sql-build` entry point in the python package now accepts wild card
-inputs. | ### 2.2.7 ### | Type | Description | | ------ | ----------- | | Fix |
-Python database table generetor respects not null columns that are integers and
-floats properly for pydantic and dataclass generation. | ### 2.2.6 ### | Type |
-Description | | ------ | ----------- | | Fix | The python encoded.databases
-[postgresql] driver was not handling null floats. Bug squashed. | ### 2.2.5 ###
-| Type | Description | | ------ | ----------- | | Fix | Changed PostgreSQL
-package dependency from `postgres` to `postgresql`. | | Fix | The python braze
-serializers now use `isinstance` instead of `type` when checking value types. |
-### 2.2.4 ### | Type | Description | | ------ | ----------- | | Fix | Improved
-package dependencies, thank-you Bradley Kirton. | | New | Added a new optional
-`global-settings.file-header` setting to projects. Allows customization or
-removal or the generated header in all generated files. | ### 2.2.3 ### | Type
-| Description | | ------ | ----------- | | New | Implemented auto (reset) to
+### 2.2.9 ### | Type | Description | | ------ | ----------- | | Fix | Fixed an
+exception priority issue with the `mettle-psycopg` driver where reset
+connections were being caught by the lock exception. | ### 2.2.8 ### | Type |
+Description | | ------ | ----------- | | New | The `mettle-sql-build` entry
+point in the python package now accepts wild card inputs. | ### 2.2.7 ### |
+Type | Description | | ------ | ----------- | | Fix | Python database table
+generetor respects not null columns that are integers and floats properly for
+pydantic and dataclass generation. | ### 2.2.6 ### | Type | Description | | ---
+--- | ----------- | | Fix | The python encoded.databases[postgresql] driver was
+not handling null floats. Bug squashed. | ### 2.2.5 ### | Type | Description |
+| ------ | ----------- | | Fix | Changed PostgreSQL package dependency from
+`postgres` to `postgresql`. | | Fix | The python braze serializers now use
+`isinstance` instead of `type` when checking value types. | ### 2.2.4 ### |
+Type | Description | | ------ | ----------- | | Fix | Improved package
+dependencies, thank-you Bradley Kirton. | | New | Added a new optional `global-
+settings.file-header` setting to projects. Allows customization or removal or
+the generated header in all generated files. | ### 2.2.3 ### | Type |
+Description | | ------ | ----------- | | New | Implemented auto (reset) to
 database connections on failure for all python database drivers. (This excludes
 `asynpg` because it uses a pool that does it for us). | | Bug | Fixed a python
 async code generation issue, where some `methods` and `with` statements were
 not using await or async. | ### 2.2.2 ### | Type | Description | | ------ | ---
 -------- | | Fix | Fixed an import issue with the Braze TCP overload in python.
 | ### 2.2.1 ### | Type | Description | | ------ | ----------- | | Fix | Applied
 `couplet` identifier improvement to braze couplets on python. | ### 2.2.0 ### |
```

### Comparing `bitsmiths-mettle-2.2.8/bitsmiths_mettle.egg-info/SOURCES.txt` & `bitsmiths-mettle-2.2.9/bitsmiths_mettle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/__main__.py` & `bitsmiths-mettle-2.2.9/mettle/__main__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/braze/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/bool_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/bool_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/char_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/char_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/client.py` & `bitsmiths-mettle-2.2.9/mettle/braze/client.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/date_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/date_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/datetime_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/datetime_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/double_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/double_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/float_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/float_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/guid_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/guid_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/http/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/braze/http/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/http/http_header.py` & `bitsmiths-mettle-2.2.9/mettle/braze/http/http_header.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/http/transport_client.py` & `bitsmiths-mettle-2.2.9/mettle/braze/http/transport_client.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/http/transport_client_settings.py` & `bitsmiths-mettle-2.2.9/mettle/braze/http/transport_client_settings.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/http/transport_server.py` & `bitsmiths-mettle-2.2.9/mettle/braze/http/transport_server.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/http/transport_server_settings.py` & `bitsmiths-mettle-2.2.9/mettle/braze/http/transport_server_settings.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/iclient_marshaler.py` & `bitsmiths-mettle-2.2.9/mettle/braze/iclient_marshaler.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/int16_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/int16_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/int32_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/int32_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/int64_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/int64_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/int8_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/int8_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/iserver_interface.py` & `bitsmiths-mettle-2.2.9/mettle/braze/iserver_interface.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/iserver_marshaler.py` & `bitsmiths-mettle-2.2.9/mettle/braze/iserver_marshaler.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/itransport.py` & `bitsmiths-mettle-2.2.9/mettle/braze/itransport.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/itransport_settings.py` & `bitsmiths-mettle-2.2.9/mettle/braze/itransport_settings.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/json_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/json_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/memblock_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/memblock_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/rdc.py` & `bitsmiths-mettle-2.2.9/mettle/braze/rdc.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/rpc_header.py` & `bitsmiths-mettle-2.2.9/mettle/braze/rpc_header.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/server.py` & `bitsmiths-mettle-2.2.9/mettle/braze/server.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/server_multimarsh.py` & `bitsmiths-mettle-2.2.9/mettle/braze/server_multimarsh.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/string_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/string_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/tcp/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/braze/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/tcp/socket_tcp.py` & `bitsmiths-mettle-2.2.9/mettle/braze/tcp/socket_tcp.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/tcp/socket_tcp_client.py` & `bitsmiths-mettle-2.2.9/mettle/braze/tcp/socket_tcp_client.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/tcp/socket_tcp_server.py` & `bitsmiths-mettle-2.2.9/mettle/braze/tcp/socket_tcp_server.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/tcp/tcp_header.py` & `bitsmiths-mettle-2.2.9/mettle/braze/tcp/tcp_header.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/tcp/transport_client.py` & `bitsmiths-mettle-2.2.9/mettle/braze/tcp/transport_client.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/tcp/transport_client_settings.py` & `bitsmiths-mettle-2.2.9/mettle/braze/tcp/transport_client_settings.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/tcp/transport_server.py` & `bitsmiths-mettle-2.2.9/mettle/braze/tcp/transport_server.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/tcp/transport_server_settings.py` & `bitsmiths-mettle-2.2.9/mettle/braze/tcp/transport_server_settings.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/time_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/time_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/uint16_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/uint16_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/uint32_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/uint32_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/uint64_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/uint64_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/braze/uint8_list.py` & `bitsmiths-mettle-2.2.9/mettle/braze/uint8_list.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/db/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/db_lock.py` & `bitsmiths-mettle-2.2.9/mettle/db/db_lock.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/encode_io_databases/aconnect.py` & `bitsmiths-mettle-2.2.9/mettle/db/encode_io_databases/aconnect.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/encode_io_databases/aconnect_postgres.py` & `bitsmiths-mettle-2.2.9/mettle/db/encode_io_databases/aconnect_postgres.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/encode_io_databases/statement.py` & `bitsmiths-mettle-2.2.9/mettle/db/encode_io_databases/statement.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/iaconnect.py` & `bitsmiths-mettle-2.2.9/mettle/db/iaconnect.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/iconnect.py` & `bitsmiths-mettle-2.2.9/mettle/db/iconnect.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/iprimary_key.py` & `bitsmiths-mettle-2.2.9/mettle/db/iprimary_key.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/psycopg2/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/db/psycopg2/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/psycopg2/connect.py` & `bitsmiths-mettle-2.2.9/mettle/db/psycopg2/connect.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -228,18 +228,14 @@
 
     def execute(self, stmnt: Statement) -> IConnect:
         in_params = self._bind_input(stmnt)
 
         try:
             stmnt.sql_subst(Connect._psyco_repl, {'%': '%%'})
             stmnt._curr.execute(stmnt._sql, in_params)
-        except psycopg2.OperationalError as x:
-            self.reset(3, 0.1)
-            raise xMettle('Connection Lost - %s' % str(x), self.name(), xMettle.eCode.DBBokenConnection)
-
         except psycopg2.errors.LockNotAvailable as x:
             self._handle_rollback(stmnt)
             raise xMettle('Sql Lock Error - %s' % str(x), self.name(), xMettle.eCode.DBLockNoWaitFailed)
 
         except psycopg2.errors.IntegrityConstraintViolation as x:
             self._handle_rollback(stmnt)
             raise xMettle('Sql Error - %s' % str(x), self.name(), xMettle.eCode.DBPrimaryKeyViolation)
@@ -248,14 +244,18 @@
             self._handle_rollback(stmnt)
             raise xMettle('Sql Error - %s' % str(x), self.name(), xMettle.eCode.DBForeignKeyViolation)
 
         except psycopg2.errors.UniqueViolation as x:
             self._handle_rollback(stmnt)
             raise xMettle('Sql Error - %s' % str(x), self.name(), xMettle.eCode.DBUniqueKeyViolation)
 
+        except psycopg2.OperationalError as x:
+            self.reset(3, 0.1)
+            raise xMettle('Connection Lost - %s' % str(x), self.name(), xMettle.eCode.DBBokenConnection)
+
         except Exception as x:
             self._handle_rollback(stmnt)
             raise xMettle('Sql Error - %s' % (str(x)), self.name(), xMettle.eCode.DBStandardError)
 
         return self
```

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/psycopg2/statement.py` & `bitsmiths-mettle-2.2.9/mettle/db/psycopg2/statement.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/psycopg3/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/db/psycopg3/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/psycopg3/aconnect.py` & `bitsmiths-mettle-2.2.9/mettle/db/psycopg3/aconnect.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/psycopg3/astatement.py` & `bitsmiths-mettle-2.2.9/mettle/db/psycopg3/astatement.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/psycopg3/connect.py` & `bitsmiths-mettle-2.2.9/mettle/db/psycopg3/connect.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -212,18 +212,14 @@
 
     def execute(self, stmnt: Statement) -> IConnect:
         in_params = self._bind_input(stmnt)
 
         try:
             stmnt.sql_subst(Connect._psyco_repl, {'%': '%%'})
             stmnt._curr.execute(stmnt._sql, in_params)
-        except psycopg.OperationalError as x:
-            self.reset(3, 0.1)
-            raise xMettle('Connection Lost - %s' % str(x), self.name(), xMettle.eCode.DBBokenConnection)
-
         except psycopg.errors.LockNotAvailable as x:
             self._handle_rollback(stmnt)
             raise xMettle('Sql Lock Error - %s' % str(x), self.name(), xMettle.eCode.DBLockNoWaitFailed)
 
         except psycopg.errors.IntegrityConstraintViolation as x:
             self._handle_rollback(stmnt)
             raise xMettle('Sql Error - %s' % str(x), self.name(), xMettle.eCode.DBPrimaryKeyViolation)
@@ -232,14 +228,18 @@
             self._handle_rollback(stmnt)
             raise xMettle('Sql Error - %s' % str(x), self.name(), xMettle.eCode.DBForeignKeyViolation)
 
         except psycopg.errors.UniqueViolation as x:
             self._handle_rollback(stmnt)
             raise xMettle('Sql Error - %s' % str(x), self.name(), xMettle.eCode.DBUniqueKeyViolation)
 
+        except psycopg.OperationalError as x:
+            self.reset(3, 0.1)
+            raise xMettle('Connection Lost - %s' % str(x), self.name(), xMettle.eCode.DBBokenConnection)
+
         except Exception as x:
             self._handle_rollback(stmnt)
             raise xMettle('Sql Error - %s' % (str(x)), self.name(), xMettle.eCode.DBStandardError)
 
         return self
```

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/psycopg3/statement.py` & `bitsmiths-mettle-2.2.9/mettle/db/psycopg3/statement.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/sqlalc/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/db/sqlalc/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/sqlalc/connect.py` & `bitsmiths-mettle-2.2.9/mettle/db/sqlalc/connect.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/sqlalc/connect_postgres.py` & `bitsmiths-mettle-2.2.9/mettle/db/sqlalc/connect_postgres.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/sqlalc/statement.py` & `bitsmiths-mettle-2.2.9/mettle/db/sqlalc/statement.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/sqlite/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/db/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/sqlite/connect.py` & `bitsmiths-mettle-2.2.9/mettle/db/sqlite/connect.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/sqlite/statement.py` & `bitsmiths-mettle-2.2.9/mettle/db/sqlite/statement.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/sqlvar.py` & `bitsmiths-mettle-2.2.9/mettle/db/sqlvar.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/db/statement.py` & `bitsmiths-mettle-2.2.9/mettle/db/statement.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/genes/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/braze/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/genes/braze/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/braze/gen_cpp.py` & `bitsmiths-mettle-2.2.9/mettle/genes/braze/gen_cpp.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/braze/gen_js.py` & `bitsmiths-mettle-2.2.9/mettle/genes/braze/gen_js.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/braze/gen_py3.py` & `bitsmiths-mettle-2.2.9/mettle/genes/braze/gen_py3.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/braze/gen_ts.py` & `bitsmiths-mettle-2.2.9/mettle/genes/braze/gen_ts.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/braze/generator.py` & `bitsmiths-mettle-2.2.9/mettle/genes/braze/generator.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/braze_project.py` & `bitsmiths-mettle-2.2.9/mettle/genes/braze_project.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/common.py` & `bitsmiths-mettle-2.2.9/mettle/genes/common.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/data_types.py` & `bitsmiths-mettle-2.2.9/mettle/genes/data_types.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/database_project.py` & `bitsmiths-mettle-2.2.9/mettle/genes/database_project.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/database.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/database.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/db_mssql.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/db_mssql.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/db_oracle.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/db_oracle.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/db_postgres.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/db_postgres.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/db_sqlite.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/db_std.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/db_std.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/gen_cpp.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/gen_cpp.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/gen_js.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/gen_js.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/gen_py3.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/gen_py3.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/gen_py3sqlalchemy.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/gen_py3sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/gen_sql.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/gen_sql.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/gen_sql_mssql.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/gen_sql_mssql.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/gen_sql_postgres.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/gen_sql_postgres.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/gen_sql_sqlite.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/gen_sql_sqlite.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/gen_ts.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/gen_ts.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/generator.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/generator.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/db/table.py` & `bitsmiths-mettle-2.2.9/mettle/genes/db/table.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/mk/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/genes/mk/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/mk/gen_angular.py` & `bitsmiths-mettle-2.2.9/mettle/genes/mk/gen_angular.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/mk/gen_cpp.py` & `bitsmiths-mettle-2.2.9/mettle/genes/mk/gen_cpp.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/mk/gen_mettleproj.py` & `bitsmiths-mettle-2.2.9/mettle/genes/mk/gen_mettleproj.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/mk/gen_mksln.py` & `bitsmiths-mettle-2.2.9/mettle/genes/mk/gen_mksln.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/mk/gen_pythondist.py` & `bitsmiths-mettle-2.2.9/mettle/genes/mk/gen_pythondist.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/mk/generator.py` & `bitsmiths-mettle-2.2.9/mettle/genes/mk/generator.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/mk_project.py` & `bitsmiths-mettle-2.2.9/mettle/genes/mk_project.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/project.py` & `bitsmiths-mettle-2.2.9/mettle/genes/project.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/service.py` & `bitsmiths-mettle-2.2.9/mettle/genes/service.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/genes/zip_buddy.py` & `bitsmiths-mettle-2.2.9/mettle/genes/zip_buddy.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/big_endian_reader.py` & `bitsmiths-mettle-2.2.9/mettle/io/big_endian_reader.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/big_endian_writer.py` & `bitsmiths-mettle-2.2.9/mettle/io/big_endian_writer.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/dict_stream.py` & `bitsmiths-mettle-2.2.9/mettle/io/dict_stream.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/ireader.py` & `bitsmiths-mettle-2.2.9/mettle/io/ireader.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/iserializable.py` & `bitsmiths-mettle-2.2.9/mettle/io/iserializable.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/istream.py` & `bitsmiths-mettle-2.2.9/mettle/io/istream.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/iwriter.py` & `bitsmiths-mettle-2.2.9/mettle/io/iwriter.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/list_stream.py` & `bitsmiths-mettle-2.2.9/mettle/io/list_stream.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/memory_stream.py` & `bitsmiths-mettle-2.2.9/mettle/io/memory_stream.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/py_dict_reader.py` & `bitsmiths-mettle-2.2.9/mettle/io/py_dict_reader.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/py_dict_writer.py` & `bitsmiths-mettle-2.2.9/mettle/io/py_dict_writer.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/py_json_dict_reader.py` & `bitsmiths-mettle-2.2.9/mettle/io/py_json_dict_reader.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/py_json_dict_writer.py` & `bitsmiths-mettle-2.2.9/mettle/io/py_json_dict_writer.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/py_json_list_reader.py` & `bitsmiths-mettle-2.2.9/mettle/io/py_json_list_reader.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/py_json_list_writer.py` & `bitsmiths-mettle-2.2.9/mettle/io/py_json_list_writer.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/py_list_reader.py` & `bitsmiths-mettle-2.2.9/mettle/io/py_list_reader.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/py_list_writer.py` & `bitsmiths-mettle-2.2.9/mettle/io/py_list_writer.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/io/util.py` & `bitsmiths-mettle-2.2.9/mettle/io/util.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/lib/__init__.py` & `bitsmiths-mettle-2.2.9/mettle/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/lib/dav.py` & `bitsmiths-mettle-2.2.9/mettle/lib/dav.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/lib/dav_cache.py` & `bitsmiths-mettle-2.2.9/mettle/lib/dav_cache.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/lib/ref.py` & `bitsmiths-mettle-2.2.9/mettle/lib/ref.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/lib/timezone.py` & `bitsmiths-mettle-2.2.9/mettle/lib/timezone.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/lib/xmettle.py` & `bitsmiths-mettle-2.2.9/mettle/lib/xmettle.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/mettle/lib/xterminate.py` & `bitsmiths-mettle-2.2.9/mettle/lib/xterminate.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-mettle-2.2.8/setup.cfg` & `bitsmiths-mettle-2.2.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = bitsmiths-mettle
 description = A three tier systems code generator that targets serveral databases and languages
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/bitsmiths_za/mettle.git
 author = Nicolas Milicevic, Steven van Niekerk, Darrly Daniels
 author_email = nicolas@bitsmiths.co.za, steven@bitsmiths.co.za, darryl@bitsmiths.co.za
-version = 2.2.8
+version = 2.2.9
 license = MIT
 license_files = LICENCE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
```

