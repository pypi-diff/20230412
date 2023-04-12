# Comparing `tmp/zenutils-0.3.8.tar.gz` & `tmp/zenutils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenutils-0.3.8.tar", last modified: Tue Oct 18 06:26:57 2022, max compression
+gzip compressed data, was "zenutils-0.3.9.tar", last modified: Sat Oct 22 13:01:51 2022, max compression
```

## Comparing `zenutils-0.3.8.tar` & `zenutils-0.3.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-18 06:26:57.243737 zenutils-0.3.8/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-06-16 09:27:11.000000 zenutils-0.3.8/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      198 2022-06-17 11:16:41.000000 zenutils-0.3.8/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)    20387 2022-10-18 06:26:57.243512 zenutils-0.3.8/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)    19786 2022-10-18 03:20:16.000000 zenutils-0.3.8/README.md
--rw-r--r--   0 test       (501) staff       (20)       16 2022-06-17 10:49:49.000000 zenutils-0.3.8/requirements.py32.txt
--rw-r--r--   0 test       (501) staff       (20)        0 2022-10-18 06:26:56.000000 zenutils-0.3.8/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2022-10-18 06:26:57.243789 zenutils-0.3.8/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1617 2022-10-18 03:24:02.000000 zenutils-0.3.8/setup.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-18 06:26:57.239378 zenutils-0.3.8/zenutils/
--rw-r--r--   0 test       (501) staff       (20)      184 2022-06-19 12:22:31.000000 zenutils-0.3.8/zenutils/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      602 2022-06-18 15:33:41.000000 zenutils-0.3.8/zenutils/base64utils.py
--rw-r--r--   0 test       (501) staff       (20)      308 2022-06-21 01:33:03.000000 zenutils-0.3.8/zenutils/baseutils.py
--rw-r--r--   0 test       (501) staff       (20)     3835 2022-09-02 15:28:21.000000 zenutils-0.3.8/zenutils/cacheutils.py
--rw-r--r--   0 test       (501) staff       (20)    16879 2022-06-21 06:14:08.000000 zenutils-0.3.8/zenutils/cipherutils.py
--rw-r--r--   0 test       (501) staff       (20)    13435 2022-08-09 12:44:33.000000 zenutils-0.3.8/zenutils/dictutils.py
--rw-r--r--   0 test       (501) staff       (20)    23236 2022-09-20 04:32:52.000000 zenutils-0.3.8/zenutils/fsutils.py
--rw-r--r--   0 test       (501) staff       (20)    12866 2022-10-18 06:15:35.000000 zenutils-0.3.8/zenutils/funcutils.py
--rw-r--r--   0 test       (501) staff       (20)    25718 2022-09-23 16:30:41.000000 zenutils-0.3.8/zenutils/hashutils.py
--rw-r--r--   0 test       (501) staff       (20)     3531 2022-06-19 11:53:27.000000 zenutils-0.3.8/zenutils/httputils.py
--rw-r--r--   0 test       (501) staff       (20)     9081 2022-08-14 02:47:51.000000 zenutils-0.3.8/zenutils/jsonutils.py
--rw-r--r--   0 test       (501) staff       (20)     8771 2022-09-23 15:38:47.000000 zenutils-0.3.8/zenutils/listutils.py
--rw-r--r--   0 test       (501) staff       (20)     7149 2022-09-20 14:26:52.000000 zenutils-0.3.8/zenutils/logutils.py
--rw-r--r--   0 test       (501) staff       (20)    18115 2022-06-19 14:11:01.000000 zenutils-0.3.8/zenutils/nameutils.py
--rw-r--r--   0 test       (501) staff       (20)     5499 2022-09-23 17:23:36.000000 zenutils-0.3.8/zenutils/numericutils.py
--rw-r--r--   0 test       (501) staff       (20)    10682 2022-09-28 07:15:34.000000 zenutils-0.3.8/zenutils/randomutils.py
--rw-r--r--   0 test       (501) staff       (20)     5562 2022-10-18 04:53:37.000000 zenutils-0.3.8/zenutils/sixutils.py
--rw-r--r--   0 test       (501) staff       (20)    31350 2022-06-21 07:26:11.000000 zenutils-0.3.8/zenutils/strutils.py
--rw-r--r--   0 test       (501) staff       (20)     7529 2022-08-28 08:48:38.000000 zenutils-0.3.8/zenutils/sysutils.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-18 06:26:57.243074 zenutils-0.3.8/zenutils/tests/
--rw-r--r--   0 test       (501) staff       (20)      171 2022-06-17 06:56:58.000000 zenutils-0.3.8/zenutils/tests/__init__.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-18 06:26:57.243303 zenutils-0.3.8/zenutils/tests/assets/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-06-19 08:45:08.000000 zenutils-0.3.8/zenutils/tests/assets/a.txt
--rw-r--r--   0 test       (501) staff       (20)      823 2022-06-21 07:48:43.000000 zenutils-0.3.8/zenutils/tests/assets/p1.jpeg
--rw-r--r--   0 test       (501) staff       (20)      143 2022-09-23 14:14:23.000000 zenutils-0.3.8/zenutils/tests/t08_01.py
--rw-r--r--   0 test       (501) staff       (20)      481 2022-06-21 01:34:38.000000 zenutils-0.3.8/zenutils/tests/test_baseutils.py
--rw-r--r--   0 test       (501) staff       (20)     1734 2022-09-02 15:28:07.000000 zenutils-0.3.8/zenutils/tests/test_cacheutils.py
--rw-r--r--   0 test       (501) staff       (20)    15419 2022-06-21 03:54:40.000000 zenutils-0.3.8/zenutils/tests/test_cipherutils.py
--rw-r--r--   0 test       (501) staff       (20)     9329 2022-08-09 06:57:09.000000 zenutils-0.3.8/zenutils/tests/test_dictutils.py
--rw-r--r--   0 test       (501) staff       (20)     7281 2022-09-20 04:29:06.000000 zenutils-0.3.8/zenutils/tests/test_fsutils.py
--rw-r--r--   0 test       (501) staff       (20)     6765 2022-09-23 14:27:53.000000 zenutils-0.3.8/zenutils/tests/test_funcutils.py
--rw-r--r--   0 test       (501) staff       (20)     5879 2022-08-28 09:03:36.000000 zenutils-0.3.8/zenutils/tests/test_hashutils.py
--rw-r--r--   0 test       (501) staff       (20)     2818 2022-08-28 08:48:38.000000 zenutils-0.3.8/zenutils/tests/test_httputils.py
--rw-r--r--   0 test       (501) staff       (20)      807 2022-08-25 16:35:30.000000 zenutils-0.3.8/zenutils/tests/test_import_all.py
--rw-r--r--   0 test       (501) staff       (20)     1821 2022-06-21 06:30:06.000000 zenutils-0.3.8/zenutils/tests/test_jsonutils.py
--rw-r--r--   0 test       (501) staff       (20)    10045 2022-06-19 14:09:18.000000 zenutils-0.3.8/zenutils/tests/test_listutils.py
--rw-r--r--   0 test       (501) staff       (20)     1051 2022-06-21 01:39:50.000000 zenutils-0.3.8/zenutils/tests/test_logutils.py
--rw-r--r--   0 test       (501) staff       (20)      980 2022-06-19 14:09:25.000000 zenutils-0.3.8/zenutils/tests/test_nameutils.py
--rw-r--r--   0 test       (501) staff       (20)    13987 2022-09-23 17:25:31.000000 zenutils-0.3.8/zenutils/tests/test_numericutils.py
--rw-r--r--   0 test       (501) staff       (20)    54463 2022-09-28 07:22:41.000000 zenutils-0.3.8/zenutils/tests/test_randomutils.py
--rw-r--r--   0 test       (501) staff       (20)     4304 2022-10-18 04:33:14.000000 zenutils-0.3.8/zenutils/tests/test_sixutils.py
--rw-r--r--   0 test       (501) staff       (20)    27083 2022-06-21 07:36:31.000000 zenutils-0.3.8/zenutils/tests/test_strutils.py
--rw-r--r--   0 test       (501) staff       (20)     2056 2022-08-16 15:10:43.000000 zenutils-0.3.8/zenutils/tests/test_sysutils.py
--rw-r--r--   0 test       (501) staff       (20)     4540 2022-06-20 13:23:51.000000 zenutils-0.3.8/zenutils/tests/test_threadutils.py
--rw-r--r--   0 test       (501) staff       (20)     3151 2022-08-05 14:11:47.000000 zenutils-0.3.8/zenutils/tests/test_treeutils.py
--rw-r--r--   0 test       (501) staff       (20)     5116 2022-06-19 14:09:58.000000 zenutils-0.3.8/zenutils/tests/test_typingutils.py
--rw-r--r--   0 test       (501) staff       (20)    20792 2022-08-03 06:49:45.000000 zenutils-0.3.8/zenutils/threadutils.py
--rw-r--r--   0 test       (501) staff       (20)     4029 2022-08-05 14:09:17.000000 zenutils-0.3.8/zenutils/treeutils.py
--rw-r--r--   0 test       (501) staff       (20)     7917 2022-06-21 01:35:25.000000 zenutils-0.3.8/zenutils/typingutils.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-18 06:26:57.240030 zenutils-0.3.8/zenutils.egg-info/
--rw-r--r--   0 test       (501) staff       (20)    20387 2022-10-18 06:26:57.000000 zenutils-0.3.8/zenutils.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1537 2022-10-18 06:26:57.000000 zenutils-0.3.8/zenutils.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2022-10-18 06:26:57.000000 zenutils-0.3.8/zenutils.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2022-10-18 06:26:56.000000 zenutils-0.3.8/zenutils.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)        9 2022-10-18 06:26:57.000000 zenutils-0.3.8/zenutils.egg-info/top_level.txt
+drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-22 13:01:51.246810 zenutils-0.3.9/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2022-06-16 09:27:11.000000 zenutils-0.3.9/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      198 2022-06-17 11:16:41.000000 zenutils-0.3.9/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)    20457 2022-10-22 13:01:51.246563 zenutils-0.3.9/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)    19856 2022-10-22 12:38:16.000000 zenutils-0.3.9/README.md
+-rw-r--r--   0 test       (501) staff       (20)       16 2022-06-17 10:49:49.000000 zenutils-0.3.9/requirements.py32.txt
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-10-22 13:01:50.000000 zenutils-0.3.9/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2022-10-22 13:01:51.246871 zenutils-0.3.9/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1617 2022-10-22 12:38:22.000000 zenutils-0.3.9/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-22 13:01:51.241927 zenutils-0.3.9/zenutils/
+-rw-r--r--   0 test       (501) staff       (20)      184 2022-06-19 12:22:31.000000 zenutils-0.3.9/zenutils/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      602 2022-06-18 15:33:41.000000 zenutils-0.3.9/zenutils/base64utils.py
+-rw-r--r--   0 test       (501) staff       (20)      308 2022-06-21 01:33:03.000000 zenutils-0.3.9/zenutils/baseutils.py
+-rw-r--r--   0 test       (501) staff       (20)     3835 2022-09-02 15:28:21.000000 zenutils-0.3.9/zenutils/cacheutils.py
+-rw-r--r--   0 test       (501) staff       (20)    16879 2022-06-21 06:14:08.000000 zenutils-0.3.9/zenutils/cipherutils.py
+-rw-r--r--   0 test       (501) staff       (20)    13435 2022-08-09 12:44:33.000000 zenutils-0.3.9/zenutils/dictutils.py
+-rw-r--r--   0 test       (501) staff       (20)    23236 2022-09-20 04:32:52.000000 zenutils-0.3.9/zenutils/fsutils.py
+-rw-r--r--   0 test       (501) staff       (20)    12866 2022-10-18 06:15:35.000000 zenutils-0.3.9/zenutils/funcutils.py
+-rw-r--r--   0 test       (501) staff       (20)    25718 2022-09-23 16:30:41.000000 zenutils-0.3.9/zenutils/hashutils.py
+-rw-r--r--   0 test       (501) staff       (20)     3531 2022-06-19 11:53:27.000000 zenutils-0.3.9/zenutils/httputils.py
+-rw-r--r--   0 test       (501) staff       (20)     9081 2022-08-14 02:47:51.000000 zenutils-0.3.9/zenutils/jsonutils.py
+-rw-r--r--   0 test       (501) staff       (20)     8771 2022-09-23 15:38:47.000000 zenutils-0.3.9/zenutils/listutils.py
+-rw-r--r--   0 test       (501) staff       (20)     7149 2022-09-20 14:26:52.000000 zenutils-0.3.9/zenutils/logutils.py
+-rw-r--r--   0 test       (501) staff       (20)    18115 2022-06-19 14:11:01.000000 zenutils-0.3.9/zenutils/nameutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5499 2022-09-23 17:23:36.000000 zenutils-0.3.9/zenutils/numericutils.py
+-rw-r--r--   0 test       (501) staff       (20)    10682 2022-09-28 07:15:34.000000 zenutils-0.3.9/zenutils/randomutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5562 2022-10-18 04:53:37.000000 zenutils-0.3.9/zenutils/sixutils.py
+-rw-r--r--   0 test       (501) staff       (20)    31350 2022-06-21 07:26:11.000000 zenutils-0.3.9/zenutils/strutils.py
+-rw-r--r--   0 test       (501) staff       (20)     7656 2022-10-22 12:36:18.000000 zenutils-0.3.9/zenutils/sysutils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-22 13:01:51.246029 zenutils-0.3.9/zenutils/tests/
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-06-17 06:56:58.000000 zenutils-0.3.9/zenutils/tests/__init__.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-22 13:01:51.246285 zenutils-0.3.9/zenutils/tests/assets/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-06-19 08:45:08.000000 zenutils-0.3.9/zenutils/tests/assets/a.txt
+-rw-r--r--   0 test       (501) staff       (20)      823 2022-06-21 07:48:43.000000 zenutils-0.3.9/zenutils/tests/assets/p1.jpeg
+-rw-r--r--   0 test       (501) staff       (20)      143 2022-09-23 14:14:23.000000 zenutils-0.3.9/zenutils/tests/t08_01.py
+-rw-r--r--   0 test       (501) staff       (20)      481 2022-06-21 01:34:38.000000 zenutils-0.3.9/zenutils/tests/test_baseutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1734 2022-09-02 15:28:07.000000 zenutils-0.3.9/zenutils/tests/test_cacheutils.py
+-rw-r--r--   0 test       (501) staff       (20)    15419 2022-06-21 03:54:40.000000 zenutils-0.3.9/zenutils/tests/test_cipherutils.py
+-rw-r--r--   0 test       (501) staff       (20)     9329 2022-08-09 06:57:09.000000 zenutils-0.3.9/zenutils/tests/test_dictutils.py
+-rw-r--r--   0 test       (501) staff       (20)     7281 2022-09-20 04:29:06.000000 zenutils-0.3.9/zenutils/tests/test_fsutils.py
+-rw-r--r--   0 test       (501) staff       (20)     6765 2022-09-23 14:27:53.000000 zenutils-0.3.9/zenutils/tests/test_funcutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5879 2022-08-28 09:03:36.000000 zenutils-0.3.9/zenutils/tests/test_hashutils.py
+-rw-r--r--   0 test       (501) staff       (20)     2818 2022-08-28 08:48:38.000000 zenutils-0.3.9/zenutils/tests/test_httputils.py
+-rw-r--r--   0 test       (501) staff       (20)      807 2022-08-25 16:35:30.000000 zenutils-0.3.9/zenutils/tests/test_import_all.py
+-rw-r--r--   0 test       (501) staff       (20)     1821 2022-06-21 06:30:06.000000 zenutils-0.3.9/zenutils/tests/test_jsonutils.py
+-rw-r--r--   0 test       (501) staff       (20)    10045 2022-06-19 14:09:18.000000 zenutils-0.3.9/zenutils/tests/test_listutils.py
+-rw-r--r--   0 test       (501) staff       (20)     1051 2022-06-21 01:39:50.000000 zenutils-0.3.9/zenutils/tests/test_logutils.py
+-rw-r--r--   0 test       (501) staff       (20)      980 2022-06-19 14:09:25.000000 zenutils-0.3.9/zenutils/tests/test_nameutils.py
+-rw-r--r--   0 test       (501) staff       (20)    13987 2022-09-23 17:25:31.000000 zenutils-0.3.9/zenutils/tests/test_numericutils.py
+-rw-r--r--   0 test       (501) staff       (20)    54463 2022-09-28 07:22:41.000000 zenutils-0.3.9/zenutils/tests/test_randomutils.py
+-rw-r--r--   0 test       (501) staff       (20)     4304 2022-10-18 04:33:14.000000 zenutils-0.3.9/zenutils/tests/test_sixutils.py
+-rw-r--r--   0 test       (501) staff       (20)    27083 2022-06-21 07:36:31.000000 zenutils-0.3.9/zenutils/tests/test_strutils.py
+-rw-r--r--   0 test       (501) staff       (20)     2056 2022-08-16 15:10:43.000000 zenutils-0.3.9/zenutils/tests/test_sysutils.py
+-rw-r--r--   0 test       (501) staff       (20)     4540 2022-06-20 13:23:51.000000 zenutils-0.3.9/zenutils/tests/test_threadutils.py
+-rw-r--r--   0 test       (501) staff       (20)     3151 2022-08-05 14:11:47.000000 zenutils-0.3.9/zenutils/tests/test_treeutils.py
+-rw-r--r--   0 test       (501) staff       (20)     5116 2022-06-19 14:09:58.000000 zenutils-0.3.9/zenutils/tests/test_typingutils.py
+-rw-r--r--   0 test       (501) staff       (20)    20792 2022-08-03 06:49:45.000000 zenutils-0.3.9/zenutils/threadutils.py
+-rw-r--r--   0 test       (501) staff       (20)     4029 2022-08-05 14:09:17.000000 zenutils-0.3.9/zenutils/treeutils.py
+-rw-r--r--   0 test       (501) staff       (20)     7917 2022-06-21 01:35:25.000000 zenutils-0.3.9/zenutils/typingutils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2022-10-22 13:01:51.242579 zenutils-0.3.9/zenutils.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)    20457 2022-10-22 13:01:51.000000 zenutils-0.3.9/zenutils.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1537 2022-10-22 13:01:51.000000 zenutils-0.3.9/zenutils.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2022-10-22 13:01:51.000000 zenutils-0.3.9/zenutils.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2022-10-22 13:01:50.000000 zenutils-0.3.9/zenutils.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)        9 2022-10-22 13:01:51.000000 zenutils-0.3.9/zenutils.egg-info/top_level.txt
```

### Comparing `zenutils-0.3.8/LICENSE` & `zenutils-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/PKG-INFO` & `zenutils-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenutils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Collection of simple utils.
 Home-page: UNKNOWN
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: zenutils
 Platform: UNKNOWN
