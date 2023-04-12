# Comparing `tmp/MindsDB-23.3.5.0.tar.gz` & `tmp/MindsDB-23.4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MindsDB-23.3.5.0.tar", last modified: Tue Mar 28 13:19:26 2023, max compression
+gzip compressed data, was "dist/MindsDB-23.4.3.0.tar", last modified: Wed Apr 12 09:33:48 2023, max compression
```

## Comparing `MindsDB-23.3.5.0.tar` & `MindsDB-23.4.3.0.tar`

### file list

```diff
@@ -1,1013 +1,1095 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/MindsDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28144 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    46839 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    28144 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26042 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    55090 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)    23115 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    63437 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    31278 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/api/nlp/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/autokeras_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/autokeras_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/file_handler/file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/huggingface_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/tests/test_jira_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ludwig_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/merlion_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/merlion_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mlflow_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26975 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/openai_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/openai_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/postgres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/rockset_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/rockset_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/solr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tpot_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_client/db_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_client/ml_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_client/ml_grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/handler_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/ml_exec_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/ml_handler_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/libs/storage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/utilities/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/base/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/kafka/kafkadb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/redis/redisdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/interfaces/stream/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/log_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 13:19:26.000000 MindsDB-23.3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-28 13:19:14.000000 MindsDB-23.3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 09:33:37.000000 MindsDB-23.4.3.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    50989 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21924 2023-04-12 09:33:37.000000 MindsDB-23.4.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56201 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23115 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63880 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31700 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/api/nlp/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autokeras_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autokeras_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/file_handler/file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/huggingface_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/tests/test_jira_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/langchain_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ludwig_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/merlion_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mlflow_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27726 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/openai_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/openai_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/postgres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/rockset_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/solr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
+-rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tpot_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_client/db_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_client/ml_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_client/ml_grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/handler_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/ml_exec_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/ml_handler_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/libs/storage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/utilities/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/base/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/kafka/kafkadb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/redis/redisdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/interfaces/stream/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:33:48.000000 MindsDB-23.4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-12 09:33:38.000000 MindsDB-23.4.3.0/setup.py
```

### Comparing `MindsDB-23.3.5.0/MindsDB.egg-info/PKG-INFO` & `MindsDB-23.4.3.0/MindsDB.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.3.5.0
+Version: 23.4.3.0
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -128,34 +128,26 @@
         | Connect your Data | Connect your Data | Connect your Data
         |-|-|-|
         | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
         | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/Apache-Pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> 
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/TiDB#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> | 
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#yugabyte"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
         | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
