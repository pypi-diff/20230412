# Comparing `tmp/xontrib-jump-to-dir-0.1.0.tar.gz` & `tmp/xontrib-jump-to-dir-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-jump-to-dir-0.1.0.tar", last modified: Mon Apr  3 14:49:25 2023, max compression
+gzip compressed data, was "xontrib-jump-to-dir-0.1.1.tar", last modified: Wed Apr 12 13:14:16 2023, max compression
```

## Comparing `xontrib-jump-to-dir-0.1.0.tar` & `xontrib-jump-to-dir-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:49:25.942036 xontrib-jump-to-dir-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-03 14:49:10.000000 xontrib-jump-to-dir-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-03 14:49:25.942036 xontrib-jump-to-dir-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-03 14:49:10.000000 xontrib-jump-to-dir-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-03 14:49:10.000000 xontrib-jump-to-dir-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 14:49:25.942036 xontrib-jump-to-dir-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-03 14:49:10.000000 xontrib-jump-to-dir-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:49:25.942036 xontrib-jump-to-dir-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-03 14:49:10.000000 xontrib-jump-to-dir-0.1.0/tests/test_xontrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:49:25.942036 xontrib-jump-to-dir-0.1.0/xontrib/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-03 14:49:10.000000 xontrib-jump-to-dir-0.1.0/xontrib/jump_to_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:49:25.942036 xontrib-jump-to-dir-0.1.0/xontrib_jump_to_dir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-03 14:49:25.000000 xontrib-jump-to-dir-0.1.0/xontrib_jump_to_dir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-03 14:49:25.000000 xontrib-jump-to-dir-0.1.0/xontrib_jump_to_dir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:49:25.000000 xontrib-jump-to-dir-0.1.0/xontrib_jump_to_dir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-03 14:49:25.000000 xontrib-jump-to-dir-0.1.0/xontrib_jump_to_dir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-03 14:49:25.000000 xontrib-jump-to-dir-0.1.0/xontrib_jump_to_dir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:14:16.165339 xontrib-jump-to-dir-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 13:14:04.000000 xontrib-jump-to-dir-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-12 13:14:16.165339 xontrib-jump-to-dir-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-12 13:14:04.000000 xontrib-jump-to-dir-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-12 13:14:04.000000 xontrib-jump-to-dir-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:14:16.165339 xontrib-jump-to-dir-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 13:14:04.000000 xontrib-jump-to-dir-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:14:16.165339 xontrib-jump-to-dir-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 13:14:04.000000 xontrib-jump-to-dir-0.1.1/tests/test_xontrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:14:16.165339 xontrib-jump-to-dir-0.1.1/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 13:14:04.000000 xontrib-jump-to-dir-0.1.1/xontrib/jump_to_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:14:16.165339 xontrib-jump-to-dir-0.1.1/xontrib_jump_to_dir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-12 13:14:16.000000 xontrib-jump-to-dir-0.1.1/xontrib_jump_to_dir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-12 13:14:16.000000 xontrib-jump-to-dir-0.1.1/xontrib_jump_to_dir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:14:16.000000 xontrib-jump-to-dir-0.1.1/xontrib_jump_to_dir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 13:14:16.000000 xontrib-jump-to-dir-0.1.1/xontrib_jump_to_dir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 13:14:16.000000 xontrib-jump-to-dir-0.1.1/xontrib_jump_to_dir.egg-info/top_level.txt
```

### Comparing `xontrib-jump-to-dir-0.1.0/LICENSE` & `xontrib-jump-to-dir-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-jump-to-dir-0.1.0/PKG-INFO` & `xontrib-jump-to-dir-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-jump-to-dir
-Version: 0.1.0
+Version: 0.1.1
 Summary: Jump to used before directory by part of the path. Lightweight zero-dependency implementation of autojump or zoxide projects functionality.
 Author-email: anki-code <no@no.no>
 License: MIT License
         
         Copyright (c) 2023, anki-code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,22 +75,28 @@
 echo 1
 echo 2
 echo 3
 cd /tmp/world
 echo 1
 cd /
 
-j           # Jump to most frequent directory i.e. `/tmp/hello` because 3 `echo` commands were executed
-j wor       # Jump to directory with `*wor*` in path i.e. `/tmp/world`
-j t he      # Jump to directory with `*t*he*` in path i.e. `/tmp/hello`
+j           # Jump to most frequent directory i.e. `/tmp/hello/` because 3 `echo` commands were executed
+j wor       # Jump to directory with `*wor*` in path i.e. `/tmp/world/`
+j t he      # Jump to directory with `*t*he*` in path i.e. `/tmp/hello/`
 ```
 
 Custom shortcut:
 ```xsh
 $XONTRIB_JUMP_TO_DIR_SHORTCUT = 'z'
 xontrib load jump_to_dir
