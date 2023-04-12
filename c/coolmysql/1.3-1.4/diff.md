# Comparing `tmp/coolmysql-1.3.tar.gz` & `tmp/coolmysql-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.3.tar", last modified: Mon Apr 10 14:26:15 2023, max compression
+gzip compressed data, was "coolmysql-1.4.tar", last modified: Wed Apr 12 15:22:07 2023, max compression
```

## Comparing `coolmysql-1.3.tar` & `coolmysql-1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.3/LICENSE
--rw-r--r--   0        0        0     4351 2023-04-09 11:16:42.051321 coolmysql-1.3/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.3/coolmysql.py
--rw-r--r--   0        0        0      562 2023-04-10 09:20:13.157209 coolmysql-1.3/pyproject.toml
--rw-r--r--   0        0        0     4603 1970-01-01 00:00:00.000000 coolmysql-1.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4/LICENSE
+-rw-r--r--   0        0        0     4351 2023-04-09 11:16:42.051321 coolmysql-1.4/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4/coolmysql.py
+-rw-r--r--   0        0        0      562 2023-04-12 15:16:36.716121 coolmysql-1.4/pyproject.toml
+-rw-r--r--   0        0        0     4603 1970-01-01 00:00:00.000000 coolmysql-1.4/PKG-INFO
```

### Comparing `coolmysql-1.3/LICENSE` & `coolmysql-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmysql-1.3/README.md` & `coolmysql-1.4/README.md`

 * *Files identical despite different names*

### Comparing `coolmysql-1.3/pyproject.toml` & `coolmysql-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmysql"
-version = "1.3"
+version = "1.4"
 description = "史上最优雅的 mysql ORM"
-dependencies = ["lccpy >=1.3"]
+dependencies = ["lccpy >=1.4"]
 keywords = ["coolmysql", "pymysql", "mysql"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `coolmysql-1.3/PKG-INFO` & `coolmysql-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: coolmysql
-Version: 1.3
+Version: 1.4
 Summary: 史上最优雅的 mysql ORM
 Keywords: coolmysql,pymysql,mysql
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.3
+Requires-Dist: lccpy >=1.4
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/coolmysql
 
 # 项目描述
 
 史上最优雅的 mysql ORM 。
 
 # 安装与教程
```