-        | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
         
         
         [:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
         
         
         ## Documentation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.3.5.0 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.4.3.0 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -87,31 +87,25 @@
 with sample data to get on-boarded as fast as possible. ## Database
 Integrations MindsDB works with most of the SQL and NoSQL databases, data
 lakes, data Streams and popular applications. | Connect your Data | Connect
 your Data | Connect your Data |-|-|-| | [Connect_Apache_Kafka] | [Connect
 Microsoft_Access] | [Oracle_Badge] | | [Connect_Amazon_Redshift] | [Airtable
 Badge] | [Pinot_Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3
 Badge] | | [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
-Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect
-CockroachDB] | [ckan_Badge] | [Supabase_Badge] | [Connect_MariaDB] | [Couchbase
-Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] | [Timescale
-Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB_Badge] | |
-[Connect_SQL_Server] | [CrateDB_Badge] | [Timescale_Badge] | | [Connect
-MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB_Badge] | | [Connect_MySQL] |
-[Databricks_Badge] | [YugabyteDB_Badge] | [Connect_PostgreSQL] | [IBMDB2_Badge]
-| [openGauss_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
-Badge] | | [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect
-PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | | [Connect_QuestDB] |
+Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
+[Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
+[Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
+Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
+[Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
 [Apache_Druid_Badge] | [StarRocks_Badge] | | [Connect_Redis] | [Vertica_Badge]
 | [DuckDB_Badge] | | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner
 Badge] | | [Connect_ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] |
-[Apache_Hive_Badge] | | [Connect_Snowflake] | [Informix_Badge] | | [Connect
-Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix_Badge] | |
-[Connect_Teradata] | [Matrixone_Badge] | | [Connect_Trino] | [Monetdb_Badge] |
-[:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/
+[Apache_Hive_Badge] | | [Connect_Teradata] | [Matrixone_Badge] | | [Connect
+Snowflake] | [Informix_Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:
+question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/
 issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml) ##
 Documentation You can find the complete documentation of MindsDB at
 [docs.mindsdb.com](https://
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ## Support If you found a bug, please submit an [issue on GitHub](https://
 github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
 can: * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity). *
```

### Comparing `MindsDB-23.3.5.0/MindsDB.egg-info/SOURCES.txt` & `MindsDB-23.4.3.0/MindsDB.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -184,21 +184,33 @@
 mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
 mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
 mindsdb/integrations/handlers/autokeras_handler/__about__.py
 mindsdb/integrations/handlers/autokeras_handler/__init__.py
 mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
 mindsdb/integrations/handlers/autokeras_handler/functions.py
 mindsdb/integrations/handlers/autokeras_handler/setup.py
+mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+mindsdb/integrations/handlers/autosklearn_handler/config.py
+mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+mindsdb/integrations/handlers/autosklearn_handler/setup.py
 mindsdb/integrations/handlers/bigquery_handler/__about__.py
 mindsdb/integrations/handlers/bigquery_handler/__init__.py
 mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
 mindsdb/integrations/handlers/bigquery_handler/logo.svg
 mindsdb/integrations/handlers/bigquery_handler/requirements.txt
 mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
 mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+mindsdb/integrations/handlers/binance_handler/__about__.py
+mindsdb/integrations/handlers/binance_handler/__init__.py
+mindsdb/integrations/handlers/binance_handler/binance_handler.py
+mindsdb/integrations/handlers/binance_handler/binance_tables.py
+mindsdb/integrations/handlers/binance_handler/icon.svg
+mindsdb/integrations/handlers/binance_handler/requirements.txt
 mindsdb/integrations/handlers/byom_handler/__about__.py
 mindsdb/integrations/handlers/byom_handler/__init__.py
 mindsdb/integrations/handlers/byom_handler/byom_handler.py
 mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
 mindsdb/integrations/handlers/cassandra_handler/__about__.py
 mindsdb/integrations/handlers/cassandra_handler/__init__.py
 mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
@@ -325,14 +337,21 @@
 mindsdb/integrations/handlers/dynamodb_handler/__about__.py
 mindsdb/integrations/handlers/dynamodb_handler/__init__.py
 mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
 mindsdb/integrations/handlers/dynamodb_handler/icon.png
 mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
 mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
 mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
 mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
 mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
 mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
 mindsdb/integrations/handlers/elasticsearch_handler/icon.png
 mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
 mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
 mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
@@ -349,14 +368,20 @@
 mindsdb/integrations/handlers/firebird_handler/__about__.py
 mindsdb/integrations/handlers/firebird_handler/__init__.py
 mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
 mindsdb/integrations/handlers/firebird_handler/icon.png
 mindsdb/integrations/handlers/firebird_handler/requirements.txt
 mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
 mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+mindsdb/integrations/handlers/github_handler/__about__.py
+mindsdb/integrations/handlers/github_handler/__init__.py
+mindsdb/integrations/handlers/github_handler/github_handler.py
+mindsdb/integrations/handlers/github_handler/github_tables.py
+mindsdb/integrations/handlers/github_handler/icon.svg
+mindsdb/integrations/handlers/github_handler/requirements.txt
 mindsdb/integrations/handlers/hana_handler/__about__.py
 mindsdb/integrations/handlers/hana_handler/__init__.py
 mindsdb/integrations/handlers/hana_handler/hana_handler.py
 mindsdb/integrations/handlers/hana_handler/icon.svg
 mindsdb/integrations/handlers/hana_handler/requirements.txt
 mindsdb/integrations/handlers/hive_handler/__about__.py
 mindsdb/integrations/handlers/hive_handler/__init__.py
@@ -392,21 +417,33 @@
 mindsdb/integrations/handlers/informix_handler/__about__.py
 mindsdb/integrations/handlers/informix_handler/__init__.py
 mindsdb/integrations/handlers/informix_handler/icon.png
 mindsdb/integrations/handlers/informix_handler/informix_handler.py
 mindsdb/integrations/handlers/informix_handler/requirements.txt
 mindsdb/integrations/handlers/informix_handler/tests/__init__.py
 mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+mindsdb/integrations/handlers/ingres_handler/__about__.py
+mindsdb/integrations/handlers/ingres_handler/__init__.py
+mindsdb/integrations/handlers/ingres_handler/icon.svg
+mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+mindsdb/integrations/handlers/ingres_handler/requirements.txt
+mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
 mindsdb/integrations/handlers/jira_handler/__about__.py
 mindsdb/integrations/handlers/jira_handler/__init__.py
 mindsdb/integrations/handlers/jira_handler/icon.png
 mindsdb/integrations/handlers/jira_handler/jira_handler.py
 mindsdb/integrations/handlers/jira_handler/requirements.txt
 mindsdb/integrations/handlers/jira_handler/tests/__init__.py
 mindsdb/integrations/handlers/jira_handler/tests/test_jira_handler.py
+mindsdb/integrations/handlers/langchain_handler/__about__.py
+mindsdb/integrations/handlers/langchain_handler/__init__.py
+mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+mindsdb/integrations/handlers/langchain_handler/requirements.txt
+mindsdb/integrations/handlers/langchain_handler/setup.py
 mindsdb/integrations/handlers/lightwood_handler/__init__.py
 mindsdb/integrations/handlers/lightwood_handler/requirements.txt
 mindsdb/integrations/handlers/lightwood_handler/setup.py
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
 mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
@@ -550,14 +587,19 @@
 mindsdb/integrations/handlers/questdb_handler/__about__.py
 mindsdb/integrations/handlers/questdb_handler/__init__.py
 mindsdb/integrations/handlers/questdb_handler/icon.svg
 mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
 mindsdb/integrations/handlers/questdb_handler/requirements.txt
 mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
 mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
+mindsdb/integrations/handlers/ray_serve_handler/setup.py
 mindsdb/integrations/handlers/redshift_handler/__about__.py
 mindsdb/integrations/handlers/redshift_handler/__init__.py
 mindsdb/integrations/handlers/redshift_handler/icon.png
 mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
 mindsdb/integrations/handlers/redshift_handler/requirements.txt
 mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
 mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
@@ -608,18 +650,30 @@
 mindsdb/integrations/handlers/sqlany_handler/__about__.py
 mindsdb/integrations/handlers/sqlany_handler/__init__.py
 mindsdb/integrations/handlers/sqlany_handler/icon.svg
 mindsdb/integrations/handlers/sqlany_handler/requirements.txt
 mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
 mindsdb/integrations/handlers/sqlite_handler/__about__.py
 mindsdb/integrations/handlers/sqlite_handler/__init__.py
+mindsdb/integrations/handlers/sqlite_handler/db_connection.png
+mindsdb/integrations/handlers/sqlite_handler/error.png
 mindsdb/integrations/handlers/sqlite_handler/icon.png
+mindsdb/integrations/handlers/sqlite_handler/model_drop.png
+mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
+mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
 mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
 mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
 mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+mindsdb/integrations/handlers/sqreamdb_handler/icon.png
+mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
 mindsdb/integrations/handlers/starrocks_handler/__about__.py
 mindsdb/integrations/handlers/starrocks_handler/__init__.py
 mindsdb/integrations/handlers/starrocks_handler/icon.png
 mindsdb/integrations/handlers/starrocks_handler/requirements.txt
 mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
 mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
 mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
@@ -631,14 +685,23 @@
 mindsdb/integrations/handlers/supabase_handler/__about__.py
 mindsdb/integrations/handlers/supabase_handler/__init__.py
 mindsdb/integrations/handlers/supabase_handler/icon.svg
 mindsdb/integrations/handlers/supabase_handler/requirements.txt
 mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
 mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
 mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+mindsdb/integrations/handlers/surrealdb_handler/icon.png
+mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
 mindsdb/integrations/handlers/tdengine_handler/__about__.py
 mindsdb/integrations/handlers/tdengine_handler/__init__.py
 mindsdb/integrations/handlers/tdengine_handler/icon.svg
 mindsdb/integrations/handlers/tdengine_handler/requirements.txt
 mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
 mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
 mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
@@ -716,16 +779,18 @@
 mindsdb/integrations/libs/handler_helpers.py
 mindsdb/integrations/libs/ml_exec_base.py
 mindsdb/integrations/libs/ml_handler_proc.py
 mindsdb/integrations/libs/net_helpers.py
 mindsdb/integrations/libs/response.py
 mindsdb/integrations/libs/storage_handler.py
 mindsdb/integrations/utilities/__init__.py
+mindsdb/integrations/utilities/date_utils.py
 mindsdb/integrations/utilities/install.py
 mindsdb/integrations/utilities/processes.py
+mindsdb/integrations/utilities/sql_utils.py
 mindsdb/integrations/utilities/test_utils.py
 mindsdb/integrations/utilities/time_series_utils.py
 mindsdb/integrations/utilities/utils.py
 mindsdb/interfaces/__init__.py
 mindsdb/interfaces/database/__init__.py
 mindsdb/interfaces/database/database.py
 mindsdb/interfaces/database/integrations.py
@@ -803,8 +868,10 @@
 mindsdb/utilities/functions.py
 mindsdb/utilities/json_encoder.py
 mindsdb/utilities/log.py
 mindsdb/utilities/log_controller.py
 mindsdb/utilities/ps.py
 mindsdb/utilities/telemetry.py
 mindsdb/utilities/wizards.py
-mindsdb/utilities/hooks/__init__.py
+mindsdb/utilities/hooks/__init__.py
+mindsdb/utilities/profiler/__init__.py
+mindsdb/utilities/profiler/profiler.py
```

### Comparing `MindsDB-23.3.5.0/MindsDB.egg-info/requires.txt` & `MindsDB-23.4.3.0/MindsDB.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lightwood<23.3.2.0,>=23.2.1.1
+lightwood<23.3.3.0,>=23.3.2.0
 markupsafe==2.0.1
 flask-restx<2.0.0,>=1.0.1
 flask<2.0,>=1.0
 python-multipart>=0.0.5
 pyparsing==2.3.1
 cryptography>=35.0
 psycopg[binary]>=1.15.3
@@ -15,15 +15,15 @@
 sqlalchemy<2.0.0,>=1.4.29
 alembic>=1.3.3
 sentry-sdk
 walrus==0.8.2
 flask-compress>=1.0.0
 kafka-python>=2.0.0
 appdirs>=1.0.0
-mindsdb-sql<0.5.0,>=0.4.9
+mindsdb-sql<0.6.0,>=0.5.1
 checksumdir>=1.2.0
 mindsdb-streams==0.1.1
 duckdb==0.4.0
 requests>=2.0.0
 mysql-connector-python
 clickhouse-driver
 clickhouse-sqlalchemy
```

### Comparing `MindsDB-23.3.5.0/PKG-INFO` & `MindsDB-23.4.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.3.5.0
+Version: 23.4.3.0
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -128,34 +128,26 @@
         | Connect your Data | Connect your Data | Connect your Data
         |-|-|-|
         | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
         | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/Apache-Pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> 
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/TiDB#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> | 
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#yugabyte"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
         | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
-        | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
-        | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
         
         
         [:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
         
         
         ## Documentation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.3.5.0 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.4.3.0 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -87,31 +87,25 @@
 with sample data to get on-boarded as fast as possible. ## Database
 Integrations MindsDB works with most of the SQL and NoSQL databases, data
 lakes, data Streams and popular applications. | Connect your Data | Connect
 your Data | Connect your Data |-|-|-| | [Connect_Apache_Kafka] | [Connect
 Microsoft_Access] | [Oracle_Badge] | | [Connect_Amazon_Redshift] | [Airtable
 Badge] | [Pinot_Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3
 Badge] | | [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
-Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect
-CockroachDB] | [ckan_Badge] | [Supabase_Badge] | [Connect_MariaDB] | [Couchbase
-Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] | [Timescale
-Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB_Badge] | |
-[Connect_SQL_Server] | [CrateDB_Badge] | [Timescale_Badge] | | [Connect
-MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB_Badge] | | [Connect_MySQL] |
-[Databricks_Badge] | [YugabyteDB_Badge] | [Connect_PostgreSQL] | [IBMDB2_Badge]
-| [openGauss_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
-Badge] | | [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect
-PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | | [Connect_QuestDB] |
+Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
+[Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
+[Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
+Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
+[Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
 [Apache_Druid_Badge] | [StarRocks_Badge] | | [Connect_Redis] | [Vertica_Badge]
 | [DuckDB_Badge] | | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner
 Badge] | | [Connect_ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] |
-[Apache_Hive_Badge] | | [Connect_Snowflake] | [Informix_Badge] | | [Connect
-Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix_Badge] | |
-[Connect_Teradata] | [Matrixone_Badge] | | [Connect_Trino] | [Monetdb_Badge] |
-[:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/
+[Apache_Hive_Badge] | | [Connect_Teradata] | [Matrixone_Badge] | | [Connect
+Snowflake] | [Informix_Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:
+question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/
 issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml) ##
 Documentation You can find the complete documentation of MindsDB at
 [docs.mindsdb.com](https://
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ## Support If you found a bug, please submit an [issue on GitHub](https://
 github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
 can: * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity). *
```

### Comparing `MindsDB-23.3.5.0/README.md` & `MindsDB-23.4.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -119,34 +119,26 @@
 | Connect your Data | Connect your Data | Connect your Data
 |-|-|-|
 | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
 | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/Apache-Pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
-| <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> 
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/TiDB#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> | 
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-| <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#yugabyte"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
 | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
-| <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
-| <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
-| <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
 
 
 [:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml)
 
 
 ## Documentation
```

#### html2text {}

```diff
@@ -82,31 +82,25 @@
 with sample data to get on-boarded as fast as possible. ## Database
 Integrations MindsDB works with most of the SQL and NoSQL databases, data
 lakes, data Streams and popular applications. | Connect your Data | Connect
 your Data | Connect your Data |-|-|-| | [Connect_Apache_Kafka] | [Connect
 Microsoft_Access] | [Oracle_Badge] | | [Connect_Amazon_Redshift] | [Airtable
 Badge] | [Pinot_Badge] | | [Connect_Cassandra] | [DataStax_Badge] | [Amazon_S3
 Badge] | | [Connect_CockroachDB] | [ckan_Badge] | [Supabase_Badge] | | [Connect
-Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect
-CockroachDB] | [ckan_Badge] | [Supabase_Badge] | [Connect_MariaDB] | [Couchbase
-Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] | [Timescale
-Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB_Badge] | |
-[Connect_SQL_Server] | [CrateDB_Badge] | [Timescale_Badge] | | [Connect
-MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB_Badge] | | [Connect_MySQL] |
-[Databricks_Badge] | [YugabyteDB_Badge] | [Connect_PostgreSQL] | [IBMDB2_Badge]
-| [openGauss_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
-Badge] | | [Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect
-PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | | [Connect_QuestDB] |
+Clickhouse] | [Google_Big_Query_Badge] | [SQLite_Badge] | | [Connect_MariaDB] |
+[Couchbase_Badge] | [TiDB_Badge] | | [Connect_SQL_Server] | [CrateDB_Badge] |
+[Timescale_Badge] | | [Connect_MongoDB] | [DoIt_Badge] | [Amazon_DynamoDB
+Badge] | | [Connect_PostgreSQL] | [IBMDB2_Badge] | [openGauss_Badge] | |
+[Connect_MySQL] | [Databricks_Badge] | [YugabyteDB_Badge] | [Connect_QuestDB] |
 [Apache_Druid_Badge] | [StarRocks_Badge] | | [Connect_Redis] | [Vertica_Badge]
 | [DuckDB_Badge] | | [Connect_SAP_HANA] | [Elastic_Badge] | [Cloud_Spanner
 Badge] | | [Connect_ScyllaDB] | [Firebird_Badge] | | [Connect_Singlestore] |
-[Apache_Hive_Badge] | | [Connect_Snowflake] | [Informix_Badge] | | [Connect
-Teradata] | [Matrixone_Badge] | | [Connect_Snowflake] | [Informix_Badge] | |
-[Connect_Teradata] | [Matrixone_Badge] | | [Connect_Trino] | [Monetdb_Badge] |
-[:question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/
+[Apache_Hive_Badge] | | [Connect_Teradata] | [Matrixone_Badge] | | [Connect
+Snowflake] | [Informix_Badge] | | [Connect_Trino] | [Monetdb_Badge] | [:
+question: :wave: Missing integration?](https://github.com/mindsdb/mindsdb/
 issues/new?assignees=&labels=&template=feature-mindsdb-request.yaml) ##
 Documentation You can find the complete documentation of MindsDB at
 [docs.mindsdb.com](https://
 docs.mindsdb.com?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo).
 ## Support If you found a bug, please submit an [issue on GitHub](https://
 github.com/mindsdb/mindsdb/issues/new/choose). To get community support, you
 can: * Post at MindsDB [Slack community](https://mindsdb.com/joincommunity). *
```

### Comparing `MindsDB-23.3.5.0/mindsdb/__main__.py` & `MindsDB-23.4.3.0/mindsdb/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from mindsdb.interfaces.stream.utilities import STOP_THREADS_EVENT
 from mindsdb.interfaces.database.integrations import IntegrationController
 import mindsdb.interfaces.storage.db as db
 from mindsdb.integrations.utilities.install import install_dependencies
 from mindsdb.utilities.fs import create_dirs_recursive
 from mindsdb.utilities.telemetry import telemetry_file_exists, disable_telemetry
 from mindsdb.utilities.context import context as ctx
-from mindsdb.utilities.auth import register_oauth_client
+from mindsdb.utilities.auth import register_oauth_client, get_aws_meta_data
 
 
 import torch.multiprocessing as mp
 try:
     mp.set_start_method('spawn')
 except RuntimeError:
     log.logger.info('Torch multiprocessing context already set, ignoring...')
@@ -127,20 +127,28 @@
     # initialization
     db.init()
     log.initialize_log()
 
     mp.freeze_support()
     config = Config()
 
-    is_marketplace = config.get('environment') == 'aws_marketplace'
-    if is_marketplace:
+    environment = config.get('environment')
+    if environment == 'aws_marketplace':
         try:
             register_oauth_client()
         except Exception as e:
             print(f'Something went wrong during client register: {e}')
+    elif environment != 'local':
+        try:
+            aws_meta_data = get_aws_meta_data()
+            Config().update({
+                'aws_meta_data': aws_meta_data
+            })
+        except Exception:
+            pass
 
     is_cloud = config.get('cloud', False)
     # need configure migration behavior by env_variables
     # leave 'is_cloud' for now, but needs to be removed further
     run_migration_separately = os.environ.get("SEPARATE_MIGRATIONS", False)
     if run_migration_separately in (False, "false", "False", 0, "0", ""):
         run_migration_separately = False
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-23.4.3.0/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/initialize.py` & `MindsDB-23.4.3.0/mindsdb/api/http/initialize.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/auth.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/config.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,16 +126,18 @@
                 file.save(file_path)
                 params[key] = file_path
 
         is_test = params.get('test', False)
         if is_test:
             del params['test']
 
+            handler_type = params.pop('type', None)
+            params.pop('publish', None)
             handler = ca.integration_controller.create_tmp_handler(
-                handler_type=params.get('type'),
+                handler_type=handler_type,
                 connection_data=params
             )
             status = handler.check_connection()
             if temp_dir is not None:
                 shutil.rmtree(temp_dir)
             return status, 200
 
@@ -143,19 +145,20 @@
         if integration is not None:
             abort(400, f"Integration with name '{name}' already exists")
 
         try:
             engine = params['type']
             if engine is not None:
                 del params['type']
+            publish = params.pop('publish', False)
             ca.integration_controller.add(name, engine, params)
 
-            if is_test is False and params.get('publish', False) is True:
+            if is_test is False and publish is True:
                 stream_controller = StreamController()
-                if engine in stream_controller.known_dbs and params.get('publish', False) is True:
+                if engine in stream_controller.known_dbs and publish is True:
                     stream_controller.setup(name)
         except Exception as e:
             log.logger.error(str(e))
             if temp_dir is not None:
                 shutil.rmtree(temp_dir)
             abort(500, f'Error during config update: {str(e)}')
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/default.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/default.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import time
 
 from flask import request, session
 from flask_restx import Resource
 from flask_restx import fields
 
+from mindsdb.__about__ import __version__ as mindsdb_version
 from mindsdb.api.http.namespaces.configs.default import ns_conf
-from mindsdb.utilities.config import Config
 from mindsdb.api.http.utils import http_error
+from mindsdb.utilities.config import Config
 from mindsdb.utilities.log import get_log
 
 
 log = get_log('http')
 
 
 def check_auth() -> bool:
@@ -98,14 +99,15 @@
 class StatusRoute(Resource):
     @ns_conf.doc(
         responses={
             200: 'Success'
         },
         model=ns_conf.model('response_status', {
             'environment': fields.String(description='The name of current environment: cloud, local or other'),
+            'mindsdb_version': fields.String(description='Current version of mindsdb'),
             'auth': fields.Nested(
                 ns_conf.model('response_status_auth', {
                     'confirmed': fields.Boolean(description='is current user autentificated'),
                     'required': fields.Boolean(description='is autentificated required'),
                     'provider': fields.Boolean(description='current autentification provider: local of 3d-party')
                 })
             )
@@ -130,14 +132,15 @@
         if config['auth']['http_auth_enabled'] is True:
             if config['auth'].get('provider') is not None:
                 auth_provider = config['auth'].get('provider')
             else:
                 auth_provider = 'local'
 
         resp = {
+            'mindsdb_version': mindsdb_version,
             'environment': environment,
             'auth': {
                 'confirmed': check_auth(),
                 'http_auth_enabled': config['auth']['http_auth_enabled'],
                 'provider': auth_provider
             }
         }
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/file.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/file.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/projects.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/sql.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/sql.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,80 +8,87 @@
 from mindsdb.api.mysql.mysql_proxy.libs.constants.response_type import RESPONSE_TYPE as SQL_RESPONSE_TYPE
 from mindsdb.api.mysql.mysql_proxy.utilities import (
     SqlApiException,
     SqlApiUnknownError
 )
 import mindsdb.utilities.hooks as hooks
 from mindsdb.utilities.context import context as ctx
+import mindsdb.utilities.profiler as profiler
+from mindsdb.utilities.config import Config
 
 
 @ns_conf.route('/query')
 @ns_conf.param('query', 'Execute query')
 class Query(Resource):
     @ns_conf.doc('query')
     def post(self):
         query = request.json['query']
         context = request.json.get('context', {})
 
+        if context.get('profiling') is True:
+            profiler.enable()
+
         error_type = None
         error_code = None
         error_text = None
         error_traceback = None
 
-        mysql_proxy = FakeMysqlProxy()
-        mysql_proxy.set_context(context)
-        try:
-            result = mysql_proxy.process_query(query)
+        profiler.set_meta(query=query, api='http', environment=Config().get('environment'))
+        with profiler.Context('http_query_processing'):
+            mysql_proxy = FakeMysqlProxy()
+            mysql_proxy.set_context(context)
+            try:
+                result = mysql_proxy.process_query(query)
+
+                if result.type == SQL_RESPONSE_TYPE.OK:
+                    query_response = {
+                        'type': SQL_RESPONSE_TYPE.OK
+                    }
+                elif result.type == SQL_RESPONSE_TYPE.TABLE:
+                    query_response = {
+                        'type': SQL_RESPONSE_TYPE.TABLE,
+                        'data': result.data,
+                        'column_names': [x['alias'] or x['name'] if 'alias' in x else x['name'] for x in result.columns]
+                    }
+            except SqlApiException as e:
+                # classified error
+                error_type = 'expected'
+                query_response = {
+                    'type': SQL_RESPONSE_TYPE.ERROR,
+                    'error_code': e.err_code,
+                    'error_message': str(e)
+                }
 
-            if result.type == SQL_RESPONSE_TYPE.OK:
+            except SqlApiUnknownError as e:
+                # unclassified
+                error_type = 'unexpected'
                 query_response = {
-                    'type': SQL_RESPONSE_TYPE.OK
+                    'type': SQL_RESPONSE_TYPE.ERROR,
+                    'error_code': e.err_code,
+                    'error_message': str(e)
                 }
-            elif result.type == SQL_RESPONSE_TYPE.TABLE:
+
+            except Exception as e:
+                error_type = 'unexpected'
                 query_response = {
-                    'type': SQL_RESPONSE_TYPE.TABLE,
-                    'data': result.data,
-                    'column_names': [x['alias'] or x['name'] if 'alias' in x else x['name'] for x in result.columns]
+                    'type': SQL_RESPONSE_TYPE.ERROR,
+                    'error_code': 0,
+                    'error_message': str(e)
                 }
-        except SqlApiException as e:
-            # classified error
-            error_type = 'expected'
-            query_response = {
-                'type': SQL_RESPONSE_TYPE.ERROR,
-                'error_code': e.err_code,
-                'error_message': str(e)
-            }
-
-        except SqlApiUnknownError as e:
-            # unclassified
-            error_type = 'unexpected'
-            query_response = {
-                'type': SQL_RESPONSE_TYPE.ERROR,
-                'error_code': e.err_code,
-                'error_message': str(e)
-            }
-
-        except Exception as e:
-            error_type = 'unexpected'
-            query_response = {
-                'type': SQL_RESPONSE_TYPE.ERROR,
-                'error_code': 0,
-                'error_message': str(e)
-            }
-            error_traceback = traceback.format_exc()
-            print(error_traceback)
-
-        if query_response.get('type') == SQL_RESPONSE_TYPE.ERROR:
-            error_type = 'expected'
-            error_code = query_response.get('error_code')
-            error_text = query_response.get('error_message')
+                error_traceback = traceback.format_exc()
+                print(error_traceback)
+
+            if query_response.get('type') == SQL_RESPONSE_TYPE.ERROR:
+                error_type = 'expected'
+                error_code = query_response.get('error_code')
+                error_text = query_response.get('error_message')
 
-        context = mysql_proxy.get_context(context)
+            context = mysql_proxy.get_context(context)
 
-        query_response['context'] = context
+            query_response['context'] = context
 
         hooks.after_api_query(
             company_id=ctx.company_id,
             api='http',
             command=None,
             payload=query,
             error_type=error_type,
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/stream.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/tab.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/tree.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/namespaces/util.py` & `MindsDB-23.4.3.0/mindsdb/api/http/namespaces/util.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/start.py` & `MindsDB-23.4.3.0/mindsdb/api/http/start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/http/utils.py` & `MindsDB-23.4.3.0/mindsdb/api/http/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/classes/responder.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/classes/scram.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/classes/session.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/company_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/delete.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/find.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/insert.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 
-from mindsdb_sql.parser.dialects.mindsdb import CreatePredictor, CreateJob, RetrainPredictor, AdjustPredictor
+from mindsdb_sql.parser.dialects.mindsdb import CreatePredictor, CreateJob, RetrainPredictor, FinetunePredictor
 from mindsdb_sql.parser.ast import Identifier, OrderBy, Insert, TableColumn, Constant
 
 import mindsdb.api.mongo.functions as helpers
 from mindsdb.api.mongo.classes import Responder
 from mindsdb.api.mongo.utilities import logger
 from mindsdb.integrations.libs.response import HandlerStatusResponse
 from mindsdb.api.mongo.responders.find import find_to_ast
@@ -134,16 +134,16 @@
             integration_name = None
             if 'connection' in doc:
                 integration_name = Identifier(doc['connection'])
 
             Class = CreatePredictor
             if action == 'retrain':
                 Class = RetrainPredictor
-            elif action == 'adjust':
-                Class = AdjustPredictor
+            elif action == 'finetune':
+                Class = FinetunePredictor
 
             create_predictor_ast = Class(
                 name=Identifier(f"{request_env['database']}.{doc['name']}"),
                 integration_name=integration_name,
                 query_str=select_data_query,
                 targets=predict,
                 order_by=order_by,
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/server.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-23.4.3.0/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     Join,
     Star,
     Insert,
     Update,
     Delete,
     Latest,
     BetweenOperation,
+    Parameter,
+    Tuple
 )
 from mindsdb_sql.planner.steps import (
     ApplyTimeseriesPredictorStep,
     ApplyPredictorRowStep,
     GetPredictorColumns,
     FetchDataframeStep,
     ApplyPredictorStep,
@@ -71,14 +73,15 @@
     ErKeyColumnDoesNotExist,
     ErNotSupportedYet,
     SqlApiUnknownError,
     ErLogicError,
     ErSqlWrongArguments
 )
 from mindsdb.utilities.cache import get_cache, json_checksum
+import mindsdb.utilities.profiler as profiler
 
 
 superset_subquery = re.compile(r'from[\s\n]*(\(.*\))[\s\n]*as[\s\n]*virtual_table', flags=re.IGNORECASE | re.MULTILINE | re.S)
 
 
 def get_preditor_alias(step, mindsdb_database):
     predictor_name = '.'.join(step.predictor.parts)
@@ -437,14 +440,15 @@
         self.fetched_data = None
         # self._process_query(sql)
         self.create_planner()
         if execute:
             self.prepare_query(prepare=False)
             self.execute_query()
 
+    @profiler.profile()
     def create_planner(self):
         databases_names = self.session.database_controller.get_list()
         databases_names = [x['name'] for x in databases_names]
 
         predictor_metadata = []
         predictors_records = get_model_records()
 
@@ -517,15 +521,15 @@
             result = data.get_records_raw()
 
         return {
             'success': True,
             'result': result
         }
 
-    def _fetch_dataframe_step(self, step):
+    def _fetch_dataframe_step(self, step, steps_data):
         dn = self.datahub.get(step.integration)
         query = step.query
 
         if dn is None:
             raise SqlApiUnknownError(f'Unknown integration name: {step.integration}')
 
         if query is None:
@@ -536,14 +540,23 @@
                 native_query=step.raw_query,
                 session=self.session
             )
         else:
             table_alias = get_table_alias(step.query.from_table, self.database)
             # TODO for information_schema we have 'database' = 'mindsdb'
 
+            # fill params
+            def fill_params(node, **kwargs):
+                if isinstance(node, Parameter):
+                    rs = steps_data[node.value.step_num]
+                    items = [Constant(i[0]) for i in rs.get_records_raw()]
+                    return Tuple(items)
+
+            query_traversal(query, fill_params)
+
             data, columns_info = dn.query(
                 query=query,
                 session=self.session
             )
 
         # if this is query: execute it
         if isinstance(data, ASTNode):
@@ -559,22 +572,22 @@
                 table_alias=table_alias[2],
                 database=table_alias[0]
             ))
         result.add_records(data)
 
         return result
 
-    def _multiple_steps(self, steps):
+    def _multiple_steps(self, steps, steps_data):
         data = ResultSet()
         for substep in steps:
-            sub_data = self._fetch_dataframe_step(substep)
+            sub_data = self._fetch_dataframe_step(substep, steps_data)
             data = join_query_data(data, sub_data)
         return data
 
-    def _multiple_steps_reduce(self, step, vars):
+    def _multiple_steps_reduce(self, step, vars, steps_data):
         if step.reduce != 'union':
             raise ErLogicError(f'Unknown MultipleSteps type: {step.reduce}')
 
         data = ResultSet()
 
         # mark vars
         steps = []
@@ -586,15 +599,15 @@
             steps.append(substep)
 
         for var_group in vars:
             steps2 = copy.deepcopy(steps)
             for name, value in var_group.items():
                 for substep in steps2:
                     replaceQueryVar(substep.query.where, value, name)
-            sub_data = self._multiple_steps(steps2)
+            sub_data = self._multiple_steps(steps2, steps_data)
             data = join_query_data(data, sub_data)
 
         return data
 
     def prepare_query(self, prepare=True):
         if prepare:
             # it is prepared statement call
@@ -635,15 +648,16 @@
         if self.fetched_data is not None:
             # no need to execute
             return
 
         steps_data = []
         try:
             for step in self.planner.execute_steps(params):
-                data = self.execute_step(step, steps_data)
+                with profiler.Context(f'step: {step.__class__.__name__}'):
+                    data = self.execute_step(step, steps_data)
                 step.set_result(data)
                 steps_data.append(data)
         except PlanningException as e:
             raise ErLogicError(e)
 
         # save updated query
         self.query = self.planner.query
@@ -715,15 +729,15 @@
                     name=column['name'],
                     type=column.get('type'),
                     table_name=table,
                     database=self.database
                 ))
 
         elif type(step) == FetchDataframeStep:
-            data = self._fetch_dataframe_step(step)
+            data = self._fetch_dataframe_step(step, steps_data)
         elif type(step) == UnionStep:
             left_result = steps_data[step.left.step_num]
             right_result = steps_data[step.right.step_num]
 
             # count of columns have to match
             if len(left_result.columns) != len(right_result.columns):
                 raise ErSqlWrongArguments(
@@ -772,23 +786,23 @@
                 substep = step.step
                 if type(substep) == FetchDataframeStep:
                     query = substep.query
                     for var_group in vars:
                         markQueryVar(query.where)
                         for name, value in var_group.items():
                             replaceQueryVar(query.where, value, name)
-                        sub_data = self._fetch_dataframe_step(substep)
+                        sub_data = self._fetch_dataframe_step(substep, steps_data)
                         if len(data.columns) == 0:
                             data = sub_data
                         else:
                             data.add_records(sub_data.get_records())
 
                         unmarkQueryVar(query.where)
                 elif type(substep) == MultipleSteps:
-                    data = self._multiple_steps_reduce(substep, vars)
+                    data = self._multiple_steps_reduce(substep, vars, steps_data)
                 else:
                     raise ErLogicError(f'Unknown step type: {step.step}')
 
             except Exception as e:
                 raise SqlApiUnknownError(f'error in map reduce step: {e}') from e
         elif type(step) == MultipleSteps:
             if step.reduce != 'union':
@@ -800,17 +814,29 @@
                     data = subdata
                 else:
                     data.add_records(subdata.get_records())
         elif type(step) == ApplyPredictorRowStep:
 
             project_name = step.namespace
             predictor_name = step.predictor.parts[0]
-            where_data = step.row_dict
+            where_data0 = step.row_dict
             project_datanode = self.datahub.get(project_name)
 
+            # fill params
+            where_data = {}
+            for key, value in where_data0.items():
+                if isinstance(value, Parameter):
+                    rs = steps_data[value.value.step_num]
+                    if rs.length() == 1:
+                        # one value, don't do list
+                        value = rs.get_records_raw()[0][0]
+                    else:
+                        value = [i[0] for i in rs.get_records_raw()]
+                where_data[key] = value
+
             version = None
             if len(step.predictor.parts) > 1 and step.predictor.parts[-1].isdigit():
                 version = int(step.predictor.parts[-1])
 
             predictions = project_datanode.predict(
                 model_name=predictor_name,
                 data=where_data,
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         self.integration_controller = IntegrationController()
         self.database_controller = DatabaseController()
 
         self.datahub = init_datahub(self)
 
         self.prepared_stmts = {}
         self.packet_sequence_number = 0
+        self.profiling = False
 
     def inc_packet_sequence_number(self):
         self.packet_sequence_number = (self.packet_sequence_number + 1) % 256
 
     def register_stmt(self, statement):
         i = 1
         while i in self.prepared_stmts and i < 100:
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 )
 
 from mindsdb_sql.parser.ast import Insert, Identifier, CreateTable, TableColumn, DropTables
 
 from mindsdb.api.mysql.mysql_proxy.datahub.datanodes.datanode import DataNode
 from mindsdb.api.mysql.mysql_proxy.libs.constants.response_type import RESPONSE_TYPE
 from mindsdb.api.mysql.mysql_proxy.datahub.classes.tables_row import TablesRow
+import mindsdb.utilities.profiler as profiler
 
 
 class DBHandlerException(Exception):
     pass
 
 
 class IntegrationDataNode(DataNode):
@@ -110,14 +111,18 @@
                 try:
                     value = python_type(value) if value is not None else value
                 except Exception:
                     pass
                 new_row.append(value)
             formatted_data.append(new_row)
 
+        if len(formatted_data) == 0:
+            # not need to insert
+            return
+
         insert_ast = Insert(
             table=table_name,
             columns=insert_columns,
             values=formatted_data
         )
 
         try:
@@ -125,39 +130,42 @@
         except Exception as e:
             msg = f'[{self.ds_type}/{self.integration_name}]: {str(e)}'
             raise DBHandlerException(msg) from e
 
         if result.type == RESPONSE_TYPE.ERROR:
             raise Exception(result.error_message)
 
+    @profiler.profile()
     def query(self, query=None, native_query=None, session=None):
-
         try:
             if query is not None:
                 result = self.integration_handler.query(query)
             else:
                 # try to fetch native query
                 result = self.integration_handler.native_query(native_query)
         except Exception as e:
-            msg = f'[{self.ds_type}/{self.integration_name}]: {str(e)}'
+            msg = str(e).strip()
+            if msg == '':
+                msg = e.__class__.__name__
+            msg = f'[{self.ds_type}/{self.integration_name}]: {msg}'
             raise DBHandlerException(msg) from e
 
         if result.type == RESPONSE_TYPE.ERROR:
             raise Exception(f'Error in {self.integration_name}: {result.error_message}')
         if result.type == RESPONSE_TYPE.OK:
-            return
+            return [], []
 
         df = result.data_frame
         # region clearing df from NaN values
         # recursion error appears in pandas 1.5.3 https://github.com/pandas-dev/pandas/pull/45749
         if isinstance(df, pd.Series):
             df = df.to_frame()
 
         try:
-            df = df.replace(np.NaN, None)
+            df = df.replace(np.NaN, pd.NA)
         except Exception as e:
             print(f'Issue with clearing DF from NaN values: {e}')
 
         try:
             df = df.where(pd.notnull(df), None)
         except Exception as e:
             print(f'Issue with clearing DF from NaN values: {e}')
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 from mindsdb.api.mysql.mysql_proxy.classes.sql_query import Column, SQLQuery
 from mindsdb.api.mysql.mysql_proxy.utilities import (
     ErBadDbError,
     SqlApiException,
     logger,
 )
-
-
+import mindsdb.utilities.profiler as profiler
 from mindsdb.api.mysql.mysql_proxy.executor.executor_commands import ExecuteCommands
 
 
 class Executor:
     """This class stores initial and intermediatea params
     between different steps of query execution. And it is also
     creates a separate instance of ExecuteCommands to execute the current
@@ -100,14 +99,15 @@
 
         # fill params
         self.query = planner_utils.fill_query_params(self.query, param_values)
 
         # execute query
         self.do_execute()
 
+    @profiler.profile()
     def query_execute(self, sql):
         logger.info("%s.query_execute: sql - %s", self.__class__.__name__, sql)
         resp = self.execute_external(sql)
         if resp is not None:
             # is already executed
             self.is_executed = True
             return
@@ -176,14 +176,15 @@
                 # } for x in result[0].keys()]
 
                 data = [[str(value) for key, value in x.items()] for x in result]
             self.columns = columns
             self.data = data
             return True
 
+    @profiler.profile()
     def parse(self, sql):
         logger.info("%s.parse: sql - %s", self.__class__.__name__, sql)
         self.sql = sql
         sql_lower = sql.lower()
         self.sql_lower = sql_lower.replace("`", "")
 
         try:
@@ -198,14 +199,15 @@
                 raise SqlApiException(
                     f"SQL statement cannot be parsed by mindsdb_sql - {sql}: {mdb_error}"
                 ) from mdb_error
 
                 # == a place for workarounds ==
                 # or run sql in integration without parsing
 
+    @profiler.profile()
     def do_execute(self):
         # it can be already run at prepare state
         logger.info("%s.do_execute", self.__class__.__name__)
         if self.is_executed:
             return
 
         ret = self.command_executor.execute_command(self.query)
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import reduce
 
 import pandas as pd
 from mindsdb_sql.parser.dialects.mindsdb import (
     CreateDatasource,
     RetrainPredictor,
     CreatePredictor,
-    AdjustPredictor,
+    FinetunePredictor,
     CreateMLEngine,
     DropMLEngine,
     DropDatasource,
     DropPredictor,
     CreateView,
     CreateJob,
     DropJob,
@@ -76,14 +76,15 @@
     get_predictor_integration,
 )
 from mindsdb.integrations.libs.const import PREDICTOR_STATUS
 from mindsdb.interfaces.database.projects import ProjectController
 from mindsdb.interfaces.jobs.jobs_controller import JobsController
 from mindsdb.interfaces.storage.model_fs import HandlerStorage
 from mindsdb.utilities.context import context as ctx
+import mindsdb.utilities.profiler as profiler
 
 
 def _get_show_where(
     statement: ASTNode,
     from_name: Optional[str] = None,
     like_name: Optional[str] = None,
     initial: Optional[ASTNode] = None,
@@ -129,14 +130,15 @@
     def __init__(self, session, executor):
         self.session = session
         self.executor = executor
 
         self.charset_text_type = CHARSET_NUMBERS["utf8_general_ci"]
         self.datahub = session.datahub
 
+    @profiler.profile()
     def execute_command(self, statement):
         sql = None
         if self.executor is None:
             if isinstance(statement, ASTNode):
                 sql = statement.to_string()
             sql_lower = sql.lower()
         else:
@@ -167,16 +169,16 @@
         elif type(statement) == DropDatasource or type(statement) == DropDatabase:
             return self.answer_drop_database(statement)
         elif type(statement) == Describe:
             # NOTE in sql 'describe table' is same as 'show columns'
             return self.answer_describe_predictor(statement)
         elif type(statement) == RetrainPredictor:
             return self.answer_retrain_predictor(statement)
-        elif type(statement) == AdjustPredictor:
-            return self.answer_adjust_predictor(statement)
+        elif type(statement) == FinetunePredictor:
+            return self.answer_finetune_predictor(statement)
         elif type(statement) == Show:
             sql_category = statement.category.lower()
             if hasattr(statement, "modes"):
                 if isinstance(statement.modes, list) is False:
                     statement.modes = []
                 statement.modes = [x.upper() for x in statement.modes]
             if sql_category in ("predictors", "models"):
@@ -475,14 +477,21 @@
             CommitTransaction,
             RollbackTransaction,
         ):
             return ExecuteAnswer(ANSWER_TYPE.OK)
         elif type(statement) == Set:
             category = (statement.category or "").lower()
             if category == "" and type(statement.arg) == BinaryOperation:
+                if statement.arg.args[0].parts[0].lower() == 'profiling':
+                    if statement.arg.args[1].value in (1, True):
+                        profiler.enable()
+                        self.session.profiling = True
+                    else:
+                        profiler.disable()
+                        self.session.profiling = False
                 return ExecuteAnswer(ANSWER_TYPE.OK)
             elif category == "autocommit":
                 return ExecuteAnswer(ANSWER_TYPE.OK)
             elif category == "names":
                 # set names utf8;
                 charsets = {
                     "utf8": CHARSET_NUMBERS["utf8_general_ci"],
@@ -632,15 +641,15 @@
 
         model_record = get_model_record(
             name=model_name, project_name=database_name, except_absent=True
         )
         return model_record
 
     def _sync_predictor_check(self, phase_name):
-        """ Checks if there is already a predictor retraining or adjusting
+        """ Checks if there is already a predictor retraining or fine-tuning
             Do not allow to run retrain if there is another model in training process in less that 1h
         """
         is_cloud = self.session.config.get('cloud', False)
         if is_cloud and ctx.user_class == 0:
             models = get_model_records(active=None)
             shortest_training = None
             for model in models:
@@ -700,29 +709,29 @@
         columns = [
             Column(col)
             for col in resp_dict['columns']
         ]
 
         return ExecuteAnswer(answer_type=ANSWER_TYPE.TABLE, columns=columns, data=resp_dict['data'])
 
-    def answer_adjust_predictor(self, statement):
+    def answer_finetune_predictor(self, statement):
         model_record = self._get_model_record(statement)
 
         if statement.using is not None:
             # repack using with lower names
             statement.using = {k.lower(): v for k, v in statement.using.items()}
 
         # use current ml handler
         integration_record = get_predictor_integration(model_record)
         if integration_record is None:
             raise Exception('The ML engine that the model was trained with does not exist.')
         ml_handler = self.session.integration_controller.get_handler(integration_record.name)
 
-        self._sync_predictor_check(phase_name='adjust')
-        df = self.session.model_controller.adjust_model(statement, ml_handler)
+        self._sync_predictor_check(phase_name='finetune')
+        df = self.session.model_controller.finetune_model(statement, ml_handler)
 
         resp_dict = df.to_dict(orient='split')
 
         columns = [
             Column(col)
             for col in resp_dict['columns']
         ]
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     STMTPrepareHeaderPacket,
     BinaryResultsetRowPacket
 )
 
 from mindsdb.api.mysql.mysql_proxy.executor import Executor
 from mindsdb.utilities.context import context as ctx
 import mindsdb.utilities.hooks as hooks
+import mindsdb.utilities.profiler as profiler
 
 
 def empty_fn():
     pass
 
 
 def check_auth(username, password, scramble_func, salt, company_id, config):
@@ -475,14 +476,15 @@
                 'alias': column_record.alias or column_record.name,
                 # NOTE all work with text-type, but if/when wanted change types to real,
                 # it will need to check all types casts in BinaryResultsetRowPacket
                 'type': column_type
             })
         return result
 
+    @profiler.profile()
     def process_query(self, sql):
         executor = Executor(
             session=self.session,
             sqlserver=self
         )
 
         executor.query_execute(sql)
@@ -673,15 +675,17 @@
             error_traceback = None
 
             try:
                 if p.type.value == COMMANDS.COM_QUERY:
                     sql = self.decode_utf(p.sql.value)
                     sql = SqlStatementParser.clear_sql(sql)
                     logger.debug(f'COM_QUERY: {sql}')
-                    response = self.process_query(sql)
+                    profiler.set_meta(query=sql, api='mysql', environment=Config().get('environment'))
+                    with profiler.Context('mysql_query_processing'):
+                        response = self.process_query(sql)
                 elif p.type.value == COMMANDS.COM_STMT_PREPARE:
                     sql = self.decode_utf(p.sql.value)
                     self.answer_stmt_prepare(sql)
                 elif p.type.value == COMMANDS.COM_STMT_EXECUTE:
                     self.answer_stmt_execute(p.stmt_id.value, p.parameters)
                 elif p.type.value == COMMANDS.COM_STMT_FETCH:
                     self.answer_stmt_fetch(p.stmt_id.value, p.limit.value)
@@ -787,19 +791,23 @@
             return self.packet(OkPacket, eof=True, status=status)
         else:
             return self.packet(EofPacket, status=status)
 
     def set_context(self, context):
         if 'db' in context:
             self.session.database = context['db']
+        if 'profiling' in context:
+            self.session.profiling = context['profiling']
 
     def get_context(self, context):
         context = {}
         if self.session.database is not None:
             context['db'] = self.session.database
+        if self.session.profiling is True:
+            context['profiling'] = True
 
         return context
 
     @staticmethod
     def startProxy():
         """
         Create a server and wait for incoming connections until Ctrl-C
```

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py` & `MindsDB-23.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/api/nlp/nlp.py` & `MindsDB-23.4.3.0/mindsdb/api/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/autokeras_handler/setup.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/autokeras_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/logo.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/logo.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,31 +57,40 @@
         if self.is_connected is True:
             return self.cluster
         
         # User Input ends here.
         endpoint = self.connection_data.get('host')
         username = self.connection_data.get('user')
         password = self.connection_data.get('password')
-        bucket_name = self.connection_data.get('bucket')
+
+        try:
+            timeout = int(self.connection_data.get('timeout'))
+        except Exception:
+            timeout = 10
         # Connect options - global timeout opts
-        timeout_opts = ClusterTimeoutOptions(kv_timeout=timedelta(seconds=10))
-        
+        timeout_opts = ClusterTimeoutOptions(kv_timeout=timedelta(seconds=timeout))
+
         auth = PasswordAuthenticator(
             username,
             password,
             # NOTE: If using SSL/TLS, add the certificate path.
             # We strongly reccomend this for production use.
             # cert_path=cert_path
         )
 
-
-        cluster = Cluster.connect(f'couchbase://{endpoint}', ClusterOptions(auth))
+        cluster = Cluster.connect(
+            f'couchbase://{endpoint}',
+            ClusterOptions(
+                authenticator=auth,
+                timeout_options=timeout_opts
+            )
+        )
         
         # # Wait until the cluster is ready for use.
-        cluster.wait_until_ready(timedelta(seconds=5))
+        cluster.wait_until_ready(timedelta(seconds=timeout))
         
         self.is_connected = cluster.connected
         self.cluster = cluster
         return self.cluster
 
     
     def disconnect(self):
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/logo.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         if 'pytorch' not in metadata.tags:
             raise Exception('Currently only PyTorch models are supported (https://huggingface.co/models?library=pytorch&sort=downloads). To request another library, please contact us on our community slack (https://mindsdbcommunity.slack.com/join/shared_invite/zt-1e2cxo4ts-dUuoryp8n2hhyymPlzjD0A#/shared-invite/email).')
 
         # check model task
         supported_tasks = ['text-classification',
                            'zero-shot-classification',
                            'translation',
-                           'summarization']
+                           'summarization',
+                           'fill-mask']
 
         if metadata.pipeline_tag not in supported_tasks:
             raise Exception(f'Not supported task for model: {metadata.pipeline_tag}.\
              Should be one of {", ".join(supported_tasks)}')
 
         if 'task' not in args:
             args['task'] = metadata.pipeline_tag
@@ -175,14 +176,22 @@
 
         def tidy_output_summarization(args, result):
             final = {}
             final[args['target']] = result['summary_text']
 
             return final
 
+        def tidy_output_fill_mask(args, result):
+            final = {}
+            final[args['target']] = result[0]['sequence']
+            explain = {elem['sequence']: elem['score'] for elem in result}
+            final[f"{args['target']}_explain"] = explain
+
+            return final
+
         ###### get stuff from model folder
         args = self.model_storage.json_get('args')
 
         hf_model_storage_path = self.engine_storage.folder_get(args['model_name'], update=False)
 
         pipeline = transformers.pipeline(task=args['task_proper'], model=hf_model_storage_path,
                                          tokenizer=hf_model_storage_path)
@@ -226,14 +235,18 @@
             output_list_tidy = [tidy_output_translation(args, x) for x in output_list_messy]
 
         elif task == 'summarization':
             output_list_messy = pipeline(input_list_str,
                                          min_length=args['min_output_length'],
                                          max_length=args['max_output_length'])
             output_list_tidy = [tidy_output_summarization(args, x) for x in output_list_messy]
+
+        elif task == 'fill-mask':
+            output_list_messy = pipeline(input_list_str)
+            output_list_tidy = [tidy_output_fill_mask(args, x) for x in output_list_messy]
         else:
             raise RuntimeError(f'Unknown task: {task}')
 
         # inject errors info
         for i, msg in errors:
             output_list_tidy.insert(i, {'error': msg})
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/huggingface_handler/setup.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/huggingface_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/jira_handler/tests/test_jira_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/jira_handler/tests/test_jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,30 +159,30 @@
     run_fit(predictor_id, df, model_storage)
 
     predictor_record.status = PREDICTOR_STATUS.COMPLETE
     predictor_record.training_stop_at = datetime.now()
     db.session.commit()
 
 
-@mark_process(name='adjust')
-def run_adjust(df: DataFrame, args: dict, model_storage):
+@mark_process(name='finetune')
+def run_finetune(df: DataFrame, args: dict, model_storage):
     try:
         base_predictor_id = args['base_model_id']
         base_predictor_record = db.Predictor.query.filter_by(
             id=base_predictor_id,
             status=PREDICTOR_STATUS.COMPLETE
         ).first()
 
         predictor_id = model_storage.predictor_id
         predictor_record = db.Predictor.query.filter_by(id=predictor_id).first()
 
         # TODO move this to ModelStorage (don't work with database directly)
         predictor_record.data = {'training_log': 'training'}
         predictor_record.training_start_at = datetime.now()
-        predictor_record.status = PREDICTOR_STATUS.ADJUSTING  # TODO: parallel execution block
+        predictor_record.status = PREDICTOR_STATUS.FINETUNING  # TODO: parallel execution block
         db.session.commit()
 
         base_fs = FileStorage(
             resource_group=RESOURCE_GROUP.PREDICTOR,
             resource_id=base_predictor_id,
             sync=True
         )
@@ -194,15 +194,15 @@
             resource_group=RESOURCE_GROUP.PREDICTOR,
             resource_id=predictor_id,
             sync=True
         )
         predictor.save(fs.folder_path / fs.folder_name)
         fs.push()
 
-        predictor_record.data = predictor.model_analysis.to_dict()  # todo: update accuracy in LW as post-adjust hook
+        predictor_record.data = predictor.model_analysis.to_dict()  # todo: update accuracy in LW as post-finetune hook
         predictor_record.code = base_predictor_record.code
         predictor_record.update_status = 'up_to_date'
         predictor_record.status = PREDICTOR_STATUS.COMPLETE
         predictor_record.training_stop_at = datetime.now()
         db.session.commit()
 
         predictor_records = get_model_records(
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 import mindsdb.interfaces.storage.db as db
 
 from mindsdb.utilities.functions import cast_row_types
 # from mindsdb.utilities.hooks import after_predict as after_predict_hook
 from mindsdb.interfaces.model.functions import get_model_record
 from mindsdb.interfaces.storage.json import get_json_storage
 from mindsdb.integrations.libs.base import BaseMLEngine
+import mindsdb.utilities.profiler as profiler
 
-from .functions import run_learn, run_adjust
+from .functions import run_learn, run_finetune
 
 IS_PY36 = sys.version_info[1] <= 6
 
 
 class NumpyJSONEncoder(json.JSONEncoder):
     """
     Use this encoder to avoid
@@ -66,35 +67,40 @@
         args['target'] = target
         run_learn(
             df,
             args,   # Problem definition and JsonAI override
             self.model_storage
         )
 
-    def update(self, df: Optional[pd.DataFrame] = None, args: Optional[Dict] = None) -> None:
-        run_adjust(
+    def finetune(self, df: Optional[pd.DataFrame] = None, args: Optional[Dict] = None) -> None:
+        run_finetune(
             df,
             args,
             self.model_storage
         )
 
+    @profiler.profile('LightwoodHandler.predict')
     def predict(self, df, args=None):
         pred_format = args['pred_format']
         predictor_code = args['code']
         learn_args = args['learn_args']
         pred_args = args.get('predict_params', {})
         self.model_storage.fileStorage.pull()
 
-        predictor = lightwood.predictor_from_state(
-            self.model_storage.fileStorage.folder_path / self.model_storage.fileStorage.folder_name,
-            predictor_code
-        )
+        with profiler.Context('load model'):
+            predictor = lightwood.predictor_from_state(
+                self.model_storage.fileStorage.folder_path / self.model_storage.fileStorage.folder_name,
+                predictor_code
+            )
+
         dtype_dict = predictor.dtype_dict
 
-        predictions = predictor.predict(df, args=pred_args)
+        with profiler.Context('predict'):
+            predictions = predictor.predict(df, args=pred_args)
+
         predictions = predictions.to_dict(orient='records')
 
         # TODO!!!
         # after_predict_hook(
         #     company_id=self.company_id,
         #     predictor_id=predictor_record.id,
         #     rows_in_count=df.shape[0],
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/setup.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/ludwig_handler/setup.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/ludwig_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/merlion_handler/setup.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/merlion_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mlflow_handler/setup.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mlflow_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import os
+from sklearn.metrics import r2_score
+import pandas as pd
 import tempfile
-import string
-import random
 from mindsdb.integrations.libs.base import BaseMLEngine
 from mindsdb.integrations.utilities.time_series_utils import (
     transform_to_nixtla_df,
     get_results_from_nixtla_df,
     infer_frequency,
+    get_model_accuracy_dict
 )
 from neuralforecast import NeuralForecast
 from neuralforecast.models import NHITS
 from neuralforecast.auto import AutoNHITS
 from ray.tune.search.hyperopt import HyperOptSearch
 
 DEFAULT_FREQUENCY = "D"
@@ -58,25 +58,27 @@
         model_args["order_by"] = time_settings["order_by"]
         model_args["group_by"] = time_settings["group_by"]
         model_args["frequency"] = (
             using_args["frequency"] if "frequency" in using_args else infer_frequency(df, time_settings["order_by"])
         )
         model_args["model_name"] = DEFAULT_MODEL_NAME
         num_trials = int(DEFAULT_TRIALS * using_args["train_time"]) if "train_time" in using_args else DEFAULT_TRIALS
-        exog_vars = using_args["exogenous_vars"] if "exogenous_vars" in using_args else []
+        model_args["exog_vars"] = using_args["exogenous_vars"] if "exogenous_vars" in using_args else []
         model_args["model_folder"] = tempfile.mkdtemp()
 
         # Train model
         model = choose_model(num_trials, time_settings["horizon"], time_settings["window"])
-        nixtla_df = transform_to_nixtla_df(df, model_args, exog_vars)
-        nf = NeuralForecast(models=[model], freq=model_args["frequency"])
-        nf.fit(nixtla_df)
-        nf.save(model_args["model_folder"], overwrite=True)
+        nixtla_df = transform_to_nixtla_df(df, model_args, model_args["exog_vars"])
+        neural = NeuralForecast(models=[model], freq=model_args["frequency"])
+        results_df = neural.cross_validation(nixtla_df)
+        # Get model accuracy
+        model_args["accuracies"] = get_model_accuracy_dict(results_df, r2_score)
 
         ###### persist changes to handler folder
+        neural.save(model_args["model_folder"], overwrite=True)
         self.model_storage.json_set("model_args", model_args)
 
     def predict(self, df, args={}):
         """Makes forecasts with the NeuralForecast Handler.
 
         NeuralForecast is setup to predict for all groups, so it won't handle
         a dataframe that's been filtered to one group very well. Instead, we make
@@ -85,11 +87,31 @@
         """
         # Load model arguments
         model_args = self.model_storage.json_get("model_args")
 
         prediction_df = transform_to_nixtla_df(df, model_args)
         groups_to_keep = prediction_df["unique_id"].unique()
 
-        nf = NeuralForecast.load(model_args["model_folder"])
-        forecast_df = nf.predict(prediction_df)
+        neural = NeuralForecast.load(model_args["model_folder"])
+        forecast_df = neural.predict(prediction_df)
         forecast_df = forecast_df[forecast_df.index.isin(groups_to_keep)]
         return get_results_from_nixtla_df(forecast_df, model_args)
+
+    def describe(self, attribute=None):
+        model_args = self.model_storage.json_get("model_args")
+
+        if attribute == "model":
+            return pd.DataFrame({k: [model_args[k]] for k in ["model_name", "frequency"]})
+
+        if attribute == "features":
+            return pd.DataFrame(
+                {"ds": [model_args["order_by"]], "y": model_args["target"], "unique_id": [model_args["group_by"]], "exog_vars": [model_args["exog_vars"]]}
+            )
+
+        if attribute == "ensemble":
+            raise Exception(f"DESCRIBE {attribute} is not supported by this Handler.")
+
+        if attribute is None:
+            outputs = model_args["target"]
+            inputs = [model_args["target"], model_args["order_by"], model_args["group_by"]] + model_args["exog_vars"]
+            accuracies = [(model, acc) for model, acc in model_args["accuracies"].items()]
+            return pd.DataFrame({"accuracies": [accuracies], "outputs": outputs, "inputs": [inputs]})
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import random
 import time
 import math
 
 import openai
 import tiktoken
 
+import mindsdb.utilities.profiler as profiler
+
 
 def retry_with_exponential_backoff(
         initial_delay: float = 1,
         hour_budget: float = 0.3,
         jitter: bool = False,
         exponential_base: int = 2,
-        errors: tuple = (openai.error.RateLimitError,),
+        errors: tuple = (openai.error.RateLimitError, openai.error.APIConnectionError),
 ):
     """
     Wrapper to enable optional arguments. It means this decorator always needs to be called with parenthesis:
     
     > @retry_with_exponential_backoff()  # optional argument override here
     > def f(): [...]
     
     """  # noqa
 
+    @profiler.profile()
     def _retry_with_exponential_backoff(func):
         """
         Exponential backoff to retry requests on a rate-limited API call, as recommended by OpenAI.
         Loops the call until a successful response or max_retries is hit or an exception is raised.
 
         Slight changes in the implementation, but originally from:
         https://github.com/openai/openai-cookbook/blob/main/examples/How_to_handle_rate_limits.ipynb
@@ -45,33 +48,34 @@
                 max_retries = 10
             max_retries = max(1, max_retries)
 
             while True:
                 try:
                     return func(*args, **kwargs)
                 except errors as e:
-                    if e.error['type'] == 'invalid_request_error' and \
-                            'Too many parallel completions' in e.error['message'] or \
-                            'Please reduce the length of the messages' in e.error['message']:
-                        raise e  # InvalidRequestError triggers batched mode in the previous call
-                    if e.error['type'] == 'insufficient_quota':
-                        raise Exception(
-                            'API key has exceeded its quota, please try 1) increasing it or 2) using another key.')  # noqa
+                    if e.error is not None:
+                        if e.error['type'] == 'invalid_request_error' and \
+                                'Too many parallel completions' in e.error['message'] or \
+                                'Please reduce the length of the messages' in e.error['message']:
+                            raise e  # InvalidRequestError triggers batched mode in the previous call
+                        if e.error['type'] == 'insufficient_quota':
+                            raise Exception(
+                                'API key has exceeded its quota, please try 1) increasing it or 2) using another key.')  # noqa
 
                     num_retries += 1
                     if num_retries > max_retries:
                         raise Exception(
                             f"Maximum number of retries ({max_retries}) exceeded."
                         )
                     # Increment the delay and wait
                     delay *= exponential_base * (1 + jitter * random.random())
                     time.sleep(delay)
 
                 except openai.error.OpenAIError as e:
-                    if e.error['type'] == 'insufficient_quota':
+                    if e.error is not None and e.error['type'] == 'insufficient_quota':
                         raise Exception(
                             'API key has exceeded its quota, please try 1) increasing it or 2) using another key.')  # noqa
                     raise e
 
                 except Exception as e:
                     raise e
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         if not args.get('mode'):
             args['mode'] = self.default_mode
         elif args['mode'] not in self.supported_modes:
             raise Exception(f"Invalid operation mode. Please use one of {self.supported_modes}")
 
         self.model_storage.json_set('args', args)
 
-    def _get_api_key(self, args):
+    def _get_openai_api_key(self, args, strict=True):
         """ 
         API_KEY preference order:
             1. provided at model creation
             2. provided at engine creation
             3. OPENAI_API_KEY env variable
             4. openai.api_key setting in config.json
         """  # noqa
@@ -95,16 +95,17 @@
             return api_key
         # 4
         config = Config()
         openai_cfg = config.get('openai', {})
         if 'api_key' in openai_cfg:
             return openai_cfg['api_key']
 
-        raise Exception('Missing API key. Either re-create this ML_ENGINE with your key in the `api_key` parameter,\
-             or re-create this model and pass the API key it with `USING` syntax.')  # noqa
+        if strict:
+            raise Exception(f'Missing API key "api_key". Either re-create this ML_ENGINE specifying the `api_key` parameter,\
+                 or re-create this model and pass the API key with `USING` syntax.')  # noqa
 
     def predict(self, df, args=None):
         """
         If there is a prompt template, we use it. Otherwise, we use the concatenation of `context_column` (optional) and `question_column` to ask for a completion.
         """ # noqa
         # TODO: support for edits, embeddings and moderation
 
@@ -116,19 +117,21 @@
             if pred_args['mode'] in self.supported_modes:
                 args['mode'] = pred_args['mode']
             else:
                 raise Exception(f"Invalid operation mode. Please use one of {self.supported_modes}.")  # noqa
 
         if pred_args.get('prompt_template', False):
             base_template = pred_args['prompt_template']  # override with predict-time template if available
-        else:
+        elif args.get('prompt_template', False):
             base_template = args['prompt_template']
+        else:
+            base_template = None
 
         # Image mode
-        if args['mode'] == 'image':
+        if args.get('mode', self.default_mode) == 'image':
             api_args = {
                 'n': pred_args.get('n', None),
                 'size': pred_args.get('size', None),
                 'response_format': pred_args.get('response_format', None),
             }
             api_args = {k: v for k, v in api_args.items() if v is not None}  # filter out non-specified api args
             model_name = 'image'
@@ -160,15 +163,15 @@
                 'presence_penalty': pred_args.get('presence_penalty', None),
                 'frequency_penalty': pred_args.get('frequency_penalty', None),
                 'best_of': pred_args.get('best_of', None),
                 'logit_bias': pred_args.get('logit_bias', None),
                 'user': pred_args.get('user', None),
             }
 
-            if args['mode'] != 'default' and model_name not in self.chat_completion_models:
+            if args.get('mode', self.default_mode) != 'default' and model_name not in self.chat_completion_models:
                 raise Exception(f"Conversational modes are only available for the following models: {', '.join(self.chat_completion_models)}")  # noqa
 
             if args.get('prompt_template', False):
                 prompts, empty_prompt_ids = self._get_completed_prompts(base_template, df)
 
             elif args.get('context_column', False):
                 empty_prompt_ids = np.where(df[[args['context_column'],
@@ -215,15 +218,15 @@
             else:
                 empty_prompt_ids = np.where(df[[args['question_column']]].isna().all(axis=1).values)[0]
                 prompts = list(df[args['question_column']].apply(lambda x: str(x)))
 
         # remove prompts without signal from completion queue
         prompts = [j for i, j in enumerate(prompts) if i not in empty_prompt_ids]
 
-        api_key = self._get_api_key(args)
+        api_key = self._get_openai_api_key(args)
         api_args = {k: v for k, v in api_args.items() if v is not None}  # filter out non-specified api args
         completion = self._completion(model_name, prompts, api_key, api_args, args, df)
 
         # add null completion for empty prompts
         for i in sorted(empty_prompt_ids):
             completion.insert(i, None)
 
@@ -411,54 +414,54 @@
                     completion['choices'].extend(p['choices'].result()['choices'])
 
         return completion
 
     def describe(self, attribute: Optional[str] = None) -> pd.DataFrame:
         # TODO: Update to use update() artifacts
         args = self.model_storage.json_get('args')
-        api_key = self._get_api_key(args)
+        api_key = self._get_openai_api_key(args)
 
         model_name = args.get('model_name', self.default_model)
         meta = openai.Model.retrieve(model_name, api_key=api_key)
 
         return pd.DataFrame([[meta['id'], meta['object'], meta['owned_by'], meta['permission'], args]],
                             columns=['id', 'object', 'owned_by', 'permission', 'model_args'])
 
-    def update(self, df: Optional[pd.DataFrame] = None, args: Optional[Dict] = None) -> None:
+    def finetune(self, df: Optional[pd.DataFrame] = None, args: Optional[Dict] = None) -> None:
         """
         Fine-tune OpenAI GPT models. Steps are roughly:
           - Analyze input data and modify it according to suggestions made by the OpenAI utility tool
           - Get a training and validation file
           - Determine base model to use
           - Submit a fine-tuning job via the OpenAI API
           - Monitor progress with exponential backoff (which has been modified for greater control given a time budget in hours), 
           - Gather stats once fine-tuning finishes
           - Modify model metadata so that the new version triggers the fine-tuned version of the model (stored in the user's OpenAI account)
 
         Caveats: 
-          - As base fine-tuning models, OpenAI only supports the original GPT ones: `ada`, `babbage`, `curie`, `davinci`. This means if you adjust successively more than once, any fine-tuning other than the most recent one is lost.
+          - As base fine-tuning models, OpenAI only supports the original GPT ones: `ada`, `babbage`, `curie`, `davinci`. This means if you fine-tune successively more than once, any fine-tuning other than the most recent one is lost.
         """  # noqa
 
         args = args if args else {}
         using_args = args.pop('using') if 'using' in args else {}
         prompt_col = using_args.get('prompt_column', 'prompt')
         completion_col = using_args.get('completion_column', 'completion')
 
         for col in [prompt_col, completion_col]:
             if col not in set(df.columns):
                 raise Exception(f"To fine-tune this OpenAI model, please format your select data query to have a `{prompt_col}` column and a `{completion_col}` column first.")  # noqa
 
         args = {**using_args, **args}
         prev_model_name = self.base_model_storage.json_get('args').get('model_name', '')
 
-        openai.api_key = self._get_api_key(args)
-        adjust_time = datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
+        openai.api_key = self._get_openai_api_key(args)
+        finetune_time = datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
 
         temp_storage_path = tempfile.mkdtemp()
-        temp_file_name = f"ft_{adjust_time}"
+        temp_file_name = f"ft_{finetune_time}"
         temp_model_storage_path = f"{temp_storage_path}/{temp_file_name}.jsonl"
         df.to_json(temp_model_storage_path, orient='records', lines=True)
 
         # TODO avoid subprocess usage once OpenAI enables non-CLI access
         subprocess.run(
             [
                 "openai", "tools", "fine_tunes.prepare_data",
@@ -466,29 +469,27 @@
                 '-q'                                            # quiet mode (accepts all suggestions)
             ],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             encoding="utf-8",
         )
 
-        file_names = [f'{temp_file_name}.jsonl',
-                      f'{temp_file_name}_prepared_train.jsonl',
-                      f'{temp_file_name}_prepared_valid.jsonl']
-        returns = []
-        for file_name in file_names:
+        file_names = {'original': f'{temp_file_name}.jsonl',
+                      'base': f'{temp_file_name}_prepared.jsonl',
+                      'train': f'{temp_file_name}_prepared_train.jsonl',
+                      'val': f'{temp_file_name}_prepared_valid.jsonl'}
+        jsons = {k: None for k in file_names.keys()}
+        for split, file_name in file_names.items():
             if os.path.isfile(os.path.join(temp_storage_path, file_name)):
-                returns.append(openai.File.create(
+                jsons[split] = openai.File.create(
                     file=open(f"{temp_storage_path}/{file_name}", "rb"),
                     purpose='fine-tune')
-                )
-            else:
-                returns.append(None)
 
-        train_file_id = returns[1].id if isinstance(returns[1], openai.File) else returns[0].id
-        val_file_id = returns[2].id if isinstance(returns[2], openai.File) else None
+        train_file_id = jsons['train'].id if isinstance(jsons['train'], openai.File) else jsons['base']
+        val_file_id = jsons['val'].id if isinstance(jsons['val'], openai.File) else None
 
         def _get_model_type(model_name: str):
             for model_type in ['ada', 'curie', 'babbage', 'davinci']:
                 if model_type in model_name.lower():
                     return model_type
             return 'ada'
 
@@ -507,15 +508,17 @@
             'classification_positive_class': using_args.get('classification_positive_class', None),
             'classification_betas': using_args.get('classification_betas', None),
         }
 
         start_time = datetime.datetime.now()
         ft_result = openai.FineTune.create(**{k: v for k, v in ft_params.items() if v is not None})
 
-        @retry_with_exponential_backoff(hour_budget=args.get('hour_budget', 8))
+        @retry_with_exponential_backoff(
+            hour_budget=args.get('hour_budget', 8),
+            errors=(openai.error.RateLimitError, openai.error.OpenAIError))
         def _check_ft_status(model_id):
             ft_retrieved = openai.FineTune.retrieve(id=model_id)
             if ft_retrieved['status'] in ('succeeded', 'failed'):
                 return ft_retrieved
             else:
                 raise openai.error.OpenAIError('Fine-tuning still pending!')
 
@@ -526,54 +529,57 @@
             raise Exception(f"Fine-tuning did not complete successfully (status: {ft_stats['status']}). Error message: {ft_stats['events'][-1]['message']}")  # noqa
 
         end_time = datetime.datetime.now()
         runtime = end_time - start_time
 
         result_file_id = openai.FineTune.retrieve(id=ft_result.id)['result_files'][0].id
         name_extension = openai.File.retrieve(id=result_file_id).filename
-        result_path = f'{temp_storage_path}/ft_{adjust_time}_result_{name_extension}'
+        result_path = f'{temp_storage_path}/ft_{finetune_time}_result_{name_extension}'
         with open(result_path, 'wb') as f:
             f.write(openai.File.download(id=result_file_id))
 
         train_stats = pd.read_csv(result_path)
         if 'validation_token_accuracy' in train_stats.columns:
             train_stats = train_stats[train_stats['validation_token_accuracy'].notnull()]
 
         args['model_name'] = ft_model_name
         args['ft_api_info'] = ft_stats.to_dict_recursive()
         args['ft_result_stats'] = train_stats.to_dict()
         args['runtime'] = runtime.total_seconds()
+        args['mode'] = self.base_model_storage.json_get('args').get('mode', self.default_mode)
 
         self.model_storage.json_set('args', args)
         shutil.rmtree(temp_storage_path)
 
     @staticmethod
     def _get_completed_prompts(base_template, df):
         columns = []
         spans = []
         matches = list(re.finditer("{{(.*?)}}", base_template))
 
+        assert len(matches) > 0, 'No placeholders found in the prompt, please provide a valid prompt template.'
+
         first_span = matches[0].start()
         last_span = matches[-1].end()
 
         for m in matches:
             columns.append(m[0].replace('{', '').replace('}', ''))
             spans.extend((m.start(), m.end()))
 
-        spans = spans[1:-1]
-        template = [base_template[s:e] for s, e in zip(spans, spans[1:])]
-        template.insert(0, base_template[0:first_span])
-        template.append(base_template[last_span:])
+        spans = spans[1:-1]  # omit first and last, they are added separately
+        template = [base_template[s:e] for s, e in list(zip(spans, spans[1:]))[::2]]  # take every other to skip placeholders  # noqa
+        template.insert(0, base_template[0:first_span])  # add prompt start
+        template.append(base_template[last_span:])  # add prompt end
 
         empty_prompt_ids = np.where(df[columns].isna().all(axis=1).values)[0]
 
         df['__mdb_prompt'] = ''
         for i in range(len(template)):
             atom = template[i]
             if i < len(columns):
                 col = df[columns[i]].replace(to_replace=[None], value='')  # add empty quote if data is missing
-                df['__mdb_prompt'] = df['__mdb_prompt'].apply(lambda x: x + atom) + col
+                df['__mdb_prompt'] = df['__mdb_prompt'].apply(lambda x: x + atom) + col.astype("string")
             else:
                 df['__mdb_prompt'] = df['__mdb_prompt'].apply(lambda x: x + atom)
         prompts = list(df['__mdb_prompt'])
 
         return prompts, empty_prompt_ids
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/openai_handler/setup.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/langchain_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/rockset_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/rockset_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/logo.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/solr.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/solr.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from mindsdb.integrations.libs.base import BaseMLEngine
 from mindsdb.integrations.utilities.time_series_utils import (
     transform_to_nixtla_df,
     get_results_from_nixtla_df,
     infer_frequency,
     get_best_model_from_results_df,
     get_model_accuracy_dict,
+    reconcile_forecasts,
+    get_hierarchy_from_df
 )
 from sklearn.metrics import r2_score
 from statsforecast import StatsForecast
 from statsforecast.models import AutoARIMA, AutoCES, AutoETS, AutoTheta
 
 DEFAULT_MODEL_NAME = "AutoARIMA"
 model_dict = {
@@ -95,15 +97,21 @@
         model_args["target"] = target
         model_args["horizon"] = time_settings["horizon"]
         model_args["order_by"] = time_settings["order_by"]
         model_args["group_by"] = time_settings["group_by"]
         model_args["frequency"] = (
             using_args["frequency"] if "frequency" in using_args else infer_frequency(df, time_settings["order_by"])
         )
-        training_df = transform_to_nixtla_df(df, model_args)
+        model_args["hierarchy"] = using_args["hierarchy"] if "hierarchy" in using_args else False
+        if model_args["hierarchy"]:
+            training_df, hier_df, hier_dict = get_hierarchy_from_df(df, model_args)
+            self.model_storage.file_set("hier_dict", dill.dumps(hier_dict))
+            self.model_storage.file_set("hier_df", dill.dumps(hier_df))
+        else:
+            training_df = transform_to_nixtla_df(df, model_args)
 
         model_args["model_name"] = DEFAULT_MODEL_NAME if "model_name" not in using_args else using_args["model_name"]
 
         results_df = get_insample_cv_results(model_args, training_df)
         model_args["accuracies"] = get_model_accuracy_dict(results_df, r2_score)
         model = choose_model(model_args, results_df)
         sf = StatsForecast([model], freq=model_args["frequency"], df=training_df)
@@ -129,22 +137,31 @@
 
         prediction_df = transform_to_nixtla_df(df, model_args)
         groups_to_keep = prediction_df["unique_id"].unique()
 
         sf = StatsForecast(models=[], freq=model_args["frequency"], df=training_df)
         sf.fitted_ = fitted_models
         forecast_df = sf.predict(model_args["horizon"])
-        forecast_df = forecast_df[forecast_df.index.isin(groups_to_keep)]
-        return get_results_from_nixtla_df(forecast_df, model_args)
+
+        if model_args["hierarchy"]:
+            hier_df = dill.loads(self.model_storage.file_get("hier_df"))
+            hier_dict = dill.loads(self.model_storage.file_get("hier_dict"))
+            reconciled_df = reconcile_forecasts(training_df, forecast_df, hier_df, hier_dict)
+            results_df = reconciled_df[reconciled_df.index.isin(groups_to_keep)]
+
+        else:
+            results_df = forecast_df[forecast_df.index.isin(groups_to_keep)]
+
+        return get_results_from_nixtla_df(results_df, model_args)
 
     def describe(self, attribute=None):
         model_args = self.model_storage.json_get("model_args")
 
         if attribute == "model":
-            return pd.DataFrame({k: [model_args[k]] for k in ["model_name", "frequency", "season_length"]})
+            return pd.DataFrame({k: [model_args[k]] for k in ["model_name", "frequency", "season_length", "hierarchy"]})
 
         if attribute == "features":
             return pd.DataFrame(
                 {"ds": [model_args["order_by"]], "y": model_args["target"], "unique_id": [model_args["group_by"]]}
             )
 
         if attribute == "ensemble":
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/teradata_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/teradata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/tpot_handler/setup.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/tpot_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/icon.png` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         :param query: The SQL query to run in Trino
         :return: returns the records from the current recordset
         """
         try:
             connection = self.connect()
             cur = connection.cursor()
             result = cur.execute(query)
-            if result:
+            if result and cur.description:
                 response = Response(
                     RESPONSE_TYPE.TABLE,
                     data_frame=pd.DataFrame(
                         result,
                         columns=[x[0] for x in cur.description]
                     )
                 )
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/twitter_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/twitter_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,109 +1,97 @@
 import re
 import os
 import datetime as dt
 import ast
+import time
 from collections import defaultdict
 import pytz
 import io
 import requests
 
 import pandas as pd
 import tweepy
 
 from mindsdb.utilities import log
 from mindsdb.utilities.config import Config
 
 from mindsdb_sql.parser import ast
-from mindsdb_sql.planner.utils import query_traversal
 
 from mindsdb.integrations.libs.api_handler import APIHandler, APITable, FuncParser
+from mindsdb.integrations.utilities.sql_utils import extract_comparison_conditions
+from mindsdb.integrations.utilities.date_utils import parse_utc_date
 
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
 
 
-def extract_conditions(binary_op):
-    conditions = []
-
-    def _extract_conditions(node, **kwargs):
-        if isinstance(node, ast.BinaryOperation):
-            op = node.op.lower()
-            if op == 'and':
-                return
-            elif op == 'or':
-                raise NotImplementedError
-            elif not isinstance(node.args[0], ast.Identifier) or not isinstance(node.args[1], ast.Constant):
-                raise NotImplementedError
-            conditions.append([op, node.args[0].parts[-1], node.args[1].value])
-
-    query_traversal(binary_op, _extract_conditions)
-    return conditions
-
-
-def parse_date(date_str):
-    if isinstance(date_str, dt.datetime):
-        return date_str
-    date_formats = ['%Y-%m-%d %H:%M:%S', '%Y-%m-%d']
-    date = None
-    for date_format in date_formats:
-        try:
-            date = dt.datetime.strptime(date_str, date_format)
-        except ValueError:
-            pass
-    if date is None:
-        raise ValueError(f"Can't parse date: {date_str}")
-    date = date.astimezone(pytz.utc)
-    return date
-
-
 class TweetsTable(APITable):
-    
+
     def select(self, query: ast.Select) -> Response:
 
-        conditions = extract_conditions(query.where)
+        conditions = extract_comparison_conditions(query.where)
 
         params = {}
+        filters = []
         for op, arg1, arg2 in conditions:
+
+            if op == 'or':
+                raise NotImplementedError(f'OR is not supported')
             if arg1 == 'created_at':
-                date = parse_date(arg2)
+                date = parse_utc_date(arg2)
                 if op == '>':
                     # "tweets/search/recent" doesn't accept dates earlier than 7 days
                     if (dt.datetime.now(dt.timezone.utc) - date).days > 7:
                         # skip this condition
                         continue
                     params['start_time'] = date
                 elif op == '<':
                     params['end_time'] = date
                 else:
                     raise NotImplementedError
-                continue
 
-            if op != '=':
-                raise NotImplementedError
+            elif arg1 == 'query':
+                if op == '=':
+                    params[arg1] = arg2
+                else:
+                    NotImplementedError(f'Unknown op: {op}')
+
+            elif arg1 == 'id':
+                if op == '>':
+                    params['since_id'] = arg2
+                elif op == '>=':
+                    raise NotImplementedError("Please use 'id > value'")
+                elif op == '<':
+                    params['until_id'] = arg2
+                elif op == '<=':
+                    raise NotImplementedError("Please use 'id < value'")
+                else:
+                    NotImplementedError('Search with "id=" is not implemented')
 
-            params[arg1] = arg2
+            else:
+                filters.append([op, arg1, arg2])
 
         if query.limit is not None:
             params['max_results'] = query.limit.value
 
         params['expansions'] = ['author_id', 'in_reply_to_user_id']
-        params['tweet_fields'] = ['created_at', 'conversation_id']
+        params['tweet_fields'] = ['created_at', 'conversation_id', 'referenced_tweets']
         params['user_fields'] = ['name', 'username']
 
         if 'query' not in params:
             # search not works without query, use 'mindsdb'
             params['query'] = 'mindsdb'
 
         result = self.handler.call_twitter_api(
             method_name='search_recent_tweets',
-            params=params
+            params=params,
+            filters=filters
         )
 
         # filter targets
         columns = []
         for target in query.targets:
             if isinstance(target, ast.Star):
                 columns = []
@@ -136,17 +124,20 @@
             'created_at',
             'text',
             'edit_history_tweet_ids',
             'author_id',
             'author_name',
             'author_username',
             'conversation_id',
+            'in_reply_to_tweet_id',
+            'in_retweeted_to_tweet_id',
+            'in_quote_to_tweet_id',
             'in_reply_to_user_id',
             'in_reply_to_user_name',
-            'in_reply_to_user_username'
+            'in_reply_to_user_username',
         ]
 
     def insert(self, query: ast.Insert):
         # https://docs.tweepy.org/en/stable/client.html#tweepy.Client.create_tweet
         columns = [col.name for col in query.columns]
 
         insert_params = ('consumer_key', 'consumer_secret', 'access_token', 'access_token_secret')
@@ -166,15 +157,15 @@
                     media_url = params['media_url']
 
                     # create an in memory file
                     resp = requests.get(media_url)
                     img = io.BytesIO(resp.content)
 
                     # upload media to twitter
-                    api_v1 = self.handler.connect(api_version=1)
+                    api_v1 = self.handler.create_connection(api_version=1)
                     content_type = resp.headers['Content-Type']
                     file_type = content_type.split('/')[-1]
                     media = api_v1.media_upload(filename="img.{file_type}".format(file_type=file_type), file=img)
 
                     del params['media_url']
                     params['media_ids'] = [media.media_id]
 
@@ -242,32 +233,35 @@
 
         self.api = None
         self.is_connected = False
 
         tweets = TweetsTable(self)
         self._register_table('tweets', tweets)
 
-    def connect(self, api_version=2):
-        """Authenticate with the Twitter API using the API keys and secrets stored in the `consumer_key`, `consumer_secret`, `access_token`, and `access_token_secret` attributes."""  # noqa
-
-        if self.is_connected is True:
-            return self.api
-        # if version 1, do not hold connection in self.api, simply return api object
+    def create_connection(self, api_version=2):
         if api_version == 1:
             auth = tweepy.OAuthHandler(
                 self.connection_args['consumer_key'],
                 self.connection_args['consumer_secret']
             )
             auth.set_access_token(
                 self.connection_args['access_token'],
                 self.connection_args['access_token_secret']
             )
             return tweepy.API(auth)
-        
-        self.api = tweepy.Client(**self.connection_args)
+
+        return tweepy.Client(**self.connection_args)
+
+    def connect(self, api_version=2):
+        """Authenticate with the Twitter API using the API keys and secrets stored in the `consumer_key`, `consumer_secret`, `access_token`, and `access_token_secret` attributes."""  # noqa
+
+        if self.is_connected is True:
+            return self.api
+
+        self.api = self.create_connection()
 
         self.is_connected = True
         return self.api
 
     def check_connection(self) -> StatusResponse:
 
         response = StatusResponse(False)
@@ -310,15 +304,52 @@
         df = self.call_twitter_api(method_name, params)
 
         return Response(
             RESPONSE_TYPE.TABLE,
             data_frame=df
         )
 
-    def call_twitter_api(self, method_name:str = None, params:dict = None):
+    def _apply_filters(self, data, filters):
+        if not filters:
+            return data
+
+        data2 = []
+        for row in data:
+            add = False
+            for op, key, value in filters:
+                value2 = row.get(key)
+                if isinstance(value, int):
+                    # twitter returns ids as string
+                    value = str(value)
+
+                if op in ('!=', '<>'):
+                    if value == value2:
+                        break
+                elif op in ('==', '='):
+                    if value != value2:
+                        break
+                elif op == 'in':
+                    if not isinstance(value, list):
+                        value = [value]
+                    if value2 not in value:
+                        break
+                elif op == 'not in':
+                    if not isinstance(value, list):
+                        value = [value]
+                    if value2 in value:
+                        break
+                else:
+                    raise NotImplementedError(f'Unknown filter: {op}')
+                # only if there wasn't breaks
+                add = True
+            if add:
+                data2.append(row)
+        return data2
+
+    def call_twitter_api(self, method_name: str = None, params: dict = None, filters: list = None):
 
         # method > table > columns
         expansions_map = {
             'search_recent_tweets': {
                 'users': ['author_id', 'in_reply_to_user_id'],
             },
             'search_all_tweets': {
@@ -338,15 +369,24 @@
         data = []
         includes = defaultdict(list)
 
         max_page_size = 100
         min_page_size = 10
         left = None
 
+        limit_exec_time = time.time() + 60
+
+        if filters:
+            # if we have filters: do big page requests
+            params['max_results'] = max_page_size
+
         while True:
+            if time.time() > limit_exec_time:
+                raise RuntimeError('Handler request timeout error')
+
             if count_results is not None:
                 left = count_results - len(data)
                 if left == 0:
                     break
                 elif left < 0:
                     # got more results that we need
                     data = data[:left]
@@ -371,14 +411,29 @@
             else:
                 if isinstance(resp.data, dict):
                     data.append(resp.data)
                 if hasattr(resp.data, 'data') and isinstance(resp.data.data, dict):
                     data.append(resp.data.data)
                 break
 
+            # unwind columns
+            for row in chunk:
+                if 'referenced_tweets' in row:
+                    refs = row['referenced_tweets']
+                    if isinstance(refs, list) and len(refs) > 0:
+                        if refs[0]['type'] == 'replied_to':
+                            row['in_reply_to_tweet_id'] = refs[0]['id']
+                        if refs[0]['type'] == 'retweeted':
+                            row['in_retweeted_to_tweet_id'] = refs[0]['id']
+                        if refs[0]['type'] == 'quoted':
+                            row['in_quote_to_tweet_id'] = refs[0]['id']
+
+            if filters:
+                chunk = self._apply_filters(chunk, filters)
+
             # limit output
             if left is not None:
                 chunk = chunk[:left]
 
             data.extend(chunk)
             # next page ?
             if count_results is not None and hasattr(resp, 'meta') and 'next_token' in resp.meta:
@@ -388,27 +443,27 @@
 
         df = pd.DataFrame(data)
 
         # enrich
         expansions = expansions_map.get(method_name)
         if expansions is not None:
             for table, records in includes.items():
-                df_ref = pd.DataFrame(records).drop_duplicates()
+                df_ref = pd.DataFrame(records)
 
                 if table not in expansions:
                     continue
 
                 for col_id in expansions[table]:
-                    col = col_id[:-3] # cut _id
+                    col = col_id[:-3]  # cut _id
                     if col_id not in df.columns:
                         continue
 
                     col_map = {
                         col_ref: f'{col}_{col_ref}'
                         for col_ref in df_ref.columns
                     }
                     df_ref2 = df_ref.rename(columns=col_map)
+                    df_ref2 = df_ref2.drop_duplicates(col_id)
 
                     df = df.merge(df_ref2, on=col_id, how='left')
 
         return df
-
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers_client/db_client_factory.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers_client/db_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers_client/ml_client_factory.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers_client/ml_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers_client/ml_grpc_client.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers_client/ml_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-23.4.3.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/libs/api_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/libs/api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/libs/base.py` & `MindsDB-23.4.3.0/mindsdb/integrations/libs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,19 +165,19 @@
         Calls a model with some input dataframe `df`, and optionally some arguments `args` that may modify the model behavior.
 
         The expected output is a dataframe with the predicted values in the target-named column.
         Additional columns can be present, and will be considered row-wise explanations if their names finish with `_explain`.
         """
         raise NotImplementedError
 
-    def update(self, df: Optional[pd.DataFrame] = None, args: Optional[Dict] = None) -> None:
+    def finetune(self, df: Optional[pd.DataFrame] = None, args: Optional[Dict] = None) -> None:
         """
         Optional.
 
-        Used to update/fine-tune/adjust a pre-existing model without resetting its internal state (e.g. weights).
+        Used to fine-tune a pre-existing model without resetting its internal state (e.g. weights).
 
         Availability will depend on underlying integration support, as not all ML models can be partially updated.
         """
         raise NotImplementedError
 
     def describe(self, attribute: Optional[str] = None) -> pd.DataFrame:
         """
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-23.4.3.0/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-23.4.3.0/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,28 @@
       output and format it into the HandlerResponse instance that MindsDB core expects.
 
     - `learn_process` method: handles async dispatch of the `learn` method in an engine, as well as registering all
       models inside of the internal MindsDB registry.
 
     - `predict_process` method: handles async dispatch of the `predict` method in an engine.
 
-""" # noqa
+"""  # noqa
 
 import datetime as dt
 import traceback
 import importlib
 from typing import Optional
 
 import pandas as pd
 
 from mindsdb_sql import parse_sql
 from mindsdb_sql.parser.ast.base import ASTNode
-from mindsdb_sql.parser.ast import Identifier, Select, Show, Star, NativeQuery
+from mindsdb_sql.parser.ast import Identifier, Select, Star, NativeQuery
 
-from mindsdb.integrations.utilities.utils import make_sql_session, get_where_data
+from mindsdb.integrations.utilities.sql_utils import make_sql_session
 from mindsdb.utilities.config import Config
 import mindsdb.interfaces.storage.db as db
 from mindsdb.integrations.libs.response import (
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
 from mindsdb import __version__ as mindsdb_version
@@ -130,19 +130,19 @@
             **kwargs
         )
 
         # create new model
         if base_predictor_id is None:
             ml_handler.create(target, df=training_data_df, args=problem_definition)
 
-        # adjust (partially train) existing model
+        # fine-tune (partially train) existing model
         else:
             # load model from previous version, use it as starting point
             problem_definition['base_model_id'] = base_predictor_id
-            ml_handler.update(df=training_data_df, args=problem_definition)
+            ml_handler.finetune(df=training_data_df, args=problem_definition)
 
         predictor_record.status = PREDICTOR_STATUS.COMPLETE
         db.session.commit()
         # if retrain and set_active after success creation
         if set_active is True:
             models = get_model_records(
                 name=predictor_record.name,
@@ -265,37 +265,14 @@
         """ Intakes a raw SQL query and returns the answer given by the ML engine. """
         query_ast = self.parser(query, dialect=self.dialect)
         return self.query(query_ast)
 
     def query_(self, query: ASTNode) -> Response:
         raise Exception('Should not be used')
 
-        """ Intakes a pre-parsed SQL query (via `mindsdb_sql`) and returns the answer given by the ML engine. """
-        statement = query
-
-        if type(statement) == Show:
-            if statement.category.lower() == 'tables':
-                return self.get_tables()
-            else:
-                response = Response(
-                    RESPONSE_TYPE.ERROR,
-                    error_message=f"Cant determine how to show '{statement.category}'"
-                )
-            return response
-        elif type(statement) == Select:
-            model_name = statement.from_table.parts[-1]
-            where_data = get_where_data(statement.where)
-            predictions = self.predict(model_name, where_data)
-            return Response(
-                RESPONSE_TYPE.TABLE,
-                data_frame=pd.DataFrame(predictions)
-            )
-        else:
-            raise Exception(f"Query type {type(statement)} not supported")
-
     def learn(
         self, model_name, project_name,
         data_integration_ref=None,
         fetch_data_query=None,
         problem_definition=None,
         join_learn_process=False,
         label=None,
@@ -391,15 +368,18 @@
             args['target'] = predictor_record.to_predict[0]
             args['dtype_dict'] = predictor_record.dtype_dict
             args['learn_args'] = predictor_record.learn_args
 
         try:
             predictions = ml_handler.predict(df, args)
         except Exception as e:
-            msg = f'[{self.name}/{model_name}]: {str(e)}'
+            msg = str(e).strip()
+            if msg == '':
+                msg = e.__class__.__name__
+            msg = f'[{self.name}/{model_name}]: {msg}'
             raise MLEngineException(msg) from e
 
         ml_handler.close()
 
         # mdb indexes
         if '__mindsdb_row_id' not in predictions.columns and '__mindsdb_row_id' in df.columns:
             predictions['__mindsdb_row_id'] = df['__mindsdb_row_id']
@@ -426,15 +406,15 @@
         project = self.database_controller.get_project(name=project_name)
         predictor_records = get_model_records(
             active=None,
             name=model_name,
         )
         predictor_records = [
             x for x in predictor_records
-            if x.training_stop_at is not None
+            if x.training_stop_at is not None and x.status == 'complete'
         ]
         predictor_records.sort(key=lambda x: x.training_stop_at, reverse=True)
 
         base_predictor_record = predictor_records[0]
         learn_args = base_predictor_record.learn_args
         learn_args['using'] = args if not learn_args.get('using', False) else {**learn_args['using'], **args}
```

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/libs/ml_handler_proc.py` & `MindsDB-23.4.3.0/mindsdb/integrations/libs/ml_handler_proc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-23.4.3.0/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/libs/response.py` & `MindsDB-23.4.3.0/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-23.4.3.0/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/utilities/install.py` & `MindsDB-23.4.3.0/mindsdb/integrations/utilities/install.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-23.4.3.0/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/database/database.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/database/database.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/database/integrations.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/database/integrations.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/database/projects.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/database/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/database/views.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/file/file_controller.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,16 +340,16 @@
                     # get previous run date
                     history_prev = db.session.query(db.JobsHistory.start_at)\
                         .filter(db.JobsHistory.job_id == record.id,
                                 db.JobsHistory.id != history_id)\
                         .order_by(db.JobsHistory.id.desc())\
                         .first()
                     if history_prev is None:
-                        # very old date
-                        value = dt.datetime(1900, 1, 1)
+                        # start date of the job
+                        value = record.created_at
                     else:
                         value = history_prev.start_at
                     value = value.strftime("%Y-%m-%d %H:%M:%S")
                     sql = sql.replace('{{PREVIOUS_START_DATETIME}}', value)
 
                 if '{{START_DATE}}' in sql:
                     value = history_record.start_at.strftime("%Y-%m-%d")
```

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/model/functions.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/model/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/model/model_controller.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/model/model_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,15 +333,15 @@
             active=True
         )
 
         model_name = params['model_name']
         if base_predictor_record is None:
             raise Exception(f"Error: model '{model_name}' does not exist")
 
-        params['version'] = self._get_retrain_adjust_version(model_name, params['project_name'], base_predictor_record)
+        params['version'] = self._get_retrain_finetune_version(model_name, params['project_name'], base_predictor_record)
 
         if params['data_integration_ref'] is None:
             params['data_integration_ref'] = base_predictor_record.data_integration_ref
         if params['fetch_data_query'] is None:
             params['fetch_data_query'] = base_predictor_record.fetch_data_query
 
         problem_definition = base_predictor_record.learn_args.copy()
@@ -351,15 +351,15 @@
         params['is_retrain'] = True
         params['set_active'] = set_active
         predictor_record = ml_handler.learn(**params)
 
         return self.get_model_info(predictor_record)
 
     @staticmethod
-    def _get_retrain_adjust_version(model_name, project_name, base_predictor_record):
+    def _get_retrain_finetune_version(model_name, project_name, base_predictor_record):
         if base_predictor_record is None:
             raise Exception(f"Error: model '{model_name}' does not exist")
 
         # get max current version
         models = get_model_records(
             name=model_name,
             project_name=project_name,
@@ -369,15 +369,15 @@
         last_version = 1
         for m in models:
             if m.version is not None:
                 last_version = max(last_version, m.version)
 
         return last_version + 1
 
-    def prepare_adjust_statement(self, statement, database_controller):
+    def prepare_finetune_statement(self, statement, database_controller):
         project_name = statement.name.parts[0].lower()
         model_name = statement.name.parts[1].lower()
         data_integration_ref, fetch_data_query = self._get_data_integration_ref(statement, database_controller)
 
         label = None
         args = {}
         if statement.using is not None:
@@ -387,15 +387,15 @@
         join_learn_process = args.pop('join_learn_process', False)
 
         base_predictor_record = get_model_record(
             name=model_name,
             project_name=project_name,
             active=True
         )
-        version = self._get_retrain_adjust_version(model_name, project_name, base_predictor_record)
+        version = self._get_retrain_finetune_version(model_name, project_name, base_predictor_record)
 
         if data_integration_ref is None:
             data_integration_ref = base_predictor_record.data_integration_ref
         if fetch_data_query is None:
             fetch_data_query = base_predictor_record.fetch_data_query
 
         return dict(
@@ -405,23 +405,23 @@
             fetch_data_query=fetch_data_query,
             version=version,
             args=args,
             join_learn_process=join_learn_process,
             label=label
         )
 
-    def adjust_model(self, statement, ml_handler):
+    def finetune_model(self, statement, ml_handler):
         # active setting
         set_active = True
         if statement.using is not None:
             set_active = statement.using.pop('active', True)
             if set_active in ('0', 0, None):
                 set_active = False
 
-        params = self.prepare_adjust_statement(statement, ml_handler.database_controller)
+        params = self.prepare_finetune_statement(statement, ml_handler.database_controller)
 
         params['set_active'] = set_active
         predictor_record = ml_handler.update(**params)
         return self.get_model_info(predictor_record)
 
     def get_model_info(self, predictor_record):
```

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/storage/db.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/storage/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     )
 
 
 class PREDICTOR_STATUS:
     __slots__ = ()
     COMPLETE = 'complete'
     TRAINING = 'training'
-    ADJUSTING = 'adjusting'
+    FINETUNING = 'finetuning'
     GENERATING = 'generating'
     ERROR = 'error'
     VALIDATION = 'validation'
     DELETED = 'deleted'  # TODO remove it?
 
 
 PREDICTOR_STATUS = PREDICTOR_STATUS()
```

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/storage/fs.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/storage/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/storage/json.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/stream/base/integration.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/stream/base/integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/stream/kafka/kafkadb.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/stream/kafka/kafkadb.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/stream/redis/redisdb.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/stream/redis/redisdb.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/interfaces/stream/stream.py` & `MindsDB-23.4.3.0/mindsdb/interfaces/stream/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-23.4.3.0/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-23.4.3.0/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-23.4.3.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-23.4.3.0/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-23.4.3.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-23.4.3.0/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-23.4.3.0/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-23.4.3.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/alembic.ini` & `MindsDB-23.4.3.0/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/env.py` & `MindsDB-23.4.3.0/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/migrate.py` & `MindsDB-23.4.3.0/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-23.4.3.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/auth.py` & `MindsDB-23.4.3.0/mindsdb/utilities/auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,18 @@
     }
     for key in aws_meta_data.keys():
         resp = requests.get(
             f'http://169.254.169.254/latest/meta-data/{key}',
             timeout=1
         )
         if resp.status_code != 200:
-            raise Exception()
+            continue
         aws_meta_data[key] = resp.text
+    if aws_meta_data['instance-id'] is None:
+        raise Exception('That is not an AWS environment')
     return aws_meta_data
 
 
 def register_oauth_client():
     ''' register new oauth client if it is not existed
     '''
     config = Config()
```

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/cache.py` & `MindsDB-23.4.3.0/mindsdb/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/config.py` & `MindsDB-23.4.3.0/mindsdb/utilities/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
                     "db": "WARNING"
                 }
             },
             "gui": {
                 "autoupdate": True
             },
             "debug": False,
+            "environment": "local",
             "integrations": {},
             "api": {
                 "http": {
                     "host": api_host,
                     "port": "47334"
                 },
                 "mysql": {
```

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/context.py` & `MindsDB-23.4.3.0/mindsdb/utilities/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 
     def __init__(self, storage) -> None:
         object.__setattr__(self, '_storage', storage)
 
     def set_default(self) -> None:
         self._storage.set({
             'company_id': None,
-            'user_class': 0
+            'user_class': 0,
+            'profiling': {
+                'level': 0,
+                'enabled': False,
+                'pointer': None,
+                'tree': None
+            }
         })
 
     def __getattr__(self, name: str) -> Any:
         storage = self._storage.get({})
         if name not in storage:
             raise AttributeError(name)
         return storage[name]
```

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/fs.py` & `MindsDB-23.4.3.0/mindsdb/utilities/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/functions.py` & `MindsDB-23.4.3.0/mindsdb/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/json_encoder.py` & `MindsDB-23.4.3.0/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/log.py` & `MindsDB-23.4.3.0/mindsdb/utilities/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/log_controller.py` & `MindsDB-23.4.3.0/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/ps.py` & `MindsDB-23.4.3.0/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/telemetry.py` & `MindsDB-23.4.3.0/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/mindsdb/utilities/wizards.py` & `MindsDB-23.4.3.0/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.3.5.0/requirements.txt` & `MindsDB-23.4.3.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lightwood >= 23.2.1.1, < 23.3.2.0
+lightwood >= 23.3.2.0, < 23.3.3.0
 markupsafe == 2.0.1
 flask-restx >= 1.0.1, < 2.0.0
 flask >= 1.0, < 2.0
 python-multipart >= 0.0.5
 pyparsing == 2.3.1
 cryptography>=35.0
 psycopg[binary] >= 1.15.3
@@ -15,15 +15,15 @@
 sqlalchemy >= 1.4.29, < 2.0.0
 alembic >= 1.3.3
 sentry-sdk
 walrus==0.8.2
 flask-compress >= 1.0.0
 kafka-python >= 2.0.0
 appdirs >= 1.0.0
-mindsdb-sql >= 0.4.9, < 0.5.0
+mindsdb-sql >= 0.5.1, < 0.6.0
 checksumdir >= 1.2.0
 mindsdb-streams == 0.1.1
 duckdb == 0.4.0
 requests >= 2.0.0
 mysql-connector-python
 clickhouse-driver
 clickhouse-sqlalchemy
```

### Comparing `MindsDB-23.3.5.0/setup.py` & `MindsDB-23.4.3.0/setup.py`

 * *Files identical despite different names*