-z tm  # Jump to `*tm*`
+z tm  # Jump to previous directory with `*tm*` in path e.g. `/tmp/`
 ```
 
+## How it works
+
+The history database has the commands you run and the directory where you was. The xontrib sorts the directories from history database by count of executed commands and filter them by mask e.g. the `j tm` command will find the directories by mask `*tm*`. Then you jump into the existing directory with the highest number of executed commands or if you already there to the previous directory by statistics. So if you have no commands that were executed in `/example` directory please avoid expectation that you can jump to it by running `j ex`.
+
+If you want to add fallback functionality to jump to any directory by partial path in case of zero result in history database (e.g. `j o lo bi` will jump to `/opt/local/bin`) feel free to create PR.
+
 ## Credits
 
 This package was created with [xontrib template](https://github.com/xonsh/xontrib-template).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-jump-to-dir Version: 0.1.0 Summary: Jump to
+Metadata-Version: 2.1 Name: xontrib-jump-to-dir Version: 0.1.1 Summary: Jump to
 used before directory by part of the path. Lightweight zero-dependency
 implementation of autojump or zoxide projects functionality. Author-email:
 anki-code
 no.no> License: MIT License Copyright (c) 2023, anki-code Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -33,13 +33,24 @@
 ## Note This xontrib is using [xonsh sqlite history backend](https://xon.sh/
 tutorial_hist.html#sqlite-history-backend) to get statistics by directories
 you're used to run commands. ## Installation To install use pip: ```bash xpip
 install xontrib-jump-to-dir # OR: xpip install -U git+https://github.com/anki-
 code/xontrib-jump-to-dir ``` ## Usage ```xsh # Check that you're using sqlite
 history in ~/.xonshrc $XONSH_HISTORY_BACKEND = 'sqlite' xontrib load
 jump_to_dir mkdir -p /tmp/hello /tmp/world cd /tmp/hello echo 1 echo 2 echo 3
