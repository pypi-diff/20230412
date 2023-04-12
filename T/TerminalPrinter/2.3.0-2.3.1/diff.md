# Comparing `tmp/TerminalPrinter-2.3.0.tar.gz` & `tmp/TerminalPrinter-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TerminalPrinter-2.3.0.tar", last modified: Wed Apr 12 13:32:10 2023, max compression
+gzip compressed data, was "dist/TerminalPrinter-2.3.1.tar", last modified: Wed Apr 12 15:11:35 2023, max compression
```

## Comparing `TerminalPrinter-2.3.0.tar` & `TerminalPrinter-2.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/
--rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/PKG-INFO
--rw-r--r--   0 hellflame   (501) staff       (20)     1077 2021-05-18 14:35:42.000000 TerminalPrinter-2.3.0/LICENSE
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/printer/
--rw-r--r--   0 hellflame   (501) staff       (20)     4454 2023-04-12 12:18:14.000000 TerminalPrinter-2.3.0/printer/run.py
--rw-r--r--   0 hellflame   (501) staff       (20)      106 2023-04-12 13:30:43.000000 TerminalPrinter-2.3.0/printer/version.py
--rw-r--r--   0 hellflame   (501) staff       (20)     5378 2023-04-10 14:11:54.000000 TerminalPrinter-2.3.0/printer/painter.py
--rw-r--r--   0 hellflame   (501) staff       (20)        0 2021-05-18 14:35:43.000000 TerminalPrinter-2.3.0/printer/__init__.py
--rw-r--r--   0 hellflame   (501) staff       (20)      753 2023-04-09 15:24:51.000000 TerminalPrinter-2.3.0/printer/utils.py
--rw-r--r--   0 hellflame   (501) staff       (20)    17831 2021-05-18 14:35:43.000000 TerminalPrinter-2.3.0/printer/http.py
--rw-r--r--   0 hellflame   (501) staff       (20)     3466 2023-04-09 15:33:02.000000 TerminalPrinter-2.3.0/printer/font_helper.py
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/
--rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/PKG-INFO
--rw-r--r--   0 hellflame   (501) staff       (20)      415 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/SOURCES.txt
--rw-r--r--   0 hellflame   (501) staff       (20)       51 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/entry_points.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        7 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/requires.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        8 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/top_level.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        1 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/dependency_links.txt
--rw-r--r--   0 hellflame   (501) staff       (20)       52 2021-05-18 14:35:42.000000 TerminalPrinter-2.3.0/MANIFEST.in
--rw-r--r--   0 hellflame   (501) staff       (20)     8729 2023-04-12 13:30:43.000000 TerminalPrinter-2.3.0/README.md
--rw-r--r--   0 hellflame   (501) staff       (20)      478 2021-05-18 14:35:42.000000 TerminalPrinter-2.3.0/CHANGES.txt
--rw-r--r--   0 hellflame   (501) staff       (20)     1186 2023-04-06 23:51:05.000000 TerminalPrinter-2.3.0/setup.py
--rw-r--r--   0 hellflame   (501) staff       (20)       38 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/setup.cfg
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-12 15:11:35.000000 TerminalPrinter-2.3.1/
+-rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-12 15:11:35.000000 TerminalPrinter-2.3.1/PKG-INFO
+-rw-r--r--   0 hellflame   (501) staff       (20)     1077 2021-05-18 14:35:42.000000 TerminalPrinter-2.3.1/LICENSE
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-12 15:11:35.000000 TerminalPrinter-2.3.1/printer/
+-rw-r--r--   0 hellflame   (501) staff       (20)     4454 2023-04-12 12:18:14.000000 TerminalPrinter-2.3.1/printer/run.py
+-rw-r--r--   0 hellflame   (501) staff       (20)      106 2023-04-12 15:08:19.000000 TerminalPrinter-2.3.1/printer/version.py
+-rw-r--r--   0 hellflame   (501) staff       (20)     5378 2023-04-10 14:11:54.000000 TerminalPrinter-2.3.1/printer/painter.py
+-rw-r--r--   0 hellflame   (501) staff       (20)        0 2021-05-18 14:35:43.000000 TerminalPrinter-2.3.1/printer/__init__.py
+-rw-r--r--   0 hellflame   (501) staff       (20)      816 2023-04-12 14:05:55.000000 TerminalPrinter-2.3.1/printer/utils.py
+-rw-r--r--   0 hellflame   (501) staff       (20)    17831 2021-05-18 14:35:43.000000 TerminalPrinter-2.3.1/printer/http.py
+-rw-r--r--   0 hellflame   (501) staff       (20)     3466 2023-04-09 15:33:02.000000 TerminalPrinter-2.3.1/printer/font_helper.py
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-12 15:11:35.000000 TerminalPrinter-2.3.1/TerminalPrinter.egg-info/
+-rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-12 15:11:34.000000 TerminalPrinter-2.3.1/TerminalPrinter.egg-info/PKG-INFO
+-rw-r--r--   0 hellflame   (501) staff       (20)      415 2023-04-12 15:11:34.000000 TerminalPrinter-2.3.1/TerminalPrinter.egg-info/SOURCES.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)       51 2023-04-12 15:11:34.000000 TerminalPrinter-2.3.1/TerminalPrinter.egg-info/entry_points.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        7 2023-04-12 15:11:34.000000 TerminalPrinter-2.3.1/TerminalPrinter.egg-info/requires.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        8 2023-04-12 15:11:34.000000 TerminalPrinter-2.3.1/TerminalPrinter.egg-info/top_level.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        1 2023-04-12 15:11:34.000000 TerminalPrinter-2.3.1/TerminalPrinter.egg-info/dependency_links.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)       52 2021-05-18 14:35:42.000000 TerminalPrinter-2.3.1/MANIFEST.in
+-rw-r--r--   0 hellflame   (501) staff       (20)     8843 2023-04-12 15:09:06.000000 TerminalPrinter-2.3.1/README.md
+-rw-r--r--   0 hellflame   (501) staff       (20)      478 2021-05-18 14:35:42.000000 TerminalPrinter-2.3.1/CHANGES.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)     1186 2023-04-06 23:51:05.000000 TerminalPrinter-2.3.1/setup.py
+-rw-r--r--   0 hellflame   (501) staff       (20)       38 2023-04-12 15:11:35.000000 TerminalPrinter-2.3.1/setup.cfg
```

### Comparing `TerminalPrinter-2.3.0/PKG-INFO` & `TerminalPrinter-2.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: TerminalPrinter
-Version: 2.3.0
+Version: 2.3.1
 Summary: 终端图片、文字生成器
 Home-page: https://github.com/hellflame/terminal_printer
 Author: hellflame
 Author-email: hellflamedly@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `TerminalPrinter-2.3.0/LICENSE` & `TerminalPrinter-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.3.0/printer/run.py` & `TerminalPrinter-2.3.1/printer/run.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.3.0/printer/painter.py` & `TerminalPrinter-2.3.1/printer/painter.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.3.0/printer/utils.py` & `TerminalPrinter-2.3.1/printer/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
+import sys
 import platform
 
 from printer.version import __version__
 from printer.painter import DEFAULT_SIZE
 from printer.font_helper import choose_font
 
 
 def print_version():
     print("TerminalPrinter v{}".format(__version__))
 
 
 def print_debug(args):
     print_version()
+    print("Interpreter: {}".format(sys.executable))
     print("Shell: {}".format(os.getenv("SHELL")))
     print("Term: {}".format(os.getenv("TERM")))
     print("Platform: {}".format("/".join(platform.uname())))
     print("Given Size: {}/{} Default Size: {}/{}".format(args.width, args.height, *DEFAULT_SIZE))
     print("Arguments: {}".format(" ".join(["{}:{}".format(k, v) for k, v in args.__dict__.items()])))
     if args.text:
         font, exist = choose_font(args.font)
```

