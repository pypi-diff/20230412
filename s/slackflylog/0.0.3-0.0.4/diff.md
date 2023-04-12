# Comparing `tmp/slackflylog-0.0.3.tar.gz` & `tmp/slackflylog-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slackflylog-0.0.3.tar", last modified: Wed Apr 12 12:05:48 2023, max compression
+gzip compressed data, was "dist/slackflylog-0.0.4.tar", last modified: Wed Apr 12 12:14:42 2023, max compression
```

## Comparing `slackflylog-0.0.3.tar` & `slackflylog-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:05:48.000000 slackflylog-0.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:05:48.000000 slackflylog-0.0.3/slackflylog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:05:48.000000 slackflylog-0.0.3/slackflylog/agent/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:05:48.000000 slackflylog-0.0.3/slackflylog/agent/backends/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/agent/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/agent/backends/send_slack.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3537 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/agent/agent.py
--rw-r--r--   0 root         (0) root         (0)      123 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/agent/log.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/agent/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:05:48.000000 slackflylog-0.0.3/slackflylog/api/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/api/client.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/api/log_handler.py
--rw-r--r--   0 root         (0) root         (0)      193 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-04-12 11:00:39.000000 slackflylog-0.0.3/slackflylog/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:05:48.000000 slackflylog-0.0.3/slackflylog.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-12 12:05:47.000000 slackflylog-0.0.3/slackflylog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      505 2023-04-12 12:05:47.000000 slackflylog-0.0.3/slackflylog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 12:05:47.000000 slackflylog-0.0.3/slackflylog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-12 12:05:47.000000 slackflylog-0.0.3/slackflylog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 12:05:47.000000 slackflylog-0.0.3/slackflylog.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      647 2023-04-12 12:05:41.000000 slackflylog-0.0.3/setup.py
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-12 12:05:48.000000 slackflylog-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 12:05:48.000000 slackflylog-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog/agent/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog/agent/backends/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/backends/send_slack.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/agent.py
+-rw-r--r--   0 root         (0) root         (0)      123 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/log.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/agent/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog/api/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/api/client.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/api/log_handler.py
+-rw-r--r--   0 root         (0) root         (0)      193 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-12 12:13:20.000000 slackflylog-0.0.4/slackflylog/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      505 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 12:14:42.000000 slackflylog-0.0.4/slackflylog.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      649 2023-04-12 12:14:31.000000 slackflylog-0.0.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)      246 2023-04-12 12:14:42.000000 slackflylog-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 12:14:42.000000 slackflylog-0.0.4/setup.cfg
```

### Comparing `slackflylog-0.0.3/slackflylog/agent/backends/send_slack.py` & `slackflylog-0.0.4/slackflylog/agent/backends/send_slack.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.3/slackflylog/agent/agent.py` & `slackflylog-0.0.4/slackflylog/agent/agent.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.3/slackflylog/agent/utils.py` & `slackflylog-0.0.4/slackflylog/agent/utils.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.3/slackflylog/api/client.py` & `slackflylog-0.0.4/slackflylog/api/client.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.3/slackflylog/api/log_handler.py` & `slackflylog-0.0.4/slackflylog/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `slackflylog-0.0.3/setup.py` & `slackflylog-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 import sys
 
 PY2 = sys.version_info[0] == 2
 
 # 基於flylog, slack-client處理
 if PY2:
     require_pack = ['slackclient==1.3.2']
-    pack_version = '0.0.3'
+    pack_version = '0.0.4'
 else:
     require_pack = ['slack_sdk==3.19.5']
-    pack_version = '1.0.3'
+    pack_version = '1.0.4'
+
 setup(
     name='slackflylog',
     version=pack_version,
     author="dkxx00",
     author_email="hymanxx6@gmail.com",
     description="基于flylog的Slack日志发送",
     license="MIT",
```

