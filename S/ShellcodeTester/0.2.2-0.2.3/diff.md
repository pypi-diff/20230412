# Comparing `tmp/ShellcodeTester-0.2.2.tar.gz` & `tmp/ShellcodeTester-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShellcodeTester-0.2.2.tar", last modified: Wed Apr 12 12:49:58 2023, max compression
+gzip compressed data, was "ShellcodeTester-0.2.3.tar", last modified: Wed Apr 12 14:30:46 2023, max compression
```

## Comparing `ShellcodeTester-0.2.2.tar` & `ShellcodeTester-0.2.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.709102 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 12:49:58.000000 ShellcodeTester-0.2.2/ShellcodeTester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.709102 ShellcodeTester-0.2.2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/bin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.709102 ShellcodeTester-0.2.2/nasmshell/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/nasmshell/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/libs/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/nasmshell/nasmshell.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/shell_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/asmfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/assembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/disassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/inlineassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shell_libs/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/shellcodetester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/shellcodetester/shellcodetester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:58.713102 ShellcodeTester-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 12:49:54.000000 ShellcodeTester-0.2.2/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.082898 ShellcodeTester-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-12 14:30:46.082898 ShellcodeTester-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.070898 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.074899 ShellcodeTester-0.2.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/bin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.074899 ShellcodeTester-0.2.3/nasmshell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.074899 ShellcodeTester-0.2.3/nasmshell/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/libs/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/nasmshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:30:46.082898 ShellcodeTester-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.078899 ShellcodeTester-0.2.3/shell_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/asmfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/disassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/inlineassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.078899 ShellcodeTester-0.2.3/shellcodetester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/shellcodetester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.078899 ShellcodeTester-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/tests/tests.py
```

### Comparing `ShellcodeTester-0.2.2/LICENSE` & `ShellcodeTester-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/PKG-INFO` & `ShellcodeTester-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.2
+Version: 0.2.3
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
@@ -159,28 +159,29 @@
 # Help
 
 ## Shellcodetester
 
 ```bash
 $ shellcodetester -h
 
-ShellcodeTester v0.2.2 by Helvio Junior (M4v3r1ck)
+ShellcodeTester v0.X.X by Helvio Junior (M4v3r1ck)
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
+  --remove                        Remove bad chars from final binary executable (EXE, ELF and Mach-O). (default: false)
   --cave-size [size]              Code cave size (default: 1024)
   --fill-with-nop                 Fill entire page with NOP (default: false)
   --list                          List all supported output format
   -f [format], --format [format]  Output format (use --list formats to list)
   -v, --verbose                   Shows more options (-h -v). Prints commands and outputs. (default: quiet)
 
 ```
```

### Comparing `ShellcodeTester-0.2.2/README.md` & `ShellcodeTester-0.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -124,28 +124,29 @@
 # Help
 
 ## Shellcodetester
 
 ```bash
 $ shellcodetester -h
 
-ShellcodeTester v0.2.2 by Helvio Junior (M4v3r1ck)
+ShellcodeTester v0.X.X by Helvio Junior (M4v3r1ck)
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
+  --remove                        Remove bad chars from final binary executable (EXE, ELF and Mach-O). (default: false)
   --cave-size [size]              Code cave size (default: 1024)
   --fill-with-nop                 Fill entire page with NOP (default: false)
   --list                          List all supported output format
   -f [format], --format [format]  Output format (use --list formats to list)
   -v, --verbose                   Shows more options (-h -v). Prints commands and outputs. (default: quiet)
 
 ```
```

### Comparing `ShellcodeTester-0.2.2/ShellcodeTester.egg-info/PKG-INFO` & `ShellcodeTester-0.2.3/ShellcodeTester.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.2
+Version: 0.2.3
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
@@ -159,28 +159,29 @@
 # Help
 
 ## Shellcodetester
 
 ```bash
 $ shellcodetester -h
 
-ShellcodeTester v0.2.2 by Helvio Junior (M4v3r1ck)
+ShellcodeTester v0.X.X by Helvio Junior (M4v3r1ck)
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
+  --remove                        Remove bad chars from final binary executable (EXE, ELF and Mach-O). (default: false)
   --cave-size [size]              Code cave size (default: 1024)
   --fill-with-nop                 Fill entire page with NOP (default: false)
   --list                          List all supported output format
   -f [format], --format [format]  Output format (use --list formats to list)
   -v, --verbose                   Shows more options (-h -v). Prints commands and outputs. (default: quiet)
 
 ```
