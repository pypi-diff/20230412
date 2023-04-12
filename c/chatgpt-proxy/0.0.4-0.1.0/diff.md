# Comparing `tmp/chatgpt-proxy-0.0.4.tar.gz` & `tmp/chatgpt-proxy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-proxy-0.0.4.tar", last modified: Wed Apr 12 10:59:12 2023, max compression
+gzip compressed data, was "chatgpt-proxy-0.1.0.tar", last modified: Wed Apr 12 14:33:41 2023, max compression
```

## Comparing `chatgpt-proxy-0.0.4.tar` & `chatgpt-proxy-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:59:12.187195 chatgpt-proxy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-12 10:58:56.000000 chatgpt-proxy-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-12 10:59:12.187195 chatgpt-proxy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-12 10:58:56.000000 chatgpt-proxy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:59:12.187195 chatgpt-proxy-0.0.4/chatgpt_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 10:58:56.000000 chatgpt-proxy-0.0.4/chatgpt_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-12 10:58:56.000000 chatgpt-proxy-0.0.4/chatgpt_proxy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-12 10:58:56.000000 chatgpt-proxy-0.0.4/chatgpt_proxy/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:59:12.187195 chatgpt-proxy-0.0.4/chatgpt_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-12 10:59:12.000000 chatgpt-proxy-0.0.4/chatgpt_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-12 10:59:12.000000 chatgpt-proxy-0.0.4/chatgpt_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:59:12.000000 chatgpt-proxy-0.0.4/chatgpt_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 10:59:12.000000 chatgpt-proxy-0.0.4/chatgpt_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 10:59:12.000000 chatgpt-proxy-0.0.4/chatgpt_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-12 10:58:56.000000 chatgpt-proxy-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:59:12.187195 chatgpt-proxy-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:41.456161 chatgpt-proxy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-12 14:33:41.456161 chatgpt-proxy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:41.456161 chatgpt-proxy-0.1.0/chatgpt_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/chatgpt_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/chatgpt_proxy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/chatgpt_proxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:41.456161 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-12 14:33:41.000000 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-12 14:33:41.000000 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:33:41.000000 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 14:33:41.000000 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 14:33:41.000000 chatgpt-proxy-0.1.0/chatgpt_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 14:33:25.000000 chatgpt-proxy-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:33:41.456161 chatgpt-proxy-0.1.0/setup.cfg
```

### Comparing `chatgpt-proxy-0.0.4/LICENSE` & `chatgpt-proxy-0.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -655,7 +655,17 @@
 solutions will be better for different programs; see section 13 for the
 specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU AGPL, see
 <https://www.gnu.org/licenses/>.
+
+"CHATGPT-PROXY" EXCEPTION TO THE AGPL
+
+  As a special exception, using this work in the following ways does not cause
+your program to be covered by the AGPL:
+
+    a) Bundling the unaltered code or binary of this work in your program; or
+
+    b) Interacting with this work through the provided inter-process
+    communication interface, such as the HTTP API.
```

### Comparing `chatgpt-proxy-0.0.4/chatgpt_proxy/proxy.py` & `chatgpt-proxy-0.1.0/chatgpt_proxy/proxy.py`

 * *Files identical despite different names*

