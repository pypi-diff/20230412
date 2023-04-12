# Comparing `tmp/TerminalPrinter-2.2.1.tar.gz` & `tmp/TerminalPrinter-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TerminalPrinter-2.2.1.tar", last modified: Mon Apr 10 14:52:31 2023, max compression
+gzip compressed data, was "dist/TerminalPrinter-2.3.0.tar", last modified: Wed Apr 12 13:32:10 2023, max compression
```

## Comparing `TerminalPrinter-2.2.1.tar` & `TerminalPrinter-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/
--rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/PKG-INFO
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/printer/
--rw-r--r--   0 hellflame   (501) staff       (20)     4280 2023-04-10 14:48:28.000000 TerminalPrinter-2.2.1/printer/run.py
--rw-r--r--   0 hellflame   (501) staff       (20)      106 2023-04-10 14:51:28.000000 TerminalPrinter-2.2.1/printer/version.py
--rw-r--r--   0 hellflame   (501) staff       (20)     5378 2023-04-10 14:11:54.000000 TerminalPrinter-2.2.1/printer/painter.py
--rw-r--r--   0 hellflame   (501) staff       (20)        0 2021-05-18 14:35:43.000000 TerminalPrinter-2.2.1/printer/__init__.py
--rw-r--r--   0 hellflame   (501) staff       (20)      753 2023-04-09 15:24:51.000000 TerminalPrinter-2.2.1/printer/utils.py
--rw-r--r--   0 hellflame   (501) staff       (20)    17831 2021-05-18 14:35:43.000000 TerminalPrinter-2.2.1/printer/http.py
--rw-r--r--   0 hellflame   (501) staff       (20)     3466 2023-04-09 15:33:02.000000 TerminalPrinter-2.2.1/printer/font_helper.py
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/
--rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/PKG-INFO
--rw-r--r--   0 hellflame   (501) staff       (20)      407 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/SOURCES.txt
--rw-r--r--   0 hellflame   (501) staff       (20)       51 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/entry_points.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        7 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/requires.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        8 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/top_level.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        1 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/TerminalPrinter.egg-info/dependency_links.txt
--rw-r--r--   0 hellflame   (501) staff       (20)       52 2021-05-18 14:35:42.000000 TerminalPrinter-2.2.1/MANIFEST.in
--rw-r--r--   0 hellflame   (501) staff       (20)     8643 2023-04-10 14:45:40.000000 TerminalPrinter-2.2.1/README.md
--rw-r--r--   0 hellflame   (501) staff       (20)      478 2021-05-18 14:35:42.000000 TerminalPrinter-2.2.1/CHANGES.txt
--rw-r--r--   0 hellflame   (501) staff       (20)     1186 2023-04-06 23:51:05.000000 TerminalPrinter-2.2.1/setup.py
--rw-r--r--   0 hellflame   (501) staff       (20)       38 2023-04-10 14:52:31.000000 TerminalPrinter-2.2.1/setup.cfg
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/
+-rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/PKG-INFO
+-rw-r--r--   0 hellflame   (501) staff       (20)     1077 2021-05-18 14:35:42.000000 TerminalPrinter-2.3.0/LICENSE
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/printer/
+-rw-r--r--   0 hellflame   (501) staff       (20)     4454 2023-04-12 12:18:14.000000 TerminalPrinter-2.3.0/printer/run.py
+-rw-r--r--   0 hellflame   (501) staff       (20)      106 2023-04-12 13:30:43.000000 TerminalPrinter-2.3.0/printer/version.py
+-rw-r--r--   0 hellflame   (501) staff       (20)     5378 2023-04-10 14:11:54.000000 TerminalPrinter-2.3.0/printer/painter.py
+-rw-r--r--   0 hellflame   (501) staff       (20)        0 2021-05-18 14:35:43.000000 TerminalPrinter-2.3.0/printer/__init__.py
+-rw-r--r--   0 hellflame   (501) staff       (20)      753 2023-04-09 15:24:51.000000 TerminalPrinter-2.3.0/printer/utils.py
+-rw-r--r--   0 hellflame   (501) staff       (20)    17831 2021-05-18 14:35:43.000000 TerminalPrinter-2.3.0/printer/http.py
+-rw-r--r--   0 hellflame   (501) staff       (20)     3466 2023-04-09 15:33:02.000000 TerminalPrinter-2.3.0/printer/font_helper.py
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/
+-rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/PKG-INFO
+-rw-r--r--   0 hellflame   (501) staff       (20)      415 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/SOURCES.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)       51 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/entry_points.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        7 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/requires.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        8 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/top_level.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        1 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/TerminalPrinter.egg-info/dependency_links.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)       52 2021-05-18 14:35:42.000000 TerminalPrinter-2.3.0/MANIFEST.in
+-rw-r--r--   0 hellflame   (501) staff       (20)     8729 2023-04-12 13:30:43.000000 TerminalPrinter-2.3.0/README.md
+-rw-r--r--   0 hellflame   (501) staff       (20)      478 2021-05-18 14:35:42.000000 TerminalPrinter-2.3.0/CHANGES.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)     1186 2023-04-06 23:51:05.000000 TerminalPrinter-2.3.0/setup.py
+-rw-r--r--   0 hellflame   (501) staff       (20)       38 2023-04-12 13:32:10.000000 TerminalPrinter-2.3.0/setup.cfg
```

### Comparing `TerminalPrinter-2.2.1/PKG-INFO` & `TerminalPrinter-2.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: TerminalPrinter
-Version: 2.2.1
+Version: 2.3.0
 Summary: 终端图片、文字生成器
 Home-page: https://github.com/hellflame/terminal_printer
 Author: hellflame
 Author-email: hellflamedly@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `TerminalPrinter-2.2.1/printer/run.py` & `TerminalPrinter-2.3.0/printer/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,17 +54,19 @@
             if 30 <= int(s) <= 50:
                 return int(s)
             raise argparse.ArgumentTypeError("颜色值若为数字，应在30～50之间")
         else:
             return _COLOR_MAP.get(s, s)
 
     def usable_filter(s):
+        if len(s) == 1 and s in MESS_FILTERS:
+            return MESS_FILTERS.index(s)
         if s.isdigit() and 1 <= int(s) <= len(MESS_FILTERS) - 1:
             return int(s)
-        raise argparse.ArgumentTypeError("填充方式索引值应在1～{}之间".format(len(MESS_FILTERS) - 1))
+        raise argparse.ArgumentTypeError("填充方式为单个字符或索引值在1～{}之间".format(len(MESS_FILTERS) - 1))
 
     def usable_font(s):
         f, exist = choose_font(s)
         if not exist:
             raise argparse.ArgumentTypeError("字体路径不存在，请检查路径或使用数字")
         return f
 
@@ -83,15 +85,16 @@
     text.add_argument("-g", '--gray', action="store_true", help="图像转换为灰度图(若指定图)")
     text.add_argument("-F", '--font', metavar="path", type=usable_font, default='0', help="设置书写字体")
     text.add_argument("-r", '--reverse', action="store_true", help="反色(对彩色输出无效)")
 
     common = parse.add_argument_group("common")
     common.add_argument('-W', "--width", metavar="w", type=int, help="设置输出宽度，需要与高度一起设置")
     common.add_argument('-H', "--height", metavar="h", type=int, help="设置输出高度，需要与宽度一起设置")
-    common.add_argument("-f", '--filter', type=usable_filter, metavar="i", default=73, help="设置打印填充方式")
+    common.add_argument("-f", '--filter', type=usable_filter, metavar="i",
+                        default='i', help="设置打印填充方式，输入单个字符或索引值，默认为 i")
 
     # 可选的位置参数
     return parse.parse_args(), parse
 
 
 def run():
     command(*parser())
```