@@ -785,8 +785,12 @@
 - Add randomutils.Lcg31Random.
 - Add randomutils.get_password_seed32.
 
 ### v0.3.8
 
 - Fix force_text in handling NON-STR type data.
 
+### v0.3.9
+
+- Add delete_script parameter in fsutils.execute_script.
+
```

### Comparing `zenutils-0.3.8/README.md` & `zenutils-0.3.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -765,7 +765,11 @@
 
 - Add randomutils.Lcg31Random.
 - Add randomutils.get_password_seed32.
 
 ### v0.3.8
 
 - Fix force_text in handling NON-STR type data.
+
+### v0.3.9
+
+- Add delete_script parameter in fsutils.execute_script.
```

### Comparing `zenutils-0.3.8/setup.py` & `zenutils-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     requires += [x.strip() for x in fobj.readlines() if x.strip()]
 if os.sys.version_info.major == 3 and os.sys.version_info.minor <= 2:
     with open(os.path.join(here, 'requirements.py32.txt'), "r", encoding="utf-8") as fobj:
         requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="zenutils",
-    version="0.3.8",
+    version="0.3.9",
     description="Collection of simple utils.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     license_files=("LICENSE",),
```

### Comparing `zenutils-0.3.8/zenutils/base64utils.py` & `zenutils-0.3.9/zenutils/base64utils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/cacheutils.py` & `zenutils-0.3.9/zenutils/cacheutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/cipherutils.py` & `zenutils-0.3.9/zenutils/cipherutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/dictutils.py` & `zenutils-0.3.9/zenutils/dictutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/fsutils.py` & `zenutils-0.3.9/zenutils/fsutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/funcutils.py` & `zenutils-0.3.9/zenutils/funcutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/hashutils.py` & `zenutils-0.3.9/zenutils/hashutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/httputils.py` & `zenutils-0.3.9/zenutils/httputils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/jsonutils.py` & `zenutils-0.3.9/zenutils/jsonutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/listutils.py` & `zenutils-0.3.9/zenutils/listutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/logutils.py` & `zenutils-0.3.9/zenutils/logutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/nameutils.py` & `zenutils-0.3.9/zenutils/nameutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/numericutils.py` & `zenutils-0.3.9/zenutils/numericutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/randomutils.py` & `zenutils-0.3.9/zenutils/randomutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/sixutils.py` & `zenutils-0.3.9/zenutils/sixutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/strutils.py` & `zenutils-0.3.9/zenutils/strutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/sysutils.py` & `zenutils-0.3.9/zenutils/sysutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     """
     import psutil
     mainp = psutil.Process(pid)
     for subp in mainp.children(recursive=True):
         os.kill(subp.pid, sig)
     os.kill(mainp.pid, sig)
 
-def execute_script(script, workspace=None, script_name=None, timeout=0, timeout_kill=None, timeout_kill_wait=1, non_block_read_timeout=2):
+def execute_script(script, workspace=None, script_name=None, timeout=0, timeout_kill=None, timeout_kill_wait=1, non_block_read_timeout=2, delete_script=True):
     """Execute a shell script under special workspace.
 
     @Returns:
         (int, str, str): Returns script exitcode, std output and std error.
     
     @Parameters:
         script(str): Script source code.
