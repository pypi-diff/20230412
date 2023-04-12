# Comparing `tmp/asmr_spider-0.0.5.tar.gz` & `tmp/asmr_spider-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmr_spider-0.0.5.tar", max compression
+gzip compressed data, was "asmr_spider-0.1.0a1.tar", max compression
```

## Comparing `asmr_spider-0.0.5.tar` & `asmr_spider-0.1.0a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/LICENSE
--rw-r--r--   0        0        0      894 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/README.md
--rw-r--r--   0        0        0      318 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/asmr_spider/__init__.py
--rw-r--r--   0        0        0      340 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/asmr_spider/__main__.py
--rw-r--r--   0        0        0     1767 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/asmr_spider/config.py
--rw-r--r--   0        0        0     5102 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/asmr_spider/spider.py
--rw-r--r--   0        0        0      940 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 asmr_spider-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0      894 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/README.md
+-rw-r--r--   0        0        0      318 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/asmr_spider/__init__.py
+-rw-r--r--   0        0        0      340 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/asmr_spider/__main__.py
+-rw-r--r--   0        0        0     1814 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/asmr_spider/config.py
+-rw-r--r--   0        0        0     5102 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/asmr_spider/spider.py
+-rw-r--r--   0        0        0      940 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1672 1970-01-01 00:00:00.000000 asmr_spider-0.1.0a1/PKG-INFO
```

### Comparing `asmr_spider-0.0.5/LICENSE` & `asmr_spider-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.5/README.md` & `asmr_spider-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.5/asmr_spider/config.py` & `asmr_spider-0.1.0a1/asmr_spider/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 import sys, yaml
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, Extra, ConfigDict
 from loguru import logger
 from rich.progress import (
     BarColumn,
     DownloadColumn,
     Progress,
     TextColumn,
     TransferSpeedColumn,
@@ -58,15 +58,16 @@
         progress.console.log(f, style='bold yellow on black')
         sys.exit(1)
 
 
 _config = yaml.safe_load(confpath.read_text('utf-8'))
 
 
-class Config(BaseModel, extra=Extra.ignore):
+class Config(BaseModel):
+    model_config = ConfigDict(extra=Extra.ignore)
     username: str = 'guest'
     password: str = 'guest'
     proxy: str = ''
     user_agent: str = 'Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)'
 
 
-config = Config.parse_obj(_config)
+config = Config.model_validate(_config)
```

### Comparing `asmr_spider-0.0.5/asmr_spider/spider.py` & `asmr_spider-0.1.0a1/asmr_spider/spider.py`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.5/pyproject.toml` & `asmr_spider-0.1.0a1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asmr-spider"
-version = "0.0.5"
+version = "0.1.0a1"
 description = "asmr.one 音声下载器"
 authors = ["月ヶ瀬"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [
     { include = "asmr_spider" },
 ]
@@ -13,23 +13,23 @@
 keywords = ["ASMR", "ASMR Downloader"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 PyYAML = ">=6.0"
 httpx = ">=0.23.0"
 loguru = ">=0.6.0"
-pydantic = "^1.10.5"
+pydantic = "^2.0a1"
 rich = ">=13.0.0"
 
 [tool.poetry.dev-dependencies]
 python = "^3.9"
 PyYAML = ">=6.0"
 httpx = ">=0.23.0"
 loguru = ">=0.6.0"
-pydantic = "^1.10.5"
+pydantic = "^2.0a1"
 rich = ">=13.0.0"
 ujson = ">=5.2.0"
 
 [tool.poetry.scripts]
 asmr = "asmr_spider.__main__:main"
 
 [tool.mypy]
```

### Comparing `asmr_spider-0.0.5/PKG-INFO` & `asmr_spider-0.1.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: asmr-spider
-Version: 0.0.5
+Version: 0.1.0a1
 Summary: asmr.one 音声下载器
 Home-page: https://github.com/tkgs0/asmr-spider
 License: GPL-3.0
 Keywords: ASMR,ASMR Downloader
 Author: 月ヶ瀬
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: loguru (>=0.6.0)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pydantic (>=2.0a1,<3.0)
 Requires-Dist: rich (>=13.0.0)
 Project-URL: Repository, https://github.com/tkgs0/asmr-spider
 Description-Content-Type: text/markdown
 
 # ASMR-Spider
 
 本项目改编自 [DiheChen/go-asmr-spider](https://github.com/DiheChen/go-asmr-spider/tree/python)
```

