# Comparing `tmp/tonggong-0.2.9.tar.gz` & `tmp/tonggong-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tonggong-0.2.9.tar", last modified: Wed Nov 10 12:26:51 2021, max compression
+gzip compressed data, was "tonggong-1.0.0.tar", last modified: Wed Apr 12 12:08:24 2023, max compression
```

## Comparing `tonggong-0.2.9.tar` & `tonggong-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,51 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-10 12:26:51.000000 tonggong-0.2.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1069 2021-11-10 12:26:24.000000 tonggong-0.2.9/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1900 2021-11-10 12:26:51.000000 tonggong-0.2.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1318 2021-11-10 12:26:24.000000 tonggong-0.2.9/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      482 2021-11-10 12:26:24.000000 tonggong-0.2.9/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-11-10 12:26:51.000000 tonggong-0.2.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      851 2021-11-10 12:26:24.000000 tonggong-0.2.9/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-10 12:26:51.000000 tonggong-0.2.9/tonggong/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      902 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/base62.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12544 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/bunch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2629 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/constant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1539 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/converter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15491 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/crontab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/enum.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5670 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/formatter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      443 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      659 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/hash.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6314 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/isoweek.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3715 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/redis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2478 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-10 12:26:51.000000 tonggong-0.2.9/tonggong/validations/
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/validations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      853 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/validations/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2006 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/validations/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10043 2021-11-10 12:26:24.000000 tonggong-0.2.9/tonggong/validations/validators.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-10 12:26:51.000000 tonggong-0.2.9/tonggong.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1900 2021-11-10 12:26:51.000000 tonggong-0.2.9/tonggong.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      552 2021-11-10 12:26:51.000000 tonggong-0.2.9/tonggong.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-11-10 12:26:51.000000 tonggong-0.2.9/tonggong.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-11-10 12:26:51.000000 tonggong-0.2.9/tonggong.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:08:24.060513 tonggong-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-12 12:08:06.000000 tonggong-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 12:08:24.056513 tonggong-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-12 12:08:06.000000 tonggong-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-12 12:08:06.000000 tonggong-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:08:24.060513 tonggong-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-12 12:08:06.000000 tonggong-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:08:24.052513 tonggong-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_base62.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_bunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_crontab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_django_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_isoweek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-12 12:08:06.000000 tonggong-1.0.0/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:08:24.056513 tonggong-1.0.0/tonggong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/base62.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/crontab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:08:24.056513 tonggong-1.0.0/tonggong/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/django/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/isoweek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:08:24.056513 tonggong-1.0.0/tonggong/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/validations/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/validations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-04-12 12:08:06.000000 tonggong-1.0.0/tonggong/validations/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:08:24.056513 tonggong-1.0.0/tonggong.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 12:08:24.000000 tonggong-1.0.0/tonggong.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-12 12:08:24.000000 tonggong-1.0.0/tonggong.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:08:24.000000 tonggong-1.0.0/tonggong.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 12:08:24.000000 tonggong-1.0.0/tonggong.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tonggong-0.2.9/LICENSE` & `tonggong-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tonggong-0.2.9/PKG-INFO` & `tonggong-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: tonggong
-Version: 0.2.9
+Version: 1.0.0
 Summary: Universal toolkit
 Home-page: https://github.com/arcticdata/tonggong
 Author: Arctic Data
 Author-email: hello@datarc.cn
 License: MIT License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 小雅·彤弓
 
 <p style="text-align: left">
     <a href="https://pypi.python.org/pypi/tonggong">
@@ -27,33 +26,30 @@
     </a>
     <a href="https://github.com/arcticdata/tonggong/blob/master/LICENSE">
         <img src="https://img.shields.io/pypi/l/tonggong?style=flat-square" alt="License" />
     </a>
     <a href="https://codecov.io/gh/arcticdata/tonggong">
         <img src="https://img.shields.io/codecov/c/gh/arcticdata/tonggong/master?style=flat-square" alt="Codecov" />
     </a>
-    <a href="https://travis-ci.com/arcticdata/tonggong">
-        <img src="https://img.shields.io/travis/com/arcticdata/tonggong?style=flat-square" alt="Travis" />
-    </a>
 </p>
 
