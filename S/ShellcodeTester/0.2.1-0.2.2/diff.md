# Comparing `tmp/ShellcodeTester-0.2.1.tar.gz` & `tmp/ShellcodeTester-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShellcodeTester-0.2.1.tar", last modified: Mon Feb 13 06:03:17 2023, max compression
+gzip compressed data, was "ShellcodeTester-0.2.2.tar", last modified: Wed Apr 12 12:49:58 2023, max compression
```

## Comparing `ShellcodeTester-0.2.1.tar` & `ShellcodeTester-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:17.300345 ShellcodeTester-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-02-13 06:03:17.300345 ShellcodeTester-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:17.296345 ShellcodeTester-0.2.1/ShellcodeTester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-02-13 06:03:17.000000 ShellcodeTester-0.2.1/ShellcodeTester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-13 06:03:17.000000 ShellcodeTester-0.2.1/ShellcodeTester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 06:03:17.000000 ShellcodeTester-0.2.1/ShellcodeTester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-13 06:03:17.000000 ShellcodeTester-0.2.1/ShellcodeTester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 06:03:17.000000 ShellcodeTester-0.2.1/ShellcodeTester.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-13 06:03:17.000000 ShellcodeTester-0.2.1/ShellcodeTester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-13 06:03:17.000000 ShellcodeTester-0.2.1/ShellcodeTester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 06:03:17.300345 ShellcodeTester-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:17.296345 ShellcodeTester-0.2.1/shellcodetester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:17.296345 ShellcodeTester-0.2.1/shellcodetester/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/libs/asmfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/libs/assembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/libs/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/libs/disassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/libs/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/shellcodetester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:17.300345 ShellcodeTester-0.2.1/shellcodetester/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/util/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/util/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/shellcodetester/util/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:17.300345 ShellcodeTester-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 06:03:12.000000 ShellcodeTester-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.709102 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.709102 ShellcodeTester-0.2.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/bin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.709102 ShellcodeTester-0.2.2/nasmshell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/nasmshell/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/libs/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/nasmshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/shell_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/asmfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/disassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/inlineassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/shellcodetester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/shellcodetester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/tests/tests.py
```

### Comparing `ShellcodeTester-0.2.1/LICENSE` & `ShellcodeTester-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.1/PKG-INFO` & `ShellcodeTester-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.1
+Version: 0.2.2
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Operating System
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Shellcode Tester
 
 [![Build](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_publish.yml/badge.svg)](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_publish.yml)
 [![Build](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_test.yml)
@@ -47,17 +47,18 @@
 
 ## Main features
 
 * [x] Assembly ASM file (32 and 64 bits)
 * [x] Assembly ASM file to Windows, Linux and MacOS
 * [x] Check badchars
 * [x] Output to several formats
+* [x] NASM Shell
 * [x] Other amazing features...
 
-## Getting stats
+## Shellcode Tester - Getting stats
 
 ```bash
 shellcodetester -asm file.asm
 ```
 
 This command will assembly the ASM file and compile an ELF binary
 
@@ -80,43 +81,132 @@
  [+] Final size of RAW data: 160 bytes
 31c0b00431dbb301eb1259ba00000000b220cd8031c0b00131dbcd80e8e9ffffff4c616220303120636f6d706c657461646f20636f6d207375636573736f210a00
 
  [+] End time 2023-02-12 01:53:56
 
 ```
 
+## Nasm Shell - Getting stats
+
+### Assembling
+
+```bash
+$ nasm_shell
+┌─[NASM Shell]─[x86 linux]─[ASM → Hex]
+└──╼➤ push eax
+[+] Payload size: 1 bytes
+[+] Final size of RAW data: 2 bytes
+50
+
+[+] Disassembly
+   0:	50                   	push   eax
+
+┌─[NASM Shell]─[x86 linux]─[ASM → Hex]
+└──╼➤ push eax ; retn 4
+[+] Payload size: 4 bytes
+[+] Final size of RAW data: 8 bytes
+50c20400
+
+[+] Disassembly
+   0:	50                   	push   eax
+   1:	c2 04 00             	ret    0x4
+```
+
+### Disassembling
+
+```bash
+$ nasm_shell --mode dis
+┌─[NASM Shell]─[x86 linux]─[Hex → ASM]
+└──╼➤ 50ff501c
+[+] Payload size: 4 bytes
+[+] Final size of RAW data: 8 bytes
+50ff501c
+
+[+] Disassembly
+   0:	50                   	push   eax
+   1:	ff 50 1c             	call   DWORD PTR [eax+0x1c]
+```
+
+### 64 bits (x86-64)
+
+```bash
+$ nasm_shell --arch x86_64
+┌─[NASM Shell]─[x86_64 linux]─[ASM → Hex]
+└──╼➤ push rax
+[+] Payload size: 1 bytes
+[+] Final size of RAW data: 2 bytes
+50
+
+[+] Disassembly
+   0:	50                   	push   rax
+
+┌─[NASM Shell]─[x86_64 linux]─[ASM → Hex]
+└──╼➤ push rax ; push rbx
+[+] Payload size: 2 bytes
+[+] Final size of RAW data: 4 bytes
+5053
+
+[+] Disassembly
+   0:	50                   	push   rax
+   1:	53                   	push   rbx
+```
+
 ## Installation
 
 ```bash
 pip3 install --upgrade shellcodetester
 ```
 
 # Help
 
+## Shellcodetester
+
 ```bash
 $ shellcodetester -h
 
-ShellcodeTester v0.2.0 by Helvio Junior (M4v3r1ck)
+ShellcodeTester v0.2.2 by Helvio Junior (M4v3r1ck)
 ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 https://github.com/helviojunior/shellcodetester
 
 options:
   -h, --help                      show this help message and exit
 
 General Setting:
   -asm [ASM file name]            Assembly file to be assembled
   -o [output file]                Save output to disk (default: none)
 
 Custom Settings:
   --break-point                   Set software breakpoint (INT3) before shellcode (default: false)
   --bad-chars [bad char list]     List of bad chars to highlight (ex: \x00\x0a, default: \0x00)
+  --cave-size [size]              Code cave size (default: 1024)
   --fill-with-nop                 Fill entire page with NOP (default: false)
   --list                          List all supported output format
   -f [format], --format [format]  Output format (use --list formats to list)
   -v, --verbose                   Shows more options (-h -v). Prints commands and outputs. (default: quiet)
+
+```
+
+## Nasmshell
+
+```bash
+$ nasm_shell -h
+options:
+  -h, --help                      show this help message and exit
+
+General Setting:
+  --mode [mode]                   Operation mode. (default: assembly, permitted: assembly and disassembly)
+  --arch [architecture]           Architecture to assembly/disassembly. (default: x86, permitted: x86_64 and x86)
+  --platform [platform]           Platform. (permitted: linux, windows and darwin)
+
+Custom Settings:
+  --bad-chars [bad char list]     List of bad chars to highlight (ex: \x00\x0a, default: \0x00)
+  --list                          List all supported output format
+  -f [format], --format [format]  Output format (use --list formats to list)
+  -v, --verbose                   Shows more options (-h -v). Prints commands and outputs. (default: quiet)
+  -q, --quiet                     Quiet mode, not show banners. (default: false)
 ```
 
 # Windows Users
 
 Check specific instructions by Windows Users
 
 [Windows Instructions](WINDOWS.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ShellcodeTester-0.2.1/ShellcodeTester.egg-info/PKG-INFO` & `ShellcodeTester-0.2.2/ShellcodeTester.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.1
+Version: 0.2.2
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Operating System
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Shellcode Tester
 
 [![Build](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_publish.yml/badge.svg)](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_publish.yml)
 [![Build](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/helviojunior/shellcodetester/actions/workflows/build_and_test.yml)
@@ -47,17 +47,18 @@
 
 ## Main features
 
 * [x] Assembly ASM file (32 and 64 bits)
 * [x] Assembly ASM file to Windows, Linux and MacOS
 * [x] Check badchars
 * [x] Output to several formats
+* [x] NASM Shell
 * [x] Other amazing features...
 
-## Getting stats
+## Shellcode Tester - Getting stats
 
 ```bash
 shellcodetester -asm file.asm
 ```
 
 This command will assembly the ASM file and compile an ELF binary
 
@@ -80,43 +81,132 @@
  [+] Final size of RAW data: 160 bytes
 31c0b00431dbb301eb1259ba00000000b220cd8031c0b00131dbcd80e8e9ffffff4c616220303120636f6d706c657461646f20636f6d207375636573736f210a00
 
  [+] End time 2023-02-12 01:53:56
 
 ```
 
+## Nasm Shell - Getting stats
+
+### Assembling
+
+```bash
+$ nasm_shell
+┌─[NASM Shell]─[x86 linux]─[ASM → Hex]
+└──╼➤ push eax
+[+] Payload size: 1 bytes
+[+] Final size of RAW data: 2 bytes
+50
+
+[+] Disassembly
+   0:	50                   	push   eax
+
+┌─[NASM Shell]─[x86 linux]─[ASM → Hex]
+└──╼➤ push eax ; retn 4
+[+] Payload size: 4 bytes
+[+] Final size of RAW data: 8 bytes
+50c20400
+
+[+] Disassembly
+   0:	50                   	push   eax
+   1:	c2 04 00             	ret    0x4
+```
+
+### Disassembling
+
+```bash
+$ nasm_shell --mode dis
+┌─[NASM Shell]─[x86 linux]─[Hex → ASM]
+└──╼➤ 50ff501c
+[+] Payload size: 4 bytes
+[+] Final size of RAW data: 8 bytes
+50ff501c
+
+[+] Disassembly
+   0:	50                   	push   eax
+   1:	ff 50 1c             	call   DWORD PTR [eax+0x1c]
+```
+
+### 64 bits (x86-64)
+
+```bash
+$ nasm_shell --arch x86_64
+┌─[NASM Shell]─[x86_64 linux]─[ASM → Hex]
+└──╼➤ push rax
+[+] Payload size: 1 bytes
+[+] Final size of RAW data: 2 bytes
+50
+
+[+] Disassembly
+   0:	50                   	push   rax
+
+┌─[NASM Shell]─[x86_64 linux]─[ASM → Hex]
+└──╼➤ push rax ; push rbx
+[+] Payload size: 2 bytes
+[+] Final size of RAW data: 4 bytes
+5053
+
+[+] Disassembly
+   0:	50                   	push   rax
+   1:	53                   	push   rbx
+```
+
 ## Installation
 
 ```bash
 pip3 install --upgrade shellcodetester
 ```
 
 # Help
 
+## Shellcodetester
+
 ```bash
 $ shellcodetester -h
 
-ShellcodeTester v0.2.0 by Helvio Junior (M4v3r1ck)
+ShellcodeTester v0.2.2 by Helvio Junior (M4v3r1ck)
 ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 https://github.com/helviojunior/shellcodetester
 
 options:
   -h, --help                      show this help message and exit
 
 General Setting:
   -asm [ASM file name]            Assembly file to be assembled
   -o [output file]                Save output to disk (default: none)
 
 Custom Settings:
   --break-point                   Set software breakpoint (INT3) before shellcode (default: false)
   --bad-chars [bad char list]     List of bad chars to highlight (ex: \x00\x0a, default: \0x00)
+  --cave-size [size]              Code cave size (default: 1024)
   --fill-with-nop                 Fill entire page with NOP (default: false)
   --list                          List all supported output format
   -f [format], --format [format]  Output format (use --list formats to list)
   -v, --verbose                   Shows more options (-h -v). Prints commands and outputs. (default: quiet)
+
+```
+
+## Nasmshell
+
+```bash
+$ nasm_shell -h
+options:
+  -h, --help                      show this help message and exit
+
+General Setting:
+  --mode [mode]                   Operation mode. (default: assembly, permitted: assembly and disassembly)
+  --arch [architecture]           Architecture to assembly/disassembly. (default: x86, permitted: x86_64 and x86)
+  --platform [platform]           Platform. (permitted: linux, windows and darwin)
+
+Custom Settings:
+  --bad-chars [bad char list]     List of bad chars to highlight (ex: \x00\x0a, default: \0x00)
+  --list                          List all supported output format
+  -f [format], --format [format]  Output format (use --list formats to list)
+  -v, --verbose                   Shows more options (-h -v). Prints commands and outputs. (default: quiet)
+  -q, --quiet                     Quiet mode, not show banners. (default: false)
 ```
 
 # Windows Users
 
 Check specific instructions by Windows Users
 
 [Windows Instructions](WINDOWS.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/args.py` & `ShellcodeTester-0.2.2/shellcodetester/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: UTF-8 -*-
 
-from .util.color import Color
+from shell_libs.color import Color
 
-import argparse, sys, os
+import argparse, sys
 
 
 class Arguments(object):
     ''' Holds arguments used by the Shellcode Tester '''
 
     def __init__(self, custom_args=''):
         self.verbose = any(['-v' in word for word in sys.argv])
@@ -66,14 +66,22 @@
         custom.add_argument('--bad-chars',
                             action='store',
                             dest='bad_chars',
                             metavar='[bad char list]',
                             type=str,
                             help=Color.s('List of bad chars to highlight (ex: {G}\\x00\\x0a{W}, default: {G}\\0x00{W})'))
 
+        custom.add_argument('--cave-size',
+                            action='store',
+                            dest='cave_size',
+                            metavar='[size]',
+                            type=int,
+                            default=1024,
+                            help=Color.s('Code cave size (default: {G}1024{W})'))
+
         custom.add_argument('--fill-with-nop',
                             action='store_true',
                             default=False,
                             dest='fill',
                             help=Color.s('Fill entire page with NOP (default: {G}false{W})'))
 
         custom.add_argument('--list',
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/config.py` & `ShellcodeTester-0.2.2/shellcodetester/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/python3
 # -*- coding: UTF-8 -*-
 
-import os, subprocess, socket, re, errno, sys, time, json, signal, base64, hashlib, random
+import os, errno, sys
 from pathlib import Path
-from urllib.parse import urlparse
 
-from .args import Arguments
-from .libs.transform import Transform
-from .util.color import Color
-from .util.logger import Logger
-from .__meta__ import __version__, __title__, __author__, __description__, __url__
-from .util.tools import Tools
+from shell_libs.transform import Transform
+from shell_libs.color import Color
+from shell_libs.logger import Logger
+from shell_libs.__meta__ import __version__, __title__, __author__, __description__, __url__
 
 
 class Configuration(object):
-    ''' Stores configuration variables and functions for TKnowsMore. '''
+    ''' Stores configuration variables and functions for Shellcode Tester. '''
     version = '0.0.0'
     name = ""
 
     initialized = False # Flag indicating config has been initialized
     verbose = 0
     cmd_line = ''
     asm_file = ''
     out_file = ''
     pwd = ''
+    platform = ''
     transform_format = 0
     breakpoint = False
     fill = False
     bad_chars = bytearray([0x00])
+    cave_size = 200
 
     @staticmethod
     def initialize():
         '''
             Sets up default initial configuration values.
             Also sets config values based on command-line arguments.
         '''
@@ -53,14 +52,19 @@
         Configuration.load_from_arguments()
 
 
     @staticmethod
     def load_from_arguments():
         ''' Sets configuration values based on Argument.args object '''
         from .args import Arguments
+        import platform
+        p = platform.system().lower()
+        if p == 'darwin':
+            p = 'macos'
+        Configuration.platform = p
 
         config_check = 0
 
         list_formats = any(['--list' in word for word in sys.argv])
 
         if list_formats:
             Color.pl('{+} {W}Transform Formats')
@@ -93,14 +97,15 @@
 
         except Exception as x:
             Logger.pl('{!} {R}error: could not parse --bad-chars %s: %s {W}\r\n' % (args.bad_chars, x))
             sys.exit(1)
 
         Color.pl('{+} {W}Startup parameters')
         Logger.pl('     {C}command line:{O} %s{W}' % Configuration.cmd_line)
+        Logger.pl('     {C}platform:{O} %s{W}' % Configuration.platform)
 
         if Configuration.verbose > 0:
             Logger.setLevel(Configuration.verbose)
 
         Logger.pl('     {C}log level:{O} %s{W}' % (Logger.getLevelName(Logger.level)))
 
         if args.asm_file is None or args.asm_file.strip() == '':
@@ -110,23 +115,28 @@
             Configuration.mandatory()
 
         Configuration.asm_file = args.asm_file
 
         if args.out_file:
             Configuration.out_file = args.out_file
 
+        Configuration.cave_size = int(args.cave_size)
         Configuration.breakpoint = args.breakpoint
         Configuration.fill = args.fill
         Configuration.transform_format = Transform.parse_format(args.transform_format)
 
+        Logger.pl('     {C}code cave size:{O} %s{W}' % Configuration.cave_size)
         Logger.pl('     {C}transform format:{O} %s{W}' % (Transform.get_name(Configuration.transform_format)))
 
-        Logger.pl('     {C}bad chars:{O} %s{W}' % (', '.join([
+        if len(Configuration.bad_chars) > 0:
+            Logger.pl('     {C}bad chars:{O} %s{W}' % (', '.join([
                 f"0x{format(x, '02x')}" for x in Configuration.bad_chars
             ])))
+        else:
+            Logger.pl('     {C}bad chars:{O} Empty{W}')
 
         if not os.path.isfile(Configuration.asm_file):
             Color.pl('{!} {R}error: ASM file not found {O}%s{R}{W}\r\n' % Configuration.asm_file)
             sys.exit(1)
 
         try:
             with open(Configuration.asm_file, 'r') as f:
@@ -180,15 +190,15 @@
 {C}{D}%s{W}
     ''' % (str(__title__), Configuration.version, __author__, __description__, __url__)
 
 
     @staticmethod
     def dump():
         ''' (Colorful) string representation of the configuration '''
-        from .util.color import Color
+        from shell_libs.color import Color
 
         max_len = 20
         for key in Configuration.__dict__.keys():
             max_len = max(max_len, len(key))
 
         result  = Color.s('{W}%s  Value{W}\n' % 'Configuration Key'.ljust(max_len))
         result += Color.s('{W}%s------------------{W}\n' % ('-' * max_len))
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/libs/asmfile.py` & `ShellcodeTester-0.2.2/shell_libs/asmfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from random import shuffle
 
 from shellcodetester.config import Configuration
-from shellcodetester.util.logger import Logger
+from shell_libs.logger import Logger
 
 _x86Instruction = [
     {'asm': 'inc %eax', 'byte': b'\x40'},
     {'asm': 'inc %ecx', 'byte': b'\x41'},
     {'asm': 'inc %edx', 'byte': b'\x42'},
     {'asm': 'inc %ebx', 'byte': b'\x43'},
     {'asm': 'inc %esp', 'byte': b'\x44'},
@@ -54,36 +54,37 @@
         self.file_path = Path(filename)
         self.file_pattern = str(Path.joinpath(
             Path(Configuration.pwd),
             f'st_{self.file_path.name.replace(self.file_path.suffix, "")}').resolve())
 
         Logger.debug("Reading file {G}%s" % self.file_path.name)
 
-        with open(self.file_path.resolve(), 'r', errors="surrogateescape") as f:
-            line = f.readline()
-            while line:
-
-                check_txt = line.strip(' \t')
-                if len(check_txt) > 0:
-                    if check_txt[0] != "#" and check_txt[0] != ";":
-                        if '[bits 64]' in line.lower():
-                            self.arch = 'x86_64'
-                            break
-
-                        elif '[bits 32]' in line.lower():
-                            self.arch = 'x86'
-                            break
-
-                try:
-                    line = f.readline()
-                except:
-                    pass
+        if self.file_path.exists():
+            with open(self.file_path.resolve(), 'r', errors="surrogateescape") as f:
+                line = f.readline()
+                while line:
+
+                    check_txt = line.strip(' \t')
+                    if len(check_txt) > 0:
+                        if check_txt[0] != "#" and check_txt[0] != ";":
+                            if '[bits 64]' in line.lower():
+                                self.arch = 'x86_64'
+                                break
+
+                            elif '[bits 32]' in line.lower():
+                                self.arch = 'x86'
+                                break
+
+                    try:
+                        line = f.readline()
+                    except:
+                        pass
 
         if self.arch == 'unsupported':
-            raise Exception('Unknown or unsupported ASM platform')
+            raise Exception('Unknown or unsupported ASM architecture')
 
         lst = _x86Instruction
         if self.arch == 'x86_64':
             lst = _x86_64Instruction
         lst_idx = list(range(len(lst)))
         shuffle(lst_idx)
         lst_idx = lst_idx[0:7]
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/libs/assembler.py` & `ShellcodeTester-0.2.2/shell_libs/assembler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 
-from shellcodetester.libs.asmfile import AsmFile
-from shellcodetester.libs.transform import Transform
-from shellcodetester.util.logger import Logger
-from shellcodetester.util.process import Process
-from shellcodetester.util.tools import Tools
+from shell_libs.asmfile import AsmFile
+from shell_libs.transform import Transform
+from shell_libs.logger import Logger
+from shell_libs.process import Process
 
 
 class Assembler(AsmFile):
     o_file = ''
     assembled_data = None
 
     def __init__(self, filename):
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/libs/compiler.py` & `ShellcodeTester-0.2.2/shell_libs/compiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import errno
-import sys
 from pathlib import Path
 
 from shellcodetester.config import Configuration
-from shellcodetester.libs.asmfile import AsmFile
-from shellcodetester.libs.transform import Transform
-from shellcodetester.util.logger import Logger
-from shellcodetester.util.process import Process
-from shellcodetester.util.tools import Tools
+from shell_libs.asmfile import AsmFile
+from shell_libs.logger import Logger
+from shell_libs.process import Process
+from shell_libs.tools import Tools
 
 _extensions = {
     'windows': '.exe',
     'linux': '',
     'darwin': '',
 }
 
@@ -48,25 +46,42 @@
             if self.c_file.is_file() and self.c_file.exists():
                 self.c_file.unlink(missing_ok=True)
 
             with open(self.c_file, 'w', encoding="utf-8") as f:
                 f.write('#include<stdio.h>\n')
                 f.write('#include<string.h>\n')
                 f.write('\n')
-                f.write('void shell();\n')
+                f.write('char ZEROARRAY[1024] = {0};\n')
                 f.write('\n')
-                f.write('void main() {\n')
+                f.write('void shell(int*, int*);\n')
+                f.write('void code_cave();\n')
+                f.write('\n')
+                f.write('int main() {\n')
                 f.write('\n')
                 f.write(f'    int size = {len(self.assembled_data)};\n')
-                f.write('    printf("Shellcode Length:  %d\\n", size);\n')
+                f.write('    size_t size2 = sizeof(ZEROARRAY);\n')
+                f.write('    printf("Shellcode Length: %d\\n", size);\n')
+
+                if self.arch == 'x86':
+                    f.write('    printf("edi = %p => code cave\\n", &code_cave);\n')
+                    f.write('    printf("esi = %p => writable memory (%zd bytes)\\n", &ZEROARRAY, size2);\n')
+                elif self.arch == 'x86_64':
+                    f.write('    printf("rdi = %p => code cave\\n", &code_cave);\n')
+                    f.write('    printf("rsi = %p => writable memory (%zd bytes)\\n", &ZEROARRAY, size2);\n')
+
                 f.write('\n')
-                f.write('    shell();\n')
+                f.write('    shell(&code_cave, &ZEROARRAY);\n')
+                f.write('    return 0;\n')
                 f.write('}\n')
                 f.write('\n')
-                f.write('void shell() {\n')
+                f.write('void shell(int *code_cave, int *data) {\n')
+
+                if self.arch == 'x86':
+                    f.write('    asm("mov 0x8(%esp),%edi");\n')
+                    f.write('    asm("mov 0xc(%esp),%esi");\n')
 
                 if Configuration.breakpoint:
                     f.write('    asm("INT3"); // INT3 -> Breakpoint\n')
 
                 f.write('    asm("NOP");\n')
 
                 pattern = bytearray()
@@ -83,14 +98,22 @@
                     f.write('    asm("%s");\n' % s['asm'])
 
                 if Configuration.fill:
                     for n in range(4096 - len(self.assembled_data)):
                         f.write('    asm("NOP");\n')
 
                 f.write('}\n')
+                f.write('\n')
+
+                f.write('void code_cave() {\n')
+
+                for n in range(Configuration.cave_size):
+                    f.write('    asm("NOP");\n')
+
+                f.write('}\n')
                 pass
 
         except IOError as x:
             if x.errno == errno.EACCES:
                 Logger.pl('{!} {R}error: could not open output file to write {O}permission denied{R}{W}\r\n')
                 raise x
             elif x.errno == errno.EISDIR:
@@ -103,23 +126,26 @@
         Logger.pl('{+} {W}Compiling {G}%s{W} binary to {O}%s{W}' % (
             self.arch, self.bin_file.resolve()))
 
         if self.bin_file.is_file() and self.bin_file.exists():
             self.bin_file.unlink(missing_ok=True)
 
         gcc_flags = '-fno-stack-protector'
-        if not Tools.is_platform_windows():
-            gcc_flags = ' -z execstack'
+        #if not Tools.is_platform_windows():
+        #    gcc_flags = ' -z execstack'
         if self.arch == 'x86':
             gcc_flags += ' -m32'
 
         # gcc source.c -o executable_file $gcc_flags -fno-stack-protector -z execstack
         (code, out, err) = Process.call(f"gcc \"{self.c_file.resolve()}\" -o \"{self.bin_file.resolve()}\" {gcc_flags}")
         if code != 0:
             Logger.pl('{!} {R}Error assembling {G}%s{R}:{O} \n{W}%s{W}' % (self.file_path.name, err))
+            if 'stdio.h' in err and 'file not found' in err and Configuration.platform == 'macos':
+                Logger.pl(('{R}NOTE: {GR}Try to run the following command before execute the shellcode tester: '
+                           '{G}export SDKROOT=$(xcrun --sdk macosx --show-sdk-path){W}\n'))
             return False
 
         stat = self.bin_file.stat()
         if stat.st_size == 0:
             Logger.pl('{!} {R}Error compiling {G}%s{R}:{O} %s{W}' % (self.file_path.name, 'Output file is empty'))
             return False
 
@@ -128,25 +154,23 @@
         if not self.replace_onfile(self.bin_file, pattern, self.assembled_data):
             Logger.pl('{!} {R}Error putting the shellcode inside of executable file {G}%s{W}' % self.bin_file.name)
             return False
 
         if Tools.is_platform_windows():
             if Configuration.breakpoint:
                 Logger.pl(
-                    '\n{+} {W}To debug your shellcode open the following application in your debugger: \n     {O}%s{W}\n' % self.bin_file.resolve())
+                    '\n{+} {W}To debug your shellcode open the following application in your debugger: \n    {O}%s{W}\n' % self.bin_file.resolve())
                 return True
-
-            Logger.pl('\n{+} {W}To run your shellcode execute the application: \n     {O}%s{W}\n' % self.bin_file.resolve())
         else:
             if Configuration.breakpoint:
                 Logger.pl(
-                    '\n{+} {W}To debug your shellcode execute the command: \n     {O}gdb -q %s{W}\n' % self.bin_file.resolve())
+                    '\n{+} {W}To debug your shellcode execute the command: \n    {O}gdb -q %s{W}\n' % self.bin_file.resolve())
                 return True
 
-            Logger.pl('\n{+} {W}To execute your shellcode execute the command: \n     {O}%s{W}\n' % self.bin_file.resolve())
+        Logger.pl('\n{+} {W}To run your shellcode execute the command: \n    {O}%s{W}\n' % self.bin_file.resolve())
         return True
 
     def replace_onfile(self, filename: [str, Path], pattern: [bytearray, bytes], replace_to: [bytearray, bytes]) -> bool:
         file = Path(filename)
         stat = self.bin_file.stat()
         if stat.st_size == 0:
             Logger.pl('{!} {R}Error putting the shellcode at {G}%s{R}:{O} %s{W}' % (file.name, 'Executable file is empty'))
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/libs/disassembler.py` & `ShellcodeTester-0.2.2/shell_libs/disassembler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,68 @@
 import re
 from pathlib import Path
 
-from shellcodetester.libs.asmfile import AsmFile
-from shellcodetester.util.logger import Logger
-from shellcodetester.util.process import Process
+from shell_libs.asmfile import AsmFile
+from shell_libs.logger import Logger
+from shell_libs.process import Process
+import tempfile, os
 
 
 class Disassembler(AsmFile):
     assembled_data = None
+    platform = None
+
+    def __init__(self, filename: str = '',
+                 assembled_data: [bytearray, bytes] = bytearray(),
+                 platform: str = '',
+                 arch: str = 'unsupported'):
+
+        write_data = False
+        if isinstance(filename, Path):
+            filename = str(Path(filename).resolve())
+
+        if filename is None or filename.strip() == '':
+            write_data = True
+            filename = os.path.join(tempfile.mkdtemp(), 'nasmshell.o')
+            if os.path.isfile(filename):
+                os.unlink(filename)
+
+        self.arch = arch
+
+        if platform is None or platform.strip() == '':
+            import platform as p
+            self.platform = p.system().lower()
+        else:
+            self.platform = platform
 
-    def __init__(self, filename: str, assembled_data: bytearray):
         super().__init__(filename)
         self.assembled_data = assembled_data
         self.o_file = Path(f"{self.file_pattern}.o")
-        if self.arch == 'x86_64':
-            self.bin_file = Path(f"{self.file_pattern}.elf64")
-        else:
-            self.bin_file = Path(f"{self.file_pattern}.elf32")
 
-    def dump(self, bad_chars: [bytearray, bytes] = bytearray()):
-        Logger.pl('{+} {W}Disassembly of {G}%s{W}' % self.o_file.name)
-        cmd = f"objdump -D -Mintel,i386 -b binary -m i386 \"{self.o_file.resolve()}\""
-        if self.arch == 'x86_64':
-            cmd = f"objdump -D -Mintel,x86-64 -b binary -m i386 \"{self.o_file.resolve()}\""
+        if write_data:
+            with open(self.o_file, 'wb') as f:
+                f.write(bytearray(assembled_data))
+
+    def dump(self, bad_chars: [bytearray, bytes] = bytearray(), quiet: bool = False):
+        if not quiet:
+            Logger.pl('{+} {W}Disassembly of {G}%s{W}' % self.o_file.name)
+
+        if self.platform == "darwin":
+            cmd = f"objdump -D -Mintel,i386 \"{self.o_file.resolve()}\""
+            if self.arch == 'x86_64':
+                cmd = f"objdump -D -Mintel,x86-64 \"{self.o_file.resolve()}\""
+        else:
+            cmd = f"objdump -D -Mintel,i386 -b binary -m i386 \"{self.o_file.resolve()}\""
+            if self.arch == 'x86_64':
+                cmd = f"objdump -D -Mintel,x86-64 -b binary -m i386 \"{self.o_file.resolve()}\""
 
         (code, out, err) = Process.call(cmd)
         if code != 0:
+            if err is not None and out is not None and len(err) == 0 and len(out) > 0:
+                err = out
             Logger.pl('{!} {R}Error disassembling {G}%s{R}: %s{W}' % (self.file_path.name, err))
             return False
 
         out.replace('\r', '')
 
         idx = out.find('00000000 <.data>:')
         if idx > 0:
@@ -39,15 +72,16 @@
         if '<.data>:' in lines[0]:
             lines = lines[1:]
 
         bc = [format(x, '02x') for x in bad_chars] + [format(x, '02x').upper() for x in bad_chars]
         if 0x00 in bad_chars:
             bc += ['0x0 ', '0x0\n']
 
-        Logger.pl(' ')
+        if not quiet:
+            Logger.pl(' ')
         for l in lines:
             search = re.search('(^[a-fA-F0-9 ]{1,20}:)(.*)', l, re.IGNORECASE)
             if search is not None:
                 l_data = search.group(2)
                 for b in bc:
                     l_data = (l_data + '\n').replace(b, '{R}%s{W}' % b).replace('\n', '')
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/libs/transform.py` & `ShellcodeTester-0.2.2/shell_libs/transform.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.1/shellcodetester/password.py` & `ShellcodeTester-0.2.2/shellcodetester/password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import hashlib
 import codecs
 import unicodedata
 
-from shellcodetester.util.color import Color
-from shellcodetester.util.tools import Tools
+from shell_libs.color import Color
 from math import log
 from Levenshtein import ratio
 
 LEETS = {"a": "aA@49\u00e1\u00c1\u00e0\u00c0\u00c2\u00c3\u00c4\u00c5\u00e2\u00e3\u00e4\u00e5", "b": "bB8", "c": "cC\u00e7\u00c7", "d": "dD", "e": "eE32\u00c8\u00c9\u00ca\u00cb\u00e8\u00e9\u00ea\u00eb", "f": "fF", "g": "gG96", "h": "hH#", "i": "iI!1\u00cc\u00cd\u00ce\u00cf\u00ec\u00ed\u00ee\u00ef", "j": "jJ", "k": "kK", "l": "lL!1", "m": "mM", "n": "nN\u00f1\u00d1", "o": "oO04\u00d2\u00d3\u00d4\u00d5\u00d6\u00f2\u00f3\u00f4\u00f5\u00f6", "p": "pP", "q": "qQ", "r": "rR", "s": "sS5$", "t": "tT7+", "u": "uU\u00d9\u00da\u00db\u00dc\u00f9\u00fa\u00fb\u00fc", "v": "vV", "w": "wW", "x": "xX", "y": "yY\u00dd\u00fd", "z": "zZ2", "0": "0", "1": "1", "2": "2", "3": "3", "4": "4", "5": "5", "6": "6", "7": "7", "8": "8", "9": "9"}
 
 class Password(object):
     weak_bits = 30
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/util/color.py` & `ShellcodeTester-0.2.2/shell_libs/color.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,26 @@
         'W' : '\033[0m',  # white (normal)
         'R' : '\033[31m', # red
         'G' : '\033[32m', # green
         'O' : '\033[33m', # orange
         'B' : '\033[34m', # blue
         'P' : '\033[35m', # purple
         'C' : '\033[36m', # cyan
-        'GR': '\033[37m', # gray
+        'GR': '\033[38;5;247m', # gray
         'D' : '\033[2m'   # dims current color. {W} resets.
     }
 
     # Helper string replacements
     replacements = {
-        '{+}': ' {W}{D}[{W}{G}+{W}{D}]{W}',
-        '{!}': ' {O}[{R}!{O}]{W}',
-        '{?}': ' {W}{D}[{W}{C}?{W}{D}]{W}',
-        '{*}': ' {W}{D}[{W}{B}*{W}{D}]{W}',
+        '{+}': '{W}{D}[{W}{G}+{W}{D}]{W}',
+        '{!}': '{O}[{R}!{O}]{W}',
+        '{?}': '{W}{D}[{W}{C}?{W}{D}]{W}',
+        '{*}': '{W}{D}[{W}{B}*{W}{D}]{W}',
     }
 
-
-
     last_sameline_length = 0
 
     @staticmethod
     def p(text):
         '''
         Prints text using colored format on same line.
         Example:
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/util/logger.py` & `ShellcodeTester-0.2.2/shell_libs/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/python3
 # -*- coding: UTF-8 -*-
-import sys
-from ..util.color import Color
+from shell_libs.color import Color
 
 DEFAULT = 0
 INFO = 1
 DEBUG = 2
 
 _levelToName = {
     INFO: 'INFO',
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/util/process.py` & `ShellcodeTester-0.2.2/shell_libs/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
+import platform
 import tempfile
 import time
 import signal
 import os
+from pathlib import Path
 
 from subprocess import Popen, PIPE
 
-from shellcodetester.util.logger import Logger
-from ..util.color import Color
-from ..config import Configuration
+from shell_libs.logger import Logger
+from shell_libs.color import Color
+from shellcodetester.config import Configuration
 
 
 class Process(object):
     ''' Represents a running/ran process '''
 
     @staticmethod
     def devnull():
@@ -36,17 +38,20 @@
                 Logger.debug("Executing (Shell): {G}%s" % command)
 
         # it cause hang on windows
         #pid = Popen(command, cwd=cwd, stdout=PIPE, stderr=PIPE, shell=shell)
         #retcode = pid.wait()
         #(stdout, stderr) = pid.communicate()
 
+        my_env = os.environ.copy()
+        my_env["PATH"] = Process.get_path()
+
         with tempfile.NamedTemporaryFile(mode="w+") as tmp_out, tempfile.NamedTemporaryFile(mode="w+") as tmp_err:
 
-            pid = Popen(command, cwd=cwd, stdout=tmp_out, stderr=tmp_err, shell=shell)
+            pid = Popen(command, env=my_env, cwd=cwd, stdout=tmp_out, stderr=tmp_err, shell=shell)
             retcode = pid.wait()
 
             # Cursor is after the last write call, reset to read output
             tmp_out.seek(0)
             tmp_err.seek(0)
             stdout = tmp_out.read()
             stderr = tmp_err.read()
@@ -58,27 +63,38 @@
             Color.pe("{P} [stdout] %s{W}" % '\n [stdout] '.join(stdout.strip().split('\n')))
         if Configuration.verbose > 1 and stderr is not None and stderr.strip() != '':
             Color.pe("{P} [stderr] %s{W}" % '\n [stderr] '.join(stderr.strip().split('\n')))
 
         return (retcode, stdout, stderr)
 
     @staticmethod
+    def get_path():
+        p = platform.system().lower()
+        if p == 'darwin':
+            p = 'macosx'
+
+        bin_path = Path(os.path.dirname(__file__) + f'../bin/{p}')
+        my_env = os.environ.copy()
+        return f"{bin_path}:" + my_env["PATH"]
+
+
+    @staticmethod
     def exists(program):
         ''' Checks if program is installed on this system '''
         #p = Process(['which', program])
         #stdout = p.stdout().strip()
         #stderr = p.stderr().strip()
 
         #if stdout == '' and stderr == '':
         #    return False
 
         #return True
 
         from shutil import which
-        return which(program) is not None
+        return which(program, path=Process.get_path()) is not None
 
 
     def __init__(self, command, devnull=False, stdout=PIPE, stderr=PIPE, cwd=None, bufsize=0):
         ''' Starts executing command '''
 
         if type(command) is str:
             # Commands have to be a list
```

### Comparing `ShellcodeTester-0.2.1/shellcodetester/util/tools.py` & `ShellcodeTester-0.2.2/shell_libs/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: UTF-8 -*-
 import os
 import string, random, sys, re
 import unicodedata
-from tabulate import _table_formats, tabulate
+from tabulate import tabulate
 
-from shellcodetester.util.color import Color
+from shell_libs.color import Color
 
 
 class Tools:
 
     def __init__(self):
         pass
```