```

### Comparing `ShellcodeTester-0.2.2/ShellcodeTester.egg-info/SOURCES.txt` & `ShellcodeTester-0.2.3/ShellcodeTester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/nasmshell/args.py` & `ShellcodeTester-0.2.3/nasmshell/args.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/nasmshell/config.py` & `ShellcodeTester-0.2.3/nasmshell/config.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/nasmshell/libs/cmd.py` & `ShellcodeTester-0.2.3/nasmshell/libs/cmd.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/nasmshell/nasmshell.py` & `ShellcodeTester-0.2.3/nasmshell/nasmshell.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/setup.py` & `ShellcodeTester-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shell_libs/asmfile.py` & `ShellcodeTester-0.2.3/shell_libs/asmfile.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shell_libs/assembler.py` & `ShellcodeTester-0.2.3/shell_libs/assembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shell_libs/color.py` & `ShellcodeTester-0.2.3/shell_libs/color.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shell_libs/compiler.py` & `ShellcodeTester-0.2.3/shell_libs/compiler.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,27 @@
 }
 
 
 class Compiler(AsmFile):
     c_file = ''
     bin_file = ''
     assembled_data = None
+    bad_chars = None
+    remove_bad_chars = False
 
-    def __init__(self, filename: str, assembled_data: bytearray):
+    def __init__(self, filename: str,
+                 assembled_data: bytearray,
+                 bad_chars: [bytearray, bytes] = bytearray(),
+                 remove_bad_chars: bool = False):
         super().__init__(filename)
         self.assembled_data = assembled_data
         self.c_file = Path(f"{self.file_pattern}.c")
         self.bin_file = Path(f"{self.get_name()}")
+        self.bad_chars = bytearray([b for b in bad_chars])
+        self.remove_bad_chars = remove_bad_chars
 
     def get_name(self) -> str:
         import platform
         p = platform.system().lower()
         e = _extensions.get(p, "")
         return f"{self.file_pattern}-{self.arch}{e}"
 
@@ -147,15 +154,15 @@
         stat = self.bin_file.stat()
         if stat.st_size == 0:
             Logger.pl('{!} {R}Error compiling {G}%s{R}:{O} %s{W}' % (self.file_path.name, 'Output file is empty'))
             return False
 
         Logger.debug("File compiled with {G}%s bytes" % stat.st_size)
 
-        if not self.replace_onfile(self.bin_file, pattern, self.assembled_data):
+        if not self.replace_on_file(self.bin_file, pattern, self.assembled_data, self.bad_chars, self.remove_bad_chars):
             Logger.pl('{!} {R}Error putting the shellcode inside of executable file {G}%s{W}' % self.bin_file.name)
             return False
 
         if Tools.is_platform_windows():
             if Configuration.breakpoint:
                 Logger.pl(
                     '\n{+} {W}To debug your shellcode open the following application in your debugger: \n    {O}%s{W}\n' % self.bin_file.resolve())
@@ -165,15 +172,19 @@
                 Logger.pl(
                     '\n{+} {W}To debug your shellcode execute the command: \n    {O}gdb -q %s{W}\n' % self.bin_file.resolve())
                 return True
 
         Logger.pl('\n{+} {W}To run your shellcode execute the command: \n    {O}%s{W}\n' % self.bin_file.resolve())
         return True
 
-    def replace_onfile(self, filename: [str, Path], pattern: [bytearray, bytes], replace_to: [bytearray, bytes]) -> bool:
+    def replace_on_file(self, filename: [str, Path],
+                        pattern: [bytearray, bytes],
+                        replace_to: [bytearray, bytes],
+                        bad_chars: [bytearray, bytes] = bytearray(),
+                        remove_bad_chars: bool = False) -> bool:
         file = Path(filename)
         stat = self.bin_file.stat()
         if stat.st_size == 0:
             Logger.pl('{!} {R}Error putting the shellcode at {G}%s{R}:{O} %s{W}' % (file.name, 'Executable file is empty'))
             return False
 
         with open(file.resolve(), 'rb') as f:
@@ -185,17 +196,20 @@
             return False
 
         if idx + len(replace_to) > len(bin_data):
             Logger.pl(
                 '{!} {R}Error putting the shellcode at {G}%s{R}:{O} %s{W}' % (file.name, 'replace_to data is greater than binary file'))
             return False
 
-        fill_data = bytearray(replace_to)
+        fill_data = bytearray([
+            b for b in replace_to
+            if not remove_bad_chars or b not in bad_chars
+        ])
 
-        for n in range(len(pattern) - len(replace_to)):
+        for n in range(len(pattern) - len(fill_data)):
             fill_data.append(0x90)
 
         new_data = bin_data[0:idx] + fill_data + bin_data[idx + len(pattern):]
 
         with open(file.resolve(), 'wb') as f:
             f.write(new_data)
```

### Comparing `ShellcodeTester-0.2.2/shell_libs/disassembler.py` & `ShellcodeTester-0.2.3/shell_libs/disassembler.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         if write_data:
             with open(self.o_file, 'wb') as f:
                 f.write(bytearray(assembled_data))
 
     def dump(self, bad_chars: [bytearray, bytes] = bytearray(), quiet: bool = False):
         if not quiet:
-            Logger.pl('{+} {W}Disassembly of {G}%s{W}' % self.o_file.name)
+            Logger.pl('{+} {W}Disassembly{W}')
 
         if self.platform == "darwin":
             cmd = f"objdump -D -Mintel,i386 \"{self.o_file.resolve()}\""
             if self.arch == 'x86_64':
                 cmd = f"objdump -D -Mintel,x86-64 \"{self.o_file.resolve()}\""
         else:
             cmd = f"objdump -D -Mintel,i386 -b binary -m i386 \"{self.o_file.resolve()}\""
```

### Comparing `ShellcodeTester-0.2.2/shell_libs/inlineassembler.py` & `ShellcodeTester-0.2.3/shell_libs/inlineassembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shell_libs/logger.py` & `ShellcodeTester-0.2.3/shell_libs/logger.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shell_libs/process.py` & `ShellcodeTester-0.2.3/shell_libs/process.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shell_libs/runner.py` & `ShellcodeTester-0.2.3/shell_libs/runner.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shell_libs/tools.py` & `ShellcodeTester-0.2.3/shell_libs/tools.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shell_libs/transform.py` & `ShellcodeTester-0.2.3/shell_libs/transform.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shellcodetester/args.py` & `ShellcodeTester-0.2.3/shellcodetester/args.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,23 +57,29 @@
                           help=Color.s('Save output to disk (default: {G}none{W})'))
 
     def _add_custom_args(self, custom):
         custom.add_argument('--break-point',
                             action='store_true',
                             default=False,
                             dest='breakpoint',
-                            help=Color.s('Set software breakpoint ({C}INT3{W}) before shellcode (default: {G}false{W})'))
+                            help=Color.s('Set software breakpoint ({G}INT3{W}) before shellcode (default: {G}false{W})'))
 
         custom.add_argument('--bad-chars',
                             action='store',
                             dest='bad_chars',
                             metavar='[bad char list]',
                             type=str,
                             help=Color.s('List of bad chars to highlight (ex: {G}\\x00\\x0a{W}, default: {G}\\0x00{W})'))
 
+        custom.add_argument('--remove',
+                            action='store_true',
+                            default=False,
+                            dest='remove',
+                            help=Color.s('Remove bad chars from final binary executable (EXE, ELF and Mach-O). (default: {G}false{W})'))
+
         custom.add_argument('--cave-size',
                             action='store',
                             dest='cave_size',
                             metavar='[size]',
                             type=int,
                             default=1024,
                             help=Color.s('Code cave size (default: {G}1024{W})'))