@@ -216,25 +216,31 @@
             break
         time.sleep(0.1)
 
     if normally_finished_flag:
         code, stdout, stderr = p.returncode, p.stdout.read(), p.stderr.read()
         stdout = strutils.force_text(stdout)
         stderr = strutils.force_text(stderr)
-        return code, stdout, stderr
+        result = code, stdout, stderr
     else:
         stdout_reader = NonBlockReader(p.stdout, wait_time=non_block_read_timeout)
         stderr_reader = NonBlockReader(p.stderr, wait_time=non_block_read_timeout)
         result = p.returncode, force_text(stdout_reader.read()), force_text(stderr_reader.read())
         try:
             p.stdout.close()
             p.stderr.close()
-        except Exception as error:
+        except Exception:
             pass
-        return result
+    
+    if delete_script:
+        try:
+            os.unlink(script_path)
+        except Exception:
+            pass
+    return result
 
 def get_node_ip():
     """get node's main ip address.
     """
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     s.settimeout(0)
     try:
```

### Comparing `zenutils-0.3.8/zenutils/tests/assets/p1.jpeg` & `zenutils-0.3.9/zenutils/tests/assets/p1.jpeg`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_cacheutils.py` & `zenutils-0.3.9/zenutils/tests/test_cacheutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_cipherutils.py` & `zenutils-0.3.9/zenutils/tests/test_cipherutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_dictutils.py` & `zenutils-0.3.9/zenutils/tests/test_dictutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_fsutils.py` & `zenutils-0.3.9/zenutils/tests/test_fsutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_funcutils.py` & `zenutils-0.3.9/zenutils/tests/test_funcutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_hashutils.py` & `zenutils-0.3.9/zenutils/tests/test_hashutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_httputils.py` & `zenutils-0.3.9/zenutils/tests/test_httputils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_import_all.py` & `zenutils-0.3.9/zenutils/tests/test_import_all.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_jsonutils.py` & `zenutils-0.3.9/zenutils/tests/test_jsonutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_listutils.py` & `zenutils-0.3.9/zenutils/tests/test_listutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_logutils.py` & `zenutils-0.3.9/zenutils/tests/test_logutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_nameutils.py` & `zenutils-0.3.9/zenutils/tests/test_nameutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_numericutils.py` & `zenutils-0.3.9/zenutils/tests/test_numericutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_randomutils.py` & `zenutils-0.3.9/zenutils/tests/test_randomutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_sixutils.py` & `zenutils-0.3.9/zenutils/tests/test_sixutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_strutils.py` & `zenutils-0.3.9/zenutils/tests/test_strutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_sysutils.py` & `zenutils-0.3.9/zenutils/tests/test_sysutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_threadutils.py` & `zenutils-0.3.9/zenutils/tests/test_threadutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_treeutils.py` & `zenutils-0.3.9/zenutils/tests/test_treeutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/tests/test_typingutils.py` & `zenutils-0.3.9/zenutils/tests/test_typingutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/threadutils.py` & `zenutils-0.3.9/zenutils/threadutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/treeutils.py` & `zenutils-0.3.9/zenutils/treeutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils/typingutils.py` & `zenutils-0.3.9/zenutils/typingutils.py`

 * *Files identical despite different names*

### Comparing `zenutils-0.3.8/zenutils.egg-info/PKG-INFO` & `zenutils-0.3.9/zenutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenutils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Collection of simple utils.
 Home-page: UNKNOWN
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: zenutils
 Platform: UNKNOWN
@@ -785,8 +785,12 @@
 - Add randomutils.Lcg31Random.
 - Add randomutils.get_password_seed32.
 
 ### v0.3.8
 
 - Fix force_text in handling NON-STR type data.
 
+### v0.3.9
+
+- Add delete_script parameter in fsutils.execute_script.
+
```

### Comparing `zenutils-0.3.8/zenutils.egg-info/SOURCES.txt` & `zenutils-0.3.9/zenutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