### Comparing `TerminalPrinter-2.3.0/printer/http.py` & `TerminalPrinter-2.3.1/printer/http.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.3.0/printer/font_helper.py` & `TerminalPrinter-2.3.1/printer/font_helper.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.3.0/TerminalPrinter.egg-info/PKG-INFO` & `TerminalPrinter-2.3.1/TerminalPrinter.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: TerminalPrinter
-Version: 2.3.0
+Version: 2.3.1
 Summary: 终端图片、文字生成器
 Home-page: https://github.com/hellflame/terminal_printer
 Author: hellflame
 Author-email: hellflamedly@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `TerminalPrinter-2.3.0/README.md` & `TerminalPrinter-2.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,16 @@
 
 首次进行文字处理
 需要执行 terminalprint -i 初始化或指定字体
 更多帮助信息请参考: https://github.com/hellflame/terminal_printer
 ```
 
 > `v2.1.0` 新增 `--debug` 参数，可与其他命令一起使用，输出调试信息
+>
+> 一般会输出终端宽度等重要信息
 
 #### ii. 版本信息
 
 ```bash
 $ terminalprint -v # terminalprint --version
 ```
 
@@ -263,10 +265,16 @@
   新增调试入口
 
 - v2.2.0
 
   新增颜色名称支持
 
   输出长宽更自由
+
+- v2.3.\*
+
+  填充字符直接支持
+
+  调试入口新增输出
 ------
 
 嗯，以上，Just For Fun!
```

### Comparing `TerminalPrinter-2.3.0/setup.py` & `TerminalPrinter-2.3.1/setup.py`

 * *Files identical despite different names*