-cd /tmp/world echo 1 cd / j # Jump to most frequent directory i.e. `/tmp/hello`
-because 3 `echo` commands were executed j wor # Jump to directory with `*wor*`
-in path i.e. `/tmp/world` j t he # Jump to directory with `*t*he*` in path i.e.
-`/tmp/hello` ``` Custom shortcut: ```xsh $XONTRIB_JUMP_TO_DIR_SHORTCUT = 'z'
-xontrib load jump_to_dir z tm # Jump to `*tm*` ``` ## Credits This package was
+cd /tmp/world echo 1 cd / j # Jump to most frequent directory i.e. `/tmp/hello/
+` because 3 `echo` commands were executed j wor # Jump to directory with
+`*wor*` in path i.e. `/tmp/world/` j t he # Jump to directory with `*t*he*` in
+path i.e. `/tmp/hello/` ``` Custom shortcut: ```xsh
+$XONTRIB_JUMP_TO_DIR_SHORTCUT = 'z' xontrib load jump_to_dir z tm # Jump to
+previous directory with `*tm*` in path e.g. `/tmp/` ``` ## How it works The
+history database has the commands you run and the directory where you was. The
+xontrib sorts the directories from history database by count of executed
+commands and filter them by mask e.g. the `j tm` command will find the
+directories by mask `*tm*`. Then you jump into the existing directory with the
+highest number of executed commands or if you already there to the previous
+directory by statistics. So if you have no commands that were executed in `/
+example` directory please avoid expectation that you can jump to it by running
+`j ex`. If you want to add fallback functionality to jump to any directory by
+partial path in case of zero result in history database (e.g. `j o lo bi` will
+jump to `/opt/local/bin`) feel free to create PR. ## Credits This package was
 created with [xontrib template](https://github.com/xonsh/xontrib-template).
```

### Comparing `xontrib-jump-to-dir-0.1.0/README.md` & `xontrib-jump-to-dir-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -32,22 +32,28 @@
 echo 1
 echo 2
 echo 3
 cd /tmp/world
 echo 1
 cd /
 
-j           # Jump to most frequent directory i.e. `/tmp/hello` because 3 `echo` commands were executed
-j wor       # Jump to directory with `*wor*` in path i.e. `/tmp/world`
-j t he      # Jump to directory with `*t*he*` in path i.e. `/tmp/hello`
+j           # Jump to most frequent directory i.e. `/tmp/hello/` because 3 `echo` commands were executed
+j wor       # Jump to directory with `*wor*` in path i.e. `/tmp/world/`
+j t he      # Jump to directory with `*t*he*` in path i.e. `/tmp/hello/`
 ```
 
 Custom shortcut:
 ```xsh
 $XONTRIB_JUMP_TO_DIR_SHORTCUT = 'z'
 xontrib load jump_to_dir
-z tm  # Jump to `*tm*`
+z tm  # Jump to previous directory with `*tm*` in path e.g. `/tmp/`
 ```
 
+## How it works
+
+The history database has the commands you run and the directory where you was. The xontrib sorts the directories from history database by count of executed commands and filter them by mask e.g. the `j tm` command will find the directories by mask `*tm*`. Then you jump into the existing directory with the highest number of executed commands or if you already there to the previous directory by statistics. So if you have no commands that were executed in `/example` directory please avoid expectation that you can jump to it by running `j ex`.
+
+If you want to add fallback functionality to jump to any directory by partial path in case of zero result in history database (e.g. `j o lo bi` will jump to `/opt/local/bin`) feel free to create PR.
+
 ## Credits
 
 This package was created with [xontrib template](https://github.com/xonsh/xontrib-template).
```

#### html2text {}

```diff
@@ -5,13 +5,24 @@
 ## Note This xontrib is using [xonsh sqlite history backend](https://xon.sh/
 tutorial_hist.html#sqlite-history-backend) to get statistics by directories
 you're used to run commands. ## Installation To install use pip: ```bash xpip
 install xontrib-jump-to-dir # OR: xpip install -U git+https://github.com/anki-
 code/xontrib-jump-to-dir ``` ## Usage ```xsh # Check that you're using sqlite
 history in ~/.xonshrc $XONSH_HISTORY_BACKEND = 'sqlite' xontrib load
 jump_to_dir mkdir -p /tmp/hello /tmp/world cd /tmp/hello echo 1 echo 2 echo 3
-cd /tmp/world echo 1 cd / j # Jump to most frequent directory i.e. `/tmp/hello`
-because 3 `echo` commands were executed j wor # Jump to directory with `*wor*`
-in path i.e. `/tmp/world` j t he # Jump to directory with `*t*he*` in path i.e.
-`/tmp/hello` ``` Custom shortcut: ```xsh $XONTRIB_JUMP_TO_DIR_SHORTCUT = 'z'
-xontrib load jump_to_dir z tm # Jump to `*tm*` ``` ## Credits This package was
+cd /tmp/world echo 1 cd / j # Jump to most frequent directory i.e. `/tmp/hello/
+` because 3 `echo` commands were executed j wor # Jump to directory with
+`*wor*` in path i.e. `/tmp/world/` j t he # Jump to directory with `*t*he*` in
+path i.e. `/tmp/hello/` ``` Custom shortcut: ```xsh
+$XONTRIB_JUMP_TO_DIR_SHORTCUT = 'z' xontrib load jump_to_dir z tm # Jump to
+previous directory with `*tm*` in path e.g. `/tmp/` ``` ## How it works The
+history database has the commands you run and the directory where you was. The
+xontrib sorts the directories from history database by count of executed
+commands and filter them by mask e.g. the `j tm` command will find the
+directories by mask `*tm*`. Then you jump into the existing directory with the
+highest number of executed commands or if you already there to the previous
+directory by statistics. So if you have no commands that were executed in `/
+example` directory please avoid expectation that you can jump to it by running
+`j ex`. If you want to add fallback functionality to jump to any directory by
+partial path in case of zero result in history database (e.g. `j o lo bi` will
+jump to `/opt/local/bin`) feel free to create PR. ## Credits This package was
 created with [xontrib template](https://github.com/xonsh/xontrib-template).
```

### Comparing `xontrib-jump-to-dir-0.1.0/pyproject.toml` & `xontrib-jump-to-dir-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "xontrib-jump-to-dir"
-version = "0.1.0"
+version = "0.1.1"
 license = {file = "LICENSE"}
 description = "Jump to used before directory by part of the path. Lightweight zero-dependency implementation of autojump or zoxide projects functionality."
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: System :: Shells",
```

### Comparing `xontrib-jump-to-dir-0.1.0/xontrib/jump_to_dir.py` & `xontrib-jump-to-dir-0.1.1/xontrib/jump_to_dir.py`

 * *Files identical despite different names*

### Comparing `xontrib-jump-to-dir-0.1.0/xontrib_jump_to_dir.egg-info/PKG-INFO` & `xontrib-jump-to-dir-0.1.1/xontrib_jump_to_dir.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-jump-to-dir
-Version: 0.1.0
+Version: 0.1.1
 Summary: Jump to used before directory by part of the path. Lightweight zero-dependency implementation of autojump or zoxide projects functionality.
 Author-email: anki-code <no@no.no>
 License: MIT License
         
         Copyright (c) 2023, anki-code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,22 +75,28 @@
 echo 1
 echo 2
 echo 3
 cd /tmp/world
 echo 1
 cd /
 
-j           # Jump to most frequent directory i.e. `/tmp/hello` because 3 `echo` commands were executed
-j wor       # Jump to directory with `*wor*` in path i.e. `/tmp/world`
-j t he      # Jump to directory with `*t*he*` in path i.e. `/tmp/hello`
+j           # Jump to most frequent directory i.e. `/tmp/hello/` because 3 `echo` commands were executed
+j wor       # Jump to directory with `*wor*` in path i.e. `/tmp/world/`
+j t he      # Jump to directory with `*t*he*` in path i.e. `/tmp/hello/`
 ```
 
 Custom shortcut:
 ```xsh
 $XONTRIB_JUMP_TO_DIR_SHORTCUT = 'z'
 xontrib load jump_to_dir
-z tm  # Jump to `*tm*`
+z tm  # Jump to previous directory with `*tm*` in path e.g. `/tmp/`
 ```
 
+## How it works
+
+The history database has the commands you run and the directory where you was. The xontrib sorts the directories from history database by count of executed commands and filter them by mask e.g. the `j tm` command will find the directories by mask `*tm*`. Then you jump into the existing directory with the highest number of executed commands or if you already there to the previous directory by statistics. So if you have no commands that were executed in `/example` directory please avoid expectation that you can jump to it by running `j ex`.
+
+If you want to add fallback functionality to jump to any directory by partial path in case of zero result in history database (e.g. `j o lo bi` will jump to `/opt/local/bin`) feel free to create PR.
+
 ## Credits
 
 This package was created with [xontrib template](https://github.com/xonsh/xontrib-template).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-jump-to-dir Version: 0.1.0 Summary: Jump to
+Metadata-Version: 2.1 Name: xontrib-jump-to-dir Version: 0.1.1 Summary: Jump to
 used before directory by part of the path. Lightweight zero-dependency
 implementation of autojump or zoxide projects functionality. Author-email:
 anki-code
 no.no> License: MIT License Copyright (c) 2023, anki-code Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -33,13 +33,24 @@
 ## Note This xontrib is using [xonsh sqlite history backend](https://xon.sh/
 tutorial_hist.html#sqlite-history-backend) to get statistics by directories
 you're used to run commands. ## Installation To install use pip: ```bash xpip
 install xontrib-jump-to-dir # OR: xpip install -U git+https://github.com/anki-
 code/xontrib-jump-to-dir ``` ## Usage ```xsh # Check that you're using sqlite
 history in ~/.xonshrc $XONSH_HISTORY_BACKEND = 'sqlite' xontrib load
 jump_to_dir mkdir -p /tmp/hello /tmp/world cd /tmp/hello echo 1 echo 2 echo 3
-cd /tmp/world echo 1 cd / j # Jump to most frequent directory i.e. `/tmp/hello`
-because 3 `echo` commands were executed j wor # Jump to directory with `*wor*`
-in path i.e. `/tmp/world` j t he # Jump to directory with `*t*he*` in path i.e.
-`/tmp/hello` ``` Custom shortcut: ```xsh $XONTRIB_JUMP_TO_DIR_SHORTCUT = 'z'
-xontrib load jump_to_dir z tm # Jump to `*tm*` ``` ## Credits This package was
+cd /tmp/world echo 1 cd / j # Jump to most frequent directory i.e. `/tmp/hello/
+` because 3 `echo` commands were executed j wor # Jump to directory with
+`*wor*` in path i.e. `/tmp/world/` j t he # Jump to directory with `*t*he*` in
+path i.e. `/tmp/hello/` ``` Custom shortcut: ```xsh
+$XONTRIB_JUMP_TO_DIR_SHORTCUT = 'z' xontrib load jump_to_dir z tm # Jump to
+previous directory with `*tm*` in path e.g. `/tmp/` ``` ## How it works The
+history database has the commands you run and the directory where you was. The
+xontrib sorts the directories from history database by count of executed
+commands and filter them by mask e.g. the `j tm` command will find the
+directories by mask `*tm*`. Then you jump into the existing directory with the
+highest number of executed commands or if you already there to the previous
+directory by statistics. So if you have no commands that were executed in `/
+example` directory please avoid expectation that you can jump to it by running
+`j ex`. If you want to add fallback functionality to jump to any directory by
+partial path in case of zero result in history database (e.g. `j o lo bi` will
+jump to `/opt/local/bin`) feel free to create PR. ## Credits This package was
 created with [xontrib template](https://github.com/xonsh/xontrib-template).
```