### Comparing `TerminalPrinter-2.2.1/printer/painter.py` & `TerminalPrinter-2.3.0/printer/painter.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.2.1/printer/utils.py` & `TerminalPrinter-2.3.0/printer/utils.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.2.1/printer/http.py` & `TerminalPrinter-2.3.0/printer/http.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.2.1/printer/font_helper.py` & `TerminalPrinter-2.3.0/printer/font_helper.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.2.1/TerminalPrinter.egg-info/PKG-INFO` & `TerminalPrinter-2.3.0/TerminalPrinter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: TerminalPrinter
-Version: 2.2.1
+Version: 2.3.0
 Summary: 终端图片、文字生成器
 Home-page: https://github.com/hellflame/terminal_printer
 Author: hellflame
 Author-email: hellflamedly@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `TerminalPrinter-2.2.1/README.md` & `TerminalPrinter-2.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,21 +33,19 @@
 ```bash
 $ terminalprint -h
 ```
 
 得到类似输出:
 
 ```bash
-usage: run.py [-h] [-i] [-v] [--debug] [-kr] [-t TEXT] [-c i] [-g] [-F path]
-              [-r] [-W w] [-H h] [-f i]
-              [picture]
+usage: run.py [-h] [-i] [-v] [--debug] [-kr] [-t TEXT] [-c i] [-g] [-F path] [-r] [-W w] [-H h] [-f i] [picture]
 
 Terminal Printer
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
 
 basics:
   -i, --init            初始化程序，下载字体
   -v, --version         输出版本信息
   --debug               输出调试信息
 
@@ -61,22 +59,22 @@
   -g, --gray            图像转换为灰度图(若指定图)
   -F path, --font path  设置书写字体
   -r, --reverse         反色(对彩色输出无效)
 
 common:
   -W w, --width w       设置输出宽度，需要与高度一起设置
   -H h, --height h      设置输出高度，需要与宽度一起设置
-  -f i, --filter i      设置打印填充方式
+  -f i, --filter i      设置打印填充方式，输入单个字符或索引值，默认为 i
 
 首次进行文字处理
 需要执行 terminalprint -i 初始化或指定字体
 更多帮助信息请参考: https://github.com/hellflame/terminal_printer
 ```
 
-> v2.1.0 新增 `--debug` 参数，可与其他命令一起使用，输出调试信息
+> `v2.1.0` 新增 `--debug` 参数，可与其他命令一起使用，输出调试信息
 
 #### ii. 版本信息
 
 ```bash
 $ terminalprint -v # terminalprint --version
 ```
 
@@ -108,14 +106,16 @@
 
 ```bash
 $ terminalprint -f [filt_char]
 ```
 
 可以设置的值范围1～223，代表ANSI可打印字符索引
 
+> `v2.3.0` 之后的版本支持输入单个字符直接作为填充字符
+
 (2) 渲染颜色
 
 > 这需要彩色终端支持
 
 ```bash
 $ terminalprint -c [color]
 ```
```

### Comparing `TerminalPrinter-2.2.1/setup.py` & `TerminalPrinter-2.3.0/setup.py`

 * *Files identical despite different names*