-```
+```chinese
 彤弓弨兮，受言藏之。我有嘉宾，中心贶之。钟鼓既设，一朝飨之。
 彤弓弨兮，受言载之。我有嘉宾，中心喜之。钟鼓既设，一朝右之。
 彤弓弨兮，受言櫜之。我有嘉宾，中心好之。钟鼓既设，一朝酬之。
 ```
 
 ## 介绍
 
 通用工具集合
 
 ### 环境安装
-> pipenv install --dev
 
-### 格式化
-> pipenv run black .
+> make install
 
-### 单元测试
+### 格式化
 
-> pipenv run pytest
+> make fmt
 
+### 单元测试
 
+> make test
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: tonggong Version: 0.2.9 Summary: Universal toolkit
+Metadata-Version: 2.1 Name: tonggong Version: 1.0.0 Summary: Universal toolkit
 Home-page: https://github.com/arcticdata/tonggong Author: Arctic Data Author-
-email: hello@datarc.cn License: MIT License Platform: UNKNOWN Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
-Content-Type: text/markdown License-File: LICENSE # å°éÂ·å½¤å¼
+email: hello@datarc.cn License: MIT License Classifier: License :: OSI Approved
+:: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
+License-File: LICENSE # å°éÂ·å½¤å¼
 [Package] [https://img.shields.io/pypi/pyversions/tonggong?style=flat-square]
-[License] [Codecov] [Travis]
-```
+[License] [Codecov]
+```chinese
 å½¤å¼å¼¨å®ï¼åè¨èä¹ãææåå®¾ï¼ä¸­å¿è´¶ä¹ãéé¼æ¢è®¾ï¼ä¸æé£¨ä¹ã
 å½¤å¼å¼¨å®ï¼åè¨è½½ä¹ãææåå®¾ï¼ä¸­å¿åä¹ãéé¼æ¢è®¾ï¼ä¸æå³ä¹ã
 å½¤å¼å¼¨å®ï¼åè¨æ«ä¹ãææåå®¾ï¼ä¸­å¿å¥½ä¹ãéé¼æ¢è®¾ï¼ä¸æé¬ä¹ã
-``` ## ä»ç» éç¨å·¥å·éå ### ç¯å¢å®è£ > pipenv install --dev ###
-æ ¼å¼å > pipenv run black . ### ååæµè¯ > pipenv run pytest
+``` ## ä»ç» éç¨å·¥å·éå ### ç¯å¢å®è£ > make install ### æ ¼å¼å
+> make fmt ### ååæµè¯ > make test
```

### Comparing `tonggong-0.2.9/README.md` & `tonggong-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,31 +9,30 @@
     </a>
     <a href="https://github.com/arcticdata/tonggong/blob/master/LICENSE">
         <img src="https://img.shields.io/pypi/l/tonggong?style=flat-square" alt="License" />
     </a>
     <a href="https://codecov.io/gh/arcticdata/tonggong">
         <img src="https://img.shields.io/codecov/c/gh/arcticdata/tonggong/master?style=flat-square" alt="Codecov" />
     </a>
-    <a href="https://travis-ci.com/arcticdata/tonggong">
-        <img src="https://img.shields.io/travis/com/arcticdata/tonggong?style=flat-square" alt="Travis" />
-    </a>
 </p>
 
-```
+```chinese
 彤弓弨兮，受言藏之。我有嘉宾，中心贶之。钟鼓既设，一朝飨之。
 彤弓弨兮，受言载之。我有嘉宾，中心喜之。钟鼓既设，一朝右之。
 彤弓弨兮，受言櫜之。我有嘉宾，中心好之。钟鼓既设，一朝酬之。
 ```
 
 ## 介绍
 
 通用工具集合
 
 ### 环境安装
-> pipenv install --dev
+
+> make install
 
 ### 格式化
-> pipenv run black .
+
+> make fmt
 
 ### 单元测试
 
-> pipenv run pytest
+> make test
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # å°éÂ·å½¤å¼
 [Package] [https://img.shields.io/pypi/pyversions/tonggong?style=flat-square]
-[License] [Codecov] [Travis]
-```
+[License] [Codecov]
+```chinese
 å½¤å¼å¼¨å®ï¼åè¨èä¹ãææåå®¾ï¼ä¸­å¿è´¶ä¹ãéé¼æ¢è®¾ï¼ä¸æé£¨ä¹ã
 å½¤å¼å¼¨å®ï¼åè¨è½½ä¹ãææåå®¾ï¼ä¸­å¿åä¹ãéé¼æ¢è®¾ï¼ä¸æå³ä¹ã
 å½¤å¼å¼¨å®ï¼åè¨æ«ä¹ãææåå®¾ï¼ä¸­å¿å¥½ä¹ãéé¼æ¢è®¾ï¼ä¸æé¬ä¹ã
-``` ## ä»ç» éç¨å·¥å·éå ### ç¯å¢å®è£ > pipenv install --dev ###
-æ ¼å¼å > pipenv run black . ### ååæµè¯ > pipenv run pytest
+``` ## ä»ç» éç¨å·¥å·éå ### ç¯å¢å®è£ > make install ### æ ¼å¼å
+> make fmt ### ååæµè¯ > make test
```