@@ -101,10 +107,10 @@
 
         custom.add_argument('-v',
                             '--verbose',
                             action='count',
                             default=0,
                             dest='verbose',
                             help=Color.s(
-                                'Shows more options ({C}-h -v{W}). Prints commands and outputs. (default: {G}quiet{W})'))
+                                'Shows more options ({G}-h -v{W}). Prints commands and outputs. (default: {G}quiet{W})'))
```

### Comparing `ShellcodeTester-0.2.2/shellcodetester/config.py` & `ShellcodeTester-0.2.3/shellcodetester/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     initialized = False # Flag indicating config has been initialized
     verbose = 0
     cmd_line = ''
     asm_file = ''
     out_file = ''
     pwd = ''
     platform = ''
+    remove = False
     transform_format = 0
     breakpoint = False
     fill = False
     bad_chars = bytearray([0x00])
     cave_size = 200
 
     @staticmethod
@@ -117,26 +118,30 @@
         Configuration.asm_file = args.asm_file
 
         if args.out_file:
             Configuration.out_file = args.out_file
 
         Configuration.cave_size = int(args.cave_size)
         Configuration.breakpoint = args.breakpoint
+        Configuration.remove = args.remove
         Configuration.fill = args.fill
         Configuration.transform_format = Transform.parse_format(args.transform_format)
 
         Logger.pl('     {C}code cave size:{O} %s{W}' % Configuration.cave_size)
         Logger.pl('     {C}transform format:{O} %s{W}' % (Transform.get_name(Configuration.transform_format)))
 
         if len(Configuration.bad_chars) > 0:
             Logger.pl('     {C}bad chars:{O} %s{W}' % (', '.join([
                 f"0x{format(x, '02x')}" for x in Configuration.bad_chars
             ])))
         else:
             Logger.pl('     {C}bad chars:{O} Empty{W}')
+            Configuration.remove = False
+
+        Logger.pl('     {C}remove bad chars:{O} %s{W}' % Configuration.remove)
 
         if not os.path.isfile(Configuration.asm_file):
             Color.pl('{!} {R}error: ASM file not found {O}%s{R}{W}\r\n' % Configuration.asm_file)
             sys.exit(1)
 
         try:
             with open(Configuration.asm_file, 'r') as f:
```

### Comparing `ShellcodeTester-0.2.2/shellcodetester/password.py` & `ShellcodeTester-0.2.3/shellcodetester/password.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.2/shellcodetester/shellcodetester.py` & `ShellcodeTester-0.2.3/shellcodetester/shellcodetester.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,28 +32,38 @@
         self.run()
 
     def run(self):
 
         try:
 
             timestamp = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            Logger.pl('{+} {C}start time {O}%s{W}' % timestamp)
+            Logger.pl('{+} {C}Start time {O}%s{W}' % timestamp)
 
             # Assembly ASM File
             asm = Assembler(Configuration.asm_file)
             if not asm.assembly():
                 sys.exit(2)
 
             if Configuration.verbose >= 1 or any(bc in asm.assembled_data for bc in Configuration.bad_chars):
                 dis = Disassembler(Configuration.asm_file, asm.assembled_data)
                 dis.dump(Configuration.bad_chars)
 
+                fill_data = bytearray([
+                    b for b in asm.assembled_data
+                    if b not in Configuration.bad_chars
+                ])
+
+                if len(asm.assembled_data) != len(fill_data):
+                    Logger.pl('{!} {R}Bad chars found. {GR}Disassembly without bad chars{W}')
+                    dis = Disassembler(filename='', assembled_data=fill_data, platform=Configuration.platform, arch=asm.arch)
+                    dis.dump(Configuration.bad_chars, quiet=True)
+
             asm.print_payload(Configuration.transform_format, Configuration.bad_chars)
 
-            comp = Compiler(Configuration.asm_file, asm.assembled_data)
+            comp = Compiler(Configuration.asm_file, asm.assembled_data, Configuration.bad_chars, Configuration.remove)
             if not comp.compile():
                 sys.exit(2)
 
         except Exception as e:
             Color.pl("\n{!} {R}Error: {O}%s" % str(e))
             if Configuration.verbose > 0 or True:
                 Color.pl('\n{!} {O}Full stack trace below')
```

