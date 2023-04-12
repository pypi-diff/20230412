# Comparing `tmp/slackflylog-0.0.2.tar.gz` & `tmp/slackflylog-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slackflylog-0.0.2.tar", last modified: Wed Apr 12 11:03:55 2023, max compression
+gzip compressed data, was "dist/slackflylog-1.0.2.tar", last modified: Wed Apr 12 11:09:52 2023, max compression
```

## Comparing `slackflylog-0.0.2.tar` & `slackflylog-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:55.000000 slackflylog-0.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:55.000000 slackflylog-0.0.2/agent/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:55.000000 slackflylog-0.0.2/agent/backends/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 11:00:39.000000 slackflylog-0.0.2/agent/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-04-12 11:00:39.000000 slackflylog-0.0.2/agent/backends/send_slack.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 11:00:39.000000 slackflylog-0.0.2/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3537 2023-04-12 11:00:39.000000 slackflylog-0.0.2/agent/agent.py
--rw-r--r--   0 root         (0) root         (0)      123 2023-04-12 11:00:39.000000 slackflylog-0.0.2/agent/log.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-04-12 11:00:39.000000 slackflylog-0.0.2/agent/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:55.000000 slackflylog-0.0.2/api/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 11:00:39.000000 slackflylog-0.0.2/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-04-12 11:00:39.000000 slackflylog-0.0.2/api/client.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-12 11:00:39.000000 slackflylog-0.0.2/api/log_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:55.000000 slackflylog-0.0.2/slackflylog.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-12 11:03:55.000000 slackflylog-0.0.2/slackflylog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2023-04-12 11:03:55.000000 slackflylog-0.0.2/slackflylog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:03:55.000000 slackflylog-0.0.2/slackflylog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-12 11:03:55.000000 slackflylog-0.0.2/slackflylog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-12 11:03:55.000000 slackflylog-0.0.2/slackflylog.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      647 2023-04-12 11:03:46.000000 slackflylog-0.0.2/setup.py
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-12 11:03:55.000000 slackflylog-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:03:55.000000 slackflylog-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:09:52.747115 slackflylog-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-04-12 10:42:59.000000 slackflylog-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      229 2023-04-12 11:09:52.747115 slackflylog-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 10:42:59.000000 slackflylog-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:09:52.746116 slackflylog-1.0.2/agent/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 10:42:59.000000 slackflylog-1.0.2/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2023-04-12 10:42:59.000000 slackflylog-1.0.2/agent/agent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:09:52.746116 slackflylog-1.0.2/agent/backends/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 10:42:59.000000 slackflylog-1.0.2/agent/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-04-12 10:42:59.000000 slackflylog-1.0.2/agent/backends/send_slack.py
+-rw-r--r--   0 root         (0) root         (0)      123 2023-04-12 10:42:59.000000 slackflylog-1.0.2/agent/log.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-04-12 10:42:59.000000 slackflylog-1.0.2/agent/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:09:52.746116 slackflylog-1.0.2/api/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 10:42:59.000000 slackflylog-1.0.2/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-04-12 10:42:59.000000 slackflylog-1.0.2/api/client.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-12 10:42:59.000000 slackflylog-1.0.2/api/log_handler.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:09:52.747115 slackflylog-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      647 2023-04-12 11:09:46.000000 slackflylog-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:09:52.747115 slackflylog-1.0.2/slackflylog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-04-12 11:09:52.000000 slackflylog-1.0.2/slackflylog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      366 2023-04-12 11:09:52.000000 slackflylog-1.0.2/slackflylog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:09:52.000000 slackflylog-1.0.2/slackflylog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 11:09:52.000000 slackflylog-1.0.2/slackflylog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-12 11:09:52.000000 slackflylog-1.0.2/slackflylog.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `slackflylog-0.0.2/agent/backends/send_slack.py` & `slackflylog-1.0.2/agent/backends/send_slack.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.2/agent/agent.py` & `slackflylog-1.0.2/agent/agent.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.2/agent/utils.py` & `slackflylog-1.0.2/agent/utils.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.2/api/client.py` & `slackflylog-1.0.2/api/client.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.2/api/log_handler.py` & `slackflylog-1.0.2/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.2/setup.py` & `slackflylog-1.0.2/setup.py`

 * *Files identical despite different names*