### Comparing `tonggong-0.2.9/setup.py` & `tonggong-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     description = f.read()
 
 setup(
     name="tonggong",
-    version="0.2.9",
+    version="1.0.0",
     description="Universal toolkit",
     long_description=description,
     long_description_content_type="text/markdown",
     author="Arctic Data",
     author_email="hello@datarc.cn",
     url="https://github.com/arcticdata/tonggong",
     license="MIT License",
     install_requires="",
     packages=find_packages(exclude=["tests"]),
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `tonggong-0.2.9/tonggong/base62.py` & `tonggong-1.0.0/tonggong/base62.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 简单实现的 Base62 编码转化
 
 https://en.wikipedia.org/wiki/Base62
 """
 
 import string
 
-
 _ALPHABET = string.ascii_uppercase + string.ascii_lowercase + string.digits
 _BASE_DICT = dict((c, v) for v, c in enumerate(_ALPHABET))
 
 
 def encode(n: int) -> str:
     """数值转换编码"""
     if not n:
```

### Comparing `tonggong-0.2.9/tonggong/bunch.py` & `tonggong-1.0.0/tonggong/bunch.py`

 * *Files identical despite different names*

### Comparing `tonggong-0.2.9/tonggong/converter.py` & `tonggong-1.0.0/tonggong/converter.py`

 * *Files identical despite different names*

### Comparing `tonggong-0.2.9/tonggong/crontab.py` & `tonggong-1.0.0/tonggong/crontab.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 Released under the GNU LGPL v2.1 and v3
 available:
 http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html
 http://www.gnu.org/licenses/lgpl.html
 Other licenses may be available upon request.
 """
 
-from collections import namedtuple
-from datetime import datetime, timedelta
 import sys
 import warnings
+from collections import namedtuple
+from datetime import datetime, timedelta
 
 _ranges = [
     (0, 59),
     (0, 59),
     (0, 23),
     (1, 31),
     (1, 12),
```

### Comparing `tonggong-0.2.9/tonggong/formatter.py` & `tonggong-1.0.0/tonggong/formatter.py`

 * *Files identical despite different names*

### Comparing `tonggong-0.2.9/tonggong/hash.py` & `tonggong-1.0.0/tonggong/hash.py`

 * *Files identical despite different names*

### Comparing `tonggong-0.2.9/tonggong/isoweek.py` & `tonggong-1.0.0/tonggong/isoweek.py`

 * *Files identical despite different names*

### Comparing `tonggong-0.2.9/tonggong/redis.py` & `tonggong-1.0.0/tonggong/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import contextlib
 import os
 import signal
 import time
 
 from redis import Redis
-from redis.lock import Lock, LockError
+from redis.exceptions import LockError
+from redis.lock import Lock
 
 from tonggong.hash import Hash
 
 _COUNT = 400
 
 
 def safe_delete_hash(conn: Redis, hash_key: str, count: int = None):
@@ -109,18 +111,17 @@
 
     @classmethod
     def get_key_name(cls, name: str) -> str:
         """Get Redis lock key name"""
         return f"redis-lock:{name}"
 
     def release(self):
-        try:
+        # 可能锁已经自动失效释放，忽略 LockError;
+        with contextlib.suppress(LockError, AttributeError):
             super(RedisLock, self).release()
-        except LockError:  # 可能锁已经自动失效释放，忽略 LockError
-            pass
 
     def _register_signal_handler(self):
         """接管信号处理函数"""
         self._prev_sigint = signal.signal(signal.SIGINT, self._signal_handler)
         self._prev_sigterm = signal.signal(signal.SIGTERM, self._signal_handler)
 
     def _restore_signal_handler(self):
```

### Comparing `tonggong-0.2.9/tonggong/util.py` & `tonggong-1.0.0/tonggong/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import calendar
 import datetime
 import json
 import logging
 import re
-from typing import Union
+from typing import Optional, Union
 
 
 def base64_encode(value: str) -> str:
     """对字符串进行 base64 编码， 去掉末尾的 ="""
     return base64.b64encode(value.encode("utf8"), altchars=b"+-").decode("utf8").rstrip("=")
 
 
@@ -19,14 +19,19 @@
 
 def padding_base64(value: str) -> str:
     num = len(value) % 4
     num = 4 - num if num else 0
     return value + "=" * num
 
 
+def first(items: Optional[iter], default=None):
+    """获取数组的第一个元素"""
+    return next(iter(items or []), default)
+
+
 def json_dumps(obj, separators=(",", ":"), sort_keys=True, ensure_ascii=False, **kwargs) -> str:
     return json.dumps(obj, separators=separators, sort_keys=sort_keys, ensure_ascii=ensure_ascii, **kwargs)
 
 
 def add_months(date: datetime.date, num: int) -> datetime.date:
     month = date.month - 1 + num
     year = date.year + month // 12
```

### Comparing `tonggong-0.2.9/tonggong/validations/errors.py` & `tonggong-1.0.0/tonggong/validations/errors.py`

 * *Files identical despite different names*

### Comparing `tonggong-0.2.9/tonggong/validations/utils.py` & `tonggong-1.0.0/tonggong/validations/utils.py`

 * *Files identical despite different names*

### Comparing `tonggong-0.2.9/tonggong/validations/validators.py` & `tonggong-1.0.0/tonggong/validations/validators.py`

 * *Files identical despite different names*

### Comparing `tonggong-0.2.9/tonggong.egg-info/PKG-INFO` & `tonggong-1.0.0/tonggong.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: tonggong
-Version: 0.2.9
+Version: 1.0.0
 Summary: Universal toolkit
 Home-page: https://github.com/arcticdata/tonggong
 Author: Arctic Data
 Author-email: hello@datarc.cn
 License: MIT License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 小雅·彤弓
 
 <p style="text-align: left">
     <a href="https://pypi.python.org/pypi/tonggong">
@@ -27,33 +26,30 @@
     </a>
     <a href="https://github.com/arcticdata/tonggong/blob/master/LICENSE">
         <img src="https://img.shields.io/pypi/l/tonggong?style=flat-square" alt="License" />
     </a>
     <a href="https://codecov.io/gh/arcticdata/tonggong">
         <img src="https://img.shields.io/codecov/c/gh/arcticdata/tonggong/master?style=flat-square" alt="Codecov" />
     </a>
-    <a href="https://travis-ci.com/arcticdata/tonggong">
-        <img src="https://img.shields.io/travis/com/arcticdata/tonggong?style=flat-square" alt="Travis" />
-    </a>
 </p>
 
-```
+```chinese
 彤弓弨兮，受言藏之。我有嘉宾，中心贶之。钟鼓既设，一朝飨之。
 彤弓弨兮，受言载之。我有嘉宾，中心喜之。钟鼓既设，一朝右之。
 彤弓弨兮，受言櫜之。我有嘉宾，中心好之。钟鼓既设，一朝酬之。
 ```
 
 ## 介绍
 
 通用工具集合
 
 ### 环境安装
-> pipenv install --dev
 
-### 格式化
-> pipenv run black .
+> make install
 
-### 单元测试
+### 格式化
 
-> pipenv run pytest
+> make fmt
 
+### 单元测试
 
+> make test
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: tonggong Version: 0.2.9 Summary: Universal toolkit
+Metadata-Version: 2.1 Name: tonggong Version: 1.0.0 Summary: Universal toolkit
 Home-page: https://github.com/arcticdata/tonggong Author: Arctic Data Author-
-email: hello@datarc.cn License: MIT License Platform: UNKNOWN Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
-Content-Type: text/markdown License-File: LICENSE # å°éÂ·å½¤å¼
+email: hello@datarc.cn License: MIT License Classifier: License :: OSI Approved
+:: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
+License-File: LICENSE # å°éÂ·å½¤å¼
 [Package] [https://img.shields.io/pypi/pyversions/tonggong?style=flat-square]
-[License] [Codecov] [Travis]
-```
+[License] [Codecov]
+```chinese
 å½¤å¼å¼¨å®ï¼åè¨èä¹ãææåå®¾ï¼ä¸­å¿è´¶ä¹ãéé¼æ¢è®¾ï¼ä¸æé£¨ä¹ã
 å½¤å¼å¼¨å®ï¼åè¨è½½ä¹ãææåå®¾ï¼ä¸­å¿åä¹ãéé¼æ¢è®¾ï¼ä¸æå³ä¹ã
 å½¤å¼å¼¨å®ï¼åè¨æ«ä¹ãææåå®¾ï¼ä¸­å¿å¥½ä¹ãéé¼æ¢è®¾ï¼ä¸æé¬ä¹ã
-``` ## ä»ç» éç¨å·¥å·éå ### ç¯å¢å®è£ > pipenv install --dev ###
-æ ¼å¼å > pipenv run black . ### ååæµè¯ > pipenv run pytest
+``` ## ä»ç» éç¨å·¥å·éå ### ç¯å¢å®è£ > make install ### æ ¼å¼å
+> make fmt ### ååæµè¯ > make test
```

